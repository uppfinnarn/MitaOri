Mitakihara Original
===================

This is Version 3.0 of the Mitakihara Original site.

Mitakihara Original
-------------------
From the [site](http://macaronicode.se/MitaOri/):

> Mitakihara Original is a fan-written story set in the Puella Magi Madoka Magica universe. Through Twitter, a dedicated group of role-players creates stories following the daily lives of a group of teenagers dealing with the consequences of a hard truth they discover. Every player takes control of a character they created and writes storylines of their own, or with other players. All these plotlines are weaved together with a lot of improvisation to tell a tale unlike that of many other roleplaying efforts.

Version History
---------------
* Version 3.0
	* Python + Flask and PostgreSQL
	* Full rewrite, because Django is WAY too slow with large datasets
	* Cleaner layout, better mobile support
	* Integrated Wiki
	* Big Red Button! (planned)
* Version 2.1
	* Backend switched to PostgreSQL for better performance
* Version 2.0
	* Python + Django and MySQL
	* Shiny new layout!
	* No Big Red Button :(
* Version 1.0
	* PHP and MySQL
	* Big Red Button!

Current Version Requirements
----------------------------
* Python 2.7
	* Flask
	* Flask-WTF
	* Flask-Admin
	* Flask-SQLAlchemy
		* Obviously a database adapter to go with this
	* markdown2

Make sure to make the cache directory writable by the webserver, and to create a file called "config.py", containing:

* `SECRET_KEY` - a long string used for hashing and CSRF protection
* `SQLALCHEMY_DATABASE_URI` - connection string to the database