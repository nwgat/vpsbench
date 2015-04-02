# vpsbench
"pigz" for multithreaded gzip
"4k" for better SSD compatibility and performance 

Benchmark VPS performance. See original authers [user submissions](https://github.com/mgutz/vpsbench/wiki/VPS-Hosts)

A script to run simple and comprehensive benchmarks on CPU and IO performance.

Tested on:

* Debian 6.0.6
* Ubuntu 12.04 LTS

## known issues
/usr/bin/time is not found on Ubuntu 14.04

## Usage

    Usage: vpsbench [OPTION...]

    -a Bench all
    -d Bench downloads
    -f Create 100M bigfile
    -x Remove temporary files
    -u Bench unixbench

Debian pre-requisites

    apt-get install time pigz
    yum install pigz
    or similar.. 


Example


    $ bash <(wget --no-check-certificate -O - https://github.com/nwgat/vpsbench/master/vpsbench)

    CPU model:  Intel(R) Core(TM) i7-3770 CPU @ 3.40GHz
    Number of cores: 4
    CPU frequency:  3417.879 MHz
    Total amount of RAM: 3265 MB
    Total amount of swap: 1021 MB
    System uptime:   8:41,
    I/O speed:  427 MB/s
    Bzip 25MB: 4.66s
    Download 100MB file: 1.64MB/s


## License

Licensed under [The MIT License](LICENSE)
