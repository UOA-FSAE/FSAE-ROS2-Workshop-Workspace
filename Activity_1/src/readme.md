# Activity 1 - interacting with the Turtlesim
Learning to use the ROS 2 CLI 

## Instructions
### Optional
Everyone has been given a unique TURTLE_NAME co-responding to their container.
Please use this variable to specificy the name of your turtle when directed. 

To set your own TURTLE_NAME use the following command. 
```bash
export TURTLE_NAME=3
```

<br><hr>
<br>

**Step 1:** Show all services
```bash
ros2 service list
```
<br><hr><br>

**Step 2:** Get the type of message used by the spawn service
```bash
ros2 service type /spawn
```
<br><hr><br>

* additionally you could list all service types using
  ```bash
  ros2 service list -t
  ```

<br><hr><br>

**Step 3:** Get the interface of /spawn
```bash
ros2 interface show <enter_spawn_type_from_step_X>
```

You should see something of the following form:
```bash
<type1> <var1>
<type2> <var2>
<type3> <var3>
string name # Optional.  A unique name will be created and returned if this is empty
---
<type5> <var5>
```

<br><hr><br>

**Step 4:** Call the spawn service (in YAML syntax) 
```bash
ros2 service call /spawn <enter_spawn_type_from_step_X> "{<var1>: 2, <var2>: 2, <var3>: 0.2, name: '$TURTLE_NAME'}"
```
* Use `$TURTLE_NAME` as your turtle's name
* **Make sure there is a space after each colon**

<br><hr><br>


**Step 5:** Start a teleop process 
```bash
ros2 run turtlesim turtle_teleop_key --ros-args -r __node:=teleop_$TURTLE_NAME --remap turtle1/cmd_vel:=$TURTLE_NAME/cmd_vel
```
* remap `turtle1/cmd_vel` to `$TURTLE_NAME/cmd_vel` (turtle's name)

<br><hr><br>

**Step 6:** Follow the prompts in your terminal to control your turtle up on the
screen.
* You need to click into the terminal for it to capture your inputs.
* You will see your turtle move on the projector. 

<br><hr><br>

**Step 7:** Call the set_pen service to change your pen color
```bash
ros2 ___ call $TURTLE_NAME/set_pen ___ "{r: _, g: _, b: _, width: 5}"
```
* Fill in the blanks using what you have learnt
* You will need to use other commands to figure out what goes in the last 2

<br><hr><br>

**Step 8:** Repeat the steps above to try and teleport your turtle

<br><hr><br>

## Additional steps

<br>

**Step 9:** try deleting your turtle using the kill service. (re-spawn it
after)

<br><hr><br>

**Step 11:** Get Ready for Tron ☠️



<!-- **Step 9:** Remap rotation actions messages to allow for fine controls 
```bash
ros2 run turtlesim turtle_teleop_key --ros-args -r /turtle1/rotate_absolute/_action/status:=/$TURTLE_NAME/rotate_absolute/_action/status -r /turtle1/rotate_absolute/_action/feedback:=/$TURTLE_NAME/rotate_absolute/_action/feedback -r __node:=teleop_$TURTLE_NAME --remap turtle1/cmd_vel:=$TURTLE_NAME/cmd_vel
``` -->