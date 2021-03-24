# macOS_CLI_Speedtest
Ookla Speedtest CLI v5 installer for macOS without homebrew

## Overview

This installation was tested with macOS 10.15.7 (Catalina)

-


## Installation

1. Open the `Terminal` Application from `/System/Applications/Utilities/Terminal.app`

2. Download the `.zip` package to your `Download` folder and unzip there.

3. It is important to go into the downloaded folder:
```
$ cd ~/Downloads/macOS_CLI_Speedtest-main
```

4. Check your current path with `$ pwd`, it hast to be: `/Users/<USERNAME>/Downloads/macOS_CLI_Speedtest-main`

5. Start the installation with `$ sudo` and the `sh` command:
```
$ sudo sh install.sh
```

6. Now you can run the `$ speedtest` command in the Terminal
```
$ speedtest
```


## Allow Software from unidentified developer

After your first run of the `$ speedtest` command, you will get an error message like this:

![Preferences1](https://raw.githubusercontent.com/zensudo/macOS_CLI_Speedtest/main/content/image1.png)

So you need to `cancel` this error message and got to your `System Preferences`.

```
$ open /System/Applications/System\ Preferences.app
```
Go to `Security` tab and click `Open Anyway`if you're not an administrator, you need to open the lock in left corner.

![Preferences1](https://raw.githubusercontent.com/zensudo/macOS_CLI_Speedtest/main/content/image2.png)

That's it! Now you can run the `$ speedtest`command in your CLI.


## Usage



## Uninstall

To uninstall the `speedtest` just run:
```
$ rm -r /usr/local/Cellar/speedtest/
```


## Contributor

Zen Sudo
