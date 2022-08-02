# spcli 
## Silverpeak/Aruba SD-WAN Command Line Interface

### Description
This CLI tool is to query the Silverpeal/Aruba SD-WAN orchestrator and output the information in your terminal.


### Getting Started
###### Requierements
* Python >=3.7
* User with API KEY

To get started, instal the CLI tool using the python3 package manager [pip]

`pip3 install git+https://github.com/NetDevLazg/spcli.git`

Once the installation is successful, you will need to create a file with your api credentials.

* Create a folder in the following directory `mkdir ~/.spcli`
* Create a yml file with your credentials in `.spcli` directory
* Using `vim` 
   * `vim ~/.spcli/creds.yml`
* Using `nano`
   * `nano ~/.spcli/creds.yml`

The yml file needs to have the following variables.

```
Example:
url: silverpeak-orch-use1.silverpeak.cloud
token: a38b3360bb4d06fed7e53f77c8752d74bb4faeb4295385a25e02ebc2594d9074a16bb115fce4d4dc9826d824950504b6d23373
```

After the file is created and saved, please verify the cli tool version using the following command.
```
❯ sp -v
version...installed: 0.0.6
```

### Help Function

To check possible commands, use the `-h` flag after a command. for example.
```
❯ sp -h
usage: sp [-h] [-d] [-v] {orch,appliance,bgp} ...

optional arguments:
  -h, --help            show this help message and exit
  -d, --debug           debug the cli
  -v, --version         shows cli tool version

Silvperpeak Commands:
  {orch,appliance,bgp}
    orch                orchesrator commands
    appliance           edge connect appliance commands
    bgp                 edge connect bgp commands

```
