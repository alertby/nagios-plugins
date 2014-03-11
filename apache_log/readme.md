App First apache access log statistic
=====================

A module parse apche access log files and calculates 
number of visitited urls and store that data in specifyed file,
by default af_apache_visited_urls.log in folder where script located.

*Dependencies*
* Requires python module: python-daemon
    `sudo apt-get install python-daemon`

* `python af_alogs.py -h` will detail configuration flags


Configuration flags
-----------
`--interval` - interval in seconds to ask apache access logs about updates, by default 60 sec

`--apache-log-file-path` - Path to apache log file , by default `/var/log/apache2/access.log`

`--output-log-file-path` - Path to file where urls count will be saved, by default `af_apache_visited_urls.log`