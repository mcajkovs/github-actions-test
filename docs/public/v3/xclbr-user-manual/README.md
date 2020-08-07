# Excalibur User manual

## Excalibur

Excalibur acts as security token for passwordless authentication using your mobile phone to verify authentication factors such as Location, PIN, Fingerprint, Face ID, etc.

To start using Excalibur you need to install Excalibur mobile phone application first. Please download it from [https://getexcalibur.com/get](https://www.google.com/url?q=https://getexcalibur.com/get&sa=D&ust=1595850862589000&usg=AOvVaw2tsX8XCv5LVkj8ObnMW-V_) and proceed with 2. Registration

<img align="center" src="images/image001.png" style="margin:0 auto; display: block;">

### Excalibur login screen

Excalibur login screen is simple User Interface which core component is dynamically changing QR code.

From login screen you may:

1.  Login to your PC
2.  Self-Register into Excalibur
3.  Check Excalibur Server connection status
4.  Connect to networks or VPN adapters
5.  Switch language
6.  Switch keyboard settings
7.  Open built-in Help section for better User Experience

<img align="center" src="images/image002.png" style="margin:0 auto; display: block;">

## Registration

Registration is a process of creating a unique link between the phone (identity) and Excalibur server (company). Setting authentication factors (such as PIN, biometric factors or location) is part of a registration process.

<img align="center" src="images/image5.png" style="margin:0 auto; display: block;" width="30%">

Registration is done by self-registration from a computer with Excalibur login screen

### Self-Registration from the PC Login screen

1.  Click “Register” on your computer’s Login screen (If there is only small QR code on your computer’s screen you can always click on it to maximize the Excalibur Login screen)
2.  Fill in your username, password and click “Register”
3.  Open Excalibur phone application and scan the QR code from computer’s screen
4.  Confirm registration on your phone by clicking “Register”
5.  Continue to 2.2 Setting factors

<img align="center" src="images/image003.png" style="margin:0 auto; display: block;">

### Setting factors

As a part of a registration, you are required to set your authentication factors. You will be asked to allow device location detection.

1.  Scan your fingerprint or provide Face ID (if available)
2.  Create your PIN code which will be used to confirm actions using
    Excalibur
<p style="text-align:center;">
<img align="center" src="images/image47.png" width="30%">
<img align="center" src="images/image32.png" width="30%">
<img align="center" src="images/image62.png" width="30%"></p>

## Login

Excalibur acts as a security token for passwordless authentication.

For logging in you just:

1.  Scan the Login QR with Excalibur mobile application
2.  Confirm by providing required authentication factors (PIN, fingerprint or Face ID)
3.  Computer should log you in automatically

Excalibur enables you to do multiple types of logins:

    3.1. Online Login
    3.2. OTP Login
    3.3. Login without Phone

If there is only small QR code on your computer’s screen you can always click on it to maximize the Excalibur Login screen

<img align="center" src="images/image004.png" style="margin:0 auto; display: block;">

### Online Login

When both your computer and your phone are online Excalibur executes Online Login which after confirming authentication factors logs you in automatically

1. Scan the Login QR from the screen of your computer with Excalibur mobile phone application
2. Confirm by providing required authentication factors (PIN, Fingerprint, Face ID)
3. Computer should log you in automatically, if not:
    1. Continue to 3.1.1 Static Password, if Excalibur asks for your current password
    2. Continue to 3.1.2 Expired Password, if your password is expired and Excalibur asks for a new password
    3. Continue to 3.2 OTP Login if Excalibur generates OTP code. When PC and Token are in the same network, the token tries to send data via SSDP protocol

<img align="center" src="images/image001.png" style="margin:0 auto; display: block;">

#### Static password

During login Excalibur might ask you for your current User password. In
that case:

1.  Fill in your current User password
2.  Click the “Login” button
3.  Computer should log you in automatically

<img align="center" src="images/image005.png" style="margin:0 auto; display: block;">

#### Expired password

When your password is expired due to your company’s password policy Excalibur might ask you for the new password. In that case:

1.  Fill in your current User password
2.  Fill in your new User password
3.  Confirm by clicking the “Change” button
4.  Computer should log you in automatically

<img align="center" src="images/image006.png" style="margin:0 auto; display: block;">

### OTP Login

When your phone or your PC is offline, the Excalibur application might generate short OTP code with expiration instead of logging you in automatically. In that case:

1.  Retype the OTP code into OTP field of your computer’s screen
2.  Confirm by pressing “ENTER” key on your keyboard or click on confirmation button

<img align="center" src="images/image007.png" style="margin:0 auto; display: block;">

### Login without Phone

When you forget your phone you might still log into the computer using Excalibur

1.  Click on “Forgotten phone” button on your computer’s login screen
2.  Fill in your username, Excalibur PIN code and the reason why you can’t use Excalibur mobile phone application to log in
3.  Confirm by clicking the “Login” button
4.  Wait for the Administrator, Service Desk operator, peer or your superior to confirm the Login
5.  Based on user’s policy, verifiers have the option to select period on theirs tokens  during which the user can logs without further verification. User just types username, PIN and the reason in this selected period.

<img align="center" src="images/image008.png" style="margin:0 auto; display: block;">

## Confirming action

When accessing services like VPN, SIP clients, or websites Excalibur might ask you for additional confirmation via notification:

1.  Verify the action that is being executed
2.  Confirm or cancel the action
3.  Provide required authentication factors (PIN, fingerprint or Face ID)

<p style="text-align:center;">
<img align="center" src="images/image054.png" width="30%">
<img align="center" src="images/image029.png" width="30%">
<img align="center" src="images/image063.png" width="30%">
</p>

## Phone application 

<img align="center" src="images/image009.png" width="30%" style="margin:0 auto; display: block;">

Excalibur application lets you log into computers and confirm actions without password just by using authentication factors

Application entry point is map screen with phone’s current location and list of active sessions. In case of no active sessions, QR scanner is started automatically.

### Main Application Menu:

![](images/image16.png)History - detailed list of all authenticated sessions (5.2)

![](images/image24.png)Scanner - scanner for all supported QRs (login, register, …)

![](images/image3.png)Settings - list of all registered companies (identities) with appropriate actions (5.3)

### Session termination (lock/logout)

Excalibur always shows you all your active sessions and enables you to lock / logout them even if you are away from the computer

For the lock/logout just:

1.  Choose the session from session list
2.  Click on <img align="center" src="images/image6.png" width="15px"> button
3.  Select “Lock” or “Logout”

<p style="text-align:center;">
<img align="center" src="images/image25.png" width="30%">
<img align="center" src="images/image40.png" width="30%">
<img align="center" src="images/image28.png" width="30%">
</p>
For the unlock/logout just:

4.  Choose the session from session list
5.  Click on <img align="center" src="images/image6.png" width="15px"> button
6.  Select “Unlock” or “Logout”


Unlock option is only available at the location of last performed login. In case that User changed location, he / she has to scan the QR code again to be able to log in.

### Sessions history

<img align="center" src="images/image07.png" width="30%" style="margin:0 auto; display: block;">

Excalibur lets you inspect your session history

1.  Click on the Session History button on the left side of bottom panel <img align="center" src="images/image16.png" width="24px%">
2.  Scroll through your session history or change the month
3.  Select specific session to see it on map and see session details

### Reset PIN

When you want to change your PIN code simply:

1.  Click on application settings <img align="center" src="images/image3.png" width="24px">
2.  Click on “Reset PIN”
3.  Confirm by providing required authentication factors (PIN, fingerprint, Face ID)
4.  Enter your new PIN code

<p style="text-align:center;">
<img align="center" src="images/image30.png" width="30%">
<img align="center" src="images/image38.png" width="30%">
<img align="center" src="images/image21.png" width="30%"></p>
<p style="text-align:center;">
<img align="center" src="images/image59.png" width="30%"> 
</p>

If it is necessary to reset PIN, then it is also necessary to provide all required verification’s factors /Fingerprint or FaceID/ and PIN. In some cases both factors can be required.

### Show password

Excalibur application provides to display your password on your registered phone. This option can be enabled or disabled by company's security policies.

1.  Click on application settings <img align="center" src="images/image3.png" width="24px">
2.  Click on your company
3.  Click on your account
4.  Select “Show password”
5.  Provide authentication factors

<p style="text-align:center;">
<img align="center" src="images/image30.png" width="30%">
<img align="center" src="images/image22.png" width="30%">
<img align="center" src="images/image14.png" width="30%">
</p>
<p style="text-align:center;">
<img align="center" src="images/image20.png" width="30%">
<img align="center" src="images/image36.png" width="30%">
</p>

### Home locations

To allow work from home scenarios it is possible to set home locations for login to PC Client. By default, Security policy doesnot allow Set location. 

Add Locations

1.  Click on application settings <img align="center" src="images/image3.png" width="24px">        
2.  Select “Home geofences”.
3.  Search your address using “Search address” bar, search result will be displayed on the map.
4.  Tap on selected place and confirm by “Add geofence”.
5.  Provide required factors

<p style="text-align:center;">
<img align="center" src="images/image58.png" width="30%">
<img align="center" src="images/image52.png" width="30%">
<img align="center" src="images/image53.png" width="30%">
</p>

 Remove Locations

1.  Navigate to “Home geofences”.
2.  Select location which you want to delete and click on it.
3.  For confirm click on “Remove geofence”

If company's policy limits the number of defined Home geofences and the user tries to define more than allowed a warning will be displayed.
<p style="text-align:center;">
<img align="center" src="images/image11.png" width="30%">
<img align="center" src="images/image39.png" width="30%">
<img align="center" src="images/image23.png" width="30%">
</p>

### Report a problem

If you have any problem with Excalibur application, you have an option to send report with problem

1.  Click on application settings <img align="center" src="images/image3.png" width="24px"> button
2.  Scroll screen
3.  Click on “Report a problem”
4.  Type  your email if you want to be contacted by developer
5.  Describe your problem and send report with “Send” button at right top.
6.  To send a report, "Usage & Diagnostics" has to be enabled.  If not, application asks you to allow it. 

<p style="text-align:center;">
<img align="center" src="images/image19.png" width="30%">
<img align="center" src="images/image50.png" width="30%">
<img align="center" src="images/image050.png" width="30%">
</p>

### Usage & Diagnostics

If some eroor occurred, applications allows to sent Token's logs to vedndor.

1.  Click on application settings <img align="center" src="images/image3.png" width="24px"> button
2.  Click on "Usage & Diagnostics" and enable it

<p style="text-align:center;">
<img align="center" src="images/image051.png" width="30%">
<img align="center" src="images/image052.png" width="30%">
<img align="center" src="images/image30.png" width="30%">
</p>

### Map Theme

Since version 3.2.7, Excalibur application provides option to set the colour of Map theme on main screen of application and colour of Map on Home geofences.

1.  Click on application settings <img align="center" src="images/image3.png" width="24px">
2.  Click on Map Theme
3.  Select required theme

<p style="text-align:center;">
<img align="center" src="images/image42.png" width="30%">
<img align="center" src="images/image30.png" width="30%">
<img align="center" src="images/image66.png" width="30%"></p>
<p style="text-align:center;">
<img align="center" src="images/image43.png" width="30%">
<img align="center" src="images/image61.png" width="30%">
</p>

### Run on background & Vibration

Excalibur application provides option to disable / enable Run on background and Vibrations. By default, these settings are enabled.

Run on background

1.  Click on application settings <img align="center" src="images/image3.png" width="24px">
2.  Click on “Background running” button
3.  Click on Disable

<p style="text-align:center;">
<img align="center" src="images/image30.png" width="30%">
<img align="center" src="images/image13.png" width="30%">
<img align="center" src="images/image68.png" width="30%"></p>


Vibrations

1.  Click on application settings <img align="center" src="images/image3.png" width="24px">
2.  Click on “Vibration” button

Note: Run on background improves better app speed when launches. App doesn’t collect any data on background.

<p style="text-align:center;">
<img align="center" src="images/image30.png" width="30%">
<img align="center" src="images/image46.png" width="30%">
</p>

### Termination of App

To close application follow steps

1.  Click on application settings <img align="center" src="images/image3.png" width="24px"> and scroll down
2.  Click on “Exit App” button
3.  Confirm Exit

<p style="text-align:center;">
<img align="center" src="images/image27.png" width="30%">
<img align="center" src="images/image10.png" width="30%">
<img align="center" src="images/image31.png" width="30%"></p>

## Verifying co-workers

When you need to verify your co-worker e.g. in case of PIN reset or login:

1.  Scan the QR code generated by your co-worker
2.  Verify his identity, executed action and click “Verify”
3.  Confirm by providing required authentication factors (PIN,
    fingerprint, Face ID)

<p style="text-align:center;">
<img align="center" src="images/image010.png" width="30%">
<img align="center" src="images/image011.png" width="30%">
<img align="center" src="images/image012.png" width="30%"></p>

PIN verification was successful.

### Peer verification

Peer verification is special type of action when two peers confirm action of theirs colleague and can be used for each action of Excalibur.