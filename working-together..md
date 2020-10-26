# Working together.

### Now we share a repo together. Good.

#### Each I'd like you to make a test, unless told differently, you'll have to :

* -&gt;`cd {Clover partition}/EFI`
* -&gt; `git fetch`
* -&gt; `git pull`
* -&gt; `git clean -f -d`
* Reboot. If it crash, or black screen, give it few seconds and then reboot on your backup solution.
* -&gt;`cd {Clover partition}/EFI`
* -&gt; `git add -A && git commit -m "{commit description}" && git push`
* Drop a message in the issue you've opened, so I get a notification.

NOTE : shell command can be chained. `git fetch && git pull && git clean -f -d` can be used.  
If you get error when fetch, pull or clean, the easiest fix is to delete the EFI folder et re-clone it :  
-&gt; `cd {Clover partition}`  
-&gt; `rm -rf EFI`  
-&gt; `git clone {repo url} EFI`  
To check your efi folder is perfectly in sync with github :  
-&gt; `git status`  
You should get :  
`On branch master  
Your branch is up to date with 'origin/master'.`

`nothing to commit, working tree clean`  
If you get anything about untracked files, modified files : re-clone.  


#### Do not copy file in and out this folder.

If you want to modify something, of course you can. After it's done, commit :  
-&gt; `cd {Clover partition}/EFI`  
-&gt; `git add -A && git commit -m "{commit description}" && git push`



