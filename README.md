# Using Eagle with oshpark and sparkfun

> This project is dependent on [Sparkfun](www.sparkfun.com)'s EAGLE libraries and also OSHPark's DRU file.

## Get EAGLE
The EAGLE download can be found [here](https://www.autodesk.com/products EAGLE/free-download). The free version is sufficient in this case

> EAGLE used to be made by CADSOFT USA, but is now under the AutoDesk umbrella.

## Download and apply design rules
We are going to be using [OSHPark's design rules](https://oshpark.com/LaenPCBOrder.dru) since this is the service we are using to make the PCBs. You should expect a file called LaenPCBOrder.dru

## Download Sparkfun's EAGLE libraries
They are made for older versions of EAGLE, but they work nonetheless. You may either clone the [repository](https://github.com/sparkfun/SparkFun-EAGLE-Libraries) or download the [zip file](https://github.com/sparkfun/SparkFun-EAGLE-Libraries/archive/master.zip)
Download Sparkfun's EAGLE libraries

They are made for older versions of EAGLE, but they work nonetheless. You may either clone the repository or download the zip file

## Setup EAGLE Directories

1. Options > Directories...
    * To add a paths by placing colons between each file path to where a the desired directory exists
2. To add the Sparkfun EAGLE libraries in the library field, append `:path/to/SparkFun EAGLE-Libraries-master`. In my case, since I have it in the root directory, I would append `:$HOME/SparkFun EAGLE-Libraries-master`
3. Repeat with the Project field. This is meant for if you do not have a project in the EAGLE created folder. I like to keep my git repositories in the root, so I would append `:$HOME/equalizerShield` to the project field

> You _may_ want to add the DRU (design rules) directory here, however it may be more intuitive to simply use the design rules check to check against OSHPark design specifications

## Open Project

From here you open the project and click on the schematics. You can view the board also by switching view via the `SCH/BRD` button in the tool bar