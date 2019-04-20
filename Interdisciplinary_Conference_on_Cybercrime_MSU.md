## [Interdisciplinary Conference on Cybercrime](https://cj.msu.edu/programs/interdisciplinary-conference-cybercrime/)

### The 6th Annual Michigan State University Interdisciplinary Conference on Cybercrime

#### April 15th and 16th, 2019 (8:30am – 5pm)

#### Day 1

##### Speaker: Dr. Thomas Holt

- The left ideologies moving towards cyberattacks
- For a while, we noticed a decrease in physical attacks (and wondered if that was due to the Obama administration)
- However, there may be a cyber element to the decrease in physical attackers (maybe the attackers are now moving towards cyberattacks instead)
- ALF and Anonymous are two left groups
- Target is small or medium businesses
- Large organizations still see the bulk of the attacks
- example of an attack is the attack in support of Harambe by Anonymous
- Anonymous going after the Department of Agriculture
- Hudson Valley Foie Gras faces attacks by left ideologists
- We do not have a lot of detail about DDoS attacks
- Doxxing of the guy who won an auction to hunt a rhino 
  - Focus on making this person have a seizure by doxxing relevant medical information
- What came first for these attackers: hacking or ideologies?

> Were they hackers first who developed ideologies or were they ideologists who acquired hacking skills?

- How does recruitment for hacking happen in the left?
- Identify online behavioral patterns to recognize radical left or right (technically it is possible, legally, not really)

##### Speaker: Dr. Betty Cheng

- Autonomous mobility ecosystem
- In a few years, we will achieve level 4 or level 5 autonomy
- Is this exciting or scary?
- connected cars: communication between cars can become a security problem
- this communication is complex; there are many sensors, AI, training data

> Wired video of compromising a Jeep Cherokee video

