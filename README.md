<h1 align="center">Honeywords Generators</h1>

## **What	are	honeywords**
<br>

Honeywords	are	a	defense	against	stolen	password	files.	
Specifically,	they are	bogus	passwords	placed	in	the	password	file	of	an	authentication	server to	deceive	attackers.	
Honeywords resemble	ordinary,	user-selected	passwords.	
It’s hard	therefore	for	an	attacker	that steals	a	honeyword-laced password	file	to	
distinguish	between	honeywords	and	true user passwords.	

“Honey” is	an	old	term for	decoy	resources in	computing	environments.	



## **How honeywords protects us?**

<br>
To be more specific about how honeywords protect us, without we even know about them, let's see the table below and explain it a lit bit more.

Before we begin, make sure that is an implementation for only a random user. 

If we have more users, we have to do the exact same for each one.

As you can view, in the left column, we have the fake passwords, that our honeywords generator assumes that created for us, or in other words, these are the honeywords we are going to use.

In the middle column, in a random row, we can view the real password of the user and finally, in the right column, we can view the final dataset of passwords for the user.

#### <h1 align="center">
  
Fake Passwords | Real Password | Final Passwords
------------   | ------------  | ------------ |
kebrton1       |               |    kebrton1  |
02123dia       |               |    forlinux  |
a71ger         |               |    avanture32|
forlinux       |    Arkantos   |    sbgo864959|
1erapc         |               |    02123dia  |
avanture32     |               |    Arkantos  |
sbgo864959     |               |    aiwkme523 |
aiwkme523      |               |    1erapc    |
   <br>        |      <br>     |    a71ger    |
  
</h1>


## **Now, it's time for us to understand how honeywords actually work.**
<br>

Before we move on, we need to understand that honeywords aren’t visible to users or anyone else and that they are created by a generator we have chosen before. 
The generator creates the honeywords, then the honeychecker shuffle them all together and then save all the possible passwords for each user.
That's why they are so powerful and crucial in cyber security.
Some generators create honeywords based on the real passwords of the users or they can create random passwords, however, something like this doesn't protect us quite enough.


Let's suppose that an attacker has stolen a password file that contains the passwords of users in groups, just like the third column in the table above we just explain. 
Given the presence of honeywords, though, such an attacker is extremely unlikely to guess a user’s true password for the first time and more likely instead to submit a honeyword while he tries to have access in a random account. 
As we all may know from maths, the possibilities of an attacker to guess the right password out of the total passwords (K) are 1/K. 
To put it simply, the biggest number K the fewer possibilities for the attacker to gain access.
For example, if we have created twenty (20) honeywords for a user, plus his real one (1) password, then the total amount of possible passwords the attacker has to guess from are twenty-one (21), K = 21. 
In other words, the possibilities are 1/21 or 0.047 or 4.7 %.


Finally. If a honeyword-enabled system detects an attempt to log in using a honeyword then raises an alarm indicating that the password file has been compromised because no one would know to type the honeywords.


<br>

**If you are interested in honeywords and how they were created click on the links below, in order to view the original papers**

1.  [Here - The original paper](https://people.csail.mit.edu/rivest/pubs/JR13.pdf)
2.  [Here - FAQ on Honeywords](https://people.csail.mit.edu/rivest/honeywords/faq.pdf)
3.  [Here - The first generators ever](https://people.csail.mit.edu/rivest/honeywords/gen.py)
