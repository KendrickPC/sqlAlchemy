## How to run the program:

1. Install Oracle's Virtual Box and Vagrant 
			https://www.virtualbox.org/
			https://www.vagrantup.com/

2. Open up the terminal and cd into the project folder - import necessary items with the following commands: 

			from sqlalchemy import create_engine
			from sqlalchemy.orm import sessionmaker
			from database_setup import Base, Restaurant, MenuItem

			engine = create_engine('sqlite:///restaurantMenu.db')
			Base.metadata.bind=engine
			DBSession = sessionmaker(bind = engine)
			session = DBSession()

3. Run the following commands:
	vagrant up
	vagrant ssh

4. cd into the vagrant folder with the following command: 
	cd /vagrant

5. run the webserver.py file with the following python command: 
	python webserver.py
