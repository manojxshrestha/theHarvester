### theHarvester

### About theHarvester
theHarvester is a very simple to use, yet powerful and effective tool designed to be used in the early stages of a penetration test or red team engagement. Use it for open source intelligence (OSINT) gathering to help determine a company's external threat landscape on the internet. The tool gathers emails, names, subdomains, IPs and URLs using multiple public data sources.

### How to install it?
This is a by default tool in kali linux. So you just need to update the harvester tool.

For confirmation open terminal and type ‘theharvester’ and verify it. If  you see ‘command not found’ error raised continue to the installation process. Else skip the installation process.

### Installation:
In terminal type:

            sudo apt-get theharvester
If it doesn’t work you can try to clone it directly from git using the following commands

            git clone https://github.com/laramies/theHarvester.git
            cd theHarvester
            sudo python ./theHarvester.py
### Upgrading:
use the following command to upgrade the harvester

  sudo apt-get upgrade theharvester
