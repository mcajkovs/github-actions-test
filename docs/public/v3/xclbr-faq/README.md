# Excalibur Enterprise - FAQ

<!-- vscode-markdown-toc -->
1. [Introduction](#Introduction)
	1.1. [What is Excalibur and what is it for?](#WhatisExcaliburandwhatisitfor)
	1.2. [What is an authentication factor?](#Whatisanauthenticationfactor)
	1.3. [What is OTP?](#WhatisOTP)
	1.4. [What can Excalibur authenticate?](#WhatcanExcaliburauthenticate)
2. [Installation](#Installation)
	2.1. [What do I need to start using Excalibur?](#WhatdoIneedtostartusingExcalibur)
	2.2. [How do I know whether my company supports Excalibur login?](#HowdoIknowwhethermycompanysupportsExcaliburlogin)
	2.3. [How do I know if I have Excalibur installed on my computer / phone?](#HowdoIknowifIhaveExcaliburinstalledonmycomputerphone)
	2.4. [How do I install Excalibur on my smartphone?](#HowdoIinstallExcaliburonmysmartphone)
	2.5. [How do I install Excalibur to my computer?](#HowdoIinstallExcaliburtomycomputer)
3. [Usage](#Usage)
	3.1. [How do I register?](#HowdoIregister)
	3.2. [How do I log into a computer, web, or RDP?](#HowdoIlogintoacomputerweborRDP)
	3.3. [How do I log in without an internet connection?](#HowdoIloginwithoutaninternetconnection)
	3.4. [How do I log out / lock a computer?](#HowdoIlogoutlockacomputer)
	3.5. [How do I change a computer password?](#HowdoIchangeacomputerpassword)
	3.6. [How do I change my PIN or another factor?](#HowdoIchangemyPINoranotherfactor)
	3.7. [What to do if I forgot my phone and I need to login?](#WhattodoifIforgotmyphoneandIneedtologin)
	3.8. [What to do if I lost / factory reset my phone?](#WhattodoifIlostfactoryresetmyphone)
	3.9. [What is an Excalibur Dashboard?](#WhatisanExcaliburDashboard)
	3.10. [How to change language in application?](#Howtochangelanguageinapplication)
	3.11. [Does the application collect data on background?](#Doestheapplicationcollectdataonbackground)
	3.12. [What “Run in the background” mean?](#WhatRuninthebackgroundmean)
	3.13. [What to do when Excalibur CPUI was not loaded properly?](#WhattodowhenExcaliburCPUIwasnotloadedproperly)
	3.14. [What is the Excalibur PAM?](#WhatistheExcaliburPAM)
	3.15. [Are Excalibur PAM sessions recorded?](#AreExcaliburPAMsessionsrecorded)
	3.16. [Can I transfer files via PAM?](#CanItransferfilesviaPAM)
	3.17. [Facade runs but doesn’t connect](#Facaderunsbutdoesntconnect)
4. [Further materials](#Furthermaterials)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

##  1. <a name='Introduction'></a>Introduction

###  1.1. <a name='WhatisExcaliburandwhatisitfor'></a>What is Excalibur and what is it for? 

Excalibur replaces passwords with your smartphone. Thus it becomes your universal digital key that allows a simple, but strong Multi-factor authentication and authorization of events in your company’s existing IT infrastructure.

###  1.2. <a name='Whatisanauthenticationfactor'></a>What is an authentication factor? 

The aim of Multi-factor authentication is to clearly verify an identity of a user by means of various mutually independent information (factors) that identifies a user. These information are called authentication factors and their best-known examples are e.g. password or PIN. There are several **types of authentication** factors, usually divided by means and form of user identification, and these are:

- **Knowledge factors** (something only a user knows) - password, PIN, pattern lock, and so on.
- **Possession factors** (something only a user owns) - smartphone, phone number, smart card / credit card, USB token, MAC address of a device and so on.
- **Inherence factors** (or also identity factors - who a user is, or simply biometrics) - fingerprint, iris, facial features, voice features and so on.
- **Contextual factors** (what and how is a current user environment) - proximity, geographic location, time, date, the day of the week, IP address and mask, and so on.

Excalibur can combine all kinds of factors and thus provide **Massive Multi-factor Authentication (MMFA), or simply - Multi-factor authentication**, conveniently via a smartphone application. **Excalibur currently supports the following factors**: PIN, fingerprint, facial recognition, geolocation, smartphone verification, time and day of the week and IP address of your computer and phone.

**Your administrator might optionally combine authentication factors into security policy rules** that could be specific to each operation, as well as organizational units, and even individual users and systems in which Excalibur is used. Because administrator might change the rules of security policies at any time, always follow the instructions during the login process in the Excalibur mobile application. If there will be some new authentication factors added to the security policy rules, on the next login you will be firstly prompted to set the new factors and from then on, you will use them for verification.

###  1.3. <a name='WhatisOTP'></a>What is OTP?

**One-Time Password (OTP)** is single-use (pseudo) random password or code. Uniqueness and validity of an OTP for a single operation are properties that address corresponding problems of static passwords (their immutability among numerous verifications). For additional security, OTPs might be further restricted - e.g. linked to specific operation details or to have a short expiration (validity) span. Therefore, OTPs in various forms are often utilized as an additional identity verification measure (authentication factor). Excalibur utilizes OTP principle and properties for 2 different purposes:

-   **offline login**, in which case a short expiration OTP is issued to a successfully authenticated user for offline login using Excalibur (user enters this OTP into a full-screen Excalibur login screen).

-   **dynamic login password**, when allowed by administrator, Excalibur automatically changes the user's Active Directory (AD) password in a background after each successful domain login for a long random sequence, which Excalibur will automatically use only once and then change again for the next login. The user never comes into a contact with this random sequence - doesn’t know it, nor uses it anywhere. The same applies to the user's old password, which the user doesn’t have to remember anymore.

###  1.4. <a name='WhatcanExcaliburauthenticate'></a>What can Excalibur authenticate?

Excalibur replaces outdated authentication systems based on names and passwords, as well as systems offering impractical methods of two and Multi-factor authentication. Excalibur offers native integrations into Windows and OSX. Other systems could be integrated via standard interfaces and protocols.

**Currently**, Excalibur can be used to **log a user into Windows which is in a domain (Active Directory), into web applications through native integrations or SAML, Citrix NetScaler and Storefront, but also for authentication and authorization through RADIUS and Kerberos protocols**. All these methods require appropriate integration / installation and configuration of Excalibur components.

In addition to the above, Excalibur integrates McAfee Drive Encryption, **where Excalibur is currently the only solution that enables Multi-factor authentication for disk encryption authentication**.

##  2. <a name='Installation'></a>Installation

###  2.1. <a name='WhatdoIneedtostartusingExcalibur'></a>What do I need to start using Excalibur? 

**If you are an end-user**, to start using Excalibur you need Excalibur mobile application that you need to initialize (register) for use with Excalibur in your company. After successful initialization (registration), you can sign with Excalibur to all systems your company supports.

If you are unsure or you don’t have Excalibur mobile application installed, please see:

[How do I know if I have Excalibur installed on your computer / phone?](#HowdoIknowifIhaveExcaliburinstalledonmycomputerphone)

[How to install Excalibur on smartphone?](#HowdoIinstallExcaliburonmysmartphone)

Also, all Excalibur components must be installed and configured for you by your system administrator in all environments and applications (Windows, VPN, web applications, etc.) where you want to log in with Excalibur.

**See also**:         

[How do I know if my company supports registration through Excalibur?](#HowdoIknowwhethermycompanysupportsExcaliburlogin)

[How to register?](#HowdoIregister)

**If you are an** administrator, to use Excalibur you need to install and configure the following Excalibur components:

- **Server** - is an Excalibur component that runs within your company and is responsible for all operations Excalibur performs, from registration, authentication of operating system login, all the way to actions authorization. This component is installed and configured by a designated system administrator.

- **Client environment (client)** - is a component (a set of components or simply an integration), which is a part of infrastructure within your company that allows a variety of authentication / authorization actions by Excalibur. From an end-user perspective, it might be e.g. in case of domain login the Excalibur login screen on the user's computer.

- **Mobile application (token)** - is a component that becomes user's personal hardware token and replaces conventional hardware tokens such as a smart card / credit card, USB token, and so on. From a moment of initialization of user's identity becomes linked to a specific smartphone and stored in a secure storage of that smartphone. In case of centralized business smartphones administration via Mobile Device Management (MDM) solution, we recommend to automatically distribute this component to employees phones, so that they won’t need to install the mobile application themselves.

If you want to try or start using Excalibur, please contact us at xclbr@xclbr.com

###  2.2. <a name='HowdoIknowwhethermycompanysupportsExcaliburlogin'></a>How do I know whether my company supports Excalibur login? 

If the Excalibur client is available for you, then **in case of a domain login you should see the Excalibur login screen - either in full-screen mode** with Excalibur’s and your company’s branding instead of the standard Windows login screen - usually with a username and password (alternatively with fingerprint / SmartCard / Windows Hello login, depending on your company security policies), **or a large login QR code in  a corner of the standard Windows login screen**.

Thus, **if you can see the Excalibur login screen, your company supports Excalibur login**.

To start using Excalibur you need the Excalibur mobile application, which you'll have to initialize - register to use the Excalibur. It could be done via self-registration. If your company manages business phones centrally (remotely) using Mobile Device Management (MDM), another indication of an Excalibur support is that you can find Excalibur mobile application already automatically installed on your business phone.

If you have any doubts about the availability of the Excalibur in your company, please contact your system administrator, who can install all necessary components either locally or remotely.

**See also**:         

[How do I know if I have Excalibur installed on your computer / phone?](#HowdoIknowifIhaveExcaliburinstalledonmycomputerphone)

[How to install Excalibur on a smartphone?](#HowdoIinstallExcaliburonmysmartphone) 

[How to install Excalibur to your computer?](#HowdoIinstallExcaliburtomycomputer)

[How to register?](HowdoIregister)

###  2.3. <a name='HowdoIknowifIhaveExcaliburinstalledonmycomputerphone'></a>How do I know if I have Excalibur installed on my computer / phone?

If you have Excalibur (client) installed **on your computer**, you should see the Excalibur login screen - for more details please see: [How do I know whether my company supports Excalibur login?](#HowdoIknowwhethermycompanysupportsExcaliburlogin)

On your Windows computer, you can check installed programs, among which you should see Excalibur Enterprise. Open the Control Panel, select category Programs and then select Programs and Features. From Windows 8 above, applications could be found in Settings \> Apps, under which you can find Apps and Features as the main tab, which lists all installed applications and also offers a search. Apps could be also searched directly in the Windows Explorer search.

**On a smartphone**, you can find Excalibur among installed applications either in Settings under Apps or Applications or under Installed Apps in a respective official app store according to your platform.

**See also**:         

[How do I know if my company supports registration through Excalibur?](#HowdoIknowwhethermycompanysupportsExcaliburlogin)

[How to install Excalibur on a smartphone?](#HowdoIinstallExcaliburonmysmartphone)

[How to install Excalibur to your computer?](#HowdoIinstallExcaliburtomycomputer)

###  2.4. <a name='HowdoIinstallExcaliburonmysmartphone'></a>How do I install Excalibur on my smartphone?

Excalibur mobile application will be **installed automatically** if your company manages business phones centrally (remotely) using Mobile Device Management (MDM). Otherwise, please install it yourself **from a respective official app store for your platform** [(Android](https://www.google.com/url?q=https://play.google.com/store/apps/details?id%3Dcom.getexcalibur.enterprise&sa=D&ust=1595947385459000&usg=AOvVaw14PFF8Htgins_d3fAEHIU1) or [iOS](https://www.google.com/url?q=https://itunes.apple.com/us/app/excalibur/id914444565&sa=D&ust=1595947385460000&usg=AOvVaw3wj2UIh4y5DNXV3pPSq6Xr)), just search for application Excalibur Enterprise and install it.

The mobile application can ask for runtime permissions necessary for its proper functioning according to your company’s security policy rules, such as access to a camera (scanning the QR code), receiving a location (geolocation as an authentication factor) and so on. In the ideal scenario, it is necessary to allow these permissions only before the first execution of the operation which requires them. However, you might be prompted to allow these permissions (again) if you rejected them in the first place, withdrawn them in application settings, deleted (cleared) application data, reinstalls the application, transferred your identity to a new phone, or if a need for a new permissions from updating the application or your phone’s OS.

In addition to runtime permissions, you may be entitled to invite applications to enable some services on your phone, such as obtaining a position with high accuracy or asked to update some components such as the OS PlayServices in the case of Android OS.

**See also**:        

[How do I know if I have Excalibur installed on your computer / phone?](#HowdoIknowifIhaveExcaliburinstalledonmycomputerphone)

[How to register?](#HowdoIregister)

###  2.5. <a name='HowdoIinstallExcaliburtomycomputer'></a>How do I install Excalibur to my computer? 

Client interface (Excalibur Client) user does not install itself. If you can not see Excalibur full-screen login screen or registration QR code in the corner of the standard login screen, contact your system administrator, who can install Excalibur remotely or locally from the installation package.

**See also**:         

[How do I know if I have Excalibur installed on your computer / phone?](#HowdoIknowifIhaveExcaliburinstalledonmycomputerphone)

##  3. <a name='Usage'></a>Usage

###  3.1. <a name='HowdoIregister'></a>How do I register?

To use Excalibur in your company you need to register. By registering you pair your corporate identity with an Excalibur Enterprise mobile application in your smartphone, in other words, initialize it for use in your company. 

If you are not sure / do not have the Excalibur mobile application installed, please see:

[How do I know if I have Excalibur installed on your computer / phone?](#HowdoIknowifIhaveExcaliburinstalledonmycomputerphone)

[How to install Excalibur on a smartphone?](#HowdoIinstallExcaliburonmysmartphone)

**The registration of Excalibur** is available from the full-screen mode of the Excalibur login screen on your computer. If you see only registration QR code in the corner of the standard login screen, clicking on it will open full-screen mode. In it **to start self-registration, click on "Register" and enter your current username and password** to verify your identity. Then registration QR code appears which you need to scan with Excalibur mobile application to proceed with registration.

In the mobile application you will be asked to provide all authentication factors according to your company's security policy required for registration. After successful registration in your Excalibur mobile application, your company name will be added to the "Settings". If the connection on your phone is working and Excalibur server is available, then the connection indicator (right of the company name) should be green.

###  3.2. <a name='HowdoIlogintoacomputerweborRDP'></a>How do I log into a computer, web, or RDP? 

**For logging in a registered user, simply scan the QR code by your phone with initialized Excalibur mobile application and then provide all authentication factors** that the application will require based on company security policies for login. Verification of factors may require enabling verification related services such as permission to turn on location or position acquisition.

Your mobile application informs you about successful login. If an error occurs, click on "More info" for more information. This will open a help with a description of the error.

###  3.3. <a name='HowdoIloginwithoutaninternetconnection'></a>How do I log in without an internet connection? 

The administrator has the option to enable offline Excalibur login security policy. If you have enabled offline login and your computer or phone is having issues with an Internet connection or Internet connection is currently not available, Excalibur will allow you to **log in using offline One-Time Password (OTP)**.

Authentication begins with a standard QR code scan using Excalibur mobile application and verification of all required authentication factors. Security policy rules for offline log may (or may not) be different from those for online login - it can be multiple authentication factors or restriction when and where it is possible to perform offline login. After successful verification of authentication factors, there is a different procedure - instead of automatic login mobile application will generate **OTP** which you have **to manually rewrite to the box under QR code in Excalibur full-screen mode login screen on the computer** and press "ENTER". If you see only registration QR code in the corner of the standard login screen, clicking on it will open Excalibur full-screen mode login screen.

Offline login has several limitations. The main limitation is that the **first offline login is possible to realize only after the first successful online login**. Therefore, please try online login immediately after successful registration with a stable Internet connection of phone and computer. OTP has a limited validity and is valid only for one offline login to your account. OTP validity timer is shown in the Excalibur mobile application. In the mobile application, you will not see your current online session (connection) immediately after logging in, as is the case with online login, but only after the computer and the phone connect to the Internet and synchronize their status with company Excalibur server.

###  3.4. <a name='HowdoIlogoutlockacomputer'></a>How do I log out / lock a computer? 

Active session (login) can be locked or terminated remotely from a mobile application. **The session is created by logging in to your computer and expires by signing out or by computer shutdown**. For online login, the session on your phone appears immediately after a successful login. For offline login, session appears after your computer and phone connect and synchronize with your company Excalibur server. For a quick overview and access, your active sessions appear in the notification.

**You can lock an active session** manually from the computer Start menu. After starting your session again you can return to your work, just as you left it before locking. Ending a **session will cause logging off** from your computer, which means that your open programs will be closed and unsaved changes will be lost as well as the manual log off or shutdown from the computer Start menu.

The bottom of the Excalibur mobile application main screen displays cards with all your active and locked sessions. On the right side of each card with notification there is the icon (button) to lock or cancel the active session. Your choice will then be to confirm or cancel the confirmation dialogue. If the session is still active, the offer will be two choices - logout or lock, and if you select logout you will be asked for confirmation of this action.  

**Sessions notification (Android)** gives you quick access to your sessions - clicking on the notification will open the main application screen, from where you can control individual sessions, but also offers you to lock all sessions button directly from the notification. When choosing lock all sessions from the notification you will be redirected to the application, which then ask you to confirm this action.

###  3.5. <a name='HowdoIchangeacomputerpassword'></a>How do I change a computer password?

Excalibur can work with passwords in one of two modes - with static and dynamic password. This setting selects your system administrator.

**In the case of a static password**, your original password preserves - it will be still possible log in manually in exceptional cases. When you first log in with Excalibur and also each time you change your password, Excalibur will ask you to enter it. If your company has a security policy to have password expiration - after the period during which it must change, Excalibur asks you to set a new password.

**In the case of a dynamic password**, Excalibur takes full control over the management of your passwords and automatically changes it to a random long sequence (without user intervention) in the background which then automatically applies only the next time you log in and repeats the process. In this case, the user no longer uses his original password (user does not need to remember it anymore), the entire process is done automatically by Excalibur. Manual change of password by users or password expiration is in this case prohibited.

###  3.6. <a name='HowdoIchangemyPINoranotherfactor'></a>How do I change my PIN or another factor?

You can change your PIN or other authentication factors in the Excalibur mobile application. On the main screen, tap on "Settings" \> "Company", select the company for which you are initialized and select *"Reset PIN"*. Excalibur will ask you to enter your old (current) authentication factors according to your company security policies and it will ask for a new one after successful verification.

###  3.7. <a name='WhattodoifIforgotmyphoneandIneedtologin'></a>What to do if I forgot my phone and I need to login?

If you have forgotten your phone or for some reason, it is not available / functional, **in the full-screen mode of your Excalibur login screen, select "Forgotten phone"**. If you can see only registration QR code in the corner of the standard login screen, clicking on it will open Excalibur full-screen mode login screen. Then enter your login name, your Excalibur PIN and the reason why you can not use your phone and how long it will not be available, and then press the "Login". Your manager / administrator will be contacted and asked to confirm or reject your request. Such authorization may be one-time or allowed to login for the next hour or the whole day.

The ability to login without a mobile phone with Excalibur may be prohibited by the administrator under the company security policies.

###  3.8. <a name='WhattodoifIlostfactoryresetmyphone'></a>What to do if I lost / factory reset my phone? 

In the event of a lost or stolen phone **first contact your system administrator to disable your account** to prevented login with this phone. **Then**, as in the case of resetting the phone to factory settings, application reinstall or its data erase, **perform a new registration**. For more information on registration or how to install the Excalibur mobile application, please see:          

[How do I register?](#HowdoIregister)

[How to install Excalibur on a smartphone?](#HowdoIinstallExcaliburonmysmartphone)

As soon as you re-register (on another phone), the original registration will automatically become invalid - Excalibur will deregister (deinitialize) your original phone and  you will only be able to login with the currently registered phone. Your Excalibur identity is always bound to only currently registered phone.

###  3.9. <a name='WhatisanExcaliburDashboard'></a>What is an Excalibur Dashboard?

Excalibur Dashboard is a User management console where every User registered to Excalibur may see **his / hers own Actions and Sessions**. On the top of that Excalibur **Administrator** may use Dashboard for monitoring purposes, to view User's activity, set rules and security policies for Users, set geofences and many more.

For detailed information about Dashboard please see **Excalibur Administrator’s Dashboard Manual** or **Excalibur User’s Dashboard Manual** documents.

###  3.10. <a name='Howtochangelanguageinapplication'></a>How to change language in application?

To change language open Excalibur application and click on **settings (gear wheel icon)**. By clicking on the Language button, the settings window will open. You may change language from the list of supported languages (currently Slovak and English).

###  3.11. <a name='Doestheapplicationcollectdataonbackground'></a>Does the application collect data on background?

No. Application doesn’t execute any process to collect any data on the background. All data such as position, biometry, PIN are inserted by the user if they are required for user’s authentication. Application doesn’t store this data.

###  3.12. <a name='WhatRuninthebackgroundmean'></a>What “Run in the background” mean?

Application has an option: Running on the background. If this option is enabled, the application is launched more quickly than is disabled.  

###  3.13. <a name='WhattodowhenExcaliburCPUIwasnotloadedproperly'></a>What to do when Excalibur CPUI was not loaded properly?

In case, that Excalibur CPUI was not loaded properly from suspend, try suspend PC Client and resume it again. Excalibur CPUI should be loaded properly. If the problem with Excalibur CPUI still persists, contact the administrator please.

###  3.14. <a name='WhatistheExcaliburPAM'></a>What is the Excalibur PAM? 

Excalibur PAM (Privileged Access Management) provides **web-based zero-trust** access to Enterprise resources. Zero-trust means the client machine doesn’t need to be trusted as nothing is installed on it and all access from it goes via browser or native client utilizing a well-known protocol such as RDP. The client machine doesn’t get access to the internal network.

###  3.15. <a name='AreExcaliburPAMsessionsrecorded'></a>Are Excalibur PAM sessions recorded?

Yes, Excalibur PAM considers all sessions “privileged” and by default recorded. Every action taken by the user is cryptographically signed to certify it was performed by the authenticated user. The effect of this is that there is continuous matching of every user action (as every user action and user PAM session is recorded and cryptographically signed) to strongly multi-factor authenticated identity. **With no way to delegate access or claim it was some other user**.

###  3.16. <a name='CanItransferfilesviaPAM'></a>Can I transfer files via PAM?

Excalibur PAM provides an option to upload files from client to target or download files from target. The files can be transferred via RDP or SSH session. For further information about files transfer, read the PAM manual please.

###  3.17. <a name='Facaderunsbutdoesntconnect'></a>Facade runs but doesn’t connect

Facade starts under gMSA and sometimes is launched earlier than Active Directory. SCM tries to launch service, but can’t verify service account (event viewer shows that account has not been found) and doesn’t allow it. **To resolve this problem, reboot the facade**.

##  4. <a name='Furthermaterials'></a>Further materials

[Excalibur Administrator’s Dashboard Manual with PAM](../xclbr-administrator-dashboard-manual/README.md)

[Excalibur User’s Dashboard Manual with PAM](../xclbr-user-dashboard-manual/README.md)

[Excalibur User’s Manual](../xclbr-user-manual/README.md)