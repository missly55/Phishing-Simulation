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
- GoPhish – A tool used for creating phishing simulations
- Ubuntu Linux – Used as the operating system to run GoPhish
- VirtualBox – To set up and manage a virtual machine for safe testing
- Web Browser – To interact with GoPhish interface

### Steps:
Step 1: Set Up GoPhish on Ubuntu

1. Navigate to [GoPhish Releases](https://github.com/gophish/gophish/releases)
2. Download `gophish-v0.12.1-linux-64bit.zip`

*Ref 1: GoPhish Download*



Step 2: In the downloads folder the file `gophish-v0.12.1-linux-64bit.zip`  was installed. You want to open the file without the .zip. 

1. Open Files → Go to Downloads
2. Right-click `gophish-v0.12.1-linux-64bit.zip`
3. Select "Extract Here"

*Ref 2: File Extraction*


Step 3: Give GoPhish Permission to Run

- Navigate to Downloads > `gophish-v0.12.1-linux-64bit.zip` > Right-click the gophish file.
- Select “Properties” > Permissions tab > Check the box that says “Allow executing file as a program”

*Ref 3: Permission Setup*


Step 4: Lauch the GoPhish using terminal. (requires admin permission)

*Error* permission denied error when running ./gophish, used sudo ./gophish to use administrative privileges.


*Ref 4: Error running GoPhish*


- Open terminal in the GoPhish folder and run command `sudo ./gophish` to start the program.

 *Ref 5: Successful running of GoPhish*



**Tells if the GoPhish is running correctly:**
```bash
starting phishing server at http://0.0.0.0:80
starting admin server at https://127.0.0.1:3333
```

Step 5: Log Into GoPhish using Web browser:
- **Restart GoPhish:**

- Navigate to your Downloads folder > `gophish-v0.12.1-linux-64bit.zip` > Right-click inside the folder > "Open Terminal"

*Ref 6: Terminal GoPhish Startup*


- Using the browser Open Firefox > Type `https://127.0.0.1:3333`
- A warning message is displayed
- Click **Advanced**  > Click **Accept the Risk and Continue**.

*Ref 7: GoPhish Login Page*


*Ref 8: GoPhish Resetting Password*




*Ref 9: GoPhish dashboard after login*


**Beginning of the GoPhish Phishing Email:**

- Create a New Sending Profile:

- In GoPhish send a phishing email:
- **Select Sending Profiles > New Profile:**

*Ref 10: GoPhish Profile (test)*

Step 6: Setting up GoPhish and connecting Email server:

- Using Mailtrap for testing phishing emails with GoPhish in a sandbox environment.

*Ref 11: Mailtrap dashboard*


*Ref 12: Sending Profile*


Step 7: Create an Email Template:

- Fake email for testing to send to users.
- In GoPhish, **Click Email Templates**.
- Then **New Template**.

Fill out the Template: (using a fake sense of urgency that phishing emails normally have)

- Name: Fake Login Alert

- Subject: Urgent: Your Account Needs Verification

- From: April Williams <aprilwilliams@example.com>

- Body: 

*Ref 13: Email template*


Step 8: Create a Landing Page:

- In GoPhish, **Click Landing Page**
- Click **New Page**
- Name Fake Login Page
- Click **Import Site**
- Click **Capture Submitted Data and Capture Passwords **
- Save

*Ref 14: Landing Page*


Step 9: Create a Group of Target(Users)

- Go to **Users & Groups.**
- Click **New Group.**
- Name: Training Simulation
- Add Recipients:
- Save Group

  *Ref 15: Target Group*

  
Step 10: Launch Campaign

- Go to **Campaign.**
- Click **New Campaign.**
- Fill out:
- Name: Phishing Test #1
- Email Template:Click the one that was created.
- Landing Page: Choose Fake Login Page.
- URL
- Launch Date:
- Sending Profile: Choose the one that was created,
- Groups: Choose the user group you created.
- Click **Launch Campaign.**

  *Ref 16: Launch Campaign*  













