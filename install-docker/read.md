Run Ubuntu server using key pair
ssh -i .\thrilledLemur3cu7LFr8s.pem ubuntu@13.233.45.190
Install docker 
Update: sudo apt update
Docker : sudo apt install docker.io
Check docker and network interface: ifconfig 

Run dockerize nginx 
sudo docker run -p 8080:80 nginx
Note: run nginx at port 8080 which will use 80 in docker  
ubuntu@13.233.45.190: Permission denied (public key).
Check docker network
sudo docker network ls
sudo docker network inspect bridge
Check docker containers
sudo docker ps
Goto terminal of container
sudo docker exec -it d8c sh     // drc is the first 3 word container id 
Check Address in container 
netstat -tnulp

To check IP table
sudo iptables -t nat -L
To check port 
sudo netstat -tunlp
To check all package in install tcpdump
sudo apt install tcpdump
To check an interface tcp packet 
sudo tcpdump -i eth0 
To use nginx locally
Curl http://localhost:8080
To check an interface tcp packet  in specific port
sudo tcpdump -i eth0 dst port 8080
sudo tcpdump -i lo dst port 8080 

Permission error in windows 
Right click the Key file first1.pem on explorer and Go to Properties > Security > Advanced > Disable Inheritance
Select "Convert inherited permissions into explicit permissions on this object"
Then delete everything there ( Including Administrator, User, User Groups ) and Click Add button.
Now select select a principal > Advanced > Find Now > [ Your User object ] > OK
Now you can tick "Read&Execute and Read  " then press OK



