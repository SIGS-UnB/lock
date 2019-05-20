# Lock
Stores all passwords with GPG


### Using GPG Keys

* Install GPG
[Tutorial GPG](https://github.com/SIGS-UnB/core/blob/develop/docs/GPG_KEYS.md)

* Tutorial to use GPG in file keys.gpg

	* You need to be inserted to the project keychain (Contact the developers)
	* To add new developer 
	```	
	gpg --keyserver keys.gnupg.net --search-keys user@example.com
	```
	* If you modify and need to encrypt message, always add list of emails the developers
	```
	gpg  --recipient [list of emails the developers] --encrypt keys.txt
	```
      * Check keychain contacts (To see if people were successfully added)
      ```
      gpg --list-keys
      #LOG
      ```
	* To decrypt message 
	VIEW ONLY
	``` 
	gpg -d keys.gpg
	```
	VIEW AND UPDATE
	```
	gpg --output <outfile> -d keys.gpg
	```