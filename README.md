# KV-Explorer
KV-Explorer is a key-value storage system with client and server.   
KV-Explorer use B+ tree as storage engine. Client and server communicate using the TCP protocol.  
  
## Compile
make

## Example  
First, run the server program :  
./exp-srv  
   
Then, run the client program :   
./exp-cli  

Insert a key-value :  
&gt; set&nbsp;&nbsp;shayne&nbsp;&nbsp;1  
   
Search a key :   
&gt; get&nbsp;&nbsp;shayne  
  
Update a key :  
&gt; update&nbsp;&nbsp;shayne&nbsp;&nbsp;2  
   
Delete a key :  
&gt; del&nbsp;&nbsp;shayne  
  
Display the current status of the storage system :  
&gt; stat  
  
Look for help :  
&gt; h  
  
Quit from client :  
&gt; q  

## Attention  
By default, the key type is string and value type is int.   
All key-values store in one file named test.db, you can change the file name or file position in source file test/kvstore/exp-server/exp-server.cc.

