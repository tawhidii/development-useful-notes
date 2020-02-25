# [Solved] XAMPP: Another web server is already running


###### Solved by running this on terminal


`sudo netstat -nap | grep :80`

###### You’ll see apache2 and there is 3–4 digit numbers before it, mine is 980

`sudo kill [number]`
###### where [number] is the number for apache2 , in this case I run sudo kill 980

###### *The number might be different than yours.

###### Start XAMPP again.

`cd /opt/lampp/ && sudo -s`

`./lampp start`
