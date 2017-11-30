terminalCode.MD

Last login: Tue Nov 28 13:50:41 on console
Kenneths-MacBook-Pro:~ everydaykenneth$ cd /Volumes/sdMemory/FullStackDeveloper/sqlAlchemy 
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Checking if box 'hashicorp/precise32' is up to date...
==> default: Clearing any previously set forwarded ports...
==> default: Clearing any previously set network interfaces...
==> default: Preparing network interfaces based on configuration...
    default: Adapter 1: nat
==> default: Forwarding ports...
    default: 22 (guest) => 2222 (host) (adapter 1)
==> default: Booting VM...
==> default: Waiting for machine to boot. This may take a few minutes...
    default: SSH address: 127.0.0.1:2222
    default: SSH username: vagrant
    default: SSH auth method: private key
==> default: Machine booted and ready!
==> default: Checking for guest additions in VM...
    default: The guest additions on this VM do not match the installed version of
    default: VirtualBox! In most cases this is fine, but in rare cases it can
    default: prevent things such as shared folders from working properly. If you see
    default: shared folder errors, please make sure the guest additions within the
    default: virtual machine match the version of VirtualBox you have installed on
    default: your host and reload your VM.
    default: 
    default: Guest Additions Version: 4.2.0
    default: VirtualBox Version: 5.2
==> default: Mounting shared folders...
    default: /vagrant => /Volumes/sdMemory/FullStackDeveloper/sqlAlchemy
==> default: Machine already provisioned. Run `vagrant provision` or use the `--provision`
==> default: flag to force provisioning. Provisioners marked to run always will still run.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant ssh
Welcome to Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic-pae i686)

 * Documentation:  https://help.ubuntu.com/
New release '14.04.5 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

Welcome to your Vagrant-built virtual machine.
Last login: Mon Nov 27 10:47:43 2017 from 10.0.2.2
vagrant@precise32:~$ python 
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> from sqlalchemy import create_engine
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ImportError: No module named sqlalchemy
>>> pip install sqlalchemy
  File "<stdin>", line 1
    pip install sqlalchemy
              ^
SyntaxError: invalid syntax
>>> from sqlalchemy import create_engine
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ImportError: No module named sqlalchemy
>>> vagrant global-status
  File "<stdin>", line 1
    vagrant global-status
                 ^
SyntaxError: invalid syntax
>>> vagrant global-status
  File "<stdin>", line 1
    vagrant global-status
                 ^
SyntaxError: invalid syntax
>>> vagrant halt
  File "<stdin>", line 1
    vagrant halt
               ^
SyntaxError: invalid syntax
>>> 
KeyboardInterrupt
>>> 
KeyboardInterrupt
>>> exit
Use exit() or Ctrl-D (i.e. EOF) to exit
>>> 
vagrant@precise32:~$ vagrant halt
The program 'vagrant' is currently not installed.  You can install it by typing:
sudo apt-get install vagrant
vagrant@precise32:~$ exit
logout
Connection to 127.0.0.1 closed.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant halt
==> default: Attempting graceful shutdown of VM...
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Checking if box 'hashicorp/precise32' is up to date...
==> default: Clearing any previously set forwarded ports...
==> default: Clearing any previously set network interfaces...
==> default: Preparing network interfaces based on configuration...
    default: Adapter 1: nat
==> default: Forwarding ports...
    default: 22 (guest) => 2222 (host) (adapter 1)
==> default: Booting VM...
==> default: Waiting for machine to boot. This may take a few minutes...
    default: SSH address: 127.0.0.1:2222
    default: SSH username: vagrant
    default: SSH auth method: private key
==> default: Machine booted and ready!
==> default: Checking for guest additions in VM...
    default: The guest additions on this VM do not match the installed version of
    default: VirtualBox! In most cases this is fine, but in rare cases it can
    default: prevent things such as shared folders from working properly. If you see
    default: shared folder errors, please make sure the guest additions within the
    default: virtual machine match the version of VirtualBox you have installed on
    default: your host and reload your VM.
    default: 
    default: Guest Additions Version: 4.2.0
    default: VirtualBox Version: 5.2
==> default: Mounting shared folders...
    default: /vagrant => /Volumes/sdMemory/FullStackDeveloper/sqlAlchemy
