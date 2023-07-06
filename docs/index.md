# Wolf OS
!!! warning inline end "Wolf OS Status"
    Wolf OS is in DEV ALPHA
Wolf OS is a in development ComputerCraft OS
## Registry
!!! propane inline end "Registry DB" 
    the Wolf OS Registry uses PropaneDB
the Wolf OS Registry is located at `/wolfos/registry`, it can also be accesed at 
```lua 
_G.registry
registry
```
## Interface
placeholder
### Programs


##### Catagorys
!!! crate inline end "Crates" 
    Crates are packaged programs for Wolf OS

| Catagory      | Use                            |
| ------------- | ------------------------------ |
| system        | programs included with Wolf OS |
| craftOS       | stock craftOS programs         |
| Crates        | programs installed thru crates |


### Setings
!!! propane inline end "Settings DB" 
    the Wolf OS settings storage uses PropaneDB
!!! danger "warning"
    settings is not yet implemented


## Programs
!!! propane inline end "Programs DB" 
    the Wolf OS programs list uses PropaneDB
The Wolf OS Programs List is located at `/wolfos/programList`.

The program list by default refrences some stock craftOS programs and all Wolf OS system programs
### Adding Programs
!!! danger "progd lib"
    the progd lib is not yet implemented
!!! crate inline end "Crates" 
    Crates are packaged programs for Wolf OS and can be used as an alternate method of adding a program. 
open lua shell (run shell then enter `lua`) and run
```lua
progd = require("/wolfos.libs.progd")
dbw = progd.load()
    :addProgram(<program name>,<path>,<program char icon>,[args])
    :close()
```

#### Required Data

| Data              | Description                          |
| ----------------- | ------------------------------------ |
| Program name      | the program's name                   |
| Path              | the path to the program              |
| program char icon | A single char for the program's icon |
| Args (optional)   | any args to pass to the program      |

### Developing

| Use               | Library                              |
| ----------------- | ------------------------------------ |
| UIs               | Basalt (pre-installed) (used by os)  |
| Shells            | Stock Craft OS                       |
| 3D                | Not suported                         |
| Logging           | Log4l  (pre-installed) (used by os)  |
| Data Storage      | PropaneDB                            |

