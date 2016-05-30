###Host your git repo in your Google Drive.###
What you gonna get after this tiny tutorial? :skull:

*	You can host your private git repository in any file hosting server.
	*	Ex
		*	Google Drive
		*	DropBox
		* Any file hosting service which can sync your file securely. :speak_no_evil:
*	You can share your repository with your contributor.
*	You can use every git luxury with this one.
*	It will take less then a minute to finish everything and get your repository ready to push and pull.

:point_right: If you delete your repository folder from Google drive you will loose your project. :no_entry_sign: :no_entry_sign: **Proceed With Caution** :+1:
#####Here we go#####
I am using **Google Drive** and **Mac** terminal here, you can use whatever you want. (Works very well with Google Drive and DropBox)

###Steps###
* Open your terminal and go to your Google Drive folder. 

	```cd ~/Google\ Drive/```

	Create a new folder. (folder name is repo)
	
	```mkdir repo```
*	Go into **repo** folder.

	```cd repo```
*	Initialise a bare repository inside repo folder

	```git init --bare```
*	Now go to location that location where you wanna start your project.

	```cd ~/Desktop```
*	Clone your repository from `/Google Drive/Repo`

	```git clone ~/Google\ Drive/Repo/ myProject/```
*	You will see these output in your terminal.
	
		Cloning into 'myProject'...
		warning: You appear to have cloned an empty repository.
		done.

*	 Your repository doesn't have any files. Add one file and make a commit.

	```cd myProject```
	
	```echo "Hello World" >> Hello.txt```

	```git add Hello.txt```
	
	```git commit -m "Init commit"```
	
######:boom::boom: You are all set and to ready push your commit.######

Use ```git push origin master``` to push your commit to repo. You will see Google Drive icon is syncing something. ![alt text](./icon/googleDriveSync.png)

#####Now you can share your repo folder with your contributor. After syncing they clone and push there commits. :grin:#####





