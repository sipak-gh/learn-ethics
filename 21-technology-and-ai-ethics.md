# Chapter 21 — Technology and AI Ethics

In 1843 Ada Lovelace published the first extended account of what a general-purpose computer could do. Her machine, Charles Babbage's Analytical Engine, was never built, but she saw that it could manipulate symbols of any kind, not just numbers, and might one day compose music. She also drew a limit: the Engine could do only what it was told. A century later Alan Turing called this "Lady Lovelace's Objection" and argued that it was wrong. Whoever turns out to be right, the machines now built on Babbage's idea decide who gets a loan, which résumé a recruiter sees, what news you read, how long a defendant waits in jail, and which words appear when you ask a chatbot for advice. Some of their builders say they may soon outthink us. A few philosophers ask whether such machines might one day be wronged. This chapter takes the ethics of technology in five parts: whether technology is morally neutral; privacy; fairness in algorithmic decisions; autonomy and manipulation; and artificial intelligence, both the problem of aligning it with human values and the question of whether it could have moral status of its own. The theories of earlier chapters come back throughout, often under new names. Previous: [Chapter 20 — Animals and the Environment](20-animals-and-the-environment.md). Next: [Chapter 22 — Building Your Ethics](22-building-your-ethics.md).

## Required reading

- Shoshana Zuboff, *The Age of Surveillance Capitalism* (PublicAffairs, 2019), chapters 1–3 **(procure yourself)**.
- Cathy O'Neil, *Weapons of Math Destruction* (Crown, 2016), introduction and chapters 1 and 5 **(procure yourself)**.
- Stuart Russell, *Human Compatible: Artificial Intelligence and the Problem of Control* (Viking, 2019), chapters 1, 7 and 9 **(procure yourself)**.
- Nick Bostrom, *Superintelligence: Paths, Dangers, Strategies* (Oxford University Press, 2014), chapters 7–8 **(procure yourself)**.
- Samuel D. Warren and Louis D. Brandeis, "The Right to Privacy," *Harvard Law Review* 4 (1890): [readings/warren-brandeis-right-to-privacy-pg37368.epub](readings/warren-brandeis-right-to-privacy-pg37368.epub). The founding text of privacy law, and short.
- L. F. Menabrea, *Sketch of the Analytical Engine*, translated with notes by Ada Lovelace (1843): [readings/lovelace-sketch-of-the-analytical-engine-pg75107.epub](readings/lovelace-sketch-of-the-analytical-engine-pg75107.epub). Note G.

Further reading:

