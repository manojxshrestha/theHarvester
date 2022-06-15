![havester](https://user-images.githubusercontent.com/106522935/173199264-f445ce77-8da7-4b4f-bef1-51ba4b72b408.png)
# theHarvester

# About theHarvester
theHarvester is a very simple to use, yet powerful and effective tool designed to be used in the early stages of a penetration test or red team engagement. Use it for open source intelligence (OSINT) gathering to help determine a company's external threat landscape on the internet. The tool gathers emails, names, subdomains, IPs and URLs using multiple public data sources.

# How to install it?
This is a by default tool in kali linux. So you just need to update the harvester tool.

For confirmation open terminal and type ‘theharvester’ and verify it. If  you see ‘command not found’ error raised continue to the installation process. Else skip the installation process.

# Installation:
In terminal type:

            $ sudo apt-get theharvester
If it doesn’t work you can try to clone it directly from git using the following commands

            $ git clone https://github.com/laramies/theHarvester.git
            $ cd theHarvester
            $ sudo python ./theHarvester.py
            
# Upgrading:
use the following command to upgrade the harvester

            $ sudo apt-get upgrade theharvester

# How to use this harvester tool ?
  theharvester -d [domain name] -b [search engine name / all ][options] [parameters]
Option’s

-d: Domain to search or company name.

-b: Data source: baidu, bing, bingapi, dogpile, google, googleCSE, googleplus, google-profiles, linkedin, pgp, twitter, vhost, yahoo, all.

-s: Start in result number X (default: 0).

-v: Verify hostname via DNS resolution and also search for virtual hosts.

-f: Save the results into an HTML and XML file (both).

-n: Perform DNS reverse query on all ranges discovered.

-c: Perform DNS brute force for the domain name.

-t: Perform DNS TLD expansion discovery.

-e: Use this DNS server.

-l: Limit the number of results to work with (bing goes from 20 to 20 results, google 100 to 100, and pgp doesn’t use this option).

-h: Use SHODAN database to query discovered hosts.

# Examples
To list available options
        theharvester
        
To search emails :
        theHarvester.py -d abc.com -b all
        
To search emails with a limit :
        theHarvester.py -d abc.com -b all -l 200
        
To save the result into an html file :
        theharvester -d abc.com -b all -h myresults.html
        
 To search in PGP(Pretty Good Privacy) only :
        theharvester -d abc.com -b pgp     


#Thanks for reading !

#Don't forget to follow me !

#Happy Hacking !

# ☞Social Media Links:
Facebook: https://www.facebook.com/manojshrestha00

Instragram: https://www.instagram.com/manojshrestha00

Twitter:  https://www.twitter.com/manojshrestha00
