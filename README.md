# Information for New Members in Valsson Research Group
Welcome to Valsson Research Group! Here are some valuable instructions, tutorials, and materials that will be helpful in your research.

## Set your Cruntch4 account:
Email Dr. Navneet Khetrapal (Navneet.Khetrapal@unt.edu) to request an account on cruntch4, the high-performance system where we perform our simulations.
You should let him know you are a new member in our group and send him your UNT EUID as this will be your username on cruntch4. Please, do not forget to cc Dr. Valsson in this email.

### Accessing cruntch4
To access cruntch4 from your laptop, you need to use a terminal program such as:
- Putty (on Windows): https://www.putty.org/
- MobaXterm (on Windows): https://mobaxterm.mobatek.net/ 
- iTerm2 (on Apple): https://iterm2.com/ 

If you are inside the UNT network, you can connect directly to cruntch4. 

If you are outside the UNT network, you need to connect to the UNT VPN first, see:   
https://itservices.cas.unt.edu/services/accounts-servers/articles/cisco-anyconnect-mobility-client-vpn

Once you have started a terminal, you will use `ssh` to log onto cruntch4:
```
ssh <USERNAME>@cruntch4.chem.unt.edu
```
where `<USERNAME>` is the user name you are given, should be the same as your UNT EUID. 

If you are logging on for the first time, you must change the password by using `passwd` command.

### Setting up a ssh key for cruntch4
To set up a ssh key for cruntch4, follow the instructions here:     
https://www.ssh.com/academy/ssh/keygen

## Perform the following tutorials to understand how to navigate in the terminal: 
- VIM tutorial: https://openvim.com/  
- VIM Cheat Sheet: http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html
- Intro to BASH: https://carpentry.library.ucsb.edu/2022-07-12-ucsb-bash/01-intro/index.html  
- BASH scripting tutorial: https://linuxconfig.org/bash-scripting-tutorial  
- Python scripting: https://education.molssi.org/python_scripting_cms/ 
## How to open a Jupyter Notebook in Cruntch4:
Open a Jupyter notebook while logged onto Cruntch4: 
```
jupyter notebook --no browser
```
Copy the link given in the terminal.
Then, open a different terminal window and use the following command:
```
ssh -L :8888:localhost:8888 cruntch4
```
Replace the '8888' numbers in this command by the ones appearing in the link given previously. Now, you will be able to login into your Cruntch4 account, as well as opening the link for your Jupyter Notebook! 
