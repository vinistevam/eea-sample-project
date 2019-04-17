# EEA Sample Project
This project provides a simple web3j application that demonstrates the EEA features of web3j connecting to Pantheon in the Private Network.

1.  Connecting to a Pantheon the Ethereum network
2.  Loading an Ethereum wallet file
3.  Deploying a private token to the network
4.  Transferring tokens privately between parties on the network
5.  Viewing events from the point of view of different parties on the network


## Getting Started

To start clone the repository and import the project:

```bash
$ git clone https://github.com/web3j/eea-sample-project.git
```

## Prerequisites

To run this tutorial, you must have the following installed:

- [Docker and Docker-compose](https://docs.docker.com/compose/install/) 

- [Git command line](https://git-scm.com/)

- MacOS or Linux 
    
    !!! important 
        The Private Network Quickstart is not supported on Windows. If using Windows, run the quickstart
        inside a Linux VM such as Ubuntu. 

- [Pantheon-Quickstart](https://github.com/PegaSysEng/pantheon-quickstart) - Setup and run the private dockerized environment.
    - [Privacy](https://github.com/PegaSysEng/pantheon-quickstart/tree/4-node-example/privacy)

- [Solidity](https://solidity.readthedocs.io/en/v0.4.24/installing-solidity.html) - Solidity version between 0.4.2 < and < 0.5.

## Setup

A step by step series of  how to get an environment setup and running.
    
    
Access the folder.

```bash
$ cd eea-sample-project/
```

Execute `./gradlew generateContractWrappers`.
It will generate the `HumanStandardToken` injecting this dependency into the project.
To mark `build` directory as `Unmark Generated Sources Root` . 

Go to build > generated > source > web3j > main > java. 
```bash
build/
├──  generated/ 
    └──── source/
            └──── web3j/
                └──── main/
                        └──── java/
``` 
Right clique > Mark Directory As > Unmark Generated Sources Root.


```bash
$ ./gradlew generateContractWrappers
```

Execute `./gradlew test`.

!!! important 
        To execute `./gradlew test` you need to have all the nodes from Pantheon-Quickstart running.
        
```bash
$ ./gradlew test
```



