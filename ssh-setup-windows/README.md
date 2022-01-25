
# Git crash course SSH setup


## Generate new ssh key:
### READ THE ENTIRE INSTRUCTION BEFORE TYPING COMMANDS SOME OF THEM ARE NOT NECESSARY DEPENDING ON THE PREVIOUS STEP.

# Adding an ssh key to your computer.
#### Windows users MUST use powershell, run it as administrator.

1. Open Powershell as administrator

2. We need to enable ssh-agent autostart
	```
	Get-Service ssh-agent | Set-Service -StartupType Automatic
	```

3. Start ssh-agent
	```
	Start-Service ssh-agent
	```

4. Move to home folder
	```
	cd c:/users/<username>/
	```

5. Open .ssh folder
	```
	cd .ssh
	```

	5.1 If the folder was not found create it with this command.
	```
	mkdir .ssh
	```
6. Create a new ssh key, use an ed25519 key, DO NOT set a name for the file, if you are asked to overwrite press y.
	```
	ssh-keygen -t ed25519
	```

8. Add the private key to ssh agent.
	```
	ssh-add <keyname>
	```

# Register the ssh-key in github
1. In the terminal open the .ssh folder.
\
	Go to home folder
    ```
	cd
    ```
    Open .ssh folder
    ```
	cd .ssh
	```

2. Print out the contents of the the public key file.
	```
	cat <keyfilename>.pub
	```
3. Copy the text and paste it into github ssh settings. Make sure there is no newline or whitespace after the last character of the copied text.





