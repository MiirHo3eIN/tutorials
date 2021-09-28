
# Script Running Steps

open a terminal by pressing ```ctrl+alt+t```

## Screen

list screen sessions: 
```bash
$ screen -ls
```
- if there is any open session, result will be: 
```
There is a screen on:                                                                 
        62227.pts-0.unibo       (28/09/2021 16:19:41)   (Attached)                    
1 Socket in /run/screen/S-miir_ho3ein.
``` 
- if there is no open session, it will be: 
```
No Sockets found in /run/screen/S-miir_ho3ein.
```
for the latest case you need to make a new session as following: 
```bash
$ screen -S <name of session>
```
Then to go the session, you can run: 
```bash
$ screen -r <number of port>
```
Now, we are in the screen, we can enter to the gpu server: 
```bash
$ ssh -X amoallemi@gpu.eees.dei.unibo.it
```
(password is "Am!R7293")

Then you can run whatever you want, like: 
```bash
$ python <name_of_file>.py
```

afterward, to leave the running script there for itself, we just need to press ```ctrl+a d``` to detach the process. and you can leave the terminal and come back to it later 
