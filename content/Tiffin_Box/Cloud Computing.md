#cloud #networking 

Using someone else's computers — over the internet — instead of buying and managing your own. 
Cloud computing means renting computing resources (servers, storage, databases, networking) from a provider. We use what we need, when we need it, and pay for what we use.

> [!info] Analogy 
> Like electricity — we don't build our own power plant. We plug into the grid and pay our bill. Cloud is the same for computing power.


### History

In the early days of computing, computers were **enormous and expensive** — only governments and big universities had them. Most of the time, these machines sat idle. The core question became:

>"Can multiple people share one powerful computer — each feeling like they have it to themselves?"

That question led, eventually, to the cloud.

---
#### Timeline 

- **1960s
	The seed: time-sharing**
	 [John McCarthy (MIT)](https://en.wikipedia.org/wiki/John_McCarthy_(computer_scientist)) proposed that computing could be delivered like a utility — just like electricity or water. Multiple users sharing one mainframe at the same time. This was called _time-sharing_.
- **1969  
	ARPANET — the ancestor of the internet**
		The US Department of Defense built ARPANET — the first network connecting computers across locations. [J.C.R. Licklider](https://en.wikipedia.org/wiki/J._C._R._Licklider) had earlier dreamed of an "Intergalactic Computer Network" where anyone could access data from anywhere. Without this, cloud is impossible.
- **1990s
	The internet goes public + "cloud" metaphor appears**
		The internet became public. Network diagrams started drawing the internet as a cloud shape — engineers didn't care what was inside, only what went in and came out. The word "cloud" stuck. Companies started offering basic hosting — renting server space online.
- **1999 
	Salesforce — first major SaaS**
		[Marc Benioff](https://en.wikipedia.org/wiki/Marc_Benioff) launched Salesforce — software delivered entirely over the internet, no installation needed. This proved the SaaS model worked at scale. It was a turning point: software didn't have to live on your machine.
- **2002 – 2006
	Amazon invents modern cloud (AWS)**
		Amazon had built massive internal infrastructure to run their e-commerce site. Most of the time, that infrastructure sat idle. They realized: _why not rent it out?_ In 2006, Amazon launched **AWS S3** (storage) and **EC2** (virtual servers) — the first true public cloud. Anyone could rent a server by the hour.
- **2008 – 2010
	Google and Microsoft join in**
		Google launched **Google App Engine** (2008) and Microsoft launched **Azure** (2010). The cloud wars began. Prices dropped, services multiplied.
- **2010s
	Cloud becomes the default**
		Startups stopped buying servers entirely. Netflix, Airbnb, Uber — all built on AWS. The question shifted from _"should we use cloud?"_ to _"which cloud?"_
- **Today
	Cloud is infrastructure**
		Most of the internet runs on AWS, Azure, or GCP. Cloud is no longer a trend — it's the foundation. New layers keep being added: serverless, edge computing, AI infrastructure.

---

### Service Model:

There are three service models -

- IaaS _(Infrastructure as a Service)_ : 
	User rent raw compute, storage, and networking. User choose the operating system, install software, manage security patches. It is the most flexible option and the most hands-on.
	
	_Examples: Amazon EC2, Google Compute Engine
	
- PaaS _(Platform as a Service)_ :
	The provider manages the underlying infrastructure. User focus on writing and deploying the application. The runtime, scaling, and patching are handled for user.
	
	_Examples: Heroku, Google App Engine, Vercel 
	
- SaaS _(Software as a Service)_ :
	A fully built application delivered over the browser. You just log in and use it. The provider owns everything from the servers to the interface.
	
	_Examples: Gmail, Notion, Figma

### Deployment Models

Beyond _how_ services are delivered, there is the question of _where_ they run and _who_ can access them.

- **Public cloud** — shared, multi-tenant infrastructure rented from a provider. The cheapest and most scalable option.
- **Private cloud** — dedicated infrastructure, either hosted on-premises or by a third party, reserved for a single organization. Offers more control.
- **Hybrid cloud** — a combination of public and private, connected so workloads can move between them. Common in enterprises with strict data requirements.
- **Multi-cloud** — using two or more public cloud providers simultaneously, often to avoid dependence on a single vendor or to use best-in-class services from each.

### Benefits of Cloud Computing

- Global reach
- Managed services
- Pay as you go
- Scalable 

---

Related Notes:

[[AWS, The GodFather]]

