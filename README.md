# Lab 1 

## Environment setup
You need to [install Go](https://golang.org/doc/install) to work with these assignments. While 
you are free to use any platform that supports Go environment, we recommend using Linux with basic tools 
like `git`, `make` and `gcc` installed. For you convenience, we created a AWS AMI image pre-configured
with proper tools which you can use to launch your AWS EC2 instance and start working right away.
Follow the instructions [here](https://aws.amazon.com/premiumsupport/knowledge-center/launch-instance-custom-ami/) to create EC2 instance from custom image, and use our publically avaialble 
image named `ucsd-223b-labs`.

### Notes
1. Detailed instructions on how to create an EC2 image and connect to it can be found [here](https://docs.aws.amazon.com/quickstarts/latest/vmlaunch/step-1-launch-instance.html).
2. Use free-tier eligible instance sizes like `t2.micro` which works fine for all labs (tried and tested). We recommend saving your AWS credits for your final open-ended projects.


## Download

1. Use the _fork link_ from the class website to create your private clone of the starter code.
2. Do `git clone https://github.com/ucsd-cse223b-sp20/lab1-XXX` where `XXX` is your private repo.
3. Go has expectations about environment variables. For convenience, you might set these variables in your `.bashrc` and/or `.bash_profile` files so that you don't have to execute the commands every time:
    ```
    export GOPATH=<path-to-repo>
    export PATH=$PATH:$GOPATH/bin
    ```

## Link to Upstream

Link your clone to the "upstream" to get any updates
```
$ make upstream
```

after this you can get "updates" (in case we modify the starter code), with

```
$ make update
```

## Do the Assignment 

1. Implement the `"todo"` methods in `src/triblab/lab1.go` following the requirements posted on class website (links below).
    - [Lab Home](https://cseweb.ucsd.edu/classes/sp20/cse223B-a/labs.html)
    - [Lab 1](https://cseweb.ucsd.edu/classes/sp20/cse223B-a/lab1.html)

2. Build and run local tests 
    ```
    $ cd src/triblab
    $ make all
    $ make test-lab1
    ```

## Submit 

Save (and submit) your work with:

```
$ make turnin
``` 
or
```
$ git commit -a -m MESSAGE
$ git push
```