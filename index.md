---
layout: default
---

# PERSMAN

**PERSMAN**, or personnel management, is a web application designed to help you, a community leader, to organize your members and gaming sessions. PERSMAN is built on the MEAN stack, meaning MongoDB, Angular, Express and NodeJS. 

# Features

* Secure user registration and authentication
* A mobile-friendly web application
* A calendar where administrators can post events and users and register.
* An application system, where website administrators can add their own questions and order them how they please.
* A unit organization tool, where website administrators can add units to that page and order them how they please.
* A user requests section, where users can request a leave of absence or a discharge from the unit.
* Certification, award, and service record fields for users

# Setup

There are two components to PERSMAN. Both are required to run the application. You will need to take the following steps to have a running application. You will need to find a hosting service for both the Angular Application, the Express API, and for the MongoDB server. This is not an extensive tutorial, and assumes you have basic knowledge of web hosting and you know the power of Google.

### Express Setup
1. In the Express API, rename _example-config.json_ to _config.json_.
2. Register an account at Sendgrid.com (free) and create an API Key, and verify a Single Sender Verification email address, assuming you have your own domain name. Do not use a Gmail address.
3. Add your Sendgrid API Key to the "apiKey" field in your _config.json_ file. Ensure there is no newline (\n) character at the end of the string, such as "SG.sendgridapikey __\n__ "
4. Add your verified email address to the "sendAddress"" field.
5. Add your database login URL to the "dbURL" field.
6. Add a custom string to the "secret" field.
7. Add your unit or website or whatever name to "websiteName".
8. Run the application.

### Angular Setup
1. In the assets/config.json file, change "API_URL" to your Express API application URL.
2. Add your unit or website or whatever name to "websiteName".
3. Run the application.



### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
