Book Catlog is a web app for organising Books. Users can view a list of categories of books and books under each category. Users can log-in using their Google authentication. Logged-in users can add, edit and delete book details.

* Server set up:
	- Install necessary software with the following commands:
		apt-get -qqy install python python-pip
		sudo pip2 install --upgrade pip
		sudo pip2 install flask packaging oauth2client redis passlib flask-httpauth
		sudo pip2 install sqlalchemy flask-sqlalchemy psycopg2-binary bleach requests
		sudo pip install --upgrade oauth2client
		sudo apt-get install sqlite3 libsqlite3-dev
		
	- Git clone the CatalogApp  with command
		$  git clone https://github.com/SathyamAP/CatalogApp.git
	- Set up data
		- Navigate to CatalogApp/catalog directory
		- from the command line, excute the command
			$  sudo python model.py
		- from the command line, excute the command
			$  sudo python populatedb.py
* Running the server:
	- Navigate to CatalogApp/catalog directory 
	- from the command line, excute the command
			$  sudo python application.py

* Accessing the Book Catalog App:
	- Open your browser and go to url http://13.233.138.138.nip.io:80



* Resources:
	- https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps#step-four-%E2%80%93-configure-and-enable-a-new-virtual-host
	- http://stackoverflow.com - a good place to go when you run into issues while developing and deploying applications 
