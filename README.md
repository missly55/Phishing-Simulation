# Phishing Awareness Simulation Lab with GoPhish

## Objective:
The aim of this project is to build a practical phishing campaign simulation using GoPhish to understand how phishing attacks work and steps organizations can illustrate during trainings to educate users of the danger of phishing attacks.

### Skills Learned:

- Install and configure GoPhish on Ubuntu
- How phishing emails are created using custom templates
- Understand the basics of social engineering and how phishing tricks users
- Create a safe environment to run security tests.
- Build a phishing landing pages to simulate real attacks
- Run a phishing campaign and monitor user responses
- How to analyze the results to understand user behavior

### Tools Used:
- GoPhish – A tool used for creating phishing simulations.
- Ubuntu Linux – Used as the operating system to run GoPhish.
- VirtualBox – To set up and manage a virtual machine for safe testing.
- Firefox – Web browser to interact with GoPhish interface.
- Mailtrap – Sandbox email server for testing.

### Steps:
Step 1: Install GoPhish on Ubuntu

1. Navigate to [GoPhish Releases](https://github.com/gophish/gophish/releases)
2. Download `gophish-v0.12.1-linux-64bit.zip`

*Ref 1: GoPhish Download*

<img src="https://github.com/missly55/Phishing-Simulation/blob/75c49d2547dc4adbfa89aad5554542e14c2644b7/images/gophish.png?raw=true" alt="GoPhish" width="550"/>

Step 2: Extract the GoPhish Zip File 

1. Open Files → Go to Downloads
2. Right-click `gophish-v0.12.1-linux-64bit.zip`
3. Select "Extract Here"

*Ref 2: File Extraction*

<img src="https://github.com/missly55/Phishing-Simulation/blob/9a9336c4e217fddeb0aa1dded2e72804eac10016/images/File%20extract.png?raw=true" alt="File Extract" width="500"/>

Step 3: Make GoPhish Executale

1. Navigate to Downloads > `gophish-v0.12.1-linux-64bit.zip` > Right-click the gophish file.
2. Select “Properties” > Permissions tab > Check the box that says “Allow executing file as a program”

*Ref 3: Permission Setup*

<img src="https://github.com/missly55/Phishing-Simulation/blob/9a9336c4e217fddeb0aa1dded2e72804eac10016/images/Permission%20setup.png?raw=true" alt="Permission" width="500"/>

Step 4: Lauch the GoPhish in Terminal (requires admin permission)

*Error* permission denied error when running ./gophish, used sudo ./gophish to use administrative privileges.

<img src="https://github.com/missly55/Phishing-Simulation/blob/836b2e7c7caa1d2ba283abfd76d5e3987493c90e/images/Error.png?raw=true" alt="Error" width="500"/>


1. Open terminal in the GoPhish folder and run command `sudo ./gophish` to start the program.

 *Ref 5: Successful running of GoPhish*

<img src="https://github.com/missly55/Phishing-Simulation/blob/3e19fa45e796062b14330cbaa31b587ce9299590/images/Sucessful%20running%20GoPhish.png?raw=true" alt="Successful GoPhish" width="500"/>

**Tells if the GoPhish is running correctly:**
```bash
starting phishing server at http://0.0.0.0:80
starting admin server at https://127.0.0.1:3333
```

Step 5: Log Into GoPhish using Web browser
- **Restart GoPhish:**

  1. Navigate to your Downloads folder > `gophish-v0.12.1-linux-64bit.zip` > Right-click inside the folder > "Open Terminal"

*Ref 6: Terminal GoPhish Startup*

<img src="https://github.com/missly55/Phishing-Simulation/blob/3e19fa45e796062b14330cbaa31b587ce9299590/images/Restart.png?raw=true" alt="GoPhish Start-Up" width="500"/>

2. Using the browser Open Firefox > Type `https://127.0.0.1:3333`
3.  A warning message is displayed
4.  Click **Advanced**  > Click **Accept the Risk and Continue**.

*Ref 7: GoPhish Login Page*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Login%20Page.png?raw=true" alt="GoPhish Login Page" width="500"/>

*Ref 8: GoPhish Resetting Password*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Reset.png?raw=true" alt="GoPhish Password Reset" width="500"/>


*Ref 9: GoPhish dashboard after login*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Dashboard.png?raw=true" alt="GoPhish Dashboard" width="500"/>

**Beginning of the GoPhish Phishing Email:**

Step 6: Create a Sending Profile (GoPhish)

1. In GoPhish send a phishing email:
2. **Select Sending Profiles > New Profile:**

*Ref 10: GoPhish Profile (test)*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Profile%20test.png?raw=true" alt="GoPhish Profile" width="500"/>

 Setting up GoPhish and connecting Email server:

3. Using Mailtrap for testing phishing emails with GoPhish in a sandbox environment.

*Ref 11: Mailtrap dashboard*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Mailtrap.png?raw=true" alt="GoPhish Login Page" width="500"/>

*Ref 12: Sending Profile*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Profile%20test.png?raw=true" alt="GoPhish Login Page" width="500"/>

Step 7: Create a Phishing Email Template

- Fake email for testing to send to users.
  1. In GoPhish, **Click Email Templates**.
  2. Then **New Template**.

Fill out the Template: (using a fake sense of urgency that phishing emails normally have)

- Name: Fake Login Alert

- Subject: Urgent: Your Account Needs Verification

- From: April Williams <aprilwilliams@example.com>

- Body: 

*Ref 13: Email template*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Email%20Template.png?raw=true" alt="GoPhish Login Page" width="500"/>

Step 8: Create a Fake Landing Page

1. In GoPhish, **Click Landing Page**
2. Click **New Page**
3. Name Fake Login Page
4. Click **Import Site**
5. Click **Capture Submitted Data and Capture Passwords **
6. Save

*Ref 14: Landing Page*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Landing%20Page.png?raw=true" alt="GoPhish Login Page" width="500"/>

Step 9: Create a Target Group

1. Go to **Users & Groups.**
2. Click **New Group.**
3. Name: Training Simulation
4. Add Recipients:
5. Save Group

  *Ref 15: Target Group*
  
<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Target%20Group.png?raw=true" alt="GoPhish Login Page" width="500"/>
  
Step 10: Launch the Campaign

1. Go to **Campaign.**
2. Click **New Campaign.**
- Select:
3. Name: Phishing Test #1
4. Email Template: Fake Login
5. Landing Page: Fake Login Page.
- URL
- Launch Date:
- Sending Profile: Choose the one that was created,
- Groups: Choose the user group you created.
- Click **Launch Campaign.**

  *Ref 16: Launch Campaign*
  
<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Campaign.png?raw=true" alt="GoPhish Login Page" width="400"/>

Step 11: Monitor Campaign Results

*Ref 17: Campaign Successful* 

<img src="https://github.com/missly55/Phishing-Simulation/blob/86c7abb150ea8c817a0e077f1fa42179a5fca868/images/Launch.png?raw=true" alt="GoPhish Login Page" width="400"/>


*Ref 18: Results* 

<img src="https://github.com/missly55/Phishing-Simulation/blob/86c7abb150ea8c817a0e077f1fa42179a5fca868/images/Results.png?raw=true" alt="GoPhish Login Page" width="450"/>

- Received an email in Mailtrap from GoPhish after initially encountering the error:
`max connection attempts exceeded - dial tcp 18.215.44.90:25: i/o timeout — indicating that port 25 was blocked.`
- To resolve this, I updated the SMTP host in GoPhish to `smtp.mailtrap.io:2525`, which successfully allowed the email to be sent to Mailtrap.


*Ref 19: Sucessful Email Sent*

<img src="https://github.com/missly55/Phishing-Simulation/blob/fe64e293a61186e6dd70b4a121692e5e1e76df45/images/Email%20Sent.png?raw=true" alt="Phish Email" width="400"/>









