# autoTreeFormat
Command line interface that creates easy to read text file of file structure.

# Quick Start
python autoTree.py -f [directory name]
```
python autoTree.py -f Example
```

Output:
```
Example
├── build
│   ├── resources
│   │   └── dog.jpg
│   └── src
│       ├── addition.py
│       └── helloworld.py
├── docs
├── License.txt
├── README_FILE_STRUCTURE.txt
├── src
├── tools
├── test
│   ├── benchmarks
│   ├── integration
│   └── unit
└── zz
```

# Parameters
| Parameter    | Description                            | Default                     |
| :---------:  |:-------------                          | :-----                      |
| -f           | Name of directory                      | Current working directory   |
| -t           | Text file name                         | README_FILE_STRUCTURE.txt   |
| -b           | Directory/File names to blacklist      | None                        |
| -s           | Include system files                   | True                        |
| -a           | Sort alphabetically                    | False                       |

## Examples
```
python autoTree.py -f Example -b tools zz helloworld
```

Output:
```
Example
├── build
│   ├── resources
│   │   └── dog.jpg
│   └── src
│       ├── addition.py
│       └── helloworld.py
├── docs
├── License.txt
├── README_FILE_STRUCTURE.txt
├── src
└── test
    ├── benchmarks
    ├── integration
    └── unit
```