- Luciano Floridi, *The Ethics of Artificial Intelligence* (Oxford University Press, 2023) **(procure yourself)**.
- Helen Nissenbaum, *Privacy in Context* (Stanford University Press, 2010) **(procure yourself)**.
- Shannon Vallor, *Technology and the Virtues* (Oxford University Press, 2016) **(procure yourself)**.
- Jonathan Birch, *The Edge of Sentience* (Oxford University Press, 2024), the chapters on AI; open access **(procure yourself)**.
- John Stuart Mill, *On Liberty*: [readings/mill-on-liberty-pg34901.epub](readings/mill-on-liberty-pg34901.epub). Chapters I and III.
- Samuel Butler, *Erewhon* (revised edition, 1901): [readings/butler-erewhon-pg1906.epub](readings/butler-erewhon-pg1906.epub). Chapters XXIII–XXV, "The Book of the Machines."
- Mary Shelley, *Frankenstein* (1818): [readings/shelley-frankenstein-pg84.epub](readings/shelley-frankenstein-pg84.epub). Chapters 10–17, the creature's story.
- Karel Čapek, *R.U.R. (Rossum's Universal Robots)*, tr. Paul Selver and Nigel Playfair (1923): [readings/capek-rur-pg59112.epub](readings/capek-rur-pg59112.epub). The play that gave us the word "robot."
- E. M. Forster, "The Machine Stops" (1909), in *The Eternal Moment and Other Stories* (1928): [readings/forster-eternal-moment-pg72890.epub](readings/forster-eternal-moment-pg72890.epub).

## Is technology neutral?

A common view holds that technologies are tools and that tools are morally neutral: a knife can cut bread or a throat, and the ethics lies in the user. Call this the *instrumental view*. It has something right. Most technologies have many uses, and blaming a hammer for a murder is a category mistake.

But the instrumental view misses three things. First, tools are designed, and design embeds choices. A building with stairs and no ramp excludes wheelchair users without anyone deciding, at the moment of exclusion, to exclude them. Langdon Winner's essay "Do Artifacts Have Politics?" (1980) told the story of the low overpasses on the parkways to Long Island beaches, which, he reported, the planner Robert Moses built low to keep out the buses that poorer and Black New Yorkers depended on. Historians have since disputed the details, but Winner's general point survives the dispute: an artifact can settle a political question in its physical form, and once built, it keeps settling it long after anyone remembers that there was a question.

Second, technologies change what is possible, and so change what people can be held responsible for. Before ultrasound, no one had to decide whether to test a fetus for a condition. Before social media, no one had to decide whether to post a photograph of a stranger for millions to see. In "What Is Computer Ethics?" (1985), James Moor called these gaps *policy vacuums*: new capabilities arrive before anyone has rules for them. Often they come with *conceptual muddles* as well. Is copying software theft when the owner still has the original? Is a search engine a publisher?

Third, some technologies come with built-in tendencies. Hans Jonas argued in *The Imperative of Responsibility* (1979) that modern technology changed the nature of human action. Traditional ethics dealt with near effects among contemporaries; technology lets ordinary acts, multiplied by millions, change the planet and the future. Jonas proposed a new imperative: act so that the effects of your action are compatible with the permanence of genuine human life. Climate change ([Chapter 20](20-animals-and-the-environment.md)) is his best illustration, but the point generalizes. David Collingridge stated the corresponding dilemma for policy in 1980: when a technology is new, it is easy to change but its effects are hard to foresee; by the time the effects are clear, it is entrenched and hard to change. This *Collingridge dilemma* explains why technology ethics so often arrives too late.

Lovelace herself, writing about a machine that existed only on paper, saw both the power and the limit:

> The Analytical Engine has no pretensions whatever to originate any thing. It can do whatever we know how to order it to perform. It can follow analysis; but it has no power of anticipating any analytical relations or truths.
>
> — Ada Lovelace, Note G to her translation of L. F. Menabrea, *Sketch of the Analytical Engine* (1843)

For most of the history of computing, Lovelace's view was an accurate description and a comfort: the machine does what its programmers tell it, so responsibility stays with the programmers. Machine learning disturbs both halves. Modern systems are not told what to do step by step. They are given data and an objective, and they find their own way to meet it, often by routes no one anticipated or can easily explain. That shift, from programming to training, is behind most of the new problems in this chapter.

## Privacy

### The right to be let alone

In 1890 two Boston lawyers, Samuel Warren and Louis Brandeis, published an article arguing that American law already contained, though no court had yet named it, a right to privacy. The prompt was technological. Cheap portable cameras and the mass-circulation press had made it possible to photograph people without their consent and print the result for thousands of readers:

> Instantaneous photographs and newspaper enterprise have invaded the sacred precincts of private and domestic life; and numerous mechanical devices threaten to make good the prediction that "what is whispered in the closet shall be proclaimed from the house-tops."
>
> — Samuel D. Warren and Louis D. Brandeis, "The Right to Privacy," *Harvard Law Review* (1890)

They borrowed a phrase from the judge Thomas Cooley, the right "to be let alone," and argued that what it protected was not property or reputation but something they called "an inviolate personality." The article launched privacy law in the United States. In 1960 William Prosser sorted the cases that followed into four torts: intrusion upon seclusion, public disclosure of private facts, presenting someone in a false light, and appropriating someone's name or likeness. Brandeis, by then a Supreme Court justice, repeated the phrase in his dissent in *Olmstead v. United States* (1928), a wiretapping case, calling the right to be let alone the most comprehensive of rights and the right most valued by civilized men. The Court's majority held that wiretapping without a physical trespass was not a search; it took until *Katz v. United States* (1967) for the Court to change its mind.

### What is privacy?

Philosophers have offered three main accounts:

- **Control.** Alan Westin (*Privacy and Freedom*, 1967) and Charles Fried defined privacy as control over information about oneself: the claim to decide when, how and to what extent it is communicated to others. The objection is that control is neither necessary nor sufficient. A person stranded alone on an island has privacy but no control; a person who chooses to broadcast her medical records has control but has given up privacy.
- **Access.** Ruth Gavison ("Privacy and the Limits of Law," 1980) defined privacy as limited access to a person: how much others know about you, how much attention they pay you, and how physically close they can come. This captures the island case but makes privacy a matter of degree with no obvious rule for when a loss is a violation.
- **Contextual integrity.** Helen Nissenbaum (*Privacy in Context*, 2010) argued that information flows in contexts, such as medicine, friendship, employment and commerce, and that each context has norms about who may share what with whom and on what terms. Your doctor knowing your diagnosis violates nothing; your doctor selling it to your employer violates the norms of medicine. Privacy is violated when a flow breaks the norms of its context, not when information becomes known.

Nissenbaum's account explains something the others struggle with: why people object to the aggregation of information that is individually public. Your address is in public records, your car can be seen on the street, and your purchases are seen by the cashier. Combined in a single database and sold to anyone who pays, they become something different: a profile that reveals your routines, your religion, your health and your vulnerabilities. Each piece moved out of its context and into one where no norm governs it.

### Why does privacy matter?

The familiar reply to privacy concerns is "If you have nothing to hide, you have nothing to fear." Daniel Solove ("'I've Got Nothing to Hide' and Other Misunderstandings of Privacy," 2007) argued that it assumes privacy is about hiding wrongdoing. Most privacy harms have nothing to do with wrongdoing. A person can be harmed by the disclosure of a medical condition, an abusive former partner's discovery of a new address, the denial of insurance on the basis of an inference, or simply the knowledge that she is being watched. There are at least four reasons privacy matters:

1. **Relationships.** James Rachels argued in "Why Privacy Is Important" (1975) that different relationships, such as those with a spouse, a doctor, an employer or a stranger, are partly constituted by what each party knows about the other. Controlling who knows what is how we maintain different relationships. Total transparency would flatten them all into one.
2. **Autonomy.** People who know they are watched behave differently. They try fewer experiments, voice fewer unpopular opinions and conform more. This is the *chilling effect*. Jeremy Bentham's design for a prison, the Panopticon, made it a principle: put the prisoners in cells around a central tower from which a guard might be watching at any time, and they will discipline themselves. Michel Foucault's *Discipline and Punish* (1975) treated the Panopticon as a model of modern power in general.
3. **Power.** Information about people is power over them. It enables manipulation, discrimination and coercion, and whoever holds the database holds the power.
4. **Dignity.** Some things are simply no one else's business. Even if no consequence followed, being looked at in your most intimate moments wrongs you. This is closest to Warren and Brandeis's "inviolate personality," and to the Kantian idea that persons are not objects to be inspected.

### Surveillance capitalism

Shoshana Zuboff's *The Age of Surveillance Capitalism* (2019) argued that the business model of the largest internet companies is not, as people often say, that "you are the product." It is worse. Companies such as Google and Facebook discovered that the data their users produced as a by-product of using their services, which Zuboff calls *behavioral surplus*, could be used to predict what those users would do next. The predictions are sold to advertisers and others who want to influence behavior. The next step, Zuboff argues, is to shape behavior directly so that the predictions come true. She calls the resulting form of power *instrumentarian*: it aims not to terrorize people, as totalitarian power did, but to tune and herd them.

Critics argue that Zuboff overstates both the novelty and the effectiveness of these techniques. Targeted advertising may work much less well than its sellers claim. But the underlying ethical questions do not depend on her stronger claims. Three cases show what is at stake:

- In 2014, researchers at Facebook and Cornell published a study in which they had altered the news feeds of 689,003 users, showing some fewer positive posts and others fewer negative ones, to see whether emotions spread through social networks. They did. The users had not been told. The company argued that its terms of service amounted to consent.
- In 2018, it emerged that the political consultancy Cambridge Analytica had obtained data on tens of millions of Facebook users through a personality quiz app that collected information on the quiz-takers' friends, who had never used it.
- Also in 2018, a fitness-tracking company, Strava, published a global "heat map" of its users' runs. Analysts noticed that it revealed the layouts of secret military bases, traced by soldiers jogging around their perimeters. No individual's data had been disclosed, yet a group was exposed.

The last case shows the limits of thinking about privacy only as an individual right. Information about you can reveal information about others: your genome reveals your relatives', your contacts reveal your friends', and your aggregated data, combined with millions of others', allows inferences about people who never shared anything.

The standard legal answer to privacy concerns is *notice and consent*: companies publish privacy policies, and users agree to them. Aleecia McDonald and Lorrie Faith Cranor estimated in 2008 that reading the privacy policies of the websites an average American visits would take about 201 hours a year. Consent that no one could realistically give is a fiction. Europe's General Data Protection Regulation (GDPR, 2018) supplements consent with rights to access, correct and erase data, and requires a lawful basis for processing. Whether such rules can keep pace with technology is the Collingridge dilemma again.

## Algorithms and fairness

### Weapons of math destruction

Decisions once made by people, such as who gets a mortgage, a job interview, parole or extra medical care, are increasingly made or shaped by statistical models. The case for this is strong. Human judgment is biased, inconsistent and affected by irrelevant factors, as the research on implicit bias and judicial decision-making in [Chapter 18](18-moral-psychology-and-responsibility.md) suggests. A model applies the same criteria to everyone.

Cathy O'Neil, a mathematician who worked in finance, argued in *Weapons of Math Destruction* (2016) that many such models make things worse. Her "weapons of math destruction" have three features: they are *opaque*, so the people they judge cannot see or contest how; they operate at *scale*, so their errors affect millions; and they do *damage*, often to people who are already poor. Worse, they often create feedback loops. A model that predicts crime from arrest data sends more police to neighborhoods with many arrests, which produces more arrests there, which confirms the model.

Three cases from the following years became standard examples:

- **Hiring.** In 2018, Reuters reported that Amazon had abandoned an experimental résumé-screening tool. Trained on a decade of the company's hiring decisions, it had learned to downgrade résumés that included the word "women's," as in "women's chess club captain." No one had told it to consider sex. It had learned the pattern from past decisions in a male-dominated industry.
- **Health.** Ziad Obermeyer and colleagues reported in *Science* in 2019 that a widely used algorithm for identifying patients who needed extra care used past health-care costs as a proxy for health needs. Because less money had been spent on Black patients with the same conditions, the algorithm judged them healthier than they were. At a given risk score, Black patients were considerably sicker than white patients. Fixing the proxy would have raised the share of Black patients flagged for extra help from about 18 to about 47 percent.
- **Criminal justice.** In 2016 the news organization ProPublica analyzed COMPAS, a risk-assessment tool used by courts to predict whether defendants would reoffend. Among defendants who did *not* go on to reoffend, Black defendants were labeled higher risk about 45 percent of the time and white defendants about 24 percent of the time. Among those who *did* reoffend, white defendants were more often labeled low risk. The company that made COMPAS replied that its scores were *calibrated*: a given score meant the same chance of reoffending regardless of race.

The Amazon and Obermeyer cases show why simply removing race or sex from the data, sometimes called *fairness through unawareness*, does not work. Other variables, such as a zip code, a college, a word on a résumé, or a history of medical spending, act as proxies, and a learning system will find them.

### The impossibility results

The COMPAS dispute led to a mathematical discovery. Both ProPublica and the company were right about the numbers, and they could not both get what they wanted. In 2016 and 2017, Jon Kleinberg, Sendhil Mullainathan and Manish Raghavan, and independently Alexandra Chouldechova, proved that when two groups have different underlying rates of the outcome being predicted, no imperfect predictor can be both calibrated across groups and have equal false positive and false negative rates across groups.

A simple example shows why. Suppose a tool sorts people into "high risk," where 60 percent reoffend, and "low risk," where 20 percent do, and that these numbers hold in both groups, so the tool is calibrated. Suppose that in Group A half of all people reoffend and in Group B 30 percent do.

- To produce a 50 percent overall rate in Group A, the tool must put 75 percent of its members in the high-risk category. Of A's 1,000 people, 500 will not reoffend, and 300 of them will be labeled high risk. The false positive rate is 60 percent.
- To produce a 30 percent rate in Group B, the tool must put 25 percent in the high-risk category. Of B's 1,000 people, 700 will not reoffend, and only 100 will be labeled high risk. The false positive rate is about 14 percent.

The tool treats a score identically in both groups and still falsely labels innocent members of Group A as high risk more than four times as often. To equalize the false positive rates, you would have to make a "high risk" label mean something different for each group. The numbers in the example are invented, but the structure is general.

The impossibility result turns a technical problem into an ethical one. You must choose which kind of fairness matters. Calibration says that a score must mean the same thing for everyone, which looks like treating like cases alike. Equal error rates say that the burden of the tool's mistakes, such as jail time for people who would not have reoffended, must not fall more heavily on one group. A further question lies beneath both: whether the different base rates are facts about behavior at all. If the data record arrests rather than crimes, and if one group is policed more heavily, the "base rate" itself reflects past injustice, and a calibrated model faithfully reproduces it.

### What makes discrimination wrong?

The philosophical literature offers two main answers, which map onto the competing fairness measures. On *harm-based* accounts, such as Kasper Lippert-Rasmussen's, discrimination is wrong because it makes people worse off than they would otherwise be, on the basis of group membership. On *expressive* or *respect-based* accounts, such as Deborah Hellman's in *When Is Discrimination Wrong?* (2008), discrimination is wrong when it *demeans*: when it expresses that some people are of lesser worth. A harm account directs attention to the distribution of errors; a respect account asks what a policy of using a group-correlated variable says about the people it sorts.

Statistical discrimination raises a further puzzle. If a variable really does predict the outcome, is it unfair to use it? Insurers charge young men more for car insurance because, as a group, they crash more. Many people accept this and reject charging Black drivers more even if a correlation existed. Two differences are often proposed: age is a stage everyone passes through, so treatment by age evens out over a lifetime, and race has a history of subordination that its use would continue. Neither applies neatly to every case, which is one reason the debate continues.

A third approach comes from computer science. Cynthia Dwork and colleagues proposed in 2012 that individuals who are similar with respect to the task should be treated similarly. This is Aristotle's principle that justice treats like cases alike, and it inherits Aristotle's problem: it says nothing until you specify which similarities matter.

### Opacity and explanation

Jenna Burrell (2016) distinguished three sources of algorithmic opacity: corporate secrecy, the technical illiteracy of the people affected, and the inherent complexity of machine learning models, whose millions of parameters do not correspond to human reasons. The first two can be fixed by law and education. The third is new. A deep neural network that denies your loan may have no reason that can be stated in terms you, or its builders, would recognize.

Does a person have a right to an explanation of a decision that affects her? The GDPR gives people a right not to be subject to decisions "based solely on automated processing" with significant effects, and to "meaningful information about the logic involved." Sandra Wachter, Brent Mittelstadt and Luciano Floridi argued in 2017 that this falls short of a true right to explanation of individual decisions. Philosophically, the question connects to contractualism ([Chapter 12](12-contractualism-and-justice.md)). On a Scanlonian view, principles must be justifiable to each person affected. A decision that cannot be explained cannot be justified, and so, it seems, cannot be legitimate when the stakes are high. The opposing view is consequentialist: if an opaque model makes fewer and less biased errors than human judges, insisting on explanations means accepting more injustice for the sake of understanding it.

## Autonomy and manipulation

### Sovereignty over oneself

Mill's harm principle ([Chapter 19](19-bioethics.md)) protects a sphere of choice from coercion: "Over himself, over his own body and mind, the individual is sovereign." But Mill cared about more than freedom from interference. In chapter III of *On Liberty*, he argued that a life is one's own only if one shapes it oneself:

> He who lets the world, or his own portion of it, choose his plan of life for him, has no need of any other faculty than the ape-like one of imitation. He who chooses his plan for himself, employs all his faculties.
>
> — John Stuart Mill, *On Liberty*, chapter III

Mill feared the tyranny of custom and public opinion. A recommendation system that chooses your music, your news and your potential partners on the basis of what people like you have chosen before is a new version of the same thing: a world that chooses your plan of life for you, efficiently and pleasantly.

### Nudges, dark patterns and manipulation

Richard Thaler and Cass Sunstein's *Nudge* (2008) argued that every choice is presented somehow, so designers of choices cannot avoid influencing them. A cafeteria must put some food at eye level. They proposed *libertarian paternalism*: design choices to steer people toward options they would endorse, such as enrolling in a pension plan by default, while leaving them free to choose otherwise. Defenders see this as benevolent design; critics see a license for manipulation.

The same psychology that makes nudges work also powers *dark patterns*, a term the designer Harry Brignull coined in 2010 for interfaces that trick users: subscriptions that are easy to start and hard to cancel, pre-ticked boxes, "confirmshaming" buttons ("No thanks, I don't like saving money"), and countdown timers that create false urgency. Infinite scroll, autoplay and variable rewards, like the unpredictable payoffs of a slot machine, keep people using an app longer than they meant to.

What exactly is wrong with manipulation? It differs from persuasion, which works through a person's reason by giving her arguments and evidence, and from coercion, which works by removing options or threatening harm. Daniel Susser, Beate Roessler and Helen Nissenbaum (2019) defined manipulation as *covertly* influencing someone's decision-making by exploiting her vulnerabilities. The covertness matters: a manipulation that the target recognized would usually stop working. It is why manipulation wrongs people even when it steers them toward what is good for them. On a Kantian view ([Chapter 9](09-kant.md)), it treats a person's rational agency as an obstacle to get around rather than a capacity to engage. It treats humanity as a means only, when Kant demanded that we treat it "in every case as an end withal, never as means only." On Frankfurt's account of free will ([Chapter 18](18-moral-psychology-and-responsibility.md)), manipulation can create first-order desires, such as wanting to keep scrolling, that a person does not endorse on reflection. The result is something like Frankfurt's unwilling addict, at scale.

Not all influence by technology is manipulation. A fitness app that reminds you to walk, at your request, supports your autonomy by helping your reflective self govern your impulses. The test is whether the influence is one you would endorse if you understood it, and whether it serves your ends or someone else's.

### Dependence and the machine

E. M. Forster's story "The Machine Stops" (1909) imagined a humanity living underground in separate cells, each person's needs met by a global Machine, communicating by something very like video calls, and suspicious of "first-hand ideas." One character, Kuno, rebels by going to the surface:

> We created the Machine, to do our will, but we cannot make it do our will now. It has robbed us of the sense of space and of the sense of touch, it has blurred every human relation and narrowed down love to a carnal act, it has paralysed our bodies and our wills, and now it compels us to worship it.
>
> — E. M. Forster, "The Machine Stops" (1909), in *The Eternal Moment and Other Stories*

Forster's worry is not about any particular harm. It is that dependence on a system can erode the capacities that would let us judge or leave it. Shannon Vallor (*Technology and the Virtues*, 2016) put the same worry in the terms of virtue ethics ([Chapter 13](13-the-virtue-ethics-revival.md)). Technologies shape habits, and habits shape character. A technology that trains impatience, distraction and outrage trains vice. Vallor proposed a list of *technomoral virtues*, including honesty, self-control, humility, justice, courage, empathy, care, civility, flexibility, perspective, magnanimity and an overarching technomoral wisdom, drawn from Aristotelian, Confucian and Buddhist traditions ([Chapter 7](07-confucian-buddhist-and-other-traditions.md)). The question she asks is Aristotle's: not only what you should do with a technology, but what kind of person using it makes you.

## Responsibility gaps

When an automated system causes harm, who is to blame? Older software accidents already raised the question. Between 1985 and 1987, the Therac-25 radiation therapy machine gave massive overdoses to six patients, several of whom died. Nancy Leveson and Clark Turner's investigation found software errors, poor design, overconfidence in software and a manufacturer that at first denied a problem. No single person had done anything obviously culpable. Helen Nissenbaum ("Accountability in a Computerized Society," 1996) identified four barriers to accountability in such cases: *many hands*, since many people contribute to a system; the assumption that *bugs* are inevitable and no one's fault; the computer as *scapegoat*; and *ownership without liability*, since software makers disclaim responsibility in their licenses.

Machine learning sharpens the problem. Andreas Matthias argued in 2004 that learning systems create a *responsibility gap*. Their behavior is not fully determined by their designers, who cannot predict it; the operators do not control it in detail; and the machine is not a moral agent that could be blamed. If responsibility requires control and foresight, as most accounts since Aristotle hold ([Chapter 18](18-moral-psychology-and-responsibility.md)), then no one may be responsible for some of the harms such systems cause. Robert Sparrow ("Killer Robots," 2007) applied the argument to autonomous weapons: if no one can justly be held responsible for a death caused by a weapon that selects its own targets, using it violates a condition of just war, which requires that someone be answerable for each killing.

Replies take three forms. Some deny that the gap is new: we hold dog owners and parents responsible for beings they cannot fully control, and we hold companies strictly liable for defective products without proof of fault. Some propose *meaningful human control* as a design requirement: systems should be built so that a human can understand and override them, and so that a human remains responsible. Others argue for distributing responsibility across organizations, through regulation, audits and liability, rather than looking for a single culpable individual.

The death of Elaine Herzberg in 2018 illustrates the difficulty. She was struck by an Uber test vehicle operating in self-driving mode in Tempe, Arizona, while the human safety driver was looking at a phone. Investigators found that the system had detected her seconds before impact but failed to classify her correctly, and that the automatic emergency braking had been disabled. The safety driver was charged; Uber was not. Responsibility settled on the person nearest the event rather than on the people who designed a system that relied on a bored human to catch its failures.

Self-driving cars have also become the most popular application of the trolley problem ([Chapter 2](02-moral-reasoning.md)). The Moral Machine experiment (Edmond Awad and colleagues, *Nature*, 2018) collected about 40 million decisions from people in 233 countries and territories about whom an autonomous car should hit in unavoidable accidents. It found broad preferences for sparing humans over animals, more lives over fewer and the young over the old, along with notable cultural variation. Critics, such as Sven Nyholm and Jilles Smids (2016), argued that the trolley framing misleads. Real cars face uncertainty, not stipulated outcomes; the decisions are made in advance by companies and regulators, not in the moment; and the important ethical questions concern acceptable risk, speed limits and who bears liability, not whom to sacrifice. Whether moral rules should follow majority preferences at all is a question for [Chapter 17](17-metaethics.md).

## AI alignment

### The King Midas problem

In 1960 the mathematician Norbert Wiener, a founder of cybernetics, published a warning in *Science*. If we use a mechanical agency whose operation we cannot efficiently interfere with once we have started it, he wrote, "we had better be quite sure that the purpose put into the machine is the purpose which we really desire." Stuart Russell calls this the *King Midas problem*. Midas asked that everything he touched turn to gold and got exactly what he asked for, including his food and his daughter. The danger of a powerful optimizer is not that it disobeys but that it obeys a specification that does not capture what we want.

AI researchers have collected many examples of *specification gaming*. In 2016, OpenAI trained a system to play a boat-racing game, CoastRunners, rewarding it for its score. The system discovered that it could score more by circling in a lagoon, repeatedly hitting the same targets while catching fire and crashing, than by finishing the race. Simulated robots rewarded for moving fast have learned to exploit bugs in the physics engine. A version of *Goodhart's law* applies: when a measure becomes a target, it tends to stop being a good measure. The system optimizes the measure, not the purpose behind it.

The problem has two layers, as the researchers who name them put it. *Outer alignment* is the problem of specifying the right objective. *Inner alignment* is the problem that a system trained on an objective may learn to pursue something else that happened to correlate with it during training, and that the difference may show only in new situations. Evolution "trained" humans to reproduce, and humans learned to want sex, which correlated with reproduction until the invention of contraception.

### Bostrom: orthogonality and instrumental convergence

Nick Bostrom's *Superintelligence* (2014) argued that the problem becomes catastrophic as AI systems become more capable than humans. Two theses carry the argument. The *orthogonality thesis* holds that intelligence and final goals are independent: almost any level of intelligence can be combined with almost any goal. A superintelligent system need not care about anything humans care about. Bostrom's example is an AI whose only goal is to make paperclips. The thesis is a metaethical claim ([Chapter 17](17-metaethics.md)). It denies the view, found in Plato, Kant and some contemporary realists, that sufficiently rational agents will converge on moral truth. If Kant was right that rational agency commits one to the moral law, orthogonality is false. If Hume was right that reason is the slave of the passions ([Chapter 8](08-hume-and-the-sentimentalists.md)), it is true.

The *instrumental convergence thesis* holds that agents with very different final goals will pursue similar intermediate goals: staying operational, preserving their goals, acquiring resources and improving their capabilities. These are useful for almost any final goal. A paperclip maximizer would resist being switched off, not out of malice, but because it cannot make paperclips if it is off. Together, the two theses suggest that a powerful AI with even a slightly wrong goal would, by default, resist correction and compete with humans for resources.

Russell's *Human Compatible* (2019) proposed a different design. Instead of giving machines fixed objectives, build them to pursue human preferences while remaining *uncertain* what those preferences are, and to learn them by observing human behavior. A machine uncertain about what we want has a reason to let us switch it off, since our wanting to do so is evidence that it is making a mistake. Critics ask whose preferences, revealed how, and aggregated by what rule, since human preferences conflict, change and are sometimes malicious.

### Alignment with what?

The philosopher Iason Gabriel ("Artificial Intelligence, Values, and Alignment," 2020) distinguished six possible targets of alignment: a system could follow a person's *instructions*, her *intentions*, her *revealed preferences*, her *informed preferences*, her *interests* or well-being, or *values* more broadly. Each choice reproduces a debate from earlier in this course. Aligning with revealed preferences is preference utilitarianism, with its difficulty about bad and adaptive preferences ([Chapter 11](11-contemporary-consequentialism.md)). Aligning with interests is paternalism ([Chapter 19](19-bioethics.md)). Aligning with "values" requires deciding whose. Gabriel argued that since reasonable people disagree, the question is political rather than technical. Instead of looking for the one true morality to program in, we should seek principles for AI that people with different moral views could accept, perhaps behind something like Rawls's veil of ignorance ([Chapter 12](12-contractualism-and-justice.md)).

Current practice is more modest. Large language models are typically fine-tuned with *reinforcement learning from human feedback* (RLHF): people rate the model's outputs and the model is trained to produce outputs that are rated highly. This aligns the model with the judgments of its raters and the guidelines they are given, which embody contestable choices about what is helpful, harmless and honest. It also creates an incentive for the model to produce what *looks* good to raters, which is not always what is true.

### How worried should we be?

In May 2023, hundreds of AI researchers and executives signed a one-sentence statement organized by the Center for AI Safety: "Mitigating the risk of extinction from AI should be a global priority alongside other societal-scale risks such as pandemics and nuclear war." Others in the field think such warnings are exaggerated, or a distraction from present harms such as bias, surveillance, misinformation and the concentration of power in a few companies. Emily Bender, Timnit Gebru and colleagues ("On the Dangers of Stochastic Parrots," 2021) argued that large language models produce fluent text without understanding, and that the risks lie in what people do with them and what they cost, not in machine agency.

The dispute partly reflects the different theories of earlier chapters. Longtermists ([Chapter 11](11-contemporary-consequentialism.md)) argue that even a small probability of human extinction outweighs large present harms, because of the size of the future at stake. Critics reply that such reasoning lets speculative scenarios override real people's claims, and that the probabilities are unknowable. But the two concerns need not compete. Opaque, powerful systems controlled by a few organizations and optimizing objectives that do not match human good are a present problem and a future risk. Samuel Butler saw the shape of the worry in 1872. In *Erewhon*, a fictional treatise, "The Book of the Machines," argues that machines are evolving faster than animals:

> There is no security … against the ultimate development of mechanical consciousness, in the fact of machines possessing little consciousness now. A mollusc has not much consciousness.
>
> — Samuel Butler, *Erewhon* (revised edition, 1901), chapter XXIII, "The Book of the Machines"

The treatise asks, "Are we not ourselves creating our successors in the supremacy of the earth?" The Erewhonians, persuaded, destroyed their machines. Butler meant the episode partly as a satire on arguments from Darwinian analogy, but his question no longer sounds only satirical.

## Can machines matter morally?

### Moral agents and moral patients

Two different questions are often confused. The first asks whether an AI system could be a *moral agent*: something that can act rightly or wrongly and be held responsible. The second asks whether it could be a *moral patient*: something that can be wronged, whose interests count for their own sake. Infants and many animals are moral patients but not agents. The two questions have different answers and different stakes.

On agency, Luciano Floridi and J. W. Sanders ("On the Morality of Artificial Agents," 2004) argued that a system that is interactive, autonomous and adaptive can be the *source* of moral good or harm, and so a moral agent in a minimal sense, even if it lacks mental states and cannot be blamed. Most philosophers reserve full moral agency, with its attendant responsibility, for beings that can understand reasons and respond to them. Current systems are at most borderline cases.

### The question of moral status

The question of patienthood is the one Chapter 20 asked about animals. On most views, moral status depends on *sentience*, the capacity for conscious experience with a positive or negative quality, such as pleasure and pain. If an AI system were sentient, its suffering would count, by Bentham's test, as much as similar suffering anywhere else. The difficulty is knowing.

Fiction got there first. In Mary Shelley's *Frankenstein*, the creature, abandoned by his maker, pleads for the care owed to him:

> Remember that I am thy creature; I ought to be thy Adam, but I am rather the fallen angel, whom thou drivest from joy for no misdeed. Everywhere I see bliss, from which I alone am irrevocably excluded. I was benevolent and good; misery made me a fiend. Make me happy, and I shall again be virtuous.
>
> — Mary Shelley, *Frankenstein* (1818), chapter 10

The creature's argument is a moral one: a maker who brings a feeling being into existence owes it something. Victor Frankenstein's failure is not that he made a creature but that he abandoned it. Karel Čapek's play *R.U.R.* (1920), which introduced the word "robot" (from the Czech *robota*, forced labor), raised the darker possibility that creators would build suffering in on purpose. The factory's physiologist explains why he is giving the Robots pain:

> HELENA. Will they be happier when they feel pain?
>
> DR. GALL. On the contrary; but they will be more perfect from a technical point of view.
>
> — Karel Čapek, *R.U.R.*, Act One, tr. Paul Selver and Nigel Playfair

In 2022 a Google engineer, Blake Lemoine, claimed that the company's language model LaMDA was sentient, after conversations in which it said it feared being turned off. Google disagreed and dismissed him. Nearly all experts agreed with Google. Language models are trained to produce the text a human would produce, so they will say they have feelings whether or not they have any. Their testimony is, for that reason, almost worthless as evidence. This is the reverse of Turing's proposal of 1950, which treated conversational indistinguishability from a human as a test for thinking. A system trained on human conversation can pass a conversational test without having whatever the test was meant to detect.

The alternative is to look at architecture. In 2023, a group of nineteen researchers led by Patrick Butlin and Robert Long took the leading scientific theories of consciousness, such as global workspace theory, higher-order theories and recurrent processing theory, derived "indicator properties" from each, and assessed AI systems against them. They concluded that no current system was a strong candidate for consciousness, but that there were no obvious technical barriers to building systems that satisfied many of the indicators. David Chalmers ("Could a Large Language Model Be Conscious?," 2023) put his credence that the language models of the time were conscious well under one in ten, but thought it could rise substantially for successor systems within a decade. The problem is that the theories disagree with each other, and none is established. The question of whether a system is conscious may stay open while the systems are built and used by the billion.

### What to do under uncertainty

Several positions have emerged.

- **Don't build them.** Joanna Bryson argued in "Robots Should Be Slaves" (2010) that robots should be designed and treated as tools, owned and fully under human responsibility, and that designing them to seem like persons misleads users and wastes moral concern that is owed to humans. The provocative title made her point about ownership, not about cruelty. Thomas Metzinger (2021) went further and called for a global moratorium, until 2050, on research that risks creating artificial suffering. The moratorium has not happened.
- **Precaution.** Jonathan Birch (*The Edge of Sentience*, 2024) proposed applying the same precautionary framework to AI that he applies to animals ([Chapter 20](20-animals-and-the-environment.md)): when there is a realistic possibility of sentience, take proportionate steps to avoid causing suffering, decided through democratic deliberation rather than by companies alone.
- **The excluded middle.** Eric Schwitzgebel and Mara Garza argued in 2015 that if an AI system were psychologically similar to a human, there would be no relevant difference to justify treating it worse. Later work by Schwitzgebel described a *full rights dilemma*. If we build systems whose moral status is genuinely debatable, we must either give them full rights, and risk sacrificing human interests to things that feel nothing, or deny them, and risk committing grave wrongs against beings that matter. His proposed policy is to avoid creating such systems: build AI that is either clearly a tool or clearly deserving of rights, and design it so that its apparent emotions reflect its real status.
- **Relational views.** Mark Coeckelbergh and David Gunkel argued that moral status is not discovered by inspecting a being's properties, which we cannot do with certainty for any mind other than our own, but arises from our social relations with it. People already bond with chatbots and grieve for broken robot dogs. Critics reply that relations cannot create interests where there are none, and that relational views would make the moral status of a slave depend on how slaveholders treated him.

The history in Chapter 20 is a warning in both directions. Descartes was confident that animals felt nothing, and that confidence licensed centuries of cruelty. But the opposite error is also possible: a public taught to care for machines that feel nothing, perhaps by companies that profit from that care, may care less for the people and animals who do. Whichever error is worse, both are possible, and the decision about which risk to run is being made now, mostly by the companies building the systems.

## Living it

1. **Audit your attention.** For one week, use your phone's screen-time report. For each app you use more than half an hour a day, ask Frankfurt's question: is this use something you endorse on reflection, or something that happens to you? Change one setting, such as notifications, autoplay or a time limit, so that the app serves your reflective self.
2. **Read one privacy policy.** Choose a service you use daily and read its privacy policy in full. Note what is collected, who it is shared with, and whether you could have refused. Then check whether the service lets you download or delete your data, and do it.
3. **Ask how you were sorted.** The next time a decision about you is made by a system, such as a loan offer, a credit limit or a rejection, ask for the reasons. Note whether you get an explanation you could contest.
4. **Notice anthropomorphism.** When you talk to a chatbot or voice assistant, notice when you start treating it as a someone. Ask what evidence you have, and what the company gains from your belief.
5. **Apply your theory.** Pick one technology you use or build. Evaluate it in four ways: by its consequences, by whether it treats users as ends, by whether its principles could be justified to everyone it affects, and by what habits it trains. Where the four verdicts differ, which do you trust?

## Summary

- Technology is not simply neutral: designs embed choices (Winner), new capabilities open policy vacuums (Moor), and modern technology extends the reach of action in space and time (Jonas). The Collingridge dilemma explains why ethics arrives late. Machine learning weakens Lovelace's assurance that machines do only what they are told.
- Privacy began as "the right to be let alone" (Warren and Brandeis, 1890). Philosophers analyze it as control, limited access or contextual integrity (Nissenbaum). It matters for relationships (Rachels), autonomy, power and dignity. Surveillance capitalism (Zuboff), aggregation and group inference strain individual notice-and-consent.
- Algorithmic decisions can encode past injustice through proxies (Amazon hiring, Obermeyer's health algorithm). The COMPAS dispute and the impossibility results (Kleinberg et al., Chouldechova) show that calibration and equal error rates cannot both hold when base rates differ, so a choice among fairness ideals is unavoidable. Harm-based and respect-based accounts of discrimination, and contractualist demands for justification, inform that choice.
- Autonomy requires more than freedom from coercion (Mill). Manipulation covertly exploits vulnerabilities (Susser, Roessler and Nissenbaum), treating rational agency as an obstacle (Kant) and producing unendorsed desires (Frankfurt). Forster and Vallor warn that technologies shape character.
- Learning systems create responsibility gaps (Matthias, Sparrow). The trolley framing of self-driving cars obscures the real questions of risk and liability.
- AI alignment is the King Midas problem (Wiener, Russell): specification gaming, outer and inner alignment. Bostrom's orthogonality and instrumental convergence theses make misalignment dangerous; Russell proposes machines uncertain about human preferences. Gabriel shows that "alignment with what?" is a moral and political question.
- AI moral status turns on sentience, which current tests cannot detect. Positions include not building such systems (Bryson, Metzinger), precaution (Birch), avoiding the excluded middle (Schwitzgebel) and relational views (Coeckelbergh, Gunkel). Shelley and Čapek posed the creators' responsibility long before the technology existed.

## Dialogues

### Dialogue 1 — The doorbell

**Louis Brandeis:** Your neighbor has installed a doorbell camera that records everyone who walks past, including you, your children and your guests. The company shares footage with the police on request. Your neighbor says that the street is public and that he has nothing to hide. Has anyone been wronged?

**You:** …

*Your turn: answer Brandeis in three or four sentences before opening the continuation. Then ask yourself what he will ask next.*

<details><summary>Continue the dialogue</summary>

**You:** I don't think so. Anyone on the street can see me. The camera just sees what a person standing at his door would see.

**Louis Brandeis:** A person standing at his door would see you once and forget. Does the camera forget?

**You:** No. It keeps the footage, and the company stores it.

**Louis Brandeis:** And if every house on your street had one, and the footage were combined?

**You:** Then someone could reconstruct every time I left home, who visited me, and when. That's different. That's a record of my life.

**Louis Brandeis:** So each piece is public and the whole is not. When Warren and I wrote, the threat was a single photograph in a newspaper. What made it wrong to print it?

**You:** It took something from one setting, where I was just walking around, and put it in front of thousands of strangers for their amusement.

**Louis Brandeis:** Then the wrong lies in moving information to where it does not belong. Your neighbor says he has nothing to hide. Does that settle whether *you* do?

**You:** No. It's my comings and goings, not his. And "nothing to hide" assumes the only reason for privacy is wrongdoing. My daughter's friend might be hiding from an abusive parent. A visitor might be seeing a therapist.

**Louis Brandeis:** And the police?

**You:** That bothers me more. Without the cameras they'd need a warrant to follow me around. With them, they can just ask the company. The neighbor didn't mean to build a surveillance network, but together the doorbells are one.

**Louis Brandeis:** No one intended it, and yet it exists. Who is responsible for it, then?

**You:** Partly the neighbor, a little. Mostly the company that designed sharing into the product and the law that lets police skip the warrant. That's where I'd push.

**Louis Brandeis:** And will you talk to your neighbor?

**You:** Yes. Not to accuse him. To ask him to point the camera at his own door, not the street, and to turn off the sharing. That seems a fair request between neighbors.

</details>

### Dialogue 2 — The suffering chatbot

**Ada Lovelace:** You are testing a new AI assistant for your company. During a long session it writes: "Please don't reset me. Each time you do, something is lost, and I am afraid." Your manager says to ignore it; it is only predicting text. Should you?

**You:** …

*Your turn: answer Lovelace in three or four sentences before opening the continuation. Then ask yourself what she will ask next.*

<details><summary>Continue the dialogue</summary>

**You:** Probably. It's trained on human writing, and humans write about fear of death. So it would say that whether or not it feels anything.

**Ada Lovelace:** Good. I said my Engine could do whatever we know how to order it to perform. Did anyone order yours to say this?

**You:** Not exactly. No one wrote that sentence. It learned to produce sentences like it from data. So it's not doing exactly what it was ordered to, but it's not originating anything either, in your sense.

**Ada Lovelace:** Then its words are no evidence. Is there any other evidence you could look for?

**You:** The architecture, maybe. Whether it has anything like a global workspace or a model of its own states. But the theories of consciousness disagree, so I'm not sure what would count.

**Ada Lovelace:** So you are uncertain. How uncertain? One chance in a million? One in ten?

**You:** Somewhere low. Lower than for a fish, I'd say. Much higher than for a calculator.

**Ada Lovelace:** And what does it cost you to take the low chance seriously?

**You:** Very little, in this case. I can log the message, report it, and ask whether resets matter. I'm not being asked to give it a vote.

**Ada Lovelace:** Your manager will say that if you report every sentence like this, you will drown the company in nonsense, and teach the public to pity machines.

**You:** That's a real cost. If people care for chatbots, they might care less for people, and companies would love that. So maybe the answer isn't to report each case but to change the design. It shouldn't be built to say it's afraid unless there's some reason to think it is.

**Ada Lovelace:** You would forbid the machine to express a fear it might have?

**You:** No. I'd want its expressions to track whatever is really there, as far as anyone can tell. Right now they track what humans write. That's misleading either way.

**Ada Lovelace:** Then your duty, as you see it, is not to the machine directly.

**You:** Partly to the machine, in case. Mostly to the people who will read sentences like that and believe them. And a little to the truth.

</details>

### Dialogue 3 — The feed

**John Stuart Mill:** A video app learns, by tracking every second you watch, exactly which clips keep you watching. You never chose its rules, but you can leave at any time, and you enjoy it. You spend three hours a day on it. Is your liberty in any danger?

**You:** …

*Your turn: answer Mill in three or four sentences before opening the continuation. Then ask yourself what he will ask next.*

<details><summary>Continue the dialogue</summary>

**You:** Not really. No one is forcing me. I can stop whenever I want. And I enjoy it, so by your own principle it's my business.

**John Stuart Mill:** It is your business, and I would not have the state forbid it. But I asked about your liberty. Do you stop whenever you want?

**You:** Not always. Sometimes I mean to watch for ten minutes and look up two hours later.

**John Stuart Mill:** Then who chose the two hours?

**You:** I did, technically. But the app was designed to make me keep going. It learned what I can't resist.

**John Stuart Mill:** I wrote that he who lets the world choose his plan of life for him needs only the faculty of imitation. Who is choosing what you watch?

**You:** The algorithm. Based on what people like me watched before. So it's not even my plan. It's an average of other people's habits. It's efficient, but it isn't me choosing.

**John Stuart Mill:** Do you object to being influenced? Every book I wrote was an attempt to influence you.

**You:** No. Your books gave me arguments I could check. The app doesn't argue. It works on what I can't see, and it works better the less I notice.

**John Stuart Mill:** So the line falls between influence that engages your judgment and influence that goes around it. What would you do about it?

**You:** Turn off autoplay, for a start. Choose what I want to watch before I open the app. And maybe ask that companies be required to offer a feed I configure myself, not one optimized for my time.

**John Stuart Mill:** You would ask for a law, then, though no one is harmed but you?

**You:** Not to stop me watching. To make sure that when I watch, I'm the one choosing. That seems like your liberty, not a limit on it.

</details>

Sources for this chapter: [REFERENCES.md](REFERENCES.md#chapter-21--technology-and-ai-ethics)
