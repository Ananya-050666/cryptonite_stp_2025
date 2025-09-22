### The Root
```pwn.college{McXp5UT937A-jg5MR7bKEodHJYg.QX4cTO0wCO4AzNzEzW}```

We need to execute the pwn program with the '/' root, '/pwn' should give us the flag

### Program and Absolute Paths
```pwn.college{42eIVsbkRq4XlRy8EPXc-ae87pc.QX1QTN0wCO4AzNzEzW}``` 

we need to run the 'run' file in the 'challenge' directory with a '/' root,  hence '/challenge/run' will give us the flag

### Position thy self 
```pwn.college{49XW1V9JOA5gbRkEoEr6jWPbR12.QX2QTN0wCO4AzNzEzW}```

executing /challenge/run give give an error saying "You are not currently in /sys/kernel directory" <br>
cd /sys/kernel<br>
/challenge/run<br>
should give us the flag

### Position elsewhere
```pwn.college{kR7-9HsxZ3NAZhkyC9jWA_LlIH8.QX3QTN0wCO4AzNzEzW}```

running /challenge/run will give the error- "Currently not in /home directory"<br>
cd /home<br>
/challenge/run<br>
will give the flag

### listing files
```pwn.college{41avRnAzO6ElUuC5s_fcYSGEoDP.QX4QTN0wCO4AzNzEzW}```

The 'ls' command lists out the contents of a directory<br>

running '~$ ls /challenge' give us the output-<br><br>
24592-renamed-run-28533  DESCRIPTION.md

hence '24592-renamed-run-28533' is the file we need to run-<br>
~$ /challenge/24592-renamed-run-28533 will give us the flag

### implicit relative paths, from /
```pwn.college{8vTrWBZWzkTOURAlWPiE3YUZQL2.QX5QTN0wCO4AzNzEzW}```

since we need to run it using a relative path-<br>
cd /<br>
challenge/run

### Position yet elsewhere
```pwn.college{gfiwd0WsWDZeb6qGRx7GG0QIPR6.QXwUTN0wCO4AzNzEzW}```

running /challenge/run gives an error saying "Currently not in /home directory"<br>
cd /home<br>
/challenge/run<br>
should give the flag

### implicit relative path
```pwn.college{oWYUEn7QLIgfIyKRJzDWABJhbCq.QXxUTN0wCO4AzNzEzW}```

since we have to run it from the /challenge directory- <br>
cd /challenge <br>
since we hv to run it using a relative path-<br>
./run

### home sweet home
```pwn.college{or4wC_8eHb8CnhJOtXqMsKnYVK7.QXzMDO0wCO4AzNzEzW}```

since we need to copy it into a file who's path is lesser than 3 characters and no premade file we can create a file named 'a', (This needs to be done inside the /home/hacker directory)-<br>
touch a<br>
now we can copy the contents of flag into a<br> 
/challenge/run ~/a<br>
This will give us the flag 
