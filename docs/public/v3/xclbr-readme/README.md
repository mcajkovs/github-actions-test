# EXC USER README EN

*Multi-Factor Authentication (MFA) is a necessity from the point of security.*

*Excalibur is just one Multi-Factor Authentication without password usage and it is more user friendly than other MFA solutions. For trouble free usage of Excalibur, is necessary to accomplish the following requirements.*

**Requirements for trouble free functioning of Excalibur application:**

1. Excalibur application **has to have** allowed all permissions, which includes:
    1. Excalibur evaluates **Localization** as one of factors **during login ONLY**, whereby no collecting of localization is not performed in the background.
    2. **Camera**, which is used by an integrated QR scanner.
    3. **Fingerprint (Face)**, if the phone supports it and it is properly configured.
    4. **Notifications**.
2. For correct **Online login**, the phone and computer **have to be** connected to the network, thus must have **Internet connectivity** (Mobile, LAN, WiFi) and active connection to Excalibur server (VPN, internet).
    1. When “2G only” mode is activated, the application cannot reach the required speed of login.
    2. When the phone is connected to the mobile internet and it has allowed WiFi (a Google Location Services / Accuracy), then **speed and specification of geolocation** will be obvious.
3. When connection is active - **the scanning of QR code is not needed again**, because the session is after login saved. By clicking on an active session on the mobile application it is possible to **lock /unlock the computer** or **log out** without scanning QR code.
4. For correct functionality of Excalibur application, **push notifications have to be allowed** - on the server, firewall as well as on phone. Push notifications serve to synchronization of sessions; notification of unauthorized login; notifications of authorized requirement.
5. If security policies allows PIN, **the PIN can be used instead of fingerprint / face recognition** ( in case that user has problem to scan finger / face. )

**Attentions:**

- In the case of Android Excalibur application, the **permanent notification (Background running)** serves to **faster running of application**. When this notification is disabled, then the operating system clears application from the memory and next launches of application have a long duration.
- **One Time Password (OTP) is not aimed for common login**. It’s a concept, which is aimed for specific situations, which don’t allow the common login - Online login (such as on an airplane, places without the Internet connectivity). If OTP code is still shown on the token, it means there is a problem with network communication and it is necessary to solve it.
- Excalibur uses the phone’s GPS **ONLY** when Security policies are checked. **Monitoring of position and data collecting are not executed in the background**.
- In case that push notifications are not allowed, there may occur the following problems with Excalibur application usage:
    - After the launch of the application, the session’s status doesn’t have to correspond with real status to reach synchronization between server and token. This time interval relies on quality of connection.
    - If an unauthorized person makes a login into a user's account, the notification describing this fact is sent to the user's token and user or company can proceed against this act immediately. When notifications are disabled, this function is not available