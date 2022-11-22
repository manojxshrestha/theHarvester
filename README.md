# theHarvester

![theharvester-logo](https://user-images.githubusercontent.com/106522935/193584706-56b7fd19-5951-4161-bdc6-1963353ff286.svg)

# About theHarvester
theHarvester is a very simple to use, yet powerful and effective tool designed to be used in the early stages of a penetration test or red team engagement. Use it for open source intelligence (OSINT) gathering to help determine a company's external threat landscape on the internet. The tool gathers emails, names, subdomains, IPs and URLs using multiple public data source.

# How to install it?
This is a by default tool in kali linux. So you just need to update the harvester tool.

For confirmation open terminal and type ‘theharvester’ and verify it. If  you see ‘command not found’ error raised continue to the installation process. Else skip the installation process.

# Installation:
In terminal type:

            $ sudo apt-get theharvester
If it doesn’t work you can try to clone it directly from git using the following commands

            $ git clone https://github.com/laramies/theHarvester.git
            $ cd theHarvester
            $ sudo pip3 install -r requirements.txt
            $ sudo python3 ./theHarvester.py
            
# Upgrading:
use the following command to upgrade the harvester

            $ sudo apt-get upgrade theharvester

# How to use this harvester tool ?

 root@kali:~# theHarvester -h
 
![173199264-f445ce77-8da7-4b4f-bef1-51ba4b72b408](https://user-images.githubusercontent.com/106522935/193582052-78b3514f-b3ab-411c-83e1-fd8dfd4fa9b3.png)

Usage:

       $ theHarvester [-h] -d DOMAIN [-l LIMIT] [-S START] [-g] [-p] [-s] [--screenshot SCREENSHOT] [-v] [-e DNS_SERVER [-t DNS_TLD] [-r] [-n] [-c] [-f FILENAME] [-b SOURCE]


 options:

    -h, --help            show this help message and exit
   
   
    -d DOMAIN, --domain DOMAIN [Company name or domain to search]
               
               
    -l LIMIT, --limit LIMIT [Limit the number of search results, default=500]
         
         
    -S START, --start START [Start with result number X, default=0]
    
    
    -g, --google-dork [Use Google Dorks for Google search]
   
   
    -p, --proxies [Use proxies for requests, enter proxies in proxies.yaml]
   
   
    -s, --shodan [Use Shodan to query discovered hosts]
   
   
    --screenshot SCREENSHOT [Take screenshots of resolved domains specify output directory: --screenshot output_directory]
                
                
    -v, --virtual-host [Verify host name via DNS resolution and search for virtual hosts]
                   
                   
    -e DNS_SERVER, --dns-server DNS_SERVER [DNS server to use for lookup]
                      
                      
    -t DNS_TLD, --dns-tld DNS_TLD [Perform a DNS TLD expansion discovery, default False]
                
                
    -r, --take-over [Check for takeovers]
   
   
    -n, --dns-lookup [Enable DNS server lookup, default False]
  
  
    -c, --dns-brute [Perform a DNS brute force on the domain]
    
    
    -f FILENAME, --filename FILENAME [Save the results to an XML and JSON file]
                       
                       
    -b SOURCE, --source SOURCE [anubis, baidu, bing, binaryedge, bingapi, bufferoverun, censys, certspotter, zoomeye
                               crtsh, dnsdumpster, duckduckgo, fullhunt, github-code, google, hackertarget, hunter,                                    
                               intelx, linkedin, linkedin_links, n45ht, omnisint, otx, pentesttools, projectdiscovery,                                
                               qwant, rapiddns, rocketreach, securityTrails, spyse, sublist3r, threatcrowd, yahoo, 
                               threatminer, trello, twitter, urlscan, virustotal]
                               
     

    -h: Use SHODAN database to query discovered hosts.

# Examples
To list available options
        
        
     To search emails : $ theHarvester.py -d abc.com -b all
        
     To search emails with a limit : $ theHarvester.py -d abc.com -b all -l 200
        
     To save the result into an html file : $ theharvester -d abc.com -b all -h myresults.html
        
     To search in PGP(Pretty Good Privacy) only : $ theharvester -d abc.com -b pgp     
