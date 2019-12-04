# GFS_19_ARRAY

Implementation of Google File System in Python 3


Testing Formats:<br>
To run the Master Server - <b>python3 Master_Server.py</b><br>
To run the BackUp Master Server - <b>python3 Backup_Master_Server.py </b><br>
<b>python3 chunk_server.py port_number(of chunkserver)</b> - To run the chunkserver (All the chunkservers to be run with their port numbers)<br>
To run the client - <b>python3 client.py</b></br>

In client after running it:
<b>upload file_name</b> - To upload the file into the chunkservers<br>
<b>download file_name</b>: To download the file from the chunkservers<br>
<b>lease file_name</b>: Put a lease/lock on the file,so that no other client can upload/download the file
<b>unlease file_name</b>: Remove the lease put on the file...





Architecture:
One Master Server<br>One BackUp Master Server<br>Four Chunkservers<br>Multiple Clients Allowed.<br>
Master Server will hold the Metadata of all the chunks of the files which will be used by clients and chunkservers to communicate with the appropriate chunkserver



