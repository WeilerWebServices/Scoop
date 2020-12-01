![Scoop](Scoop.png)

---

[***Scoop***](https://scoop.sh/) is a command-line package manager for Windows which makes it easier to install and use common programs and tools. ***Scoop*** includes support for a wide variety of Windows software, as well as favourites from the Unix world. It addresses many of the common painpoints with Windows' software ecosystem, compared to the package manager models of Unix systems.

When using ***Scoop***, you can download and install supported programs with a single command: "***scoop*** install program," where program is the name of the program. It's similarly simple to update, uninstall and find software, avoiding longwinded trips to websites and the Windows Settings app.

![Scoop](https://www.onmsft.com/wp-content/uploads/2019/07/scw.png)

This guide will just scratch the surface of what's possible with ***Scoop***. We'll show you how to install ***Scoop*** so you can add apps to your system with the command shown above. We'll be publishing further guides over the coming weeks to help you understand the Scoop ecosystem.

The recommended way to install ***Scoop*** is by downloading and running the automated installer, which is distributed as a PowerShell script. Launch PowerShell and run the following command:

```powershell
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
```

(Warning: This allows the current user to run scripts which have originated from a remote source. Use with caution and read the notes on the ***Scoop*** website for further details.)

![***Scoop***](https://www.onmsft.com/wp-content/uploads/2019/07/scoopi.png)

Next, use the following command to download and install ***Scoop***. You may also want to check the ***Scoop*** website to ensure you're using the latest version of the command. If you're worried about what the script does, you can read its source at [get.scoop.sh](http://get.scoop.sh/).

iex (new-object net.webclient).downloadstring('https://get.scoop.sh')

***Scoop*** should now install successfully. If you hit an error, ensure the PowerShell execution policy is properly set (see above) and consult the Scoop documentation.

![Installing 7zip with Scoop](https://www.onmsft.com/wp-content/uploads/2019/07/scoop6.png)

With ***Scoop*** installed, you can go ahead and use the tool to install software to your machine. One popular utility is the 7zip archive manager. With ***Scoop***, you can install it by running "***scoop*** install 7zip" from the Command Prompt. Scoop will automatically download and install the latest version of 7zip, including any dependencies it requires. You'll find a shortcut to the program in the "***Scoop*** Apps" folder in your Start menu.

![Installing 7zip with Scoop](https://www.onmsft.com/wp-content/uploads/2019/07/scoop72.png)

***Scoop*** supports [dozens of programs](https://github.com/ScoopInstaller/Main/tree/master/bucket) out-of-the-box and many more are available using third-party repositories ("buckets"). For more detailed guidance on using ***Scoop***, we recommend reading the wiki. This includes a [complete reference](https://github.com/lukesampson/scoop/wiki/Commands) for all the commands which are available.

***Scoop*** may seem complicated to setup but once running it makes program management extremely simple. It brings the best bits of Unix package management to the Windows desktop, avoiding the need to click through clunky, ad-riddled download sites and graphical installer prompts.

---
