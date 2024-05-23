# File-Management-SystemVersion2
<h2>File Management System project with React,Websockets, Java Spring and PostgreSQL</h2>

This project is designed to create a comprehensive file management system integrating React for the frontend, Java Spring for the backend, and PostgreSQL for the database. The system features authentication through Google login or a conventional form. In addition, the system will have two types of users: normal users and administrators.

<h3>System functionalities:</h3>

<h4>Authentication:</h4>
Login via Google</br>
Login via conventional form

<h4>Types of users:</h4>
 Normal user</br>
 Administrator

 <h4>Operations:</h4>
  Uploading .zip files only</br>
  File download capability </br>
  Normal users can delete their own files</br>
  Administrators have the authority to : </br>
     ...Delete any file </br>
     ...Delete normal users</br>
     ...View user information</br>

  <h4>Technologies used:</h4>
   Frontend: React</br>
   Backend: Java Spring</br>
   Database: PostgreSQL</br>
   Security: JSON Web Token </br>
   WebSockets</b>

   <h4>Real-Time Notifications:</h4>
WebSocket Notifications : The site is updated in real-time whenever there are changes, such as when a user adds or deletes a file. Notifications are sent to all connected users to reflect the latest state of the file system.

<h4>How to Use the Project:</h4>

1. Database Configuration:
Configure the PostgreSQL database according to the settings in the application.properties file.</br>

Example using Docker

    sudo docker run -d -p 5000:5432 -e POSTGRES_DB=filesApi -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=postgres --name files-api-db postgres:latest

2. Backend Server:
Ensure that the Java Spring environment is correctly set up and start the backend server.

3. Frontend Server: Start the frontend server.

4. Accessing the System: Access the system via your browser using the address

       http://localhost:3000


</br>
By integrating WebSockets, users will experience real-time updates without needing to refresh the page, making the file management system more dynamic and interactive.

</br>
<h4>Reminder: Create a Project in Google Cloud Console</h4>

 It's essential to create a project in the Google Cloud Console. Follow these steps:

    Visit Google Cloud Console:
        Go to Google Cloud Console and sign in with your Google account.

    Create a New Project:
        Click on the project drop-down menu at the top of the screen.
        Select "New Project" and enter a project name.
        Click "Create" to create the project.

    Enable APIs:
        In the newly created project, navigate to "APIs & Services" > "Library".
        Search for the APIs you need (e.g., Google Sign-In API) and enable them.

    Set Up OAuth Consent Screen:
        Navigate to "APIs & Services" > "OAuth consent screen".
        Configure the necessary details for your application, such as application name and authorized domains.

    Create OAuth Client ID:
        Still in "APIs & Services", go to "Credentials".
        Click on "Create credentials" and select "OAuth client ID".
        Choose the application type, configure the redirect URI, and click "Create".

    Store Credentials Securely:
        Ensure that you securely store the OAuth client ID and client secret. These will be used in your application's configuration.
