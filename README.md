# BTP
## This repository contains the work done in the project under the guidance of Dr. Anshu Anand 
- Clone the Repository
-  Install LIGGGHTS [https://www.cfdem.com/media/DEM/docu/Manual.html]
-  GO to scripts folder 
-  run the file named in.run 

## Detailed Setup Instructions (on ubuntu/Debian)
### Installing Git
```sh
-  sudo apt install git
```
### Clone this Repository
```sh
-  git clone --recursive https://github.com/nishantsikarwar/BTP.git 
```
make sure LIGGGHTS-PUBLIC folder is inside the repo.

### Install LIGGGHTS (on ubuntu/Debain)

- Run Following Commands
```sh
-  cd BTP/LIGGGHTS-PUBLIC
-  sudo apt install openmpi-bin libopenmpi-dev libvtk6.3 libvtk6-dev
-  cd src
-  make auto
-  sudo ln -s lmp_auto /usr/local/bin
-  sudo mv /usr/local/bin/lmp_auto /usr/local/bin/liggghts
-  liggghts
-  If you see the liggghts version correctly the everthing worked fine press ctrl+c to exit.
```

### Running Simulation (on ubuntu/Debain)
```sh
-  go to BTP/scripts
-  Open in Terminal
-  liggghts < in.run
```
### Visualizing Simulation (on ubuntu/Debain)
```sh
-  sudo apt install paraview
-  paraview
-  Open the dump files formed in  /post directory
```