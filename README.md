Two utilities made in Node.js

The encrypt.js program accepts the file name (assuming that it is a text file) and password on the command line. For example:
**node encrypt.js home/importantDataFile.txt mypassword**

It overwrites the indicated text file. Saves to it encrypted (not hashed) data in JSON format.

-----
The decrypt.js program accepts the file name (assuming that it is encrypted) and the password on the command line. For example:
**node decrypt.js home/importantDataFile.txt mypassword**

It overwrites the indicated text file. The program tries to decrypt the data by reading the JSON.