==> default: Machine already provisioned. Run `vagrant provision` or use the `--provision`
==> default: flag to force provisioning. Provisioners marked to run always will still run.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant update box
Usage: vagrant [options] <command> [<args>]

    -v, --version                    Print the version and exit.
    -h, --help                       Print this help.

Common commands:
     box             manages boxes: installation, removal, etc.
     connect         connect to a remotely shared Vagrant environment
     destroy         stops and deletes all traces of the vagrant machine
     global-status   outputs status Vagrant environments for this user
     halt            stops the vagrant machine
     help            shows the help for a subcommand
     init            initializes a new Vagrant environment by creating a Vagrantfile
     login           log in to HashiCorp's Vagrant Cloud
     package         packages a running vagrant environment into a box
     plugin          manages plugins: install, uninstall, update, etc.
     port            displays information about guest port mappings
     powershell      connects to machine via powershell remoting
     provision       provisions the vagrant machine
     push            deploys code in this environment to a configured destination
     rdp             connects to machine via RDP
     reload          restarts vagrant machine, loads new Vagrantfile configuration
     resume          resume a suspended vagrant machine
     share           share your Vagrant environment with anyone in the world
     snapshot        manages snapshots: saving, restoring, etc.
     ssh             connects to machine via SSH
     ssh-config      outputs OpenSSH valid configuration to connect to the machine
     status          outputs status of the vagrant machine
     suspend         suspends the machine
     up              starts and provisions the vagrant environment
     validate        validates the Vagrantfile
     version         prints current and latest Vagrant version

For help on any individual command run `vagrant COMMAND -h`

Additional subcommands are available, but are either more advanced
or not commonly used. To see all subcommands, run the command
`vagrant list-commands`.

Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant provision
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Checking if box 'hashicorp/precise32' is up to date...
==> default: Machine already provisioned. Run `vagrant provision` or use the `--provision`
==> default: flag to force provisioning. Provisioners marked to run always will still run.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant ssh
Welcome to Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic-pae i686)

 * Documentation:  https://help.ubuntu.com/
New release '14.04.5 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

Welcome to your Vagrant-built virtual machine.
Last login: Tue Nov 28 06:04:10 2017 from 10.0.2.2
vagrant@precise32:~$ ls
postinstall.sh
vagrant@precise32:~$ cd vagrant
-bash: cd: vagrant: No such file or directory
vagrant@precise32:~$ python
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> 
KeyboardInterrupt
>>> 
vagrant@precise32:~$ vagrant halt
The program 'vagrant' is currently not installed.  You can install it by typing:
sudo apt-get install vagrant
vagrant@precise32:~$ exit
logout
Connection to 127.0.0.1 closed.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant halt
==> default: Attempting graceful shutdown of VM...
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ pip install sqlalchemy
Requirement already satisfied: sqlalchemy in /Library/Frameworks/Python.framework/Versions/2.7/lib/python2.7/site-packages
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Checking if box 'hashicorp/precise32' is up to date...
==> default: Clearing any previously set forwarded ports...
==> default: Clearing any previously set network interfaces...
==> default: Preparing network interfaces based on configuration...
    default: Adapter 1: nat
==> default: Forwarding ports...
    default: 22 (guest) => 2222 (host) (adapter 1)
==> default: Booting VM...
==> default: Waiting for machine to boot. This may take a few minutes...
    default: SSH address: 127.0.0.1:2222
    default: SSH username: vagrant
    default: SSH auth method: private key
==> default: Machine booted and ready!
==> default: Checking for guest additions in VM...
    default: The guest additions on this VM do not match the installed version of
    default: VirtualBox! In most cases this is fine, but in rare cases it can
    default: prevent things such as shared folders from working properly. If you see
    default: shared folder errors, please make sure the guest additions within the
    default: virtual machine match the version of VirtualBox you have installed on
    default: your host and reload your VM.
    default: 
    default: Guest Additions Version: 4.2.0
    default: VirtualBox Version: 5.2
==> default: Mounting shared folders...
    default: /vagrant => /Volumes/sdMemory/FullStackDeveloper/sqlAlchemy
==> default: Machine already provisioned. Run `vagrant provision` or use the `--provision`
==> default: flag to force provisioning. Provisioners marked to run always will still run.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant ssh
Welcome to Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic-pae i686)

 * Documentation:  https://help.ubuntu.com/
New release '14.04.5 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

