Version: NAFATH-V1
Track: Cybersecurity

 ## Overview

A government Single Sign-On (SSO) system allows people to use one account to access different government services. To keep this system safe, six technology areas work together. Software uses OAuth 2.0 and OpenID Connect to help users log in securely and confirm their identity. Cybersecurity uses FIDO2 and passkeys to protect users from fake websites and phishing attacks. Mobile security uses Android permissions to control what an app can access on a phone. Networking uses DNS over HTTPS (DoH) to encrypt DNS requests and make it harder for others on the network to see them. Artificial intelligence (AI) helps detect unusual login activity that may be a sign of an attack. Finally, Oman's Personal Data Protection Law helps ensure that citizens' personal information is handled safely and responsibly. Together, these six areas help protect user accounts, keep personal data private, and make government online services safer and more private, and more trustworthy for citizens.

## Software OAuth 2.0 vs OpenID Connect

Question: Which one is for logging in, and which one gives apps access to data?

OpenID Connect (OIDC) is used to log users in and confirm their identity. OAuth 2.0 allows an app to access certain user data or services with permission. OIDC is built on top of OAuth 2.0, and they work together to support secure login systems.

Sources: OAuth 2.0 FAQ - https://oauth.net/faq/
OpenID Connect https://openid.net/foundation/how-connect-works/

## AI  Risks of Detecting Fake Logins

Question: What can go wrong when AI detects suspicious login attempts?

AI can make mistakes when checking logins. A false positive happens when it blocks a real user, while a false negative happens when it misses a hacker. AI may also treat some groups unfairly if its training data is biased. Over time, changes in user behavior can make the model less accurate. Regular testing and human review can help reduce these risks.

Sources: NIST AI Risk Management Framework -https://www.nist.gov/itl/ai-risk-management-framework

## Mobile  Android Permissions

Question: How does Android ask for app permissions?

On Android, some permissions are requested while you are using the app, not just when you install it. For example, an app may ask to use your camera, location, or contacts. You can allow or deny the request, helping you control what the app can access. Some permissions follow different rules depending on the Android version and permission type.

Source: Android Developers -https://developer.android.com/training/permissions/requesting

## Networking  DNS over HTTPS (DoH)

Question: What does DoH protect, and what does it not protect?

DNS over HTTPS encrypts DNS requests between your device and the DNS resolver. This makes it harder for your internet service provider (ISP) and other people on the network to read or change those requests. However, DoH does not make you anonymous. The websites you visit can still identify your connection, and DoH does not encrypt all web traffic. HTTPS protects the connection between your browser and a website.

Source: RFC 8484 — DNS Queries over HTTPS -https://www.rfc-editor.org/rfc/rfc8484.html

## Cybersecurity  Phishing-Resistant MFA
Question: What makes a login phishing-resistant?

Phishing-resistant authentication helps stop fake websites from stealing login information. Passkeys and FIDO2 security keys are good examples because they connect authentication to the real website. SMS codes and codes from authenticator apps are not considered phishing-resistant because users can be tricked into entering them on a fake website. Using passkeys can make government accounts safer.
Sources: NIST Digital Identity Guidelines- https://pages.nist.gov/800-63-4/sp800-63b.html

## Data  Oman's Personal Data Protection Law

Question: What must organizations do with citizens' personal data?

Oman's Personal Data Protection Law, issued under Royal Decree 6/2022, sets rules for handling personal information. Organizations must obtain consent when required, protect personal data, and respect people's rights. People can request access to their data, ask for corrections, and request deletion where the law allows it. Organizations must also report certain personal data breaches to the relevant authorities and affected people.

Sources: MTCIT — Personal Data Protection -https://mtcit.gov.om/sectors/governance/personal

## Misconception in My Track

Myth: Using an SMS code or an authenticator app makes every login safe from phishing.

Many people believe that using a verification code is enough to protect their accounts. However, hackers can create fake websites and trick users into entering their codes. This means that even with two-factor authentication, an account can still be at risk. Passkeys and FIDO2 security keys offer better protection because they check that the user is logging in to the real website.

## Open Question

How can a government login system use AI to detect hackers without blocking real users who log in from a new device or location?


