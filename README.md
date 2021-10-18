<h1 align="center">Honeywords Generators</h1>


* Honeywords	are	a	defense	against	stolen	password	files.	Specifically,	they	
are	bogus	passwords	placed	in	the	password	file	of	an	authentication	server to	
deceive	attackers.	Honeywords resemble	ordinary,	user-selected	passwords.	It’s
hard	therefore	for	an	attacker	that steals	a	honeyword-laced password	file	to	
distinguish	between	honeywords	and	true user passwords.	(“Honey” is	an	old	term	
for	decoy	resources in	computing	environments.	To	the	best	of	our	knowledge,	the	
term	“honeywords”	was	coined	in	this	paper.)

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


An attacker	that	has	stolen	a	password	file may	crack its	hashed	passwords	(see	
Questions	4	and	5	 below)	and	attempt to	impersonate	users.	Given	the	presence	of	
honeywords,	though,	such	an attacker is	unlikely to	guess	a	user’s true	password	
and	likely	instead	to	submit	a	honeyword.	If	a honeyword-enabled	system	detects	
an	attempt	to	login	using a	honeyword,	it	raises	an	alarm indicating that	the	
password	file	has been	compromised.	
Honeywords	aren’t	visible	to	users and	don’t	in	any	way	change	their experience
when	they	log	in	using	passwords.

<br>

**If you are interested in honeywords and how they were created click on the links below, in order to view the original papers**

1.  [Here - The original paper](https://people.csail.mit.edu/rivest/pubs/JR13.pdf)
2.  [Here - FAQ on Honeywords](https://people.csail.mit.edu/rivest/honeywords/faq.pdf)
3.  [Here - The first generators ever](https://people.csail.mit.edu/rivest/honeywords/gen.py)