Welcome to your Vagrant-built virtual machine.
Last login: Tue Nov 28 06:23:33 2017 from 10.0.2.2
vagrant@precise32:~$ cd /vagrant
vagrant@precise32:/vagrant$ ls
database_setup2.py  README.md          Vagrantfile
database_setup.py   restaurantmenu.db
vagrant@precise32:/vagrant$ python
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> from sqlalchemy import create_engine
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ImportError: No module named sqlalchemy
>>> 
vagrant@precise32:/vagrant$ pip install sqlalchemy
The program 'pip' is currently not installed.  You can install it by typing:
sudo apt-get install python-pip
vagrant@precise32:/vagrant$ sup apt-get install python-pip
The program 'sup' is currently not installed.  You can install it by typing:
sudo apt-get install sup
vagrant@precise32:/vagrant$ sudo apt-get install python-pip
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following extra packages will be installed:
  python-pkg-resources python-setuptools
Suggested packages:
  python-distribute python-distribute-doc
The following NEW packages will be installed:
  python-pip python-pkg-resources python-setuptools
0 upgraded, 3 newly installed, 0 to remove and 66 not upgraded.
Need to get 599 kB of archives.
After this operation, 1,647 kB of additional disk space will be used.
Do you want to continue [Y/n]? y
Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main python-pkg-resources all 0.6.24-1ubuntu1 [63.1 kB]
Get:2 http://us.archive.ubuntu.com/ubuntu/ precise/main python-setuptools all 0.6.24-1ubuntu1 [441 kB]
Get:3 http://us.archive.ubuntu.com/ubuntu/ precise/universe python-pip all 1.0-1build1 [95.1 kB]
Fetched 599 kB in 3s (157 kB/s)  
Selecting previously unselected package python-pkg-resources.
(Reading database ... 29361 files and directories currently installed.)
Unpacking python-pkg-resources (from .../python-pkg-resources_0.6.24-1ubuntu1_all.deb) ...
Selecting previously unselected package python-setuptools.
Unpacking python-setuptools (from .../python-setuptools_0.6.24-1ubuntu1_all.deb) ...
Selecting previously unselected package python-pip.
Unpacking python-pip (from .../python-pip_1.0-1build1_all.deb) ...
Processing triggers for man-db ...
Setting up python-pkg-resources (0.6.24-1ubuntu1) ...
Setting up python-setuptools (0.6.24-1ubuntu1) ...
Setting up python-pip (1.0-1build1) ...
vagrant@precise32:/vagrant$ pip install sqlalchemy
Downloading/unpacking sqlalchemy
  Cannot fetch index base URL http://pypi.python.org/simple/
  Could not find any downloads that satisfy the requirement sqlalchemy
No distributions at all found for sqlalchemy
Storing complete log in /home/vagrant/.pip/pip.log
vagrant@precise32:/vagrant$ sudo -H pip install sqlalchemy
Downloading/unpacking sqlalchemy
  Cannot fetch index base URL http://pypi.python.org/simple/
  Could not find any downloads that satisfy the requirement sqlalchemy
No distributions at all found for sqlalchemy
Storing complete log in /root/.pip/pip.log
vagrant@precise32:/vagrant$ python  
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> from sqlalchemy import create_engine
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ImportError: No module named sqlalchemy
>>> sudo apt-get -qqy install python-sqlalchemy
  File "<stdin>", line 1
    sudo apt-get -qqy install python-sqlalchemy
           ^
SyntaxError: invalid syntax
>>> 
vagrant@precise32:/vagrant$ sudo apt-get -qqy install python-sqlalchemy
Selecting previously unselected package python-sqlalchemy.
(Reading database ... 29583 files and directories currently installed.)
Unpacking python-sqlalchemy (from .../python-sqlalchemy_0.7.4-1ubuntu0.1_all.deb) ...
Selecting previously unselected package python-sqlalchemy-ext.
Unpacking python-sqlalchemy-ext (from .../python-sqlalchemy-ext_0.7.4-1ubuntu0.1_i386.deb) ...
Setting up python-sqlalchemy (0.7.4-1ubuntu0.1) ...
Setting up python-sqlalchemy-ext (0.7.4-1ubuntu0.1) ...
vagrant@precise32:/vagrant$ ls
build               database_setup.py  restaurantmenu.db
database_setup2.py  README.md          Vagrantfile
vagrant@precise32:/vagrant$ python
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> from sqlalchemy import create_engine
>>> from sqlalchemy.orm import sessionmaker
>>> from database_setup import Base, Restaurant, Menu Item
  File "<stdin>", line 1
    from database_setup import Base, Restaurant, Menu Item
                                                         ^
