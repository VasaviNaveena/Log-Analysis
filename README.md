# Log Analysis Project
This is a project for Udacity's [Full Stack Web Developer Nanodegree](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd004)

## Project Description:
This project is to create a reporting tool that prints out reports (in plain text) 
based on the data in the database. This reporting tool is a Python program 
using the "psycopg2" module to connect to the database.

## This Project Requires a Bit of Setup:
This project should run in a virutal machine created using Vagrant so there are a few steps to get set up:

#### Installing the dependencies and setting up the files:
* Install [Vagrant](https://www.vagrantup.com/)
* Install [VirtualBox](https://www.virtualbox.org/)
* Download the vagrant setup files from [Udacity's Github](https://github.com/udacity/fullstack-nanodegree-vm)
These files configure the virtual machine and install all the tools needed to run this project.
* Download the database setup: [data](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip)
* Unzip the data to get the newsdata.sql file.
* Put the newsdata.sql file into the vagrant directory into a folder called log-analysis

#### Start the Virtual Machine:
* Open Terminal and navigate to the project folders we setup above.
* cd into the vagrant directory
* Run ``` vagrant up ``` to build the VM for the first time.
* Once it is built, run ``` vagrant ssh ``` to connect.
* cd into the correct project directory: ``` cd /vagrant/log-analysis ```

#### Load the data into the database:
* Load the data using the following command: ``` psql -d news -f newsdata.sql ```


## Run The Project Already!
1. You should already have vagrant up and be connected to it. 
1. If you aren't already, cd into the correct project directory: ``` cd /vagrant/log-analysis ```
1. Run ``` python loganalysis.py ```

Generating this information will take several seconds.   