> Link to study automobile vulnerabilities: [link](https://www.upstream.auto/)

- Number of attacks on automobiles have risen
1. Threat analysis
2. Develop a model targeting malicious actors
3. Criminological theory
- Prevention, detection, mitigation
- Concerns:
  1. Safety
  2. Information
  3. Stakeholders
  
- Threat:
  1. Interruption
  2. Interception
  3. Modification
  4. Fabrication
  
- 25 techniques of situational prevention
- SCP applied to cybersecurity
- Traditional security has lots of computation; cannot be done vehicle (wouldn't want to drive at 35 mph)
- Cars were built for safety, not cybersecurity

> While ABS braking, you cannot have your car thinking whether that's a trusted request

- OTA updates -> convenience versus safety

> We still don't have a lot of data to understand the range of vulnerabilities

- Automotive industry is competitive. How do OEMs, suppliers, and everyone work together?
- First steps:
  - Map the threat surface
  - How much knowledge do you need to attack?
  - Do you need physical access?
  - What kind of impact?
  
- Threat surfaces:
  - OBD2 port
  - Key fob
  - Media player
  - Dealer pass-through
  
> Key fob attacks are the only vehicle cyberattacks that we have seen in the wild

- The motivation for criminals to perform the key fob attack is immediate gratification (steal the vehicle)
- Security design patterns
- Security certification of autonomous systems

##### Speaker: Mr. Nils Kessler

- Build logs into your system by law and an entity cannot say 'no' to law officers requesting logs
- Easier to do in countries such as China which is an authoritarian state

> We are going to do it or we will throw you out. On the other hand, we must convince a lot of people.

- These days organizations are observed saying "we're the privacy guys, we don't do it (provide logs to law enforcement)"
- The argument against providing backdoors is "if we install a backdoor, bad guys can access it too"
- San Bernardino iPhone case. 
- Motive: cause damage to computer system. Example: stance against animal cruelty
- Ransomware:
  1. Publish sensitive information
  2. Destroy critical information
  3. Deny access to the system
  
- Motive: DDoS attacks
- Motive: Data theft
- Theft of PII (Personally Identifiable information)
- Theft of IP (Intellectual Property)
  - Example: trade secret of steel manufacturing company

> Follow the money

- Example: wire transfer, trace the bank records
  - lot harder in the case of ransomware
  - no bread crumbs anymore
  - easier to cyberattack from outside of the United States
  - harder to get cooperation from foreign governments
  
- Carding schemes
- Fraud schemes:
  - romance scheme
  - investment scams
  - elderly fraud
    - elderly are mostly vulnerable because of the time they grew up in (more implicit trust)
    
- Sex-tortion (compromising material)
  - younger people are more vulnerable
  - younger people tend to overshare on social media
  
- Stalking and harassment
- Doxxing
- Book recommendation: `Midnight in Chernobyl`
- IoT security (Ring doorbell)

> Everything is integrated with the network

- Social engineering (not so technical)
  -example scenario: phone rings, number identified on phone as bank, doesn't jump right into asking for private info, you think it's legit, 5 minutes deep asks for PIN number, transfers a huge amount of money after hanging up.
  
> Not everything (that pops up) on your phone is authentic 

- Business email compromise (BEC)
  - example: vulnerability inside Outlook as installed straight out-of-the-box makes it easier to get inside.
  - scenario: email coming from supervisor asking to authorize wire transfer to a vendor. The vender is a shell company.
  - rules are set up such that the email alert never shows up.
  
- Introducing malware

> Security does not matter if somebody has already got a keylogger in

- Botnets: turn zombies to perform DDoS
- Hop point: basically, a proxy between your computer and the attacker's computer
- RAT (trojan)

#### Day 2

##### Mr. Douglas McKee

- ATR (threat research team discovering 0-days)
- Team consists of reverse engineering, threat hunting, general security experts (e.g. an expert in cryptocurrency)
- Why do vulnerability research?
  - discover weaknesses that can be exploited
  - hold vendors accountable
  - keep the bad guys in check (bad guys generally have more time to discover security flaws)
  - bring awareness in the industry

> minor flaws can have major impact!

- Example: medical systems, surveillance software
- Responsible disclosure:
  - software - 90 days
  - hardware - 180 days
  - > goal is not to expose vendors
  - different timelines for critical systems
  - example: IoT device, automotive, malware operation
  
- Hacking patient vitals
- could directly impact human life
- vitals are integrated into critical decision making
  - example: heartrate, O2 level
- influencing vitals is highly impactful

> We have implicit trust - Dr. Jess Tully

- communication between patient monitor and CMS
- they create their own protocol -- this is a problem
  - no authentication, no encryption, traffic is broadcasted
  
> demo of the hack

- people doubt the impact of this hack since you have to be on the same broadcast network
  - you can easily get inside waiting rooms
  - in some cases, guest network is where medical devices are connected as well
  - nurses can walk away without locking their workstations
  
> treatment that you don't need is probably not a good treatment

- doctors can do an inside job for an insurance fraud

IoT
- Wemo insight smart plug
- fuzzing caused a crash
- 2 months of exploitation to exploit a buffer overflow
- can only send some printable XML because of UpNp limitations
- WiFi: crack the WPA2 password, perform recon on the network, find Wemo, use exploit
- UpNp for opening a port on the router
- lesson: don't put consumer electronics on business network

Box lock
- features: unlock via barcode scanner or via mobile application
- requires WiFi
- hardware interface: JTAG
- JTAG was secure
- BLE: had no encryption or authentication
- all fields are r/w enabled
- reversed the Android app and discovered the 'sendopenSignal'
- Nordic app
- unlock box

> lesson: security has not kept up with the explosion in connectivity

- we need to keep an eye on what vendors are allowed to produce
- compliance should not be just to pass a test
- lots security products and solutions. We should not get caught up with false sense of security

#### Speaker: Mr. Joshua Dalman

- RDP-based ransomware

> Demo of restore point to get deleted files back

- Top trends in 2019:
  - ransomware
  - business email compromise
 
- 12.5 billion in losses from 2013 - 2018 due to business email compromise
- Docusign (phishing link)
- creating the auto forward rule in Outlook
- Trick finance department into wiring money to the hacker's account
- Nation state Iranian threat actors
- prevent business email compromise:
  - audit logging
  - user awareness
  - multi factor authentication
  - perform internal checks for accounts
  
- Office 365 logs (unified audit log)
- acquire audit logs through portal.office.com
  - 50,000 limit
  - powershell

- Splunk primer
  - geo-location
  - visualization
  - JSON blob import
  
- compromised user can be looked at with land speed violations
  - example: somebody traveling at 450 mph
 
- did the attacker download PII? Look at trace logs.

- What is ransomware?
- attack vectors: RDP, phishing etc.
- cryptolocker
- email-based ransomware
  - cryptolocker
  - locky
  - scarab
  - sigma
 
- if you have backups, you might be able to just wipe the system and reinstall the OS
- sigma ransomware: attacker sends a password protected document, it prompts to enable the macro, encrypts files and demands $400 in ransom. This ransomware also seeks to encrypt network shares
- RDP-based ransomware looking to exploit port 3389
  - easy to discover 1.8 million systems with RDP exposed on the Internet
- Samsam (RDP-based), uses an AES matrix
  - Ransomware-as-a-service
  - demands large ransom amount from the city of Atlanta
  - generated $5.9 million in total payments
  - developers were Iranian hackers (extradition becomes tricky)
  
- Dharma ransomware
  - has a long dwell time
  - comparatively script kiddies
  - run everything from romance scams to spams

- protection against ransomware
  - disable RDP if not needed
  - use VPN
  - use MFA
  - use strong passwords
  - good email security (examine attachments)
  - user awareness and training
  - disable smb1
  - if threat is found, quickly isolate the machine
  - keep offline backups
  
#### Speaker: Dr. Cassandra Cross

- Reporting cybercrimes in Australia
- Overview of ACORN (Australian cybercrime online)
- Reporting network:
  - online scams
  - cyber bullying
  - online buying and selling
  
- online, self-reporting
- UK equivalent (Action Fraud)
- ACORN by ACIC (federal agency)
- objective:
  - central online agency
  - refer to police
  - collect and aggregate database

- issues observed:
  - reporting at multiple places
  - little change in public awareness
  - low satisfaction with the outcome
  
- evaluation results:
  - victims have unrealistic expectations
  - victims feel they are unique, but you're dealing with thousands of other victims
  - only 3 victims said that their offender was arrested
  - victims were using the portal to get some attention to their issues
  - there are challenges on the police and law enforcement side 


##### Speaker: Mr. Seth Edgar

- top 3 security trends:
  - email scams
  - web apps
  - end point
  
- university is a collection of a lot of businesses
- out of the 200 million emails received in a month, 177 are spam
- Since the days of ARPANET, we have publicly routed IPs at MSU
  - everyone is able to put up a web server on these IPs that MSU has to clean up
  
- researchers have grants that require legacy systems up and running
- security for such heterogenous devices is difficult at scale
- security trends at MSU:

  | Trends | Statistics |
  | ------ | ------ |
  | Vulnerability remediation | 156,309 |
  | Antivirus | 21,012 |
  
> all data is meant to be available everywhere implies a massive cleanup effort

- identify high value assets
- data threats:
  - loss
  - theft
  - exposure
  - modification
  
- prioritization:
  - severity
  - probability
  - delivery
  - tactics
  
- MSU is a collection of number of industries and threats faced are hence multidimensional

   
