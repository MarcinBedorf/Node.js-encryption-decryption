Two utilities made in Node.js  
The encrypt.js program accepts the file name (assuming that it is a text file) and password on the command line.

For example:
>_**node encrypt.js home/importantDataFile.txt mypassword**_

It overwrites the indicated text file. Saves to it encrypted (not hashed) data in JSON format.

-----
The decrypt.js program accepts the file name (assuming that it is encrypted) and the password on the command line.

For example:
>_**node decrypt.js home/importantDataFile.txt mypassword**_

It overwrites the indicated text file. The program tries to decrypt the data by reading the JSON.

----
The program verifies that the encrypted data has not been replaced.

The checksum (in this case the SHA512 hash function used) is saved in JSON when encrypting the file in encrypt.js. The decrypt.js program gets the created checksum and checks if the restored file has the same.
