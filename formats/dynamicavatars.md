# Dynamic Avatars
First line is format version. Each line after that is a avatar entry.\
Each line should be seperated by a `\r\n`, and should include one at the end of
the file.\
Each line is seperated by a `:`.\
To get the zip file name, subtract 135 from the Avatar ID. 
If female is specified, then add 1 to the Avatar ID.

## Version 1
Each entry has 3 values:
* Revision
* Gender (0 If female, 1 if male or neutral)
* Avatar ID

## Version 2
Each entry has 6 values:
* Revision
* Gender
* Avatar ID
* Unknown, possibly "wings"
* Zip size
* Revision? (Again?)