# Information-Security
Solutions for Information Security hands-on lab at HCMUTE written by `Nguyen Tien Huy - 22110037`

## Before doing the lab
To do this lab, you are required to have a Dockerfile, which is used to build a Docker image with all the required packages for Hands-On Assembly & Security labs.

### Setup
**On host machine**
1. Open Docker Desktop on your computer.
2. On terminal:
    ```
    git clone https://github.com/quang-ute/myprojects
    ```
3. Navigate to the `myprojects` folder and build the Docker image.
    ```
    docker build -t img4lab .
    ```
4. Run docker container from previously built image
    ```
    docker run -it --privileged -v $HOME/seclabs:/home/seed/seclabs img4lab
    ```
**On seed machine**
1. Navigate to seclabs folder on your home folder, make a direction for a new file, named `bof` <br>
    ```
    mkdir bof 
    ```
2. And move to that folder
    ```
    cd bof
    ```

## Lab #1: 
Conduct buffer overflow attack on `bof1.c`, `bof2.c`, and `bof3.c` programs.

## Lab #2: 
Inject code to delete a file: `file_del.asm` is provided on GitHub.
Conduct attack on `ctf.c`.

[Link to project repository](https://github.com/quang-ute/myprojects)
