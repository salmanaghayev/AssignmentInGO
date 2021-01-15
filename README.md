# Assignment in GO

## About The Project

There are two utilities in this project that are in GO. ip.go lists information about interfaces and env.go lists env variables


## ip.go

ip.go lists information such as IP, Mac address etc. about all network interfaces

ip.go utility uses net package in order to get information about interfaces. 

"Interfaces" is a variable assigned to net.interfaces() method. It returns slice and there are information in form of arrays for each interfaces. In this utility using for loop I print interface index, name, hardware address, MTU, flag. There is another for loop runs and gets IP addresses of the interface. In the end I print the result of loop.



## env.go

env.go lists enviroment variables in key/value pairs that delimited by "=".

env.go utility uses os.environ package to get information about system env variables.

Environ returns a slice of string containing all the environment variables in the form of key=value. 
In order to print them in new lines I used for loop and strings package to split string into key/value pairs. Then printed the same "="delimited key/values one by one in a new line

## Source
For both utilities I used internet resources. Read some docs to understand data types.

## Usage

Usage is simple just clone the repo change directory to AssignmentInGO and run utilities

```sh
git clone https://github.com/salmanaghayev/AssignmentInGO && cd AssignmentInGO

go run ip.go

go run env.go
 ```
