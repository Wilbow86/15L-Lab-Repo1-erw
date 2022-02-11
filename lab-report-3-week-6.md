# Copying Whole Directories with ```scp -r```

In this lab report, I will be demonstrating how to move directories as a whole to a remote server.  
This will be extremely helpful because it means we will not have to run dozens if not hundreds of scp commands, let alone creating new directories, 
to put a project on the server. We can do this with the ```-r``` extention.  For demonstration I will use my markdown-parse directory.

## copying whole directory into server

To copy a directory into the server, run 

  ```scp -r direcotoryPath accountName@serverName:~```
  
***Images***

## Junit Tests in Server

