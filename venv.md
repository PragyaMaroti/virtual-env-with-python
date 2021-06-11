A virtual environment is a tool that helps to keep dependencies required by different projects separate by creating isolated python virtual environments for them.  

__Why virtual environment?__  
magine a scenario where you are working on two web based python projects and one of them uses a Django 1.9 and the other uses Django 1.10 and so on. In such situations virtual environment can be really useful to maintain dependencies of both the projects  
__Where to use virtual environment?__  
By default, every project on your system will use these same directories to store and retrieve site packages (third party libraries).  
Python since it can’t differentiate between versions in the “site-packages” directory. So both v1.9 and v1.10 would reside in the same directory with the same name. To solve this problem, we just need to create two separate virtual environments for both the projects.  
To solve this problem, we just need to create two separate virtual environments for both the projects.  
We use a module named virtualenv which is a tool to create isolated Python environments. virtualenv creates a folder which contains all the necessary executables to use the packages that a Python project would need.

#### commands to install virtual environment:
pip install virtualenv

__to check the version:  virtualenv -- version__

__to create a virtual environment:__  virtualenv name    
After running this command, a directory named my_name will be created. This is the directory which contains all the necessary executables to use the packages that a Python project would need.
If you want to specify Python interpreter of your choice, for example Python 3, it can be done using the following command:
virtualenv -p /usr/bin/python3 virtualenv_name  
To create a Python 2.7 virtual environment, use the following command:  

$ virtualenv -p /usr/bin/python2.7 virtualenv_name  

After creating virtual environment, you need to activate it. Remember to activate the relevant virtual environment every time you work on the project.
Command for activation:  source virtualenv_name/bin/activate  
Now you can install dependencies related to the project in this virtual environment.

Once you are done with the work, you can deactivate the virtual environment by the following command:

(virtualenv_name)$ deactivate  


### steps with python 3:(3.8)
- have python installed
- have pip installed
- pip install virtualenv
- cd (the folder where virtual env has to be created)
- virtualenv _name of the virtual env to be given_ . Ex : virtaulenc venv    (a folder name venv will be created in the location, containing a set of files likw scripts etc)
- venv\Scripts\activate ( then it looks like: (venv) C:\Users\PRAGY\Desktop\rasa project>  (depending on your addresses)) . The virtual env is now active.

Python virtual env documentation link: https://docs.python.org/3/library/venv.html

