# macOS_CLI_Speedtest
Ookla Speedtest CLI installer for macOS without homebrew.
This installation was tested on macOS 10.15.7 (Catalina)

-> The easiest way to install the `$ speedtest` command is, to download and install the .pkg file.

-> Otherwise you can follow the [Installation instructions](#Installation)



## Overview

- [Installation](#Installation)
- [Allow unidentified developer](#Allow-Software-from-unidentified-developer)
- [Usage](#Usage)
- [Uninstall](#Uninstall)


## Installation

1. Open the `Terminal` Application from `/System/Applications/Utilities/Terminal.app`

2. Download the `.zip` package to your `Download` folder and unzip there.

3. It is important to go into the downloaded folder:
```
$ cd ~/Downloads/macOS_CLI_Speedtest-main
```

4. Check your current path with `$ pwd`, it hast to be: `/Users/<USERNAME>/Downloads/macOS_CLI_Speedtest-main`
```
$ pwd
```

5. Start the installation with `$ sudo` and the `sh` command:
```
$ sudo sh installer.sh
```

6. Now you can run the `$ speedtest` command in the Terminal
```
$ speedtest
```


## Allow Software from unidentified developer

After your first run of the `$ speedtest` command, you will get an error message like this:

![Preferences1](https://raw.githubusercontent.com/zensudo/macOS_CLI_Speedtest/main/content/image1.png |  width=100)

So you need to `cancel` this error message and got to your `System Preferences`.

```
$ open /System/Applications/System\ Preferences.app
```
Go to `Security` tab and click `Open Anyway`if you're not an administrator, you need to open the lock in left corner.

![Preferences1](https://raw.githubusercontent.com/zensudo/macOS_CLI_Speedtest/main/content/image2.png |  width=100)

That's it! Now you can run the `$ speedtest`command in your CLI.


## Usage

```
peedtest by Ookla is the official command line client for testing the speed and performance of your internet connection.

Version: speedtest 1.0.0.2

Usage: speedtest [<options>]
  -h, --help                        Print usage information
  -V, --version                     Print version number
  -L, --servers                     List nearest servers
  -s, --server-id=#                 Specify a server from the server list using its id
  -I, --interface=ARG               Attempt to bind to the specified interface when connecting to servers
  -i, --ip=ARG                      Attempt to bind to the specified IP address when connecting to servers
  -o, --host=ARG                    Specify a server, from the server list, using its host's fully qualified domain name
  -p, --progress=yes|no             Enable or disable progress bar (Note: only available for 'human-readable'
                                    or 'json' and defaults to yes when interactive)
  -P, --precision=#                 Number of decimals to use (0-8, default=2)
  -f, --format=ARG                  Output format (see below for valid formats)
  -u, --unit[=ARG]                  Output unit for displaying speeds (Note: this is only applicable
                                    for ‘human-readable’ output format and the default unit is Mbps)
  -a                                Shortcut for [-u auto-decimal-bits]
  -A                                Shortcut for [-u auto-decimal-bytes]
  -b                                Shortcut for [-u auto-binary-bits]
  -B                                Shortcut for [-u auto-binary-bytes]
      --selection-details           Show server selection details
      --ca-certificate=ARG          CA Certificate bundle path
  -v                                Logging verbosity. Specify multiple times for higher verbosity
      --output-header               Show output header for CSV and TSV formats

 Valid output formats: human-readable (default), csv, tsv, json, jsonl, json-pretty

 Machine readable formats (csv, tsv, json, jsonl, json-pretty) use bytes as the unit of measure with max precision

 Valid units for [-u] flag:
   Decimal prefix, bits per second:  bps, kbps, Mbps, Gbps
   Decimal prefix, bytes per second: B/s, kB/s, MB/s, GB/s
   Binary prefix, bits per second:   kibps, Mibps, Gibps
   Binary prefix, bytes per second:  kiB/s, MiB/s, GiB/s
   Auto-scaled prefix: auto-binary-bits, auto-binary-bytes, auto-decimal-bits, auto-decimal-bytes
```



## Uninstall

To uninstall the `speedtest` just run:
```
$ sudo rm -r /usr/local/Cellar/speedtest/
```


## Contributor

Zen Sudo
