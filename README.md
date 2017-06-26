# LFI-sploit
# Simple Local File Inclusion Exploiter, version 1.2
# by r0otz-ee
 
# ASCII FOR BREAKFAST
 
# ---------- [Description]
# This tool helps you to exploit LFI (Local File Inclusion) vulnerabilities.
# After you found a LFI vulnerability simply pass the affected URL
# and vulnerable parameter to this tool.
# You can also use this tool to scan a URL for LFI vulnerabilities.
 
# ---------- [Features]
# - This time with working random user agents ^_^
# - Checks if a connection to the target can be established
# - Some error handling
# - Scans a parameter of a URL for a LFI vulnerability
# - Finds out how a LFI vulnerability can be exploited (e.g. directory depth)
# - Supports nullbytes
# - Dumps a list of interesting files (e.g. /etc/passwd and logs) to the hard disk
# - Supports common *nix targets, but no Windows systems.
# - Creates a small log file.
# Supports no SEO URLs, such as www.example.com/local-news/
# But in most cases it is possible to find out the real URL and pass it to this script.
 
# ---------- [Usage example]
# ./lfi_sploiter.py --exploit-url="http://www.example.com/page.php?url=main" --vulnerable-parameter="url"
# The tool then assumes that the parameter "url" is vulnerable and attacks the target.
# When you do not know which parameter is vulnerable simply try one parameter after another,
# this tool will scan the parameter and tell you if it is vulnerable :) But only pass one parameter at once!
 
# ---------- [Known issues]
# - I know there is more about LFI than it is covered in this tool. But this is the first release,
#   and more features will be implemented in future versions.
# - This tool is only able to handle "simple" LFI vulnerabilities, but not complex ones.
#   For example: Some LFI vulnerabilities consist of two URL parameters or require to
#   find a way around filters. In those cases, this tool unfortunately does not work.
# - Like most other LFI exploiter / scanner, this tool here also has problems with
#   handling certain server responses. So this tool does not work with every website.
 
# ---------- [Tested with]
# Targets: Apache2 servers and PHP websites, various Linux systems
# Script platform: Ubuntu Lucid Lynx and Python 2.6.5
 
# ---------- [Notes]
# - This tool was developed using a Python 2.6.5 interpreter.
# - I admit: This tool is a little bit slow and not very efficient (too many variables etc.). Sorry about that :P
# - Modify, distribute, share and copy this code in any way you like!
# - Please note that this tool was created and published for educational purposes only, e.g. for pentesting
#   your own website. Do not use it in an illegal way and always know + respect your local laws.
#   I am not responsible if you cause any damage with it.
 
# ---------- [Changelog]
# - Version 1.2 :
#  - Added some more "interesting files"
#
# - Version 1.1 (23th November 2010):
#   - Added new log file <domain name>-details.txt which contains some information about the current scan
#   - Added some more "interesting files"
#   - Added some more user agents
#
# - Version 1.0 :
#    - Initial release
 
# Power to the lulz!
