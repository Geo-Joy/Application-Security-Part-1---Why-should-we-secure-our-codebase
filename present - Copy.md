%title: Application Security Part 1 - Why should we secure our codebase
%author: Geo Joy
 

-> # Welcome <-


you have been
██████╗ ██╗    ██╗███╗   ██╗███████╗██████╗ 
██╔══██╗██║    ██║████╗  ██║██╔════╝██╔══██╗
██████╔╝██║ █╗ ██║██╔██╗ ██║█████╗  ██║  ██║
██╔═══╝ ██║███╗██║██║╚██╗██║██╔══╝  ██║  ██║
██║     ╚███╔███╔╝██║ ╚████║███████╗██████╔╝
╚═╝      ╚══╝╚══╝ ╚═╝  ╚═══╝╚══════╝╚═════╝ 


*** use the knowledge gained for ethical purposes only.

*** this presentation is to create awareness, 
	which i strongly believe will help the audience to 
	build a better / safe apps on the internet.

-------------------------------------------------------------------------

-> # About Me <-

  - [profile](profile.jpg)
  - [LinkedIn](https://linkedin.com/in/geojoy/)
  - into IT since 2009(12th grade) freelance works
  - professional experience since 2013 building a startup
  - Hobbies:
	- finding bugs, gaming, learn how others work on big companies.
  - technology timeline:
	- android, php, aws & DO, nodejs, hybrid mobile, blockchain, 
		mining & trading crypto, python, ML & AI, 
	- *cyber security*
  

-------------------------------------------------------------------------

-> # Why should we secure our code <-

  - open question!

-------------------------------------------------
  
-> # What motivates unethical hackers? <-

- Financial Gain
  - BTC, ETH, XMR

- Espionage
  - Political
  - Military documents

- Fun
  - Hacked by pages when it was trending
  - changing traffic light/messages

- Ideology
  - religion, economy

- Disruption
	- hacktivist
	- DDoS

- Control
	- internet-enabled devices

-------------------------------------------------
  
-> # What motivates *ethical* hackers? <-

# Hackers Weren't Always Bad...
## The term "hacker" usually carries negative connotations.

	- Often when hackers find security vulnerabilities in code, 
		they provide information to the organization that’s 
		who wrote the software. 

	- They help to fix the problem. 

	- Some companies are now even offering a 
		bounty reward to hackers who find bugs in their software.

	- Learn how different company design their database / API etc.

	- eg:


-------------------------------------------------
  
-> # What's the value of stolen data? how do they make money <-

	- Use the data themselves
		- Purchase items online
		- Extract money from your bank account
		- Pay off debt

	- Sell login credentials
		- Gaming platform accounts: $0.50-$12
		- Video and music streaming accounts: $0.10-$2
		- Cloud service accounts: $5-$10
		- Online banking accounts: 0.5%-10% of the account’s value

	- Sell PII/PHI to buyers on the black market
		- Medical notes and prescriptions: $15-$20
		- ID/passport scans or templates: $1-$35
		- Full ID packages (name, address, phone, 
			SSN, email, bank account): $30-$100.

	- Sell your credit card information $1-$45
	- Hold your data to ransom
	- Sell valuable intellectual property
	- Crypto mining - distributed malware

# data is often sold in enormous batches.
# attack multiple companies and create a portfolio of each users.

-------------------------------------------------

-> # Analysing Latest Data leaks <-

	* Facebook 533 Million
    	- Name, Mobile, Email-ID, Gender, Occupation, 
			City, Country, Marital Status ETC
			
		- News Articles
			- [Google](https://z.itsg.dev/3gGvTN8)
			- [Twitter](https://z.itsg.dev/3eAzWbe)
			
		- Impact
			- 103 counties
			- India 6,162,450
			
		- Dataset
			- [proof](fb-2.png)
			- [proof 2](fb.txt)
			- [sample](fb-1.png)

-------------------------------------------------

-> # Analysing Latest Data leaks <-

	* Dominos India 13TB
    	- internal files of 250 employees from IT, Legal, 
			Finance, Marketing, Operations etc. 
		- customers details and 180M order details 
		- 1M credit cards used to purchase
			
		- News Articles
			- [Google](https://z.itsg.dev/3t1Y2AP)
			- [Twitter](https://z.itsg.dev/3eHgqJU)
			
		- Impact
			- India
			- data range 2015-2021
			- outlook mail archives
			
		- Dataset
			- [proof](dominos-1.png)
			- [sample 1](1_loaded_dbs_stats.txt)
			- [sample 2](3_mongo_stats.txt)

-------------------------------------------------

-> # Analysing Latest Data leaks <-

	* Upstox India 13TB
		- One of the largest low-cost brokerage firms in India.
    	- Most of the user data including KYC document 
			with signatures & bank statements.
			
		- News Articles
			- [Google](https://z.itsg.dev/32U6lDV)
			- [Twitter](https://z.itsg.dev/2R7CkxM)
			
		- Impact
			- ~25 Lakh users
			- KYC data
			- Raw signatures
			
		- Dataset
			- [sample 1](upstox-1.png)
			- [sample 2](upstox-2.png)

-------------------------------------------------

-> # Analysing Latest Data leaks <-

	* Bigbasket 20Million
		- India's leading online supermarket.
    	- Complete User data
			
		- News Articles
			- [Google](https://z.itsg.dev/32XcNuc)
			- [Twitter](https://z.itsg.dev/3u6jfe8)
			
		- Impact
			- Use Cookies
			- GPS Location
			- Hashed passwords cracked 
				(mostly commonly used passwords)
			
		- Dataset
			- [sample 1](bb-1.png)
			- [sample 2](upstox-2.png)

-------------------------------------------------

-> # Analysing Latest Data leaks <-

	* Mobikwik 8TB - company hasn't acknowledge
		- Total 350GB mysql dumps - >500 dbs
		- 99 million - mail, phno, passwords, addresses, 
			apps installed, ip address, gps location
		- 40 million - 10 digit card, month, year, 
			card hash (sha256)
		- lots of dbs with all company data
		- ~7.5 TB of ~3 million Merchant KYC data - 
			passports, aadhaar, pan cards, selfie

		- Dataset
			- [sample 1](mobikwik.jfif)
			- [sample 2](mobikwik.png)

-------------------------------------------------
  
-> # What Techniques do attackers use? <-

	- [Attack Vectors](attack-1.jpg)
		- infected executables (.exe, .apk, .dmg ...)
		- infected npm, pip packages
		- cache injection - click jacking - image tags
		- MITM - HTTPS - TLS/SSL - HSTS (flaws in cryptography)
		- password + OTPs
	- [OWASP Overlaps](owasp_top-10_2017_risks_overlap.png)
	- [OWASP Top 10-2021 proposal](owasp_top-2021.png)
	- [Hackerone top 10](https://z.itsg.dev/3xAexY2)
	- [Shodan](https://z.itsg.dev/3vtm9d6)
	- [CVE - Common Vulnerabilities and Exposures](https://beta.shodan.io/)

	- [Wordpress - CVE-2021-29447](wordpress.mp4)
	- [OWASP TOP 10](https://z.itsg.dev/3nDeYMP)
	- OWASP Membership: geo.joy@owasp.org

	- *think like a hacker!*
	- *hack your own site*

-------------------------------------------------

-> # SSRF: Server Side Request Forgery <-

  - [SSRF Flow](SSRF-1.jpg)
  - the attacker might cause the server to make a connection back to itself, 
  	or to other web-based services within the organization's infrastructure, 
	or to external third-party systems.
``
POST /product/stock HTTP/1.0
Content-Type: application/x-www-form-urlencoded
Content-Length: 118

stockApi=http://stock.weliketoshop.net:8080/product/stock/check%3FproductId%3D6%26storeId%3D1
``

``
POST /product/stock HTTP/1.0
Content-Type: application/x-www-form-urlencoded
Content-Length: 118

stockApi=http://localhost/admin
``

-------------------------------------------------

-> # Where do they sell these stolen data? <-

	- clear net
	- dark net
		- [TOR](tor-net.png)
		- [Site sample](onion-sample-1.png)

-------------------------------------------------

-> # How can we protect ourselves <-

## there is no one answer

	- OWASP
		- countless resources
		- OWASP top 10
		- not just OWASP
	- security scanning
		- tools free and paid
		- dont just rely on these
			- lot of cons in these tools
		- manual test always
			- code review
			- overflow attacks
			- eg: crypto randomization issue	
	- Formalizing SDLC process
		- on every stage before going to production
	- Web Application Firewalls (WAF)
		- may detect pattern in attack 
			(exploit based on some vulnerability)
	- Independent security assesments
		- external review certificates
		- different point of view
		- red team strategy

-------------------------------------------------

-> # stats <-


 ▄▄▄▄▄▄▄▄▄▄▄   ▄▄▄▄▄▄▄▄▄           ▄
▐░░░░░░░░░░░▌ ▐░░░░░░░░░▌   ▄     ▐░
 ▀▀▀▀▀▀▀▀▀█░▌▐░█░█▀▀▀▀▀█░▌ ▐░▌   ▐░▌
         ▐░▌ ▐░▌▐░▌    ▐░▌  ▀   ▐░▌ 
        ▐░▌  ▐░▌ ▐░▌   ▐░▌     ▐░▌  
       ▐░▌   ▐░▌  ▐░▌  ▐░▌    ▐░▌   
      ▐░▌    ▐░▌   ▐░▌ ▐░▌   ▐░▌    
     ▐░▌     ▐░▌    ▐░▌▐░▌  ▐░▌   ▄ 
    ▐░▌      ▐░█▄▄▄▄▄█░█░▌ ▐░▌   ▐░▌
   ▐░▌        ▐░░░░░░░░░▌ ▐░▌     ▀ 
    ▀          ▀▀▀▀▀▀▀▀▀   ▀        
                                    

  - *vulnerabilities unpatched for more than 3 months*
  - *some go more than a year!*

-------------------------------------------------

-> # So who should do all these <-

	- EVERYONE!!!
	- *review each others code* :P

-------------------------------------------------

-> Thank you <-

``
  ██████ ▄▄▄█████▓ ▄▄▄      ▓██   ██▓     ██████  ▄▄▄        █████▒▓█████ 
▒██    ▒ ▓  ██▒ ▓▒▒████▄     ▒██  ██▒   ▒██    ▒ ▒████▄    ▓██   ▒ ▓█   ▀ 
░ ▓██▄   ▒ ▓██░ ▒░▒██  ▀█▄    ▒██ ██░   ░ ▓██▄   ▒██  ▀█▄  ▒████ ░ ▒███   
  ▒   ██▒░ ▓██▓ ░ ░██▄▄▄▄██   ░ ▐██▓░     ▒   ██▒░██▄▄▄▄██ ░▓█▒  ░ ▒▓█  ▄ 
▒██████▒▒  ▒██▒ ░  ▓█   ▓██▒  ░ ██▒▓░   ▒██████▒▒ ▓█   ▓██▒░▒█░    ░▒████▒
▒ ▒▓▒ ▒ ░  ▒ ░░    ▒▒   ▓▒█░   ██▒▒▒    ▒ ▒▓▒ ▒ ░ ▒▒   ▓▒█░ ▒ ░    ░░ ▒░ ░
░ ░▒  ░ ░    ░      ▒   ▒▒ ░ ▓██ ░▒░    ░ ░▒  ░ ░  ▒   ▒▒ ░ ░       ░ ░  ░
░  ░  ░    ░        ░   ▒    ▒ ▒ ░░     ░  ░  ░    ░   ▒    ░ ░       ░   
      ░                 ░  ░ ░ ░              ░        ░  ░           ░  ░
                             ░ ░                                          
``

