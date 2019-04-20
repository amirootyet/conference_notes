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
- Example of an attack is the attack in support of Harambe by Anonymous
- Anonymous going after the Department of Agriculture
- Hudson Valley Foie Gras faces attacks by left ideologists
- We do not have a lot of detail about DDoS attacks
- Doxxing of the guy who won an auction to hunt a rhino 
  - Focus on making this person have a seizure by doxxing relevant medical information
- What came first for these attackers: hacking or ideologies?

> Were they hackers first who developed ideologies or were they ideologists who acquired hacking skills?

- How does recruitment for hacking happen in the left?
- Identify online behavioral patterns to recognize radical left or right (technically it is possible, legally, not really)

* * *

##### Speaker: Dr. Betty Cheng

- Autonomous mobility ecosystem
- In a few years, we will achieve level 4 or level 5 autonomy
- Is this exciting or scary?
- Connected cars: communication between cars can become a security problem
- This communication is complex; there are many sensors, AI, training data

> Wired video of compromising a Jeep Cherokee video

> [Link](https://www.upstream.auto/) to study automobile vulnerabilities

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

* * *

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
  - Lot harder in the case of ransomware
  - No bread crumbs anymore
  - Easier to cyberattack from outside of the United States
  - Harder to get cooperation from foreign governments
  
- Carding schemes
- Fraud schemes:
  - Romance scheme
  - Investment scams
  - Elderly fraud
    - Elderly are mostly vulnerable because of the time they grew up in (more implicit trust)
    
- Sex-tortion (compromising material)
  - Younger people are more vulnerable
  - Younger people tend to overshare on social media
  
- Stalking and harassment
- Doxxing
- Book recommendation: `Midnight in Chernobyl`
- IoT security (Ring doorbell)

> Everything is integrated with the network

- Social engineering (not so technical)
  -Example scenario: phone rings, number identified on phone as bank, doesn't jump right into asking for private info, you think it's legit, 5 minutes deep asks for PIN number, transfers a huge amount of money after hanging up.
  
> Not everything (that pops up) on your phone is authentic 

- Business email compromise (BEC)
  - Example: vulnerability inside Outlook as installed straight out-of-the-box makes it easier to get inside.
  - Scenario: email coming from supervisor asking to authorize wire transfer to a vendor. The vender is a shell company.
  - Rules are set up such that the email alert never shows up.
  
- Introducing malware

> Security does not matter if somebody has already got a keylogger in

- Botnets: turn zombies to perform DDoS
- Hop point: basically, a proxy between your computer and the attacker's computer
- RAT (trojan)

* * *

* * *

#### Day 2

##### Mr. Douglas McKee

- ATR (threat research team discovering 0-days)
- Team consists of reverse engineering, threat hunting, general security experts (e.g. an expert in cryptocurrency)
- Why do vulnerability research?
  - Discover weaknesses that can be exploited
  - Hold vendors accountable
  - Keep the bad guys in check (bad guys generally have more time to discover security flaws)
  - Bring awareness in the industry

> Minor flaws can have major impact!

- Example: medical systems, surveillance software
- Responsible disclosure:
  - Software - 90 days
  - Hardware - 180 days
  
  > Goal is not to expose vendors
  
  - Different timelines for critical systems
  - Example: IoT device, automotive, malware operation
  
- Hacking patient vitals
- Could directly impact human life
- Vitals are integrated into critical decision making
  - Example: heartrate, O2 level
- Influencing vitals is highly impactful

> We have implicit trust - Dr. Jess Tully

- Communication between patient monitor and CMS
- They create their own protocol -- this is a problem
  - No authentication, no encryption, traffic is broadcasted
  
> Demo of the hack

- People doubt the impact of this hack since you have to be on the same broadcast network
  - You can easily get inside waiting rooms
  - In some cases, guest network is where medical devices are connected as well
  - Nurses can walk away without locking their workstations
  
> Treatment that you don't need is probably not a good treatment

- Doctors can do an inside job for an insurance fraud

IoT
- Wemo insight smart plug
- Fuzzing caused a crash
- 2 months of exploitation to exploit a buffer overflow
- Can only send some printable XML because of UpNp limitations
- WiFi: crack the WPA2 password, perform recon on the network, find Wemo, use exploit
- UpNp for opening a port on the router
- Lesson: don't put consumer electronics on business network

Box lock
- Features: unlock via barcode scanner or via mobile application
- Requires WiFi
- Hardware interface: JTAG
- JTAG was secure
- BLE: had no encryption or authentication
- All fields are r/w enabled
- Reversed the Android app and discovered the 'sendopenSignal'
- Nordic app
- Unlock box

> Lesson: security has not kept up with the explosion in connectivity

- We need to keep an eye on what vendors are allowed to produce
- Compliance should not be just to pass a test
- Lots security products and solutions. We should not get caught up with false sense of security

* * *

#### Speaker: Mr. Joshua Dalman

- RDP-based ransomware

> Demo of restore point to get deleted files back

- Top trends in 2019:
  - Ransomware
  - Business email compromise
 
- 12.5 billion in losses from 2013 - 2018 due to business email compromise
- Docusign (phishing link)
- Creating the auto forward rule in Outlook
- Trick finance department into wiring money to the hacker's account
- Nation state Iranian threat actors
- Prevent business email compromise:
  - audit logging
  - User awareness
  - Multi factor authentication
  - Perform internal checks for accounts
  
- Office 365 logs (unified audit log)
- Acquire audit logs through portal.office.com
  - 50,000 limit
  - Powershell

- Splunk primer
  - Geo-location
  - Visualization
  - JSON blob import
  
- Compromised user can be looked at with land speed violations
  - Example: somebody traveling at 450 mph
 
- Did the attacker download PII? Look at trace logs.

- What is ransomware?
- Attack vectors: RDP, phishing etc.
- Cryptolocker
- Email-based ransomware
  - Cryptolocker
  - Locky
  - Scarab
  - Sigma
 
- If you have backups, you might be able to just wipe the system and reinstall the OS
- Sigma ransomware: attacker sends a password protected document, it prompts to enable the macro, encrypts files and demands $400 in ransom. This ransomware also seeks to encrypt network shares
- RDP-based ransomware looking to exploit port 3389
  - Easy to discover 1.8 million systems with RDP exposed on the Internet
- Samsam (RDP-based), uses an AES matrix
  - Ransomware-as-a-service
  - Demands large ransom amount from the city of Atlanta
  - Generated $5.9 million in total payments
  - Developers were Iranian hackers (extradition becomes tricky)
  
- Dharma ransomware
  - Has a long dwell time
  - Comparatively script kiddies
  - Run everything from romance scams to spams

- Protection against ransomware
  - Disable RDP if not needed
  - Use VPN
  - Use MFA
  - Use strong passwords
  - Good email security (examine attachments)
  - User awareness and training
  - Disable smb1
  - If threat is found, quickly isolate the machine
  - Keep offline backups
  
* * *
  
#### Speaker: Dr. Cassandra Cross

- Reporting cybercrimes in Australia
- Overview of ACORN (Australian cybercrime online)
- Reporting network:
  - Online scams
  - Cyber bullying
  - Online buying and selling
  
- Online, self-reporting
- UK equivalent (Action Fraud)
- ACORN by ACIC (federal agency)
- Objective:
  - Central online agency
  - Refer to police
  - Collect and aggregate database

- Issues observed:
  - Reporting at multiple places
  - Little change in public awareness
  - Low satisfaction with the outcome
  
- Evaluation results:
  - Victims have unrealistic expectations
  - Victims feel they are unique, but you're dealing with thousands of other victims
  - Only 3 victims said that their offender was arrested
  - Victims were using the portal to get some attention to their issues
  - There are challenges on the police and law enforcement side 

* * *

##### Speaker: Mr. Seth Edgar

- Top 3 security trends:
  - Email scams
  - Web apps
  - End point
  
- University is a collection of a lot of businesses
- Out of the 200 million emails received in a month, 177 are spam
- Since the days of ARPANET, we have publicly routed IPs at MSU
  - Everyone is able to put up a web server on these IPs that MSU has to clean up
  
- Researchers have grants that require legacy systems up and running
- Security for such heterogenous devices is difficult at scale
- Security trends at MSU:

  | Trends | Statistics |
  | ------ | ------ |
  | Vulnerability remediation | 156,309 |
  | Antivirus | 21,012 |
  
> All data is meant to be available everywhere implies a massive cleanup effort

- Identify high value assets
- Data threats:
  - Loss
  - Theft
  - Exposure
  - Modification
  
- Prioritization:
  - Severity
  - Probability
  - Delivery
  - Tactics
  
- MSU is a collection of number of industries and threats faced are hence multidimensional

   
