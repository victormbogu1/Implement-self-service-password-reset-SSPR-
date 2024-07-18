# Implement-self-service-password-reset)SSPR
## Description
This project demonstrates how to implement self-service password reset (SSPR) in Microsoft Entra ID for an organization. I will configure and test SSPR using a mobile phone, which will be necessary to complete the password reset process. This lab simulates a business environment setup, utilizing Azure Microsoft Azure portal. SSPR is essential for most large organizations due to the high number of users. Users often complain about delays with password resets, and not finding a solution to enhance password management can slow down processes as too many passwords are being reset manually.

## Environments Used
  + Azure Portal
## Program walk-through
The first step I took was to sign into the Azure portal and create a new user, ensuring I had an Azure AD Premium P2 license to enable the use of SSPR. I then created a security group to roll out SSPR to a limited set of users initially. This approach allows me to verify that the SSPR configuration works as expected before a full deployment.


[![Screenshot-2024-07-18-213732.png](https://i.postimg.cc/5ttdqwnV/Screenshot-2024-07-18-213732.png)](https://postimg.cc/87x0Tf2K)

[![Screenshot-2024-07-18-220047.png](https://i.postimg.cc/mrQ4rbXc/Screenshot-2024-07-18-220047.png)](https://postimg.cc/Jy4v6WWm)

[![Screenshot-2024-07-18-220546.png](https://i.postimg.cc/L4Qc2Y9C/Screenshot-2024-07-18-220546.png)](https://postimg.cc/K4Lq5YgB)

Next, To enable SSPR for the group, I configured the password reset settings. Afterward, I set the authentication methods. It is essential to verify a user's identity before allowing a password reset, as malicious users might exploit system weaknesses to impersonate others. Azure supports six different methods for authenticating reset requests, such as mobile app notification, app code, and security questions.

[![Screenshot-2024-07-18-220948.png](https://i.postimg.cc/9MMLnb7W/Screenshot-2024-07-18-220948.png)](https://postimg.cc/67kV7dcS)

With the SSPR configuration now complete, I proceed to register a mobile phone number for the test user. Go to the SSPR setup website and sign in with the test user's credentials. I was prompted to enter a phone number, as illustrated below.

[![Screenshot-2024-07-18-223113.png](https://i.postimg.cc/d1pgRpxM/Screenshot-2024-07-18-223113.png)](https://postimg.cc/DJQCnjh5)

Next, I'll test whether the user can successfully reset their password.

[![Screenshot-2024-07-18-223551.png](https://i.postimg.cc/QC7wfm2F/Screenshot-2024-07-18-223551.png)](https://postimg.cc/1V9vtG5S)

[![Screenshot-2024-07-18-223736.png](https://i.postimg.cc/rFS7WhGb/Screenshot-2024-07-18-223736.png)](https://postimg.cc/Wh19cwH6)

[![Screenshot-2024-07-18-223845.png](https://i.postimg.cc/43F0ZjZK/Screenshot-2024-07-18-223845.png)](https://postimg.cc/QB1mJ4Fs)

[![Screenshot-2024-07-18-224016.png](https://i.postimg.cc/qq2DsRKn/Screenshot-2024-07-18-224016.png)](https://postimg.cc/30JZ73nJ)

[![Screenshot-2024-07-18-224109.png](https://i.postimg.cc/66ZPJHP3/Screenshot-2024-07-18-224109.png)](https://postimg.cc/Z0TH6L4t)

