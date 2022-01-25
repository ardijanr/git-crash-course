
# Git crash course Exercise


## Create a new repository in github.

1. On github, create a new repository using the new button, make sure you check "Add a README file"
2. Click the green "Code" button, make sure you have SSH selected, and copy the link.

3. Open a terminal and navigate to a folder where you want to place the repository.
	\
	 3.1 Its often nice to just create a repos folder where you can place cloned repositories.
	 \
	 3.2 From your home folder type ``` mkdir repos ```
	 \
	 3.3 Open the folder ``` cd repos ```

4. In your terminal use the ``git clone`` command from the cheatsheat to clone the repository.
5. Open the repository folder ``cd <folder name>``
6. Create a new python file ``touch <file name>.py``
7. Open the repository in your favourite code editor, and edit your newly created file. Write something, ex. `` print("Hello World") ``
8. Add the file to git using the ``git add`` command (use cheatsheet).
9. Commit the file using ``git commit`` (use cheatsheet).
9. Push the file to remote using ``git push`` command.
11. Check github to see if the file is there.


# Branching


### 1. Create Two Branches
1.  Create TWO new branches using the ``git branch <branch name>`` command, run the command twice.
2. Push the branches to remote, use ``` git push -u origin <branch name>```

### 2. Edit one of the branches
1. Move over to one of the branches using the ``git checkout <branch name>`` command.
5. Verify that you are in the correct branch using ``git branch -a``
4. Edit the file, ex. change it to ``print("hello me")``
6. Commit the changes you have made, use the commit command from the cheatsheet.
7. Push the changes. 

### 3. Edit the second branch
1. Move over to the second branch using the ``git checkout <branch name>`` command.
5. Verify that you are in the correct branch using ``git branch -a``
4. Edit the file, ex. change it to ``print("hello me")``
6. Commit the changes you have made, use the commit command from the cheatsheet.
7. Push the changes. 


#### Verify:
On github you should now have three branches if we include main with three versions of the same file. 

# Merging & Conflicts
1. Make sure you are in the main branch. Use ``git branch -a`` to check.
	\
	1.1 If you are not in main, use ``git checkout main`` to move over to main.

3. Use the ``git merge`` command from the cheatsheet to merge your two branches into main. A conflict should occur.
4. Follow presentation.
