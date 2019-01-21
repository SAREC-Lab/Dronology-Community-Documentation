# Dronology Documentation


## Installation

Setting up and Installing Dronology requires 3 different parts to be installed: 

[Python, Dronekit and SITL](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/install/install-dronekitsitl.md)
is requried to run the Groundcontrol Station and simulate Virtual UAVs using the [Ardupilot](http://ardupilot.org/dev/docs/sitl-simulator-software-in-the-loop.html) Software-in-the-Loop SITL simulator

The [Dronology Groundstation - GCS (Python)](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/install/install-gcs.md)

The [Dronology Core (Java)](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/install/install-dronology.md)


### Scripts: 

We provide shell scripts for installing Dronekit and SITL [setup_dronekit.sh](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/scripts/setup_dronekit.sh), installing the 
Dronology-GCS [setup_dronology_GCS.sh](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/scripts/setup_dronology-GCS.sh), and installing the
Dronology Core [setup_dronology_core.sh](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/scripts/setup_dronology-core.sh) in Linux (tested in Ubuntu 16 and 18)

## Setup
Per default Dronology is configured to run on a single machine. If either the Dronology UI and/or the Dronology GCS are supposed to run on a different machine please follow these instructions: [Distributed Setup](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/install/install-distributed.md)


## Run

[Run Dronology](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/run/dronology.md)


### Scripts: 

We provide scripts for running Dronogy [shell script](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/scripts/run_dronology.sh) or [tmux script](https://github.com/SAREC-Lab/Dronology-documentation/blob/master/scripts/run_dronology_tmux.sh) (requires tmux 2.6 or higher) and the 
Dronology Groundstation [GCS-UI shell script](http://), [GCS Runner shell script](http://)
## Misc

### Docker Container
comming soon..

### VM Image

We provide a fully configured VMWare and VirtualBox image.
Dronology and GCS code can be found found in the /home/uav/git folder.
To start Dronology execute the run-dronology.sh shell script on the Desktop.

Please contact us for further information on the VM Image and the download link.



### Quick Installation Guide:

Please check the scripts before running and adapt target installation locations if necessary!

1. Clone this repository
1. run ```setup_dronekit.sh``` in scripts Folder
1. run ```setup_dronology_GCS.sh``` in scripts Folder
1. run ```setup_dronology_core.sh``` in scripts Folder
1. run ```mvn clean```  in Dronology folder
1. run ```mvn install``` in Dronology folder
1. run ```run_dronology.sh``` or ```scripts/run_dronology_tmux.sh``` in scripts Folder



