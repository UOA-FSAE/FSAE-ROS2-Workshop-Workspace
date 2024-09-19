<div class="bg">
    <div class="container">
        <img src="assets/fsae-logo.png" alt="devs-logo" height="50"/>
        <img src="assets/devs-logo-black.png" alt="devs-logo" height="100"/>
    </div>
    <h1>ROS 2 workshop</h1>
</div>
<br>

# Workshop Outline
In this workshop you will learn about the the basic concepts of ROS 2 (the
second version of Robot Operating System), a framework for that enables easy
communication between systems to discover, send, and receive data
particular you will be using the Humble Hawksbill LTS version, as this is the
one used in our FSAE team. *There is a new ROS 2 distribution released yearly on
May 23rd (World Turtle Day).* Humble Hawkbill was initially released in 2022 and
will be supported until 2027. 


Over this workshop we will go through a series of 3 interactive activities. You are
highly encouraged to follow along. Between each demonstration we will give you
time to play around on your own and attempt to complete each activity.

### You will learn about:
* ROS nodes 
* ROS Topics and Services
* Learn to use the CLI
* Creating your own custom ROS 2 node in Python
* Package management
* Using the Colcon build tool 

No additional installation is required. Everything you need has been provided for
you within this workspace. If you need help with anything please raise
your hand and one of our member will come and assist you.
The environment you are working in is a docker container hosted on our machines.
For resource saving purposes you have not been provided with graphical
capabilities. **Effects you have across the ROS network will be visible on the
projector at the front.** 

We do not recommend this, but if you **have experience with ROS 2 already** and
wish to use your own local machine please ensure you are connected to our club's local
network, and have set ROS_DOMAIN_ID=24 as an environment variable.

You can find a link to this repo here: https://github.com/UOA-FSAE/FSAE-ROS2-Workshop-Workspace

Feel free to save your work in GitHub or consider forking this project
 

### Disclaimers
The material compiled in this workspace is incomplete and supplimentary to our
presentation. Follow along with is happening up on the projector and refer back
to the provided documentation if you forget anything.


## Housekeeping rules
To ensure a pleasant learning for all participants we ask you to follow a few
rules:

1. No trying to hack into our systems beyond the workspaces provided
2. No unauthorised tampering with other users workspaces.
3. Please adhere to the game rules of activity 1
4. Be kind to others and help them learn
5. And most importantly, have a good time!

### Activity 1
You will learn about the ROS2 command line interface, and using introspection
tool in RQT.

If you miss anything refere to the readme [here](./Activity_1/readme.md)


### Activity 2
You will create your own ROS2 node in python that allows you to publish and
subscribe to  

### Additional resources
if you wish to learn more about ROS 2 you can refer to these sources:
* [Official ROS 2 Docs](https://docs.ros.org/en/humble/index.html)
* 





















<style>
    .container {
        grid-gap: 20px;
        display: grid;
        align-items: center;
        align-self: center;
        justify-content: center;
        grid-template-columns: repeat(2, auto);
    }
    .bg {
        background-color: rgb(255,255,255);
        display: grid;
        align-items: center;
        align-self: center;
        justify-items: center;
    }
    .bg h1 {
        color: rgb(100,100,100);
        font-weight: bold;
        font-size: 30px;
    }
</style>
