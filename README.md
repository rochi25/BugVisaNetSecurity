# BugVisaNetSecurity

<h3>Working on a specific task, I found a security bug while trying to log in to the Visa Net website.</h3><br>

When you fill "Contraseña" with an invalid data, the website show an alert that say "Su contraseña es incorrecta". This message is dangerous !<br>

The message should be generic like "Su usuario o contraseña es incorrecto". <br>

If the message say that de password is incorrect, it´s like say, Hey!, hackeen my account!

<h3>Bug Report:<br></h3>
<p>
<b>Summary:</b> Error message not recommended.<br>
<p>
<b>Precondition:</b> The user has a VisaNet account and is on the index  https://acceso.vnet.uy/index.php/apps/user_saml/saml/selectUserBackEnd?redirectUrl=/index.php/apps/files/?dir%3D/%26fileid%3D73982 to login. <br>

<b>Steps to reproduce:</b>
1.	Click on “Ingresar” button.
2.	Fill “Correo electrónico” with a valid e-mail.
3.	Fill “Contraseña” with an invalid value.
4.	Click on “Iniciar sesión” button.<br>
<p>
<b>Expected Result:</b> The website should show an alert like " la contraseña o usuario es incorrecto".<br>
<p>  
<b>Actual Result:</b> The alert reveals that the wrong data is the password..<br>
<p>  
<b>Info. adicional:</b> Firefox Versión 94.0.2 (64-bit). Windows 7 Professional.<br>
<p>  
<b>Severidad:</b> Medium<br>
<b>Prioridad:</b> Critic <br>


Here is the evidence:

![image](https://user-images.githubusercontent.com/88468127/144684621-a0b5ae0f-46ef-46dd-a097-6b5a8764bde7.png)
