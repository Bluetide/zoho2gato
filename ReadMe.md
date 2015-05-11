#Zoho Fiscal
This applications retrieves invoices from Zoho and create independent JSON's for each invoice in the required input format for GatoMalo.

#Dependencies
This application is written in python3 and requires:

- Uses flask as the web server
- Requests (pip3 install requests)

#notas
- se utiliza el precio total de cada item para generar el json de gatomalo porque no hay forma de aplicar el descuento correctamente en gatomalo. Por eso se usa en cantidad siempre "1". 

If you are on Mac OS X or Linux, chances are that one of the following two commands will work for you:

$ sudo easy_install virtualenv
or even better:

$ sudo pip install virtualenv
One of these will probably install virtualenv on your system. Maybe it’s even in your package manager. If you use Ubuntu, try:

$ sudo apt-get install python-virtualenv
If you are on Windows and don’t have the easy_install command, you must install it first. Check the pip and distribute on Windows section for more information about how to do that. Once you have it installed, run the same commands as above, but without the sudo prefix.

Once you have virtualenv installed, just fire up a shell and create your own environment. I usually create a project folder and a venv folder within:

$ mkdir myproject
$ cd myproject
$ virtualenv venv
New python executable in venv/bin/python
Installing distribute............done.
Now, whenever you want to work on a project, you only have to activate the corresponding environment. On OS X and Linux, do the following:

$ . venv/bin/activate
If you are a Windows user, the following command is for you:

$ venv\scripts\activate
Either way, you should now be using your virtualenv (notice how the prompt of your shell has changed to show the active environment).

Now you can just enter the following command to get Flask activated in your virtualenv:

$ pip install Flask
A few seconds later and you are good to go.
