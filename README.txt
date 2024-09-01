You can download docker image form
https://hub.docker.com/r/danialemamian/sudo-privilege
--------------------------------------------------------------------------
HELP:

Step 1: (Deploy the Docker image using the command below)
docker run -it -p 2200:20 <docker_image_name>
Step 2: (start ssh with)
service ssh start
Step 3: (check ssh service)
service --status-all
Step 4: (ssh)
ssh ubuntu@localhost -p 2200
ubuntu@localhost's password: ubuntu
Step 5:
now you access to machine as ubuntu user.
if you go to home directory , you can see we have two user => ubuntu , user
run sudo -l command to see privilege.
Oh! You don't have permission :>
Now, you need to find the user password and login with it.
Search the regular folders... you will find it.
go to /var/www/html/user
There is a .txt file, but it is encoded in Base64. If you decode it, you will find the user password.
Step 6: (login as user)
run su user
Step 7: (find vulnerability)
There are two vulnerabilities
We explain them in the PDF file

HAVE A GOOD HACKING ;>
