# GoldmanSachs-Virtual-Programme
This repo contains my report for GoldmanSachs Password Cracking task I started 3 weeks ago.

##The Task:
> As a governance analyst it is part of your duties to assess the level of protection offered by implemented controls and minimize the probability of a successful breach. To be successful at your job you often need to know the techniques used by hackers to circumvent implemented controls and propose uplifts to increase the overall level of security in an organization. Gaining valid credentials gives the attackers access to the organization’s IT system, thus circumventing most of perimeter controls in place.

###Your job is to crack as many passwords as possible with available tools `(e.g. use Hashcat)`. Here are your Task instructions:
* Review the links provided in the additional resources below to gain a background understanding of password cracking
* Try to crack the passwords provided in the 'password dump' file below using available tools
* Assess the 5 questions in the task instructions below in relation to the passwords provided (type of hashing algorithm, level of protection, possible controls that could be implemented, password policy, changes in policy)
* Draft an email/memo briefly explaining your findings in relation to controls used by the organization and your proposed uplifts.

###You must determine the following:
* What type of hashing algorithm was used to protect passwords?
* What level of protection does the mechanism offer for passwords?
* What controls could be implemented to make cracking much harder for the hacker in the event of a password database leaking again?
* What can you tell about the organization’s password policy (e.g. password length, key space, etc.)?
* What would you change in the password policy to make breaking the passwords harder?

##Resources:
<a href="https://cdn.theforage.com/vinternships/companyassets/MBA4MnZTNFEoJZGnk/passwd_dump.txt" target="_blank">Password Dump.txt</a>
```
experthead:e10adc3949ba59abbe56e057f20f883e
interestec:25f9e794323b453885f5181f1b624d0b
ortspoon:d8578edf8458ce06fbc5bb76a58c5ca4
reallychel:5f4dcc3b5aa765d61d8327deb882cf99
simmson56:96e79218965eb72c92a549dd5a330112
bookma:25d55ad283aa400af464c76d713c07ad
popularkiya7:e99a18c428cb38d5f260853678922e03
eatingcake1994:fcea920f7412b5da7be0cf42b8c93759
heroanhart:7c6a180b36896a0a8c02787eeafb0e4c
edi_tesla89:6c569aabbf7775ef8fc570e228c16b98
liveltekah:3f230640b78d7e71ac5514e57935eb69
blikimore:917eb5e9d6d6bca820922a0c6f7cc28b
johnwick007:f6a0cb102c62879d397b12b62c092c06
flamesbria2001:9b3b269ad0a208090309f091b3aba9db
oranolio:16ced47d3fc931483e24933665cded6d
spuffyffet:1f5c5683982d7c3814d4d9e6d749b21e
moodie:8d763385e0476ae208f21bc63956f748
nabox:defebde7b6ab6f24d5824682a16c3ae4
bandalls:bdda5f03128bcbdfa78d8934529048cf
```

#The Report:

Dear Sir/Maam,

I would like to inform you about the multiple weaknesses I found in your password policy when trying to decode all the stolen passwords from the password dump, and this email summarizes my findings and offers recommendations on how to strengthen your password policy.
Message Digest (MD5) and Secure Hash Algorithm (SHA) are the two most widely used cryptographic hash functions for data security and authentication. All of the leaked passwords were generated using MD5, a less secure hashing algorithm that is prone to collisions.
With the help of Hashcat.com and the wordlist rockyou.txt, it was relatively simple to break using a terminal and online browser. We can also conclude that the minimum length for password is set to 6 and there is no specific requirement for the password creation.

Your password policy can now have these recommended additions:
- avoid well-know or common terms and letter combinations
- make the passwords longer, and include special characters, numbers, capital and small letter
- avoid reusing the same passwords across different platforms
- avoid using usernames, Real name, date of birth, or other obvious information in passwords 


The cracked passwords:

experthead:e10adc3949ba59abbe56e057f20f883e - 123456
interestec:25f9e794323b453885f5181f1b624d0b - 123456789
ortspoon:d8578edf8458ce06fbc5bb76a58c5ca4 - qwerty
reallychel:5f4dcc3b5aa765d61d8327deb882cf99 - password
simmson56:96e79218965eb72c92a549dd5a330112 - 111111
bookma:25d55ad283aa400af464c76d713c07ad - 12345678
popularkiya7:e99a18c428cb38d5f260853678922e03 - abc123
eatingcake1994:fcea920f7412b5da7be0cf42b8c93759 - 1234567
heroanhart:7c6a180b36896a0a8c02787eeafb0e4c - password1
edi_tesla89:6c569aabbf7775ef8fc570e228c16b98 - password!
liveltekah:3f230640b78d7e71ac5514e57935eb69 - qazxsw
blikimore:917eb5e9d6d6bca820922a0c6f7cc28b - Pa$$word1
johnwick007:f6a0cb102c62879d397b12b62c092c06 - bluered



Thanking You,

Arindal Char

B.Tech Computer Science Undergraduate

