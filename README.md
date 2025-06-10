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

## Steps:
Step 1: Setup GoPhish in Ubuntu

Download and Install GoPhish Using the web browser github.com/gophish/gophish/releases.

*Ref 1: Download of GoPhish*



Step 2: In the downloads folder the file **gophish-v0.12.1-linux-64bit.zip**  was installed.

1. Open Files → Go to Downloads
2. Right-click gophish-v0.12.1-linux-64bit.zip
3. Select "Extract Here"

*Ref 2: File Extraction*


Step 3: Give GoPhish Permission to Run

- Go to Downloads > gophish-v0.12.1-linux-64bit > Right-click the gophish file.
- Select “Properties” > Permissions tab > Check the box that says “Allow executing file as a program”

*Ref 3:show permission setup*


Step 4: Lauch the GoPhish using terminal. (requires admin permission)

*Ref 4: Error running GoPhish*


- Open terminal in the GoPhish folder and run command _sudo ./gophish_ 

 *Ref 5: Successful running of GoPhish*



**Tells if the GoPhish is running correctly:**
starting phishing server at http://0.0.0.0:80
starting admin server at https://127.0.0.1:3333

Step 5:Log Into GoPhish using Web browser:

Firefox > https://127.0.0.1:3333 > Advanced > Accept Risk and continue 
Enter login: Username:  , Password: 

*Ref 6: GoPhish login Page*


*Ref 7: GoPhish dashboard after login*



downloads folder > gophish-v0.12.1-linux-64bit > right click open terminal





