#basic #networking 

Cookie is a small piece of data that is stored on computer. 

It was invented by [Lou Montulli](https://en.wikipedia.org/wiki/Lou_Montulli) in 1994, at the age of 23. He invented it by solving a simple problem of online shopping cart. From then it become the most important and most controversial technology on web.
<span class="lal">He named it after **Magic Cookie**--- a term from Unix programming for a small token passed between programs to maintain state.</span>

### Why we need 'Cookie' ?

HTTP was design to be **stateless**. Every single request was completely independent. The server processes it, sends a response, and immediately *forgets about previous request.* A fresh start every time.

This was fine in 1991. The web was just static documents — physics papers, research notes. No need to log in to read a document. Just fetch and read.
But early 1990s it become a serious problem. People started to -
- Online shopping
- Login system
- Personalization
- Multi-step form
All of these require the server to remember something about user across multiple request. But HTTP has no memory, every single request was anonymous.

>[!info] Possible solution tried before
>To solve this problem, people tried some method---
> - **Option-1: Put everything in the URL**
> ```
> 	/dashboard?user=alice&session=abc123&cart=item1,item2
> ```
> Problems — ugly, insecure, URLs get shared and bookmarked, session tokens leak everywhere.
>  - **Option-2: Hidden form fields**
> 	 Every page embeds hidden inputs carrying session data, submitted with every form.
> ```
> 	<input type="hidden" name="session" value="abc123">
> ```
> Problems — only works with forms, breaks on regular links, messy.
> - **Option-3: IP address Tracking**
> 	Server identifies by user's IP address.
> Problems — multiple people share IPs (offices, universities), one person can have multiple IPs (mobile networks), completely unreliable.

---
### The CONTROVERSIAL side of Cookie

**Act-1: The beginning**
	Lou Montulli invented cookies in 1994, they were purely functional. Store a session id. A small technical advantage


**Act-2: The birth of The third party cookie**
	A company called [DoubleClick](https://en.wikipedia.org/wiki/DoubleClick) (an advertising company) realized something clever in 1996:
		*Cookies don't have to be set by the website that user is visiting. They can be set by anyone whose content appears on that page — including us.*
	DoubleClick was present on thousands of websites simultaneously. Every site which have an ad from DoubleClick, in first visit DoubleClick set a cookie on the browser. Whenever a user visit another website (which also have a DoubleClick ad), it reads the same cookie and recognize the user.
	That's how they build a profile of you, where have you been, you choice and taste.


**Act-3: The profile building Machine**
	The advertising network figure it out what they can track

 1. News sites you read  --> Your political views
 2. Health sites you visited   --> Your medical conditions
 3. Shopping sites you browsed   --> Your income level
 4. Dating sites you used   -->  Your relationship status
 5. Job sites you browsed   --> Your career situation

All of this without you ever signing up, logging in, or giving consent. Just by visiting websites that had ads on them.


**Act-4: The first Scandal**
	In 1999, DoubleClick announced it was merging with [Abacus Direct] (a company that had real names and addresses of millions of people from catalog purchases.)
>  *The plan: combine anonymous cookie profiles with real identities.*	

Suddenly your anonymous browsing history would be tied to your actual name and address. DoubleClick backed down under pressure.


**Act-5: Google buys DoubleClick   :)**
	In 2007, Google buyed DoubleClick for $3.1 billion.
	Google already knew
	- What you searched for
	- what you mailed (Gmail-2004)
	- where you went (Google Map)

Now with DoubleClick they knew
- every website you visited that had Google Ads

Combined — Google could build the most detailed picture of a human being ever assembled in history. Your thoughts, your conversations, your movements, your browsing — all of it.

- [ ] Then 'Facebook' came out at 2010, with the same machine from the social side. The surveillance economy was fully operational.


**Act-6: The scale become clear**
By the 2010s, researchers started revealing just how extensive the tracking had become.
Studies found:
- The average webpage loaded *dozens of trackers*
- A single news article could ping *50+ third-party domains*
- Your profile could contain *thousands of data points*
- Data brokers were selling profiles for *fractions of a cent each*

But you know what, these all are ==technically legal==. You had "Agreed" by using the internet.

**Act-7: The Cambridge Analytica explosion**
In 2018, it was revealed that *Cambridge Analytica* had harvested Facebook data of *87 million people* without their consent and used it to target political advertising — potentially influencing the *2016 US election* and [Brexit vote](https://en.wikipedia.org/wiki/Brexit).

Suddenly cookie tracking wasn't just a privacy issue. It was a democracy issue.

Governments woke up. The public was outraged. Mark Zuckerberg testified before Congress. The conversation shifted from "is this annoying?" to "is this dangerous?"


**Act-8: The law fight back**
Governments around the world started legislating:

*GDPR — Europe (2018)*
- You must explicitly consent before non-essential cookies are set
- Companies must explain exactly what they track
- Users have the right to see, download, and delete their data
- Fines up to *€20 million or 4% of global revenue* — whichever is higher
- Google fined €150 million. Facebook fined €60 million. Amazon fined €746 million.

*CCPA — California (2020)
- Californians can opt out of data sales
- Companies must disclose what data they collect
- Users can request deletion of their data

**Similar laws followed in Brazil, Canada, Japan, India, and more.**

This is why every website now greets you with a cookie consent banner. That popup you hate? That's GDPR.


**Act-9:  The browsers rebel**
	Browser makers started blocking third party cookies by default
	
+ Safari introduces Intelligent Tracking Prevention in 2017
+ Firefox blocks third-party cookies by default in 2019
+ Safari blocks ALL third-party cookies in 2020
+ Google announces plan to kill third-party cookies in Chrome by 2022 in 2020
+ Google delays to 2023 
+ Google delays AGAIN to 2024 
+ Google delays AGAIN — still ongoing

	Google's delay is itself controversial — Google's entire business model depends on tracking. Killing third-party cookies would a disaster to their ad revenue. So they keep postponing while claiming to protect privacy.


**Act-10: The cookie banner nightmare**
	GDPR required consent banners. But companies found clever ways to make them manipulative. like-
	
-  Designs that make "Accept All" big and green
-  "Reject All" hidden in tiny grey text or buried 3 clicks deep
-  Pre-ticked boxes for tracking
-  Confusing language nobody understands
-  Dark patterns that guilt you into accepting

	These are called *dark patterns* — deliberately deceptive UI designed to trick you into consenting.
```handwriting
The cat and mouse game continues.................................. :)
```


>[!tip] Lets think again
>**Why Google hadn't face what Facebook had face??**
>
>The real answer is --- Money & Lobby.
>You see google had taken some smart moves. Google tracking system is framed as "Just ad". Commercial but not political. Google's tracking was invisible infrastructure, most people dont know about it
>Facebook was visible and personal, people understand easily. Facebook's scandals were messy and public — Zuckerberg's arrogance made him an easy villain
>
>Google spent hundreds of millions on lobbying governments worldwide. By 2007 they were one of the most powerful companies on earth
