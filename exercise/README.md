# Git crash course Exercise


## Create a new repository in github.

1. On github, create a new repository using the new button, make sure you check "Add a README file"
2. Click the green "Code" button, make sure you have SSH selected, and copy the link.

3. Open a terminal and navigate to a folder where you want to place the repository.
	 3.1 Its often nice to just create a repos folder where you can place cloned repositories.
	 3.2 From your home folder type ``` mkdir repos ```
	 3.3 Open the folder ``` cd repos ```

4. In your terminal use the ``git clone`` command from the cheatsheat to clone the repository.
5. Open the repository folder ``cd <folder name>``
6. Create a new python file ``touch <file name>.py``
7. Open your favourite code editor and write something into the file ex. `` print("Hello World") ``
8. Add the file to git using the ``git add`` command (use cheatsheet).
9. Push the file to remote using ``git push`` command.
10. Check github to see if the file is there.


# Branching

1.  Use the cheatsheet to create a new branch.
2. Make sure you are in the branch check with the ``git branch -a`` command.
	2.1 If you are not in the branch use the ``git checkout <branch name>`` command from the cheatsheet to move into the branch.

3. Push the branch to remote use the cheatsheet command.
4. Edit the python file you created earlier ex. ``print("hello me")``  and save.
5. Commit the changes you made to the file, and push. 

#### Verify:
On github you should now have two branches with to versions of the same file. 

# Merging & Conflicts
1. Make sure you are in the main branch. Use ``git branch -a`` to check
	1.1 If you are not in main, use ``git checkout main`` to move over to main.

2. Use the ``git merge`` command from the cheatsheet to merge your two branches. A conflict should occur.
3. Follow presentation.