SyntaxError: invalid syntax
>>> from database_setup import Base, Restaurant, MenuItem 
>>> engine = create_engine('sqlite:///restaurantmenu.db')
>>> Base.metadata.bind = engine
>>> DBSession = sessionmaker(bind = engine)
>>> session = DBSession()
>>> myFirstRestaurant = Restaurant(name = "Pizza Palace")
>>> session.add(myFirstRestaurant)
>>> session.commit()
>>> session.query(Restaurant).all()
[<database_setup.Restaurant object at 0x97395cc>]
>>> cheesepizza = MenuItme(name = "Cheese Pizza", description = "Made with all natural ingredients and fresh mozzarella", course = "Entree", price = "$9.99", restaurant = myFirstRestaurant)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'MenuItme' is not defined
>>> cheesepizza = MenuItem(name = "Cheese Pizza", description = "Made with all natural ingredients and fresh mozzarella", course = "Entree", price = "$9.99", restaurant = myFirstRestaurant)
>>> session.add(cheesepizza)
>>> session.commit()
>>> session.query(MenuItem).all()
[<database_setup.MenuItem object at 0x973fc8c>]
>>> firstResult = session.query(Restaurant).first()
>>> firstResult.name
u'Pizza Palace'
>>> 
vagrant@precise32:/vagrant$ python lotsofmenus.py
added menu items!
vagrant@precise32:/vagrant$ python
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> session.query(Restaurant).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'session' is not defined
>>> from sqlalchemy import create_engine
>>> from sqlalchemy.orm import sessionmaker
>>> from database_setup import Restaurant, Base, MenuItem
>>> engine = create_engine('sqlite:///restaurantmenu.db')
>>> Base.metadata.bind = engine
>>> DBSession = sessionmaker(bind=engine)
>>> session = DBSession()
>>> session.query(Restaurant).all()
[<database_setup.Restaurant object at 0xa48464c>, <database_setup.Restaurant object at 0xa48472c>, <database_setup.Restaurant object at 0xa4846cc>, <database_setup.Restaurant object at 0xa4847ec>, <database_setup.Restaurant object at 0xa48486c>, <database_setup.Restaurant object at 0xa4848ec>, <database_setup.Restaurant object at 0xa48496c>, <database_setup.Restaurant object at 0xa4849ec>, <database_setup.Restaurant object at 0xa484a6c>, <database_setup.Restaurant object at 0xa484aec>]
>>> session.query(MenuItem).all()
[<database_setup.MenuItem object at 0xa47efac>, <database_setup.MenuItem object at 0xa48a50c>, <database_setup.MenuItem object at 0xa47efcc>, <database_setup.MenuItem object at 0xa48a5ac>, <database_setup.MenuItem object at 0xa48a60c>, <database_setup.MenuItem object at 0xa48a66c>, <database_setup.MenuItem object at 0xa48a6cc>, <database_setup.MenuItem object at 0xa48a72c>, <database_setup.MenuItem object at 0xa48a78c>, <database_setup.MenuItem object at 0xa48a7ec>, <database_setup.MenuItem object at 0xa48a86c>, <database_setup.MenuItem object at 0xa48a8ec>, <database_setup.MenuItem object at 0xa48a96c>, <database_setup.MenuItem object at 0xa48a9ec>, <database_setup.MenuItem object at 0xa48aa6c>, <database_setup.MenuItem object at 0xa48aaec>, <database_setup.MenuItem object at 0xa48ab6c>, <database_setup.MenuItem object at 0xa48abec>, <database_setup.MenuItem object at 0xa48ac6c>, <database_setup.MenuItem object at 0xa48acec>, <database_setup.MenuItem object at 0xa48ad6c>, <database_setup.MenuItem object at 0xa48adec>, <database_setup.MenuItem object at 0xa48ae6c>, <database_setup.MenuItem object at 0xa48aeec>, <database_setup.MenuItem object at 0xa48af6c>, <database_setup.MenuItem object at 0xa48afec>, <database_setup.MenuItem object at 0xa49208c>, <database_setup.MenuItem object at 0xa49210c>, <database_setup.MenuItem object at 0xa49218c>, <database_setup.MenuItem object at 0xa49220c>, <database_setup.MenuItem object at 0xa49228c>, <database_setup.MenuItem object at 0xa49230c>, <database_setup.MenuItem object at 0xa49238c>, <database_setup.MenuItem object at 0xa49240c>, <database_setup.MenuItem object at 0xa49248c>, <database_setup.MenuItem object at 0xa49250c>, <database_setup.MenuItem object at 0xa49258c>, <database_setup.MenuItem object at 0xa49260c>, <database_setup.MenuItem object at 0xa49268c>, <database_setup.MenuItem object at 0xa49270c>, <database_setup.MenuItem object at 0xa49278c>, <database_setup.MenuItem object at 0xa49280c>, <database_setup.MenuItem object at 0xa49288c>, <database_setup.MenuItem object at 0xa49290c>, <database_setup.MenuItem object at 0xa49298c>, <database_setup.MenuItem object at 0xa492a0c>, <database_setup.MenuItem object at 0xa492a8c>, <database_setup.MenuItem object at 0xa492b0c>, <database_setup.MenuItem object at 0xa492b8c>]
>>> session.query(Base).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "/usr/lib/python2.7/dist-packages/sqlalchemy/orm/session.py", line 969, in query
    return self._query_cls(entities, self, **kwargs)
  File "/usr/lib/python2.7/dist-packages/sqlalchemy/orm/query.py", line 107, in __init__
    self._set_entities(entities)
  File "/usr/lib/python2.7/dist-packages/sqlalchemy/orm/query.py", line 114, in _set_entities
    entity_wrapper(self, ent)
  File "/usr/lib/python2.7/dist-packages/sqlalchemy/orm/query.py", line 3081, in __init__
    "expected - got '%r'" % (column, )
