This program returns an IP's latitude and longitude values, using the API provided by https://ipstack.com/.

With the base URL "http://api.ipstack.com/", the API key, and the IP address, we got the endpoint URL.

Before running the program we must confirm that we have Python and the "requests" library installed; if not, we must install them. To install the "request" libray, in the command lines, we must type "pip3 install requests" or "pip install requests".

This program can be run in Linux, to run it correctly, we must type "python get_latitude_longitude.py 'ip'" or "python3 get_latitude_longitude.py 'ip'" in the Linux console, according to your python version, in the 'ip' field, you must type the ip from which you want to know the latitude and longitude.

As a manner of increasing security, the program has the next characteristics:
•	The program also checks that is executing independently.
•	The program checks if the call of the app is correctly input in the prompt line.
•	The program checks if the correct quantity of arguments is inputed.
•	The program manages exceptions which include:
        - HTTP request error.
        - Errors when making requests.
        - Error analyzing the JSON response.

As example of running, in the linux command line, we write: "python3 get_latitude_longitude.py 186.96.147.58" and we should get the output:
20.785789489746094 -103.4727783203125