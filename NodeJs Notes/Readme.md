
Node.js is an open source server environment
Node.js is free
Node.js runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
Node.js uses JavaScript on the server


Common use for the File System module:
    - Read files
    - Create files
    - Update files
    - Delete files
    - Rename files

Read Files----------
The fs.readFile() method is used to read files on your computer.

Create Files---------
The File System module has methods for creating new files:
fs.appendFile()
fs.open()
fs.writeFile()
- The fs.appendFile() method appends specified content to a file. If the file does not exist, the file will be created.
- The fs.open() method takes a "flag" as the second argument, if the flag is "w" for "writing", the specified file is opened for writing. If the file does not exist, an empty file is created.
- The fs.writeFile() method replaces the specified file and content if it exists. If the file does not exist, a new file, containing the specified content, will be created.

Update Files---------
The File System module has methods for updating files:
fs.appendFile()
fs.writeFile()
- The fs.appendFile() method appends the specified content at the end of the specified file.
- The fs.writeFile() method replaces the specified file and content.

Delete Files---------
To delete a file with the File System module,  use the fs.unlink() method.
- The fs.unlink() method deletes the specified file.

Rename Files----------
To rename a file with the File System module,  use the fs.rename() method.
The fs.rename() method renames the specified file.


URL Module------------->>>>>>>>>>>>>>>>>>>>>>>>>>>
The Built-in URL Module---------
- The URL module splits up a web address into readable parts.

    To include the URL module, use the require() method.

    Parse an address with the url.parse() method, and it will return a URL object with each part of the address as properties

    Node.js File Server
        - Now we know how to parse the query string, and in the previous chapter we learned how to make Node.js behave as a file server. Let us combine the two, and serve the file requested by the client.


NPM----------------------->>>>>>>>>>>>>>>>>>>>>>>>>>>>>
NPM is a package manager for Node.js packages, or modules if you like.
www.npmjs.com hosts thousands of free packages to download and use.
The NPM program is installed on your computer when you install Node.js

What is a Package?
    - A package in Node.js contains all the files you need for a module.
    - Modules are JavaScript libraries you can include in your project.

Download a Package
    - Downloading a package is very easy.
    - Open the command line interface and tell NPM to download the package you want.
    - I want to download a package called "upper-case"
    - NPM creates a folder named "node_modules", where the package will be placed. All packages you install in the future will be placed in this folder.

Using a Package
    - Once the package is installed, it is ready to use.
    - Include the "upper-case" package the same way you include any other module

Events in Node.js------------------>>>>>>>>>>>>>>>>>>>>>>>>
    - Node.js is perfect for event-driven applications.
    - Every action on a computer is an event. Like when a connection is made or a file is opened.
    - Objects in Node.js can fire events, like the readStream object fires events when opening and closing a file.

Events Module------------------>>>>>>>>>>>>
    - Node.js has a built-in module, called "Events", where you can create-, fire-, and listen for- your own events.
    - To include the built-in Events module use the require() method. In addition, all event properties and methods are an instance of an EventEmitter object. To be able to access these properties and methods, create an EventEmitter object.

The EventEmitter Object
    - You can assign event handlers to your own events with the EventEmitter object.
    - In the example below we have created a function that will be executed when a "scream" event is fired.
    - To fire an event, use the emit() method.

Upload Files---------------->>>>>>>>>>>>>>>>>>>>>>
The Formidable Module-----------
    - There is a very good module for working with file uploads, called "Formidable".
    - The Formidable module can be downloaded and installed using NPM.
    - After you have downloaded the Formidable module, you can include the module in any application.

    Upload Files----
    - Now you are ready to make a web page in Node.js that lets the user upload files to your computer

    - Step 1: Create an Upload Form
        Create a Node.js file that writes an HTML form, with an upload field
    - Step 2: Parse the Uploaded File
        Include the Formidable module to be able to parse the uploaded file once it reaches the server.

        When the file is uploaded and parsed, it gets placed on a temporary folder on your computer.
    - Step 3: Save the File
        When a file is successfully uploaded to the server, it is placed on a temporary folder.

        The path to this directory can be found in the "files" object, passed as the third argument in the parse() method's callback function.

        To move the file to the folder of your choice, use the File System module, and rename the file.

Send an Email----------------->>>>>>>>>>>>>>>>>>>>>>
The Nodemailer Module----------
    - The Nodemailer module makes it easy to send emails from your computer.
    - The Nodemailer module can be downloaded and installed using npm.
    - After you have downloaded the Nodemailer module, you can include the module in any application

Send an Email
    - Now you are ready to send emails from your server.
    - Use the username and password from your selected email provider to send an email. This tutorial will show you how to use your Gmail account to send an email.
    - And that's it! Now your server is able to send emails.

Multiple Receivers
    - To send an email to more than one receiver, add them to the "to" property of the mailOptions object, separated by commas.

Send HTML
    - To send HTML formatted text in your email, use the "html" property instead of the "text" property
