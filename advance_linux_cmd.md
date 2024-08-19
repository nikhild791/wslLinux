#### To see file, file-size file-permission
```
ls -l
ls -lh
ls -l [folder name]/ 
ls ../.. To look at the parent directories
```
##### Brief information about directory sub-directory
```ls -R [folder name nhi diya to usi directory ka sb kuch batyehga]```
#### To see the latest modified files
```ls -t newdir``` or ```ls -lt newidr```
if you want reverse modified date
```ls -lr [folder name]``` 
files by size
```ls -s [folder name]```
#### To see all files
```ls -a``` or ```ls -la``` or ```ls -lRa newdir```
### To search for the file with the .json
```ls -lR | grep .json``` we get all the .json file inside the directory and sub-directories becaus R stands for recursive
```ls | grep .json``` or ```ls *.json```
#### To search for name starting with some letters
```ls nik*```
```touch [filename]```
#### To write file using cat command
```cat [filename]``` 
```cat > newfile.txt``` to write a new file old data will be erased
```cat >> newfile.txt``` to append data inside the file
#### To make directory recursively directory inside of it
```mkdir -p frontend/scripts```
```mkdir -p frontend/css```
#### To remove an empty folder
```rmdir <folder name>```
#### To remove bhara hua folder
```rm -r <folder name> -rf for forcefully```
#### To change the password of the system
```passwd```
#### To change the password of the another user
```sudo passwd user1 ```
#### To uninstall the packages 
```sudo apt remove <package Name>``` keep the configuration file of the package 
#### to avoid confirmation      
```sudo apt remove -y firefox```
```sudo apt purge <package Name>``` deletes the configuration file of the package also
#### For post uninstall and clean up
```sudo apt clean && sudo apt autoremove```
