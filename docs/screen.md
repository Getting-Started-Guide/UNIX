### Guide

> GNU Screen is a full-screen Window Manager that works with Serial Terminals as well.

http://www.gnu.org/software/screen/


1. install gnu screen   
    `apt-get install screen`   
    OR   
    `yum install screen`   
    OR   
    > On Linux distributions where GNU Screen is not available through package managers, building GNU Screen manually is an option.   
    ```sh
    # Download the source and extract

    $ wget http://git.savannah.gnu.org/cgit/screen.git/snapshot/v.4.3.1.tar.gz
    $ tar -xvf v.4.3.1.tar.gz
    $ cd v.4.3.1/src/

    #Build GNU Screen

    $ ./autogen.sh
    $ ./configure
    $ make

    #Run GNU Screen. Replace /dev/ttyACM0 with appropriate device name.

    $ sudo ./screen /dev/ttyACM0
    ``` 


2. interact with screen   
    a) `CTRL-a d`   
    > Exits the current screen (but it continues to run in the background)   
    b) `CTRL-a c`   
    > Creates a new screen   
    c) `CTRL-a ?`   
    > Help   
    d) `CTRL-a "`   
    > Lists active screens   
    e) `CTRL-a`   
    > Switches to the next screen     

#### Scroll   
`CTRL-a ESC`   
> Activates output buffer   

`CTRL+f`   
> Scroll forward   

`CTRL+b`   
> Scroll backward   


#### Remote   


`screen -x`   
> Connect to shared console   
