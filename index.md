---
layout: default
---

# PERSMAN

**PERSMAN**, or personnel management, is a web application designed to help you, a community leader, to organize your members and gaming sessions. PERSMAN is built on the MEAN stack, meaning MongoDB, Angular, Express and NodeJS. 

# Features

* Secure user registration and authentication
* A mobile-friendly web application
* A calendar where administrators can post events and users can register.
* An application system, where website administrators can add their own questions and order them how they please.
* A unit organization tool, where website administrators can add units to that page and order them how they please.
* A user requests section, where users can request a leave of absence or a discharge from the unit.
* Certification, award, and service record fields for users.
* Dates localized to the user's computer timezone.

# Setup

There are two components to PERSMAN. Both are required to run the application. You will need to take the following steps to have a running application. You will need to find a hosting service for both the Angular Application, the Express API, and for the MongoDB server. This is not an extensive tutorial, and assumes you have knowledge of web hosting and you know the power of Google.

### Express Setup
1. In the Express API, rename _example-config.json_ to _config.json_.
2. Register an account at Sendgrid.com (free) and create an API Key, and verify a Single Sender Verification email address, assuming you have your own domain name. Do not use a Gmail address.
3. Add your Sendgrid API Key to the "apiKey" field in your _config.json_ file. Ensure there is no newline (\n) character at the end of the string, such as "SG.sendgridapikey __\n__ "
4. Add your verified email address to the "sendAddress"" field.
5. Add your database login URL to the "dbURL" field./
6. Add a custom string to the "secret" field.
7. Add your unit or website or whatever name to "websiteName".
8. Add your default administrator email in the "adminAccountEmail" field. When you register with this email, the role of that user will be set to Admin.
9. Run the application.

### Angular Setup
1. In the _assets/config.json_ file, change "API_URL" to your Express API application URL.
2. Add your unit or website or whatever name to "websiteName".
3. Set your desired units in "units".
4. Set your desired home page text in "homeText".
5. Run the application.

# Important Notes
Do not, I repeat **_DO NOT_**, remove any 'none' values in any of the config files. Do not otherwise you will break some systems of the website.

# Future

PERSMAN will receive regular updates, both on the API and Angular Application. I am not planning to abandon it. However I will not promise any features as I develop this in my own free time. Although, With that being said, feel free to request features and suggestions on my [Discord](discord.persman.online).

### Planned Features
* Revamped Certification, Award, and Service Record components with images
* Image support for events
* Beautified UI (make it less boring)
* Theming System (especially a Dark theme)

# Support

I will not hand hold anyone wanting to setup my application. The steps are relatively straight forward. However, if you run into issues, bugs, or have a suggestion, while running the actual application, contact me on my [Discord](discord.persman.online).