sqlalchemy.exc.InvalidRequestError: SQL expression, column, or mapped entity expected - got '<class 'sqlalchemy.ext.declarative.Base'>'
>>> session.query(Restaurants).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'Restaurants' is not defined
>>> session.query(Restaurant).all()
[<database_setup.Restaurant object at 0xa48474c>, <database_setup.Restaurant object at 0xa4847ec>, <database_setup.Restaurant object at 0xa48478c>, <database_setup.Restaurant object at 0xa48486c>, <database_setup.Restaurant object at 0xa4848ec>, <database_setup.Restaurant object at 0xa48496c>, <database_setup.Restaurant object at 0xa4849ec>, <database_setup.Restaurant object at 0xa484a6c>, <database_setup.Restaurant object at 0xa484aec>, <database_setup.Restaurant object at 0xa484f0c>]
>>> session.query(MenuItems).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'MenuItems' is not defined
>>> session.query(MenuItem).all()
[<database_setup.MenuItem object at 0xa49210c>, <database_setup.MenuItem object at 0xa492bec>, <database_setup.MenuItem object at 0xa49218c>, <database_setup.MenuItem object at 0xa49220c>, <database_setup.MenuItem object at 0xa49228c>, <database_setup.MenuItem object at 0xa49230c>, <database_setup.MenuItem object at 0xa49238c>, <database_setup.MenuItem object at 0xa49240c>, <database_setup.MenuItem object at 0xa49248c>, <database_setup.MenuItem object at 0xa49250c>, <database_setup.MenuItem object at 0xa49258c>, <database_setup.MenuItem object at 0xa49260c>, <database_setup.MenuItem object at 0xa49268c>, <database_setup.MenuItem object at 0xa49270c>, <database_setup.MenuItem object at 0xa49278c>, <database_setup.MenuItem object at 0xa49280c>, <database_setup.MenuItem object at 0xa49288c>, <database_setup.MenuItem object at 0xa49290c>, <database_setup.MenuItem object at 0xa49298c>, <database_setup.MenuItem object at 0xa492a0c>, <database_setup.MenuItem object at 0xa492a8c>, <database_setup.MenuItem object at 0xa492b0c>, <database_setup.MenuItem object at 0xa492b8c>, <database_setup.MenuItem object at 0xb722ba4c>, <database_setup.MenuItem object at 0xb722b34c>, <database_setup.MenuItem object at 0xa48472c>, <database_setup.MenuItem object at 0xa484eec>, <database_setup.MenuItem object at 0xa484eac>, <database_setup.MenuItem object at 0xa48468c>, <database_setup.MenuItem object at 0xa47e6ac>, <database_setup.MenuItem object at 0xa47efac>, <database_setup.MenuItem object at 0xa47efcc>, <database_setup.MenuItem object at 0xa47e68c>, <database_setup.MenuItem object at 0xa47e1ec>, <database_setup.MenuItem object at 0xa47e0cc>, <database_setup.MenuItem object at 0xa50a6ec>, <database_setup.MenuItem object at 0xa50a96c>, <database_setup.MenuItem object at 0xa50a9ac>, <database_setup.MenuItem object at 0xa50a9ec>, <database_setup.MenuItem object at 0xa50aa2c>, <database_setup.MenuItem object at 0xa50aa6c>, <database_setup.MenuItem object at 0xa50aaac>, <database_setup.MenuItem object at 0xa50aaec>, <database_setup.MenuItem object at 0xa50ab2c>, <database_setup.MenuItem object at 0xa50ab6c>, <database_setup.MenuItem object at 0xa50abac>, <database_setup.MenuItem object at 0xa50abec>, <database_setup.MenuItem object at 0xa50ac2c>, <database_setup.MenuItem object at 0xa50ac6c>]
>>> 
>>> 
>>> 
>>> 
>>> items = session.query(MenuItem).all()
>>> items = session.query(MenuItems).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'MenuItems' is not defined
>>> items = session.query(MenuItem).all()
>>> for item in items
  File "<stdin>", line 1
    for item in items
                    ^
