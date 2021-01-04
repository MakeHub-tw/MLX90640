# MLX90640

MLX90640 code for various platforms

## Use `git submodule` command to download other repositories

Most of the subdirectories in this repository are selectively cloned from other open source projects as submodules. Thank the authors for their selfless dedication. Use the command below to clone the full repository

    git clone --recursive https://github.com/MakeHub-tw/MLX90640.git

Or alternatively, if you've already cloned this repository. Just `cd` to it and execute the following commands inside:

    git submodule init
    git submodule update

Enjoy!

## What's included

### MLX90640-library for `mbed`

This is the official library from Melexis - https://github.com/melexis/MLX90640-library

The driver inside the repository is designed to work on [mbed](https://www.mbed.com/), but it seems not so hard to port it to other platforms. 

### SparkFun MLX90640 Arduino Example

We've tested SparkFun's devices on Arduino with https://github.com/sparkfun/SparkFun_MLX90640_Arduino_Example

### Pimoroni MLX90640 (Mainly for Raspberry Pi)

We've tested Pimoroni's examples on Raspberry Pi with https://github.com/pimoroni/mlx90640-library

This should be the starting point if you'd like to play with MLX90640

### WARINGS. Especially for Jetson Nano

By the way, it's said that some code might try to "WRITE" to the EEPROM inside MLX90640 and cause the device damanged. See https://github.com/pimoroni/mlx90640-library/issues/38

Be careful about this! And we are trying to investigate the problem.