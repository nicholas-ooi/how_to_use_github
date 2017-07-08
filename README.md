## Why Git and store codes in GitHub?
Storing and transferring codes via other means such as sending through an email, uploading it via google drive or Dropbox   
They would cause potential missing files, mis-configuration, difficulty in merging codes when it comes to a team project.  
Using Git technology and GitHub, we are able to leverage Git to help us manage our code and let GitHub be our online code storage.  
***

## Objective of using GitHub
* To **copy/clone** an existing code repository into our computer  
* To **view/modify/add/remove** codes in our copied code repository in our computer  
* To **get the latest updated code** from our peers/team members that submitted into the code repository  
* To **commit/transfer our code changes** and update it into the online code repository  
* To **merge** any conflicting codes, keeping **track** code changes, and **reverting**/going back to previous revision of the code  

## How to GitHub

To **copy/clone** an existing code repository into our computer
1. Install GitHub for Desktop  [https://desktop.github.com/](https://desktop.github.com/)
1. Open github, at the top left, press the add icon, go to clone tab section.  
![](https://github.com/nicholas-ooi/how_to_use_github/blob/master/images/snip_20170708183100.png)  
1. You will see all your **own repositories** and invited repositories.  
1. Click the repository that you wish to clone, for this example, clone how_to_use_github  

To **view/modify/add/remove** codes in our copied code repository in our computer  
1. At GitHub Desktop, click the how_to_use_github repository  
1. At the top right hand, click Atom, it will open up the Atom IDE with the code repository  
![](https://github.com/nicholas-ooi/how_to_use_github/blob/master/images/snip_20170708202622.png)  
1. Atom IDE can be installed at [https://atom.io/](https://atom.io/), you can of course open the code repository using any other IDE that you have such as Netbeans, Eclipse, etc.
1. Create a new file with your (your name here).html  
1. Copy code -> `<html><body>I am a tester here</body></html>` and paste into your html file  
![](https://github.com/nicholas-ooi/how_to_use_github/blob/master/images/snip_20170708203503.png)  
1. Go back to your GitHub Desktop Application, Right click the how_to_use_github repository, Click open git shell  
![](https://github.com/nicholas-ooi/how_to_use_github/blob/master/images/snip_20170708204605.png)  
1. type `git pull --rebase --prune`
1. type `git add .` and enter, there is a dot!  
1. type `git commit -m "your message"`  
1. type `git push`  
![](https://github.com/nicholas-ooi/how_to_use_github/blob/master/images/snip_20170708211023.png)  

***

## What did I just do from the above commands?
1. `git pull --rebase --prune` - Gets the latest code and updates from the online code repository. --rebase is a flag that informs git to merge the updated codes from the online repository intelligently to our codes that we have. --prune is a flag that informs Git to remove any orphan objects linked to the commit such as file removal, sometimes bug occur within git itself because of weird objects that are stuck  
1. `git add .` - add all the files that you have changed, created, or removed into the staging area.  
1. `git commit -m "your message"` - add all the files that you have changed, created, or removed from the staging area into the commit area.  
1. `git push` transfers all the files from commit area into the online code repository.  

Git technology has four areas - staging area, commit area, online code repository.  
1. Staging area lets you choose the files you want to submit into commit area, you can also choose all the files, which we did above  
1. commit area lets you send all the files committed into the online git repository with a message  


## File and folder Atom Colors
1. If you are using Atom IDE. you will see there are colors highlighted on the file  
1. **green color** refers to a new file that does not exist in the online code repository, **yellow color** refers to a file that has differences from the online code repository  
1. **darker black color** for example the LICENSE file is a file that will be ignored and not transferred into the online code repository  
