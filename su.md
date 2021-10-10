Skip to:
content
search
login
University Information
Technology Services
About
Toggle About navigation
Services
Toggle Services navigation
Initiatives
Toggle Initiatives navigation
News & Events
Get Help
Toggle Get Help navigation
Search
Knowledge Base
Menus
About the team
KNOWLEDGE BASE
Search the Knowledge Base...
Search Log in
Options Help Chat with a consultant
About Unix sudo and su commands
The Unix commands sudo and su allow access to other commands as a different user.

The sudo command
The sudo command allows you to run programs with the security privileges of another user (by default, as the superuser). It prompts you for your personal password and confirms your request to execute a command by checking a file, called sudoers, which the system administrator configures. Using the sudoers file, system administrators can give certain users or groups access to some or all commands without those users having to know the root password. It also logs all commands and arguments so there is a record of who used it for what, and when.

To use the sudo command, at the command prompt, enter:

sudo command
Replace command with the command for which you want to use sudo.

The sudo command also makes it easier to practice the principle of least privilege (PoLP), which is a computer security concept that helps control system access and potential system exploits and compromises. For more information about the sudo command, visit A. P. Lawrence's Using sudo page.

The su command
The su command allows you to become another user. To use the su command on a per-command basis, enter:

su user -c command
Replace user with the name of the account which you'd like to run the command as, and command with the command you need to run as another user. To switch users before running many commands, enter:

su user
Replace user with the name of the account which you'd like to run the commands as.

The user feature is optional; if you don't provide a user, the su command defaults to the root account, which in Unix is the system administrator account. In either case, you'll be prompted for the password associated with the account for which you're trying to run the command. If you supply a user, you will be logged in as that account until you exit it. To do so, press Ctrl-d or type exit at the command prompt.

Using su creates security hazards, is potentially dangerous, and requires more administrative maintenance. It's not good practice to have numerous people knowing and using the root password because when logged in as root, you can do anything to the system. This could provide too much power for inexperienced users, who could unintentionally damage the system. Additionally, each time a user should no longer use the root account (for example, an employee leaves), the system administrator will have to change the root password.

At Indiana University, for personal or departmental Linux or Unix systems support, see Get help for Linux or Unix at IU.

Related documents
Find information about Unix workstation security
This is document amyi in the Knowledge Base.
Last modified on 2019-06-18 14:46:42.

Social media
Facebook for UITS
Twitter for UITS
Instagram for UITS
YouTube for UITS
Additional resources
Support & More
General support or comments:
Email the UITS Support Center
Research technology support:
Contact Research Technologies
Chat with a consultant
AskIU
One.IU
Navigation
Home
Menus
About us
IT@IU
About IT
IT staff
Jobs in IT
OVPIT
Accessibility
Privacy
Copyright © 2021 The Trustees of Indiana University
