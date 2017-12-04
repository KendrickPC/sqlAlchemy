DEVELOPERNOTES.md

December 04, 2017



December 03, 2017

For creating a new restaurant, note the following: 

messagecontent = fields.get('newRestaurantName') should be indented such that it is inside the 'if' block

December 01, 2017

PYTHON BaseHTTPServer 
https://docs.python.org/2/library/basehttpserver.html

Objectives:
[] list all restaurants
[] add edit and delete links
[] create new restaurants
[] rename a restaurant
[] delete a restaurant


November 27th, 2017

sqlAlchemy setup 


November 30th, 2017

SQL Alchemy search queries documentation - very useful as a reference: 
http://docs.sqlalchemy.org/en/rel_0_9/orm/query.html

[tab] print item.name 
<!-- press enter again in python -->


CRUD Notes
Operations with SQLAlchemy
I performed all CRUD operations with SQLAlchemy on an SQLite database. Before I perform any operations, I must first import the necessary libraries, connect to our restaurantMenu.db, and create a session to interface with the database:

from sqlalchemy import create_engine
from sqlalchemy.orm import sessionmaker
from database_setup import Base, Restaurant, MenuItem

engine = create_engine('sqlite:///restaurantMenu.db')
Base.metadata.bind=engine
DBSession = sessionmaker(bind = engine)
session = DBSession()
CREATE
We created a new Restaurant and called it Pizza Palace:
myFirstRestaurant = Restaurant(name = "Pizza Palace")
session.add(myFirstRestaurant)
sesssion.commit()
We created a cheese pizza menu item and added it to the Pizza Palace Menu:
cheesepizza = menuItem(name="Cheese Pizza", description = "Made with all natural ingredients and fresh mozzarella", course="Entree", price="$8.99", restaurant=myFirstRestaurant)
session.add(cheesepizza)
session.commit()
# READ We read out information in our database using the query method in SQLAlchemy:
firstResult = session.query(Restaurant).first()
firstResult.name

items = session.query(MenuItem).all()
for item in items:
    print item.name
UPDATE
In order to update and existing entry in my database, I must execute the following commands:

Find Entry
Reset value(s)
Add to session
Execute session.commit()
I found the veggie burger that belonged to the Urban Burger restaurant by executing the following query:
veggieBurgers = session.query(MenuItem).filter_by(name= 'Veggie Burger')
for veggieBurger in veggieBurgers:
    print veggieBurger.id
    print veggieBurger.price
    print veggieBurger.restaurant.name
    print "\n"
Then I updated the price of the veggie burger to 3.33: (I forgot the dollar sign)

UrbanVeggieBurger = session.query(MenuItem).filter_by(id=8).one()
UrbanVeggieBurger.price = '$2.99'
session.add(UrbanVeggieBurger)
session.commit() 
DELETE
To delete an item from my database, I must follow the following steps:

Find the entry
Session.delete(Entry)
Session.commit()
I deleted spinach Ice Cream from our Menu Items database with the following operations:

spinach = session.query(MenuItem).filter_by(name = 'Spinach Ice Cream').one()
session.delete(spinach)
session.commit() 