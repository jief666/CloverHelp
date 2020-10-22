# Initial setup

* Create a github repository. Name it `"EFI4{your name on insanelymac}"`.
* Get to repo URL in Gitbug : ![](.gitbook/assets/screenshot-2020-10-22-at-10.12.42%20%281%29.png) 
* -&gt;`"cd {Clover partition}"`. Remember, not the `Clover folder`.
* -&gt; `"git clone {repo url} EFI"`.
* Get BootloaderChooser BootX64.efi from here : [`https://github.com/jief666/BootloaderChooser/releases`](https://github.com/jief666/BootloaderChooser/releases).
* Copy BootX64.efi in `"{Clover partition}/EFI/BOOT"`.
* Set up your **working** Clover folder in `"{Clover partition}/EFI/CLOVER"`.
* Check that it boots fine.
* -&gt; "rm {`Clover partition}/EFI/CLOVER/misc/preboot.log" .`
* -&gt; "rm {`Clover partition}/EFI/CLOVER/misc/debug.log" .`
* reboot.
* -&gt;`"cd {Clover partition}/EFI"`.
* -&gt; `"git add -A && git commit -m "..." && git push"`.
* Invite me as a collaborator for your github repo. Go in "Settings" -&gt; "Manage access". See picture below. Invite `"jief666"` : ![](.gitbook/assets/screenshot-2020-10-22-at-10.34.44.png)             

![](.gitbook/assets/screenshot-2020-10-22-at-10.34.44.png)





