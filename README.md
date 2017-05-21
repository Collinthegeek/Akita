# arch installer thingy
A graphical arch linux installer in python/pygtk

![screenshot](http://i.imgur.com/0bV3MdO.png "Super early")


The idea of this is that every screen will have multiple options which 
will change variables for that screen. When you hit the next button it 
puts those variables together into a command which it appends to a file 
"install" which is just a bash script that will run at the end.

Ex:

On the partitioning screen you chose to partition /dev/sda1 as ext4. It 
will set a varible for the partition type and one for the partition 
you're formatting then when you hit next it 
will add the command "mkfs.ext4 /dev/sda1" to the install script. 
Everything is done in python/pygtk so it can be material with Liri's gtk 
theme/flat-plat


