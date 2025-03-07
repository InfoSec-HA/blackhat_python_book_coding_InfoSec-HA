# Code and exercises from the book "Black Hat Python: Python Programming for Hackers and Pentesters", refactored and ported to Python 3 
Examples, source code and exercises from the book "Black Hat Python" by Justin Seitz.

![](https://img.shields.io/github/stars/carloocchiena/blackhat_python_book_code?style=social)

![](https://img.shields.io/tokei/lines/github/carloocchiena/blackhat_python_book_code)

![image](https://user-images.githubusercontent.com/57464184/138901408-984413ab-2648-4dbe-b40c-37ac7b59fc63.png)

--------------------------------
### About the book
The book is a milestone for pentesting with Python.<br>
Although its publication is quite recent (2014), it is all written in Python 2.7.<br>

You can find the book on <a href="https://www.amazon.it/Black-Hat-Python-Programming-Pentesters-ebook/dp/B00QL616DW#customerReviews">Amazon</a>, 
while the official book page is on <a href="https://nostarch.com/black-hat-python2E#updates">No Starch Press</a> website.<br>

You should be able to download the book's source code from here http://www.nostarch.com/download/BHP-Code.zip, but apparently the link is broken or the file has been deleted (checked October 2021).<br>
Please note that I did the whole job straight from book pages with no codes available (and believe me, my nearsightedness did not appreciate XD).<br>

No Starch Press is offering also an Errata Corrige on the book code, but at the moment (November 2021) this section is actually 3 rows long :).

--------------------------------

### Reason for this repo
I quite enjoyed the book, but as 2021 it looks quite outdated, not just for the choice of using Python 2.7.<br>

Deliberately, as expressed by the author, the scripts are written _rought & dirty_ to simulate the approach he uses during a penetration testing.<br>
However, this sometimes leads to code that is not very understandable, and not very efficient.<br>

Since I had to convert all the source codes anyway, to run them on my machine (Kali Linux VM + Win10 OS + Win10 VM + Python 3.9) I decided to go extra-mile and save them in a repo, in the meantime trying to optimize the code and making it a little more elegant (see below).

The code in the book does not always run flawlessy. It may depends on the local configuration on your machine, the test you are running, and also, outdated code presented in the book. So expect a bit of tweak here and there.<br> As a rule of thumb I found of great help the many <a href="https://stackoverflow.com/search?q=black+hat+python+book">threads already opened on Stack Overflow</a>.<br> 
Some good advices also from <a href="https://medium.com/search?q=black%20hat%20python">Medium Black Hat Python</a>.<br>
I also starred this repo from EONRaider for reference, that I might use in the case I'll be getting stuck:
<a href="https://github.com/EONRaider/blackhat-python3">EON RIDER Repo</a>.

--------------------------------

### Improvement made from the book's code
- Refactoring to Python 3 and code testing (unless otherwise specified)
- Update to PEP8 standards
- Upgraded readability (es. comments, indentation, variable names, file names)
- Update of obsolete methods (es. print -s %)
- Better context management (es. open with, server.close()) 
- Disregard of unsupported libs 
- Minor tweaks and bugs found while testing the code 
- Search for additional files requested throughout the book and not provided, or provided at outdated links, and included in individual chapters
- Additional information and resources that I searched for and found useful as I made my way through the book

--------------------------------

### What you'll find in the repo
Chapter summary and titles are my own, for clarity. The book uses different titles and has no chapter summary.<br>
When needed, an additional `README.md`has been added inside each chapter folder for clarification and further details. 

#### Chapter 1: Intro
- This is an introductory chapter and it's mostly about installing Linux VM and Python. No coding here.

#### Chapter 2: Networking Basics
- bhp_net.py
- bhp_server.py
- bhp_reverse_ssh_cmd.py
- bhp_ssh_cmd.py
- rforward.py
- tcp_server.py
- tcp_client.py
- tcp_proxy.py
- udp_client.py
- test_rsa.key

#### Chapter 3: Sniffing Tools
- scanner.py
- sniffer.py
- sniffer_ip_header_decode.py
- sniffer_with_icmp.py

#### Chapter 4: Scapy & ARP Poisoning (with an extra flavour of image reco)
- arper.py
- mail_sniffer.py
- pic_carver.py

#### Chapter 5: CMS Brute Force
- content_bruter.py
- joomla_killer.py
- web_app_mapper.py
- wordpress_killer.py

#### Chapter 6: Burp Suite Integrations 
- bhp_bing.py
- bhp_fuzzer.py
- bhp_wordlist.py

#### Chapter 7: GitHub Trojan
- folder structure
- git_trojan.py

#### Chapter 8: Trojan for Windows OS
- keylogger.py
- sandbox_detector.py
- screenshotter.py
- shell_exec.py

#### Chapter 9: Hacking thru Internet Explorer
- cred_server.py
- decryptor.py
- ie_exfil.py
- keygen.py
- mitb.py

#### Chapter 10: Windows Process Monitoring and File Injection
- file_monitor.py
- process_monitor.py

#### Chapter 11: Windows Forensics
- grab_hashes.py
- code_coverage.py
- grab_hashes.py

--------------------------------

### Contributions
All contributions are welcome :).<br>
Since I have not (yet?) made a specific routine for that, please follow a best-practice, common-sense based approach, opening an Issue first and starting a discussion on the change you'd wish to make.<br>
As a starting point, in each chapter folder I stated any known issues if any. <br>
A list of contributor will be displayed in the README of the repository.