SyntaxError: invalid syntax
>>> for item in items
  File "<stdin>", line 1
    for item in items
                    ^
SyntaxError: invalid syntax
>>> for item in items print items.name
  File "<stdin>", line 1
    for item in items print items.name
                          ^
SyntaxError: invalid syntax
>>> for item in items:
... print items.name
  File "<stdin>", line 2
    print items.name
        ^
IndentationError: expected an indented block
>>> print item.name
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'item' is not defined
>>> for item in items:
... print item.name
  File "<stdin>", line 2
    print item.name
        ^
IndentationError: expected an indented block
>>>     print item.name
  File "<stdin>", line 1
    print item.name
    ^
IndentationError: unexpected indent
>>> items = session.query(MenuItem).all()
>>> for item in items:
...     print item.name
...   print item.name
  File "<stdin>", line 3
    print item.name
                  ^
IndentationError: unindent does not match any outer indentation level
>>> items = session.query(MenuItem).all()
>>> for item in items:
...   print item.name
...     print item.name
  File "<stdin>", line 3
    print item.name
    ^
IndentationError: unexpected indent
>>>     print items.name
  File "<stdin>", line 1
    print items.name
    ^
IndentationError: unexpected indent
>>> for item in items:
...     print items.name
... items = session.query(MenuItem).all()
  File "<stdin>", line 3
    items = session.query(MenuItem).all()
        ^
SyntaxError: invalid syntax
>>> items = session.query(MenuItem).all()
>>> for item in items:
...     print items.name
... Connection to 127.0.0.1 closed by remote host.
Connection to 127.0.0.1 closed.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ 
  [Restored Nov 30, 2017 at 2:09:06 PM]
Last login: Thu Nov 30 14:09:04 on console
Restored session: Wed Nov 29 18:02:50 CST 2017
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ git log
commit 53ef0e37c7e245ed4bcc0160dac33d6002ec34b3 (HEAD -> master, origin/master)
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Tue Nov 28 15:07:40 2017 +0800

    added data to the database

commit 10416d1cf23e9041ad3a6855aaf0973fe81a4f0f
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Mon Nov 27 18:51:54 2017 +0800

    database_setup.py working with virtualbox and sqlalchemy

commit 2a094579b9605ebdebbf3e585b9fc05e78e06041
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Mon Nov 27 18:51:16 2017 +0800

    pep8 code checked

commit e8943c44f52a70510f897a5e767629bcbe40cf85
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Mon Nov 27 18:03:29 2017 +0800

    SQL mapper class written out in psuedocode

commit 4f99a03545d4730f775002373f6532ac7186b786
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Mon Nov 27 17:53:44 2017 +0800

    created a class and table for menu items

commit 11f9acecdb54c13e1c78e166e4e9c81cc9cf1b5a
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Mon Nov 27 17:49:25 2017 +0800

    database_setup configuration for SQLalchemy

