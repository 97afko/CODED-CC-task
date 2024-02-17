```
Starting Nmap 7.80 ( https://nmap.org ) at 2020-11-09 19:19 GMT
Nmap scan report for startup (10.10.48.14)
Host is up (0.073s latency).
Not shown: 997 closed ports
PORT   STATE SERVICE VERSION
21/tcp open  ftp     vsftpd 3.0.3                                                                                  
| ftp-anon: Anonymous FTP login allowed (FTP code 230)                                                             
| drwxrwxrwx    2 65534    65534        4096 Nov 09 02:12 ftp [NSE: writeable]                                     
|_-rw-r--r--    1 0        0             208 Nov 09 02:12 notice.txt                                               
| ftp-syst:                                                                                                        
|   STAT:                                                                                                          
| FTP server status:                                                                                               
|      Connected to 10.9.0.218                                                                                     
|      Logged in as ftp                                                                                            
|      TYPE: ASCII                                                                                                 
|      No session bandwidth limit                                                                                  
|      Session timeout in seconds is 300                                                                           
|      Control connection is plain text                                                                            
|      Data connections will be plain text                                                                         
|      At session startup, client count was 2                                                                      
|      vsFTPd 3.0.3 - secure, fast, stable                                                                         
|_End of status                                                                                                    
22/tcp open  ssh     OpenSSH 7.2p2 Ubuntu 4ubuntu2.10 (Ubuntu Linux; protocol 2.0)                                 
| ssh-hostkey:                                                                                                     
|   2048 42:67:c9:25:f8:04:62:85:4c:00:c0:95:95:62:97:cf (RSA)                                                     
|   256 dd:97:11:35:74:2c:dd:e3:c1:75:26:b1:df:eb:a4:82 (ECDSA)                                                    
|_  256 27:72:6c:e1:2a:a5:5b:d2:6a:69:ca:f9:b9:82:2c:b9 (ED25519)                                                  
80/tcp open  http    Apache httpd 2.4.18 ((Ubuntu))                                                                
|_http-server-header: Apache/2.4.18 (Ubuntu)                                                                       
|_http-title: Maintenance                                                                                          
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel 
```
```
OK so we find some open ports 
21 FTP
22 SSH
80 HTTP
```
