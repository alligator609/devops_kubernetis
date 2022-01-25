## PWD => print working directory

## CD => Change Directory
1. cd / (Goto Root)
2. cd /home(goto home)
3. cd ~ (goto home)
4. cd ~/(Goto home directory to any directory)
5. cd ../(Up one level)
6. cd nick (next directory)

## LS => List
1. ls (list)
2. l (list)
3. ls -l (long list)
4. ls -r (Alphabetic manner)
5. ls -p (File type)
6. ls -s (File size)
7. ls /usr/share (Exact directory list)
8. ls –help (list help )

## SUDO =>  Super User Do

## NANO => Terminal application to open file
1. nano ./file (open exact file in current directory)
2. nano ./file(create file)

## SU => Switch User

sudo su (switch user to super user)

## !! => Run previous command

## pplication install and remove

## APT-GET =>  Apptitude

apt-get install bluefish (install bluefish from reposotory)
sudo apt-get remove bluefish (use superuser to remove bluefish)
sudo apt-get upgrade (to see if any update are available)

## APT-CACHE => Search or see if install)

apt-cache search bluefish ( search for bluefish )
apt-cache policy bluefish (search for bluefish if its install in system)

## SUDU DPKG =>  ( To install .dev (.dev for debian file / .rpm for redhat ))
  
  sudo dpkg -i ./google-chrome.dev (install google chrome Debian file)
                      
## File permission & File Ownership

sudo nano file.txt =>  (crate a file in  directory)
                                
 ls -l   owner-group-public   user : group  date time  file.txt(file name)

Here : 4=only read
       6=read+write
       7=directory

 


## To chane ownership  of File  =>  
                
sudo chown alligato:alligator file.txt         ( change user and group to alligator )
sudo chmod 646 file.txt  (change file owner-group-public to RW-R-RW)

## To remove file =>

rm file.txt (Remove file.txt)
rm ./*cpp  (Remove everything in current dir with extention.cpp)
rm ./*         (  Remove everything in current dir )
rm ./main.* (remove everything which name is main)

## To create a directory =>
  
sudo mkdir mydir (make a directory named mydir)

## To chane file ownership in a directory =.

sudo chown -R alligator:alligator ./mydir  

## To remove dir =>
                 
rm -rf dir ( to remove directory name dir )

## To rename dir =>

rm mydir mydir1       ( change mydir name to mydir1)


## COPY or MOVE FILE

## cp => To copy file
 
cp filedir/filename cpdir/filename                  ( 1st file dir is where it located next where to copy  . cp means copy and if you change last file name it will change copied file name into last file name)

example :
                      cp mydir/file.txt mydir1/file.tst                    

mv => to move file
             
 mv filedir/filename cpdir/filename     ( 1st file dir is where it located next where to move  . mv means move if you change last file name it will change moved file name into last file name)   

example :

 mv mydir/file.txt mydir1/file.txt


## Find Command

find . -type f -name “.txt” (search every file on current directory that has .txt extention)
find . -type f -name “*.txt” (search every file on current directory that has .txt extention avoiding case )
find . -type d -iname “dir”  (search every dir named dir)
find . -perm 664 (search everything (file+dir) that has 664 permission )



find . -maxdepth 1 -perm 664 (search everything on current or +1current directory(file+dir) that has 664 permission )
find . -size +10k (search file or dir which size is more than 10kb)
find . -size -10k (search file or dir which size is less than 10kb)
find . -size 1m (search file or dir which size is exact  1mb)

                                                         
## Extract file

tar -xvjf filename  (file located in current directory)
 

example :

tar -xvjf tor64.tar.xz       ( extract file named tor.64.tar.xz in current directory)
