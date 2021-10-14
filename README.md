# Student Information

This is a command-line-interface application designed for a user to access their Student Information System, add/delete or update&display the Information. This project has been designed for educational purposes and uses the Code Institutes mock terminal to run.

[Live application here.](https://student--information.herokuapp.com/)
<img src= "assets/Capture of media.PNG">

## How is working the system

1. A person's whole name, including their first name and surname, and often any middle names.
2. Roll numbers are unique identification numbers that can be assigned to students at the time of admission or after admission.
3. ADDRESS - a place where a person or organization may be communicated with.
4. An email address identifies an email box to which messages are delivered. ... An email address, such as john.smith@example.com, is made up from a local-part, the symbol @, and a domain, which may be a domain name or an IP address enclosed in brackets.
5. The length of time that a person has lived or a thing has existed.
6. A series of numbers which you use to call a particular telephone
7. The group of students which attends a specific course or lesson at a university, school, or other educational institution.


# Features

The features included in this programme are listed in the main menu and they can be seen below:

<img src= "assets/Capture of main menu.PNG">

---

## Add Student Information:

- From the main menu there is an option to Add Student Information.
- Press 1 to choose this option.
- Once the user has selected this option, they are then asked to input a value for Student Name, Roll Number, Age, Class, Email, Address, Mobile Number.
- Once all fields have been entered the Student is saved.

<img src= "assets/Capture of add.PNG">
 
---

## Delete Student Information:

- From the main menu there is an option to Delete Student Information.
- Press 2 to choose this option.
- Once the user has selected this option, they are then asked to input a value for Roll Number.

<img src= "assets/Capture of delete.PNG">

---

## Update Student Information:

- From the main menu there is an option to Update Student Information.
- Press 3 to choose this option.
- Once the user has selected this option, they are then asked to input a value for Name, Roll Number, Age, Mobile NR, Address, Email, Class.

<img src= "assets/Capture of update.PNG">

--- 

## Display Student Information:

- From the main menu there is an option to Display Student Information.
- Press 4 to choose this option.
- Once the user has selected this option, they will show the Information Student.

<img src= "assets/Capture of display.PNG">

--- 

## Exit System
- From the main menu there is an option to Exit Student Information.
- Press 5 to choose this option.
- Once the use has selected this option, they will Exit your system.

<img src= "assets/Capture of exit.PNG">

---

# Technologies Used

I have used several technologies that have enabled this design to work:

- [Python](https://www.python.org/)
    - Python is the core programming language used to write all of the code in this application to make it fully functional.
    - In addition to core Python I have used the following Python modules:
        - [Gspread](https://docs.gspread.org/en/latest/)
            - Used to access my google sheets document throughout the application, to access and edit data.
        - [Google Auth](https://google-auth.readthedocs.io/en/master/)
            - Used to provide access to the application to interact with my google sheet.
        - [pyinputplus](https://pyinputplus.readthedocs.io/en/latest/)
            - Used to validate all of the user inputs.
- [GitHub](https://github.com/)
    - Used to store code for the project after being pushed.
- [Git](https://git-scm.com/)
    - Used for version control by utilising the Gitpod terminal to commit to Git and Push to GitHub.
- [Gitpod](https://www.gitpod.io/)
    - Used as the development environment.
- [Heroku](https://dashboard.heroku.com/apps)
    - Used to deploy my application.
- [Grammarly](https://www.grammarly.com/)
    - Used to fix the thousands of grammar errors across the project.
- [Google Sheets](https://www.google.co.uk/sheets/about/)
    - Used to store the 'Contacts' data used for the application.
- [Pep8](http://pep8online.com/)
    - Used to test my code for any issues or errors.


# Testing

In addition to my own testing of the programme I passed my code through the [Pep8](http://pep8online.com/checkresult) online validator which passed through with 0 issues:
---
<img src="assets/Capture of validator.PNG">
---


# Bugs

## Solved bugs
- When I wrote "import gspread" I forget to give the command on the terminal "pip3 install gspread google-auth".

## Remaining bugs
- Show the  infos problems.


# Deployment

The master branch of this repository has been used for the deployed version of this application.

## Using Github & Gitpod

To deploy my command-line interface application, I had to use the [Code Institute Python Essentials Template](https://github.com/Code-Institute-Org/python-essentials-template), as this enables the application to be properly viewed on Heroku using a mock terminal. 

- Click the `Use This Template` button.
- Add a repository name and brief description.
- Click the `Create Repository from Template` to create your repository.
- To create a Gitpod workspace you then need to click `Gitpod`, this can take a few minutes.
- When you want to work on the project it is best to open the workspace from Gitpod (rather than Github) as this will open your previous workspace rather than creating a new one. You should pin the workspace so that it isn't deleted.
-  Committing your work should be done often and should have clear/explanatory messages, use the following commands to make your commits:
    - `git add .`: adds all modified files to a staging area
    - `git commit -m "A message explaining your commit"`: commits all changes to a local repository.
    - `git push`: pushes all your committed changes to your Github repository.

*Forking the GitHub Repository*

If you want to make changes to your repository without affecting it, you can make a copy of it by 'Forking' it. This ensures your original repository remains unchanged.

1. Find the relevant GitHub repository
2. In the top right corner of the page, click the Fork button (under your account)
3. Your repository has now been 'Forked' and you have a copy to work on

*Cloning the GitHub Repository*

Cloning your repository will allow you to download a local version of the repository to be worked on. Cloning can also be a great way to backup your work.

1. Find the relevant GitHub repository
2. Press the arrow on the Code button
3. Copy the link that is shown in the drop-down
4. Now open Gitpod & select the directory location where you would like the clone created
5. In the terminal type 'git clone' & then paste the link you copied in GitHub
6. Press enter and your local clone will be created.

## Creating an Application with Heroku

I followed the below steps using the Code Institute tutorial:

- The following command in the Gitpod CLI will create the relevant files needed for Heroku to install your project dependencies `pip3 freeze --local > requirements.txt`. Please note this file should be added to a .gitignore file to prevent the file from being committed.

1. Go to [Heroku.com](https://dashboard.heroku.com/apps) and log in; if you do not already have an account then you will need to create one.
2. Click the `New` dropdown and select `Create New App`.
3. Enter a name for your new project, all Heroku apps need to have a unique name, you will be prompted if you need to change it.
4. Select the region you are working in.

*Heroku Settings*
You will need to set your Environment Variables - this is a key step to ensuring your application is deployed properly.
- In the Settings tab, click on `Reveal Config Vars` and set the following variables:
    - If using credentials you will need to add the credentials as a variable, the key is the name 'CREDS' and the value is the contents of your creds JSON
    - Add key: `PORT` & value `8000`
- Buildpacks are also required for proper deployment, simply click `Add buildpack` and search for the ones that you require.
    - For this project, I needed to add `Python` and `Node.js`, in this order.

*Heroku Deployment*
In the Deploy tab:
1. Connect your Heroku account to your Github Repository following these steps:
    1. Click on the `Deploy` tab and choose `Github-Connect to Github`.
    2. Enter the GitHub repository name and click on `Search`.
    3. Choose the correct repository for your application and click on `Connect`.
2. You can then choose to deploy the project manually or automatically, automatic deployment will generate a new application every time you push a change to Github, whereas manual deployment requires you to push the `Deploy Branch` button whenever you want a change made.
3. Once you have chosen your deployment method and have clicked `Deploy Branch` your application will be built and you should see the below `View` button, click this to open your application:

<img src="assets/Capture of heroko.PNG">

---
# Credits

All of this code has been written by me, I have used [Stack Overflow](https://stackoverflow.com/) , `Gspread` and `Slack` to help my code and fix any issues that I had.

[Zfill method help](https://www.w3schools.com/python/ref_string_zfill.asp)



# Acknowledgements
I would like to thank my mentor Adegbenga Adeye and the slack community for their great advice, tips and the code review.