commit 82bccb4d23fc661d5ac0d2547b86a03616f8210a
Author: KendrickPC <kennethpchang@gmail.com>
Date:   Mon Nov 27 17:43:05 2017 +0800

    first commit

Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Checking if box 'hashicorp/precise32' is up to date...
==> default: Resuming suspended VM...
==> default: Booting VM...
==> default: Waiting for machine to boot. This may take a few minutes...
    default: SSH address: 127.0.0.1:2222
    default: SSH username: vagrant
    default: SSH auth method: private key
==> default: Machine booted and ready!
==> default: Machine already provisioned. Run `vagrant provision` or use the `--provision`
==> default: flag to force provisioning. Provisioners marked to run always will still run.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant halt
==> default: Attempting graceful shutdown of VM...
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Checking if box 'hashicorp/precise32' is up to date...
==> default: Clearing any previously set forwarded ports...
==> default: Clearing any previously set network interfaces...
==> default: Preparing network interfaces based on configuration...
    default: Adapter 1: nat
==> default: Forwarding ports...
    default: 22 (guest) => 2222 (host) (adapter 1)
==> default: Booting VM...
==> default: Waiting for machine to boot. This may take a few minutes...
    default: SSH address: 127.0.0.1:2222
    default: SSH username: vagrant
    default: SSH auth method: private key
==> default: Machine booted and ready!
==> default: Checking for guest additions in VM...
    default: The guest additions on this VM do not match the installed version of
    default: VirtualBox! In most cases this is fine, but in rare cases it can
    default: prevent things such as shared folders from working properly. If you see
    default: shared folder errors, please make sure the guest additions within the
    default: virtual machine match the version of VirtualBox you have installed on
    default: your host and reload your VM.
    default: 
    default: Guest Additions Version: 4.2.0
    default: VirtualBox Version: 5.2
==> default: Mounting shared folders...
    default: /vagrant => /Volumes/sdMemory/FullStackDeveloper/sqlAlchemy
==> default: Machine already provisioned. Run `vagrant provision` or use the `--provision`
==> default: flag to force provisioning. Provisioners marked to run always will still run.
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagramt ssh
-bash: vagramt: command not found
Kenneths-MacBook-Pro:sqlAlchemy everydaykenneth$ vagrant ssh
Welcome to Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic-pae i686)

 * Documentation:  https://help.ubuntu.com/
New release '14.04.5 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

