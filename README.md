# pylinvstmanage
Python script to manage Windows VSTs bridged with LinVST according to a config file.

## Features
- Update/Create *.so files for all VSTs listed in config file
- Enable/Disable VSTs by adding/removing a softlink to the respective *.so file.
  All softlinks are mapped to a _link folder_ which can be scanned by your preferred DAW.

## Dependencies
- python3
- optional: _termcolor_ package for colored status output

## Usage
### Setup the config file
It's an ini-format config file with basically two parts:
    1) General settings
    2) Variable amount of sections per folder that contains one or more VST-dlls
    
Further documentation can be found within the config file *pylinvstmanage.ini* itself.

### Run the script
Simply run *pylinvstmanage* from the console.
It will look for the config file at two possible locations:
    1) current directory
    2) ~/.config/linvst/manage/pylinvstmanage.ini

    
