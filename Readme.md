# FILE MANAGEMENT 



## LinuX commands 

 * ls - list of files and directories

   ex:- ls
 
    desktop bin dev opt usr temp file 
 
 * cat - to display the content of a file

   ex: cat > file1

  Hai....this is srinivas

 * more - to display content of a file in large format

  ex : more filename

 * head - to display the content of a file it displays first 10 lines
 
  ex : head filename
  
 * tail - to display the content of a file it displays last 10 lines
 
   ex : tail filename

 * tail -f - it shows the errors in the file content
 
   ex : tail -f filename 
  
 * locate - to find search files 

  ex : locate filename
 
 * cd - which represents the parent directory

        root@srinivas:dic1/dic2$

   ex : cd ..

        root@srinivas:dic1$
  
 * touch - to create a new file
 
     ex : touch filename
      
 * mkdir - to create a new directory 
 
    ex : mkdir directory name
     
 * move - to move from file1 to file2 (or) directory1 to directory2
 
          ex : move file1 file2 
          ex : move directory1 directory2
                    
 * rm - to delete a file 
 
     ex : rm filename
     
 * rmdir - to delete directory 
 
    ex : rmdir directoryname
  
 * cp - to copy file1 to file2 (or) directory1 to directory2
  
  ex : cp file1 file2 (or) directory1 to directory2
    
 * cp -r - copy directories recursively(must)

    ex : cp -r file1 file2 (or) directory1 directory2
  
 * sed - it is a stream editor
  
 * date - used to display current date/time
  
 * find - used to find/ search files

  ex : find filename

 * grep - used to search through the file ,looking for matches to the pattern specified 

  ex : grep 'word'filename
 
 * grep -i - to search particular word in a file content
   
   ex : write something in the file  to search
      
      grep -i "something" filename 

 * du - show disk usage space
  
 * df - show disk free space
  
 * diff - show difference between files
  
 * wc - to find number of lines, word count, characters count byte in the file
 
    ex : wc filename     
    
 * tar - to saving several files into an archive

  ex : tar cf file.tar file -- tar files into the file.tar

       tar xf file.tar file -- untar into the current directory

       tar tf file.tar file -- show contents of archive         
                
 * zip - used to compress and archive data

  ex : gzip filename
  
 * unzip - used to decompress and extract the content from the compress archived

 ex : gunzip filename

  * ln - used to create links to files or directories.

 * vim/vi - used to create files

  ex : vim/vi file name

   --  i - insert mode 

   --  esc - to exit from the insert mode 

   --  wq - to save and exit

   --  q! - forcely exit without saving file
   
   --  x - Delete the current character
   
   --  d - Delete the current line from current character to the end of the line
   
   -- dd - delete the current line

## USER MANAGEMENT 

 * useradd - to add new user 
 
    ex : sudo useradd username
   
 * userdel - to remove user 

   ex : sudo userdel username 

        sudo userdel -r username --delete users home directory

        sudo userdel -r -f username --delete user others files in othet location

 * passwd - to change the user account passwords
  
    ex : passwd user1 
    
    ex : passwd root 
    
           
## ACCCESS MANAGEMENT

 * ssh - to access remote server
   
   ex :  192.168.256.26

 * scp - copy a file from local to remote server
 
    ex : scp desktop/sample_example.txt root@192.168.741.47:/home/remote_dir
        
 * sudo - to give permission to the user 
 
  ex : sudo apt-get update
  
  ex : sudo apt-get upgrade

 * su - switch current user to another user
 
  ex : su username
    
 * chmod - to give permissions to files or directories
   
   ex : r       Permission to read the file.
   
        w       Permission to write (or delete) the file.
        
        x       Permission to execute the file, or, in the case of a directory, search it.
 

       BEFORE: -rw-rw-r--  mik  mik  assgn1_client.c
       
                chmod u=r assgn1_client.c

       AFTER: -r--rw-r--  mik   mik   assgn1_client.c
       
 * chown - to change the file Owner or group.
 
     ex : chown owner_name file_name
     
     ex : chown root file1.txt
       
## CONFIGURATION MANAGEMENT


 * env - used to display your current environment or run a specified command in a changed environment

     ex : env
 
 * echo $ PATH - used to display the path of the url
 
 * export -  used to mark variables and functions to be passed to child process

      ex : export
 
 * hostname - used to display machine hostname
 
 * netstat - display connection information
  
 * crontab -he first five fields define the time and date of execution, and the 6’th field is used for command execution.
 
 * crontab -e - to add or update job in crontab, use below given command.
 
 * crontab -l - Command to view crontab entries of current user
 
 * kill - used to stop running process and also used to way of communicate a process 

       - its suspend, terminate, stop, break, pause, restart, continue

   ex : kill -l dispaly a list of commands that you want to run on a regular  
   
 * pkill - used to send signal to the process
 
 * crontab -  dispaly a list of commands that you want to run on a regular schedule
 
 * curl - used to access our website through cli
 
 * wget - the wget is the free non-interactive file download , can work in background when user to get disconnected with the system while wget finish its work 

  ex : wget file

       wget -c file -- continue stopped download

       wget -r curl --recursively download files from curl

 * history - to display all used commands
  
 * ping - used to know our machine is able  comminicate or not with server

  ex : ping google.com

 * uname - displays the information about the system.

 * ps -ef|grep<pid> - 
 
 * ps ux - a tool to monitor processes running on your Linux system
 
## LOG MANAGEMENT

 * syslog - a standard protocol used to send system log or event messages to a specific server
 
 * journalctl - used for viewing logs collected by systemd
   
   ex : journalctl
   
 * custom logs - 
 
 
## NETWORK MANAGEMENT

 * ifconfig - Display and manipulate route and network interfaces.
     
     ex :      ifconfig eth0 <address> netmask <address>  
     
 * http - http stands for a hypertext transfer protocol used for transferring data over a network , includes website content and API calls ,uses http protocol. There are two main kinds of http         messages: request and responses.

 * https -The S in https stands for secure. Https uses TLS(SSL) to encrypt normal  http requests and responses.As a result ,https is far more secure than http.
 
 * internal network -  An internal network, called an intranet, is one which is restricted to a defined set of users. An example would be a network accessed only by the employees of a specific company.
 
 * external network - An external network (e.g., the Internet) allows users of all types access. Besides the Internet, an example would include a network that allows customers to connect to s company to place orders. 
 
 * TCP - TCP means transmission control protocol , is a connection based protocol while tcp is more reliable,it transfers data more slowly .
 
 * UDP - UDP means user datagram protocol ,is a connectionless. UDP is less reliable but works more quickly.
 
 * private subnets -  A private subnet, on the other hand, is a subnet that does not have a route to the Internet Gateway
 
 * public subnets - A public subnet is a subnet that has a route to the Internet Gateway. 
 
 * CIDR Range - to count the number of leading 1 bits in the binary representation of the subnet mask
 
      ex : 255.255. 255.0 (in dotted decimal notation) has 24 leading 1 bits, so its CIDR prefix is /24
      
 * kinds of ports - to identify a specific process to which an internet or other network message is to be forwarded when it arrives at a server.
 
    ex :     Ports 20 and 21: File Transfer Protocol (FTP). ...
             Port 22: Secure Shell (SSH). ...
             Port 25: Historically, Simple Mail Transfer Protocol (SMTP). ...
             Port 53: Domain Name System (DNS). ...
             Port 80: Hypertext Transfer Protocol (HTTP). ...
             Port 123: Network Time Protocol (NTP).
 
 * 
 
 
 
 
 




























 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
