# The Game of Life Simulator
----------------------------

<img src="https://img.shields.io/badge/language-C++-ff69b4.svg"/>

This programme can simulate the [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life). It can randomly create an initial grid or fetch it from a file based on the user's needs. And then the grid iterates according to the rules of the game of life. It can also search for still lives automatically.



## Build
--------

This programme can be build actomatically by CMake. To build it:

```
$ mkdir build
$ cd build
$ cmake ..
$ make
```

You may need to wait for a while when compiling and generating executable files. Then all the executable files are under ./bin folder.



## Usage
--------

1. Game of life simulator

To use the simulator, you need to open the executable file:

        ```
        $ cd build
        ```
        
(Do this if your terminal is not under build folder)

        ```
        $ ./bin/gofSimulator [parameter]
        ```

Optional parameters: 

&emsp;&emsp;[1] : Obtain the initial conditions from a text file.

&emsp;&emsp;&emsp;&emsp;example: 
        
```
$ ./bin/gofSimulator 1
Please enter the file path:
>> ../Testing/Data/glider.txt
Please enter the number of generations:
>> 5
...
```
                
    [2] : Starting with random cell contents for the initial conditions.

        example: 
                ```
                $ ./bin/gofSimulator 2
                Please enter the grid size and alive cells number:
                >> 4 4 8
                Please enter the number of generations:
                >> 5
                ...
                ```

    [-h/--help] : Show the help information.





2. Find still lives


## License
----------

See [`LICENSE`](./LICENSE.txt) for more information.