Welcome to your Vagrant-built virtual machine.
Last login: Tue Nov 28 06:26:44 2017 from 10.0.2.2
vagrant@precise32:~$ cd /vagrant
vagrant@precise32:/vagrant$ ls
build  database_setup.py  database_setup.pyc  lotsofmenus.py  README.md  restaurantmenu.db  Vagrantfile
vagrant@precise32:/vagrant$ session.query(Restaurant).all()
-bash: syntax error near unexpected token `Restaurant'
vagrant@precise32:/vagrant$ python
Python 2.7.3 (default, Apr 20 2012, 22:44:07) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> session.query(Restaurant).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'session' is not defined
>>> from sqlalchemy import create_engine
>>> from sqlalchemy.orm import sessionmaker
>>> from database_setup import Restaurant, Base, MenuItem
>>> engine = create_engine('sqlite:///restaurantmenu.db')
>>> Base.metadata.bind = engine
>>> DBSession = sessionmaker(bind=engine)
>>> session = DBSession()
>>> session.query(Restaurant).all()
[<database_setup.Restaurant object at 0xa76a64c>, <database_setup.Restaurant object at 0xa76a72c>, <database_setup.Restaurant object at 0xa76a6cc>, <database_setup.Restaurant object at 0xa76a7ec>, <database_setup.Restaurant object at 0xa76a86c>, <database_setup.Restaurant object at 0xa76a8ec>, <database_setup.Restaurant object at 0xa76a96c>, <database_setup.Restaurant object at 0xa76a9ec>, <database_setup.Restaurant object at 0xa76aa6c>, <database_setup.Restaurant object at 0xa76aaec>]
>>> session.query(MenuItem).all()
[<database_setup.MenuItem object at 0xa764fac>, <database_setup.MenuItem object at 0xa77050c>, <database_setup.MenuItem object at 0xa764fcc>, <database_setup.MenuItem object at 0xa7705ac>, <database_setup.MenuItem object at 0xa77060c>, <database_setup.MenuItem object at 0xa77066c>, <database_setup.MenuItem object at 0xa7706cc>, <database_setup.MenuItem object at 0xa77072c>, <database_setup.MenuItem object at 0xa77078c>, <database_setup.MenuItem object at 0xa7707ec>, <database_setup.MenuItem object at 0xa77086c>, <database_setup.MenuItem object at 0xa7708ec>, <database_setup.MenuItem object at 0xa77096c>, <database_setup.MenuItem object at 0xa7709ec>, <database_setup.MenuItem object at 0xa770a6c>, <database_setup.MenuItem object at 0xa770aec>, <database_setup.MenuItem object at 0xa770b6c>, <database_setup.MenuItem object at 0xa770bec>, <database_setup.MenuItem object at 0xa770c6c>, <database_setup.MenuItem object at 0xa770cec>, <database_setup.MenuItem object at 0xa770d6c>, <database_setup.MenuItem object at 0xa770dec>, <database_setup.MenuItem object at 0xa770e6c>, <database_setup.MenuItem object at 0xa770eec>, <database_setup.MenuItem object at 0xa770f6c>, <database_setup.MenuItem object at 0xa770fec>, <database_setup.MenuItem object at 0xa77808c>, <database_setup.MenuItem object at 0xa77810c>, <database_setup.MenuItem object at 0xa77818c>, <database_setup.MenuItem object at 0xa77820c>, <database_setup.MenuItem object at 0xa77828c>, <database_setup.MenuItem object at 0xa77830c>, <database_setup.MenuItem object at 0xa77838c>, <database_setup.MenuItem object at 0xa77840c>, <database_setup.MenuItem object at 0xa77848c>, <database_setup.MenuItem object at 0xa77850c>, <database_setup.MenuItem object at 0xa77858c>, <database_setup.MenuItem object at 0xa77860c>, <database_setup.MenuItem object at 0xa77868c>, <database_setup.MenuItem object at 0xa77870c>, <database_setup.MenuItem object at 0xa77878c>, <database_setup.MenuItem object at 0xa77880c>, <database_setup.MenuItem object at 0xa77888c>, <database_setup.MenuItem object at 0xa77890c>, <database_setup.MenuItem object at 0xa77898c>, <database_setup.MenuItem object at 0xa778a0c>, <database_setup.MenuItem object at 0xa778a8c>, <database_setup.MenuItem object at 0xa778b0c>, <database_setup.MenuItem object at 0xa778b8c>]
>>> firstResult = session.query(Restuarant).first()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'Restuarant' is not defined
>>> firstResult = session.query(Restaurant).first()
>>> firstResult.name
u'Pizza Palace'
>>> 
>>> 
>>> 
>>> 
>>> 
>>> 
>>> items = session.query(MenuItems).all()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'MenuItems' is not defined
>>> items = session.query(MenuItem).all()
>>> for item in items:
...     print item.name
...     print item.name
  File "<stdin>", line 3
    print item.name
                  ^
IndentationError: unindent does not match any outer indentation level
>>>   print item.name
  File "<stdin>", line 1
    print item.name
    ^
IndentationError: unexpected indent
>>>     print item.name
  File "<stdin>", line 1
    print item.name
    ^
IndentationError: unexpected indent
>>>     print item.name
  File "<stdin>", line 1
    print item.name
    ^
IndentationError: unexpected indent
>>> for item in items:
...     print item.name
... 
Cheese Pizza
Veggie Burger
French Fries
Chicken Burger
Chocolate Cake
Sirloin Burger
Root Beer
Iced Tea
Grilled Cheese Sandwich
Veggie Burger
Chicken Stir Fry
Peking Duck
Spicy Tuna Roll
Nepali Momo 
Beef Noodle Soup
Ramen
Pho
Chinese Dumplings
Gyoza
Stinky Tofu
Veggie Burger
Tres Leches Cake
Mushroom risotto
Honey Boba Shaved Snow
Cauliflower Manchurian
Aloo Gobi Burrito
Veggie Burger
Shellfish Tower
Chicken and Rice
Mom's Spaghetti
Choc Full O' Mint (Smitten's Fresh Mint Chip ice cream)
Tonkatsu Ramen
Lamb Curry
Chicken Marsala
Potstickers
Nigiri Sampler
Veggie Burger
Chicken Fried Steak
Boysenberry Sorbet
Broiled salmon
Morels on toast (seasonal)
Tandoori Chicken
Veggie Burger
Spinach Ice Cream
Super Burrito Al Pastor
Cachapa
Chantrelle Toast
Guanciale Chawanmushi
Lemon Curd Ice Cream Sandwich
>>> 
