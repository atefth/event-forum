##Instructions for setting up a Rails5 project

###Dependency Requirements for Windows
1. Ruby Installer (Version 2.2.5)  

	First, we need to install the Ruby programming language and we'll use the Ruby Installer available at [rubyinstaller.org](https://rubyinstaller.org/downloads/). Follow the steps below:

	  1. Download and run the [Ruby Installer](http://dl.bintray.com/oneclick/rubyinstaller/rubyinstaller-2.2.5.exe). An installation wizard will open:  
	    1. Check **Add Ruby executables to your PATH**
	    2. Click *Install*.  
	    3. Click *Finish* when installation completed.  
	  2. Verify the installation:  
	    1. Go to the *Windows menu* and click **All Programs**.  
	    2. Scroll down to *Ruby* and click **Start Command Prompt with Ruby**. A command prompt terminal will open.  
	    3. Type `ruby -v` and press Enter and you should see the Ruby version number that you installed.

2. Ruby Development Kit

	This kit contains additional **build tools** required by Rails that Windows doesn't have by default. Follow the steps below:

	1. Download and run the [Ruby Development Kit Installer](http://dl.bintray.com/oneclick/rubyinstaller/DevKit-mingw64-32-4.7.2-20130224-1151-sfx.exe). An Installation wizard will open: 
	  2. Specify a folder to install the Development Kit. *Recommended installation directory*: **C:\RubyDevKit**.
	2. Add the development kit to ruby:  
	  1. **Start Command Prompt with Ruby**.  
	  2. Type `cd C:\RubyDevKit` to change your directory to the development kit installation directory.  
	  3. Type `ruby dk.rb init` to run the initialization script for the development kit setup.  
		4. Type `ruby dk.rb install` to add the development kit to our Ruby installation.  

3. Rails

	Rails is a ruby *gem*. A gem is essentially a **library** that can be downloaded and installed using the *gem* tool included in the development kit. Follow the steps below:

	1. **Start Command Prompt with Ruby**. 
	2. Type `gem install rails --version 5.2.0`.  
	3. Type `rails --version` to verify the installation.

4. Node.js

	Rails require a **JavaScript runtime** for some of it's dependencies and **Node.js** provides us with just that. Follow the steps:

	1. Download and run the [Node.js Installer](https://nodejs.org/dist/v8.11.2/node-v8.11.2-x86.msi).  
	2. Accept the terms.  
	3. Keep the default settings and click next through the entire wizard.  
	4. Click **Yes** when Windows asks to grant permission to the app.  
	5. Restart your computer.  

###Initializing a new Rails project
1. **Start Command Prompt with Ruby**.  
2. Change directory to your work directory, eg: `cd D:\Work`.  
3. Type `rails new event-forum` to **create** a new rails project.  
4. Type `cd event-form`.  
4. Type `rails s` to run the rails **server**.  
5. Go to the [local server](http://localhost:3000) to view the default Rails Welcome Page.
6. Press `Ctrl+c` to **terminate** the rails server.  