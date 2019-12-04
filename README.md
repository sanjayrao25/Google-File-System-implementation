# GFS_19_ARRAY

Implementation of Google File System in Python 3


Testing Formats:<br>
To run the Master Server - <b>python3 Master_Server.py</b><br>
To run the BackUp Master Server - <b>python3 Backup_Master_Server.py </b><br>
To run the chunkserver (All the chunkservers to be run with their port numbers) - <b>python3 chunk_server.py port_number(of chunkserver)</b><br>
To run the client - <b>python3 client.py</b></br>

In client after running it:
upload file_name: To upload the file into the chunkservers
download file_name: To download the file from the chunkservers
lease file_name: Put a lease/lock on the file,so that no other client can upload/download the file
unlease file_name: Remove the lease put on the file...





Architecture:
One Master Server, One BackUp Master Server,Four Chunkservers,Multiple Clients Allowed.
Master Server will hold the Metadata of all the chunks of the files which will be used by clients and chunkservers to communicate with the appropriate chunkserver



