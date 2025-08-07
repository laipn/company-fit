# Lai's Structured Assessment for Company Fit

## Foreword

It has always seem odd to me that there's plenty of info on structured employee interviews, but candidates themselves tend to lack that same structure when deciding whether a company is a good fit.  I thought I'd remedy that for myself.  

The idea is to fork this doc for each company I interview for and answer the questions inline -- markdown doesn't have great form input support.  Sections can be filled out piecemeal during the "Q&A" stage of each interview but note the job role (IC, manager, etc) for each section.

I've made the doc public because a couple of people have asked me about it.  Coincidentally it also serves as good way for prospective companies to glean whether I would be a good fit for them.

I've written in a mostly third-person voice to help me maintain objectivity.  First person voice is used for instances that I assume to be subjective to my own personal values. 

I was tempted at first to just provide questions and rubrics, but I'm reminded:

> "The fish trap exists because of the fish. Once you’ve gotten the fish you can forget the trap. Words exist because of meaning. Once you’ve gotten the meaning, you can forget the words." - Zhuangzi, Chuang Tsu: Inner Chapters

Providing questions would be pointless without also providing the goal in asking them.  Interview questions quickly become [outdated over timereasons](https://web.archive.org/web/20240520214850/https://careercup.com/page?pid=amazon-interview-questions), but the objectives and rationale behind them do not.  

I've also attempted to make the question resilient to [Hawthorne Effects](https://en.wikipedia.org/wiki/Hawthorne_effect).  That is to say while HR could attempt to coach interviewers on which rubrics to target, it would ultimately erode trust in HR.  Few things would be more discouraging than say being made to memorize corporate values.  Nevertheless, I have omitted rubric details in cases where providing unambiguous details could be detrimental.

> [!TODO]
> If other people find this useful, then this document should be templated for re-use and sections conditioned on the personal values of the assessor.  GPL license has been used to encourage that.  Feel free to send a commit for review.

## Introduction

The company aspects examined are:

1. Work Culture: What company-wide mechanisms exist to ensure a non-toxic workplace.
2. Engineering Culture: Measured by reviewing tech-infrastructure decisions and employee attitudes towards tech-debt.
3. Management Culture: Employee engagement with management and management transparency with employees
4. Leadership: What mechanisms exists to ensure leaders produce healthy orgs.
5. Personal ethics: Whether the company is compatible with my own set of ethics.

> [!NOTE]
> To avoid confusion:
>
> *Assessor* refers to the person using this doc to assess a company
> *Assessee* refers to the person being asked questions.  However, it is the company they work for which is being assessed. The assessor just serves as proxy.
>
> It is important to observe that we aren't trying to "interview the interviewer".  The actual management or technical skills of the interviewer is irrelevant.  We are "interviewing the company" and its processes.

## Work Culture

> [!IMPORTANT]
> Only managers should answer this section

Manager's [headcount](^manager_ratio). 
- [ ] O(1)
- [ ] O(10)
- [ ] O(100)
- [ ] Director

[^manager_ratio]: O(10^X) headcount chosen because manager to employee ratio in tech usually sits at about 1:10

> [!NOTE]
> We use the term ["jerks"](https://en.wikipedia.org/wiki/The_No_Asshole_Rule) as shorthand indicating employees who create a toxic workplace. 	

**Objective**: Find out what a company does to create a non-toxic work environment

Each subsection asks about a common mechanism to control for jerks.  The goal of each subsection is to see how each mechanisms in used at a prospective company. 

> [!NOTE]:
> These questions have no perfect [solution](#no-solve-problem).  Consider a pre-amble with an assessee stating that there is no perfect solution and the goal is to see if corporate policies are sufficiently nuanced.

> Question: "How do you filter our jerks during the interview process?"

Background: 

  Situational interviews (e.g. [STAR](https://capd.mit.edu/resources/the-star-method-for-behavioral-interviews/)) have a good proven track records in interviews.  There is however little evidence around their efficacy in removing jerks despite heavy use for exactly that in the tech industry.

  Studies [suggests](https://pmc.ncbi.nlm.nih.gov/articles/PMC4856718/) that the reason for their efficacy is that it selects for individuals that "Knowing How You Should Behave" rather than "How You Would Behave".  This is fine if selecting for technical skills, but works poorly for selecting out jerks because there is no incentive for such employees to act that way in practice.  In fact such employees will often be [promoted](https://www.researchgate.net/publication/350589033_How_So_Many_Toxic_Employees_Ascend_to_Leadership).

- [ ] Mechanism is used
- [ ] Complexities/weaknesses are understood
- [ ] Additional novelty present. <Describe them>

> Question: "What mechanisms exists to ensure jerks are selected out in the promotion process?"

Background:

  Strictly speaking, this does not remove jerks.  It only ensures they aren't placed in positions of power where toxicity spreads further.  Common mechanisms are to use peer feedback as artifacts informing the promotion process. The weaknesses in this mechanisms is that this enforcement is typically at the candidate's manager discretion; and managers are disincentivized to block a promotion if they want to keep their reports happy.

- [ ] Mechanism is used.
- [ ] Complexities/weaknesses are understood.
- [ ] Additional novelty present. <Describe them>

> Question: "In what circumstances will HR intervene to remove a jerk?"

Background:

  This typically happens if enough HR complaints are levied.  I've only seen this happen for gross violations of explicit HR rules.  This leaves a lot of leeway where toxicity can spread especially given that HR has little day-to-day interaction with an employee.  In other words, it doesn't do much against workplace [chameleons](https://www.sciencedirect.com/science/article/abs/pii/S0263237316300263)

- [ ] Mechanism is used.
- [ ] Complexities/weaknesses are understood.
- [ ] Additional novelty present. <Describe them>

> Question: "Have you ever [managed out](https://medium.com/@janetkahr/the-managing-out-process-d60f94704564) out an employee?  What rationale and methods did you use?"

Background:

  A lot of junior people are confused about this mechanism since they expect lower-performers to be something HR issue addresses. What they don't understand is that HR and Managers operate under different hierarchies reporting to the CEO.  This is to a classic ["separation of powers"](https://www.investopedia.com/terms/s/separation-powers.asp) situation.  Without a separation of powers, you'd see manager favoritism and nepotism abound.  By separating the organization that creates HR policies and the organization that executes those policies, no individual can arbitrarily hire/fire people and objectivity is maintained in both.

  This is the mechanism that I see most often used in practice to remove jerks. But still is limited because HR typically requires a "for-cause" reasons and probationary period.

- [ ] Mechanism is used.
- [ ] Complexities/weaknesses are understood.
- [ ] Additional novelty present. <Describe them>

> Question: "What is the purpose of the technical hiearchy at the company?  Do mechanisms exist to avoid promoting jerks?"

Background: Power has a [corrupting effect](https://pmc.ncbi.nlm.nih.gov/articles/PMC10461512/) on orgs. Care must be taken when creating power structures to minimize those effects. For example, not creating hierachy in the first place is one the reasons why [flatter orgs](https://www.tandfonline.com/doi/full/10.1080/00221309.2024.2317247) tend to be less corrupt than taller ones -- though don't mistake cause for effect in that case. While management requires a hierarchy for [compartmentalization](https://en.wikipedia.org/wiki/Compartmentalization_(information_security)) reasons, this is less justifiable in a technical hiearachy.  The goal of this section is to assess whether a tech hiearachy is in a way that does not select jerks.

Common Answers:

- Projects are delivered top-down.  Project leads are assigned to those at appropriate tech levels. 
  - Weaknesses: Requires people to ascend the tech hiearachy in order to work on fun problems.  Difficulty is also determined by management and smart engineers can exploit this. e.g. sandbagging
- Promotion requires delivering value to a company. Seniority is incentive for employees to work on projects more valuable to the company.
  - Weaknesses: Requires HR to be able to align tech skills with business needs and so  is likely to promote people with better tech skills.
- Tech hierarchy is meritocratic.  Higher level indicates higher technical skill.  Typically tech leads must be looped into the promo process for this to work
  - Weaknesses: Less alignment with business needs. Susceptible to "terminal"
- Promotion level has no actual power (implicit or otherwise)
  - Weaknesses: How do technical disagreements get resolved?

- [ ] One of the common answers above was given
- [ ] Assessee understand the nuance in that answer
- [ ] Additional novelty was present. <Describe them>


## Engineering Culture 

> [!IMPORTANT]
> Only ICs should answer

In my experience, good engineering culture can  be inferred by the state of a company's technical infrastructure. Soundness in technical infrastructure decisions can often be judged objectively (especially retrospectively). However, it is often unclear whether a lack of good infrastructure stems from a legitimate need. Example: In order to deliver a product on time, a startup uses [JNI](https://en.wikipedia.org/wiki/Java_Native_Interface) to link in existing legacy code.

This ultimately creates different forms of tech debt. The difference in healthy engineering culture is that people understand why such tech-debt was created and why why it persists.

1.  Source Code Eco-System

Relevant aspects: 
- Repo choice. Example: Mono vs distributed repo Examples: Git, perforce, etc
- Front-end code-viewing support. Examples: Github, Code search
- Code-review support. Examples: Ferrit, critique.
- IDEs. Examples: Visual Studio, Intellij, etc.
- Code Symbol search support. Typically requires some tight between build and IDE (or code-search) tools 
- Coding standards. Auto-formatting.  Presubmit checks for coding standards.  [Example](https://github.com/google/yapf)
- Functional testing code-coverage and other tools. Are all tests run on every build or is there pruning?

- [ ] No Red Flags
- [ ] Red Flags. Follow Up:
  - [ ] Understands reason for tech-debt creation
  - [ ] Plan for removal 
  - [ ] There exists rationale for continuing tech-debt

2.  Build and Deployment

Relevant dimensions: 
- CI/CD - Examples: jenkins, travis, bazel, github actions, etc
- Execution environment. Examples VMs, containers, bare-metal, lambdas
- Build reproducibility. Can you build code shipped 10 years ago? Are the build tools themselves compileable from source?
- Build to source-code trackability.  Can you tell which source code file and version was in a build. 
- Dynamically linked libraries vs static compiled.  DLLs more annoying for debugging and produces limits compiler optimization.
- *Bonus points*: Verifiable builds and provenance. How do you bisect changes in order to root-cause a bug?

- [ ] No Red Flags
- [ ] Red Flags. Follow Up:
  - [ ] Understands reason for tech-debt creation
  - [ ] Plan for removal 
  - [ ] There exists rationale for continuing tech-debt

3.  Production Tools

- SLO/SLAs
- On-call rotation.  
  - Pager tools
  - Compensation
- Production monitoring. Example [Prometheus](https://en.wikipedia.org/wiki/Prometheus_(software)), [Grafana](https://grafana.com/)
- Production logging, collection and aggregation. Example. [Syslog-ng](https://en.wikipedia.org/wiki/Syslog-ng)
- Customer log/core collection

- [ ] No Red Flags. 
- [ ] Red Flags. Follow Up:
  - [ ] Understands reason for tech-debt creation
  - [ ] Plan for removal 
  - [ ] There exists rationale for continuing tech-debt


4.  Debugging Tools

- Core Dump analysis tools
- CPU-level perf tools. perf cli,  perf counters 
- Network debugging tools. ip cli, traceroute, 
- Cross-server tracing.  Example: RPC Tracing
- Kernel debugging. Example: strace, tcpdump, eBPF program

- [ ] No Red Flags. 
- [ ] Red Flags. Follow Up:
  - [ ] Understands reason for tech-debt creation
  - [ ] Plan for removal 
  - [ ] There exists rationale for continuing tech-debt


5.  Security:

> [!TODO] 
> Add stuff here

## Management Culture:

> [!IMPORTANT]
> Only ICs should answer

### Employee engagement with management


> Question: "What are your company's core values? Either implicit or explicit."

Background:

  This question assumes that an workforce engaged with leadership ought to know the answer to these questions.

- [ ] Assesee knows
- [ ] Assesee somewhat knows
- [ ] Assesee does not know
- [ ] N/A. Company does not have core values
- [ ] Assesee states company is too small to have them

> Follow up: "Can you give an example of how you (or your management) employed these values in the past?"

- [ ] Assesee provides a concrete example
- [ ] Assesee provides a vague answer
- [ ] Assesee cannot recall
- [ ] N/A

If the assess states the company is too small to have core values instead ask instead: 

> Question: "Does your company do Q&As?.  If not, why not?"

- [ ] Yes
- [ ] No. Reason: <insert text>


> Follow up: "Can you give an example of an Q&A that resulted in an action taken by management."

- [ ] Assesee provides a concrete example
- [ ] Assesee provides a vague answer
- [ ] Assesee cannot recall
- [ ] N/A


### Management transparency with employees

> Question: "Does your company do exit interviews? If not why not?"

Background:

  It's actually pretty common for large companies not to do exit interviews.  I've heard this is often the case because doing so would provide evidence that could be used for discovery in employments lawsuits.  The decision to do an exit-interview is thus emblematic of a chosen trade-off between transparency vs financial liability.

- [ ] Company does do exit interview (with survey records)
- [ ] Company provided credible reason for not doing exit-interview.  Example: Company is too small.


> Question: "Have you ever disagreed strongly with a management decision? Preferably one that ultimately you had to agree to disagree."

Background: The goal of this question is to figure out of how if employees are reluctant to approach leadership about concerns. The actual concern is mostly irrelevant but can be provided if deemed important.

- [ ] Yes
- [ ] No

> Follow up: "What did you do about it?"

- [ ] Assesee did nothing
- [ ] Assesee escalated the issue but was eventually convinced they were wrong
- [ ] Assesee escalated the issue but agreed to disagree
- [ ] Aassese escalated the issue initially but eventually gave up
- [ ] N/A

If the issue was escalated:

> Follow up: "How far was the issue eventually escalated?"

- [ ] The issue bubbled up to their manager
- [ ] The issue bubbled up to a skip-level manager
- [ ] The issue bubbled up to a an executive
- [ ] The issue bubbled up to HR
- [ ] N/A


## Leadership

> [!IMPORTANT]
> Only managers should answer the following

Manager's [headcount](^manager_ratio). 
- [ ] O(1)
- [ ] O(10)
- [ ] O(100)
- [ ] Director


The selection of leaders is important because:

> “Good governance never depends upon laws, but upon the personal qualities of those who govern. The machinery of government is always subordinate to the will of those who administer that machinery. The most important element of government, therefore, is the method of choosing leaders." - Frank Hebert

Leader are created from either the promotion process, from reorganizations and lost via [attrition](https://www.gartner.com/en/human-resources/glossary/attrition).  This section examines these processes to see if they select for good leaders.  Specifically leaders that won't produce "jerks".


### Promoting leaders

Managers are usually evaluated accounting for excellence in strategy execution and overall org healthiness.  For myself, promoting strong performers in the latter is most important. 

> Question: "How does the company measure org health?"

[Common answers](#no-solve-problem): 
- HR complaints
  - Weakness: People are wary to HR because it starts a tit-for-tat war between reporter and reportee
- Org surveys
  - Weakness: There's often pressure from execs to score well
- manager/report/peer feedback
  - Weakness: If peers are chosen by reviewee then this is often exploited

- [ ] Common answer provided. 
- [ ] Weaknesses are understood
- [ ] Additional novelty present. Describe them

> Question "How does the promotion process account for org health when evaluating managers for promotion?  Specifically if a manager executes well but has poor org feedback."

Common answers:
- HR set a minimum standard during the promo process share a-priori.  HR intervenes during promotion.
  - Weaknesses: HR is reluctant to intervene directly since they lack firsthand knowledge

- [ ] Common Answer provided. Example given.
- [ ] Weaknesses are understood
- [ ] Additional novelty present. Describe them


### Reorganizations

Background: 

  Constant reorganizations are known to be red flags for good leader selection:

  > "When power sensitized teams are confronted with organizational change, internal power struggles are a likely consequence. " - [The dysfunctions of power in teams: A review and emergent conflict perspective](https://www.sciencedirect.com/science/article/pii/S0191308517300084)

> Question: "When was your last re-org.  That is to say how often have you lost a direct-report due to a re-org."

- [ ] < 1 year
- [ ] < 2 year
- [ ] < 3 year
- [ ] 3+ years

> Question: "What was the stated goal in your last re-org?"

- [ ] Don't know
- [ ] Better align with business need 
- [ ] Goal was quantifiable
- [ ] Answer not in above.  <Provide Details>
  
> Follow up: "What were the success criteria to determine if the re-org was successful?"

- [ ] No criteria
- [ ] Qualitative success criteria. <Provide Details>
- [ ] Quantifiable success criteria (KPI). <Provide Details>

### Leadership Attrition

Background:

  I find that the only time you can get honest feedback is when employees leave a company.  Employees will only give honest feedback if they are not at risk of burning bridges.  This is true for an attritioning employee giving management feedback and for other employees giving feedback about that attritioning employee. 

  Most companies don't do exit-interviews.  This is often for legal [reasons](https://www.law.com/thelegalintelligencer/2019/04/29/exit-interviews-do-the-benefits-outweigh-the-risks/?slreturn=20250806172058) as any exit interview records would subject to discovery from employment lawsuits. Thus an company that chooses to perform and record exit-interviews makes a conscious decision to trading better leaders at the cost of their legal liabilities.

> Question: "Does your company do exit-interviews?"

- [ ] Yes
- [ ] No. Follow Up: "Why not?"
   - [ ] Not sure
   - [ ] Data wasn't worth the legal cost
   - [ ] Other reason: <Provide Details>

## Personal Ethics

> [!IMPORTANT]
> This section is unfinished.  It remains unfinished because unless I'm interviewing for a particularly "evil" company or one that doesn't pay well (e.g. a charity), this section isn't necessary to fill out. My opinion is that money solves most social problems, therefore the ability to provide money for charities (through donation matching or just large salary) satisfies my personal ethical requirements.

> [!TODO]
> Finish this section.  It should focus on two ideas:
>
> > "I do not expect leadership to have perfect ethic principles.  However, I do expect them to be able articulate those ethical principles." - Unknown Engineer.  He was pretty cool though.
>
> Ask about a ["past behavior"](https://pmc.ncbi.nlm.nih.gov/articles/PMC4803420/) ethical problem encountered by the company and ask for the ethical principles used to resolve it.
>
> "All religious stuff aside, the fact is, people who can't kill will always be subject to those who can" - Sergeant Brad "Iceman" Colbert 
>
> Similarly people without morals will always be an disadvantage to those without morals -- since an immoral person is bound by strictly fewer rules than a moral one. Thus at the level of the individual, natural selection in social contests tends to [select](https://pmc.ncbi.nlm.nih.gov/articles/PMC10558718/) for the immoral over the moral. The only question then is given a company's processes, how much of an advantage does immorality net you?


## Appendix


### No-solve problem {#no-solve-problem}:

An example of a [no-**win** scenario](https://en.wikipedia.org/wiki/No-win_situation) is the [Kobayashi Maru](https://en.wikipedia.org/wiki/Kobayashi_Maru) wherein the goal is in "testing the character of cadets rather than their actual skills".  

A "no-solve", ["situational"](https://en.wikipedia.org/wiki/Situation,_task,_action,_result) interview is similar except that the goal is still to assess the technical skills of the candidate. They are common in "Large Systems Design" interviews as well as "Systems Debugging" interviews wherein problem constraints are shrunk until the candidate can no longer produce a working solution.  

Examples:

*Large System Design*: 

Example: design a URL shortener that can return a query in less than 10ms.

Interview: "Okay no design the system to return an answer in less than a millisecond"
Candidate: "I'll store data in-memory to get O(micro-second) response times"
Interviewer: "Okay but note you've lost data durability by doing this.  Now pretend like the data set spans millions of names. "
Candidate: "Okay so it can't fit onto one machine.  I partition the data onto multiple servers."
Interviewer: "Okay but now you've increased the probability of dependent services going down if any single server fails.  Can you accommodate for that?"
Candidate: "Not without violating some [CAP](https://en.wikipedia.org/wiki/CAP_theorem) I think... but maybe if you could give more details?"

*Systems Debugging*:

Example: Our service returns a query in >10ms for 1% customer queries.  Find out why.

Candidate: "I check service dashboards to try to figure out which service is slow."
Interviewer: "Okay. Turns out database service is slow but only for 99th percentile of all requests."
Candidate: "I take a look at front-end logs or an RPC trace to figure out if a particular back-end server is slow."
Interviewer: "Yes.  The front end sees database requests time out occasionally on a particular host."
Candidate: "I ping the back-end to figure out if it's a network issue."
Interviewer: "Okay. Root-cause is a network issue but let's roll-back and pretend like the ping didn't show any issue."
Candidate: "Okay. I log onto a machine and check its logs to see if it received the request"
Interviewer: "It did receive a request, but returned it in 10ms."
Candidate: "Oh so that's probably why it didn't failover.  Check logs to see if the database application logs anything interesting errors."
Interviewer: "It does not."
Candidate: "Does it call any outside services or anything?"
Interviewer: "How would you check?"
Candidate: "strace or maybe tpcdump maybe?  Tricky to do but do-able."
Interviewer: "Let's say there's no other downstream service."""
Candidate: "Huh interesting.  Wonder if it's CPU slowness..  does your threading or RPC library support counting instructions executed?"
Interviewer: "Huh... I've never heard of that.  Tell me more."

Strictly speaking, a solution could exist in these scenarios.  However ample human effort has been dedicated to such problems with no solution invented yet.  The classic example of this "P == NP" where attempts at a solution has led to many [insights](https://en.wikipedia.org/wiki/P_versus_NP_problem#Results_about_difficulty_of_proof) into mathematics.

Note that these questions can also be used to evaluate companies by asking an employee to run through a company process.  Examples: promotion, exit-interviews, etc.  Same as in systems design/debugging, the goal is to evaluate whether 
the candidate company understands the common breadth of solutions and if companies have their own novel spin on them.  As such it is important for such questions to include "common solutions". From there nuances can be discussed. If a company does not recognizes the common solutions at all, they are unlikely to be able to avoid the common pitfalls.



## Unused Work

Most of these are difficult [no-solve](#no-solve-problem) situational question.  They could be used if I figure out the right rubrics.

### Organizational building theory

> [!NOTE]
> Question deemed too difficult

Questions:

"Companies tend to form hierarchies?  Why?"

Note: This is a deceptively simple question.  Most will observe that companies with hierarchies tend to out-compete those without, but rarely can explain why.

The follow up question then becomes:

"Given hierarchies are necessary, what is the ideal method for deciding how to organize that hierarchy?"

Most managers will answer meritocracy which [alone](https://gap.hks.harvard.edu/paradox-meritocracy-organizations) isn't a great answer.  Ask for elaboration on what determines merit.

"It's interesting to observe that companies do not form strict meritorious hierarchies.  For example HR is typically silo-ed from the rest of the company.  In what situation should we consider creating that kind of vertical silo?"

"Typically companies have two hierarchies with one leadership track for ICs and one for management.  What kind of prerogative and responsibilities (explicit or implicit) does each type of leader wield at your company?  What kind of reporting structure is used between ICs and managers? Does a level 3 team lead report to a level 4 manager? Why?"

### Promo Process Theory

Tech promo process are often similar to how the legislative and executive branches effectuate laws.  HR communicates a set of (fairly ambiguous) rules to follow. Managers then interpret and applies those rules to their respective domains.  Typically each domain comes up with their own (less ambiguous) rules and gets their respective sub-domains to interpret and execute those rules.  This recurses until we get to the actual candidate being promoted.

Much like legislation, the laws themselves are often well-intended however often lead to [unintended consequences](https://en.wikipedia.org/wiki/Unintended_consequences)

Note: Performance rating usually follows the same type of strategy but using different committees to figure out those rulings

> Question: "What is your company's goal in promoting people?" 

- "As a reward for good work."
  Follow up: "Why not just pay them more as a reward?"

- "To ensure we get meritocratic leaders to make decision."
  Follow up: 
    - "Does this mean non-leaders are not permitted to make those decision?"

- "To establish a meritocratic hierarchy in which technical decisions disagreements are decided by the technical (IC) hiearachy and management decision tie-breaks are decided by the management hierarchy."

- "To decide what level of employee should be assigned what level or project"
  Follow up:
    - "Are ICs generally fungible like that?"

