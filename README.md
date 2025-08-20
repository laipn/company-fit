# Company Fit Interview

## Foreword

It has always seem odd to me that there's plenty of info on structured employee interviews, but candidates themselves lack that same structure when deciding company fit. I thought I'd remedy that for myself.

I've made the doc public because people have asked me about it. Coincidentally it also serves as good way for prospective companies to glean whether I would be a good fit.

I've written in a mostly third-person voice to help me maintain objectivity. First person voice is used for instances that I assume to be subjective to my own personal values.

I was tempted at first to just provide questions and rubrics, but I'm reminded:

> "The fish trap exists because of the fish. Once you’ve gotten the fish you can forget the trap. Words exist because of meaning. Once you’ve gotten the meaning, you can forget the words." - Zhuangzi, Chuang Tsu: Inner Chapters

Providing questions would be pointless without also providing the goal in asking them. Interview questions become [outdated over time](https://web.archive.org/web/20240520214850/https://careercup.com/page?pid=amazon-interview-questions), but the objectives and rationale behind them rarely do.

I've attempted to make the question resilient to [Hawthorne Effects](https://en.wikipedia.org/wiki/Hawthorne_effect). That is to say while HR could attempt to coach interviewers on which rubrics to target, it would ultimately erode trust in HR. For example few things would be more discouraging than say being made to memorize corporate values for an interview. Neverthless, I have ommitted details for a handful of rubrics.

> [!TODO]
> If other people find this useful, then this document should be templated for re-use and sections conditioned on the personal values of the assessor. GPL license has been used to encourage that. Feel free to send a commit for review.

## Introduction

_Defnitions_:

- _Assessor_ refers to the person using this doc to assess a company
- _Assessee_ refers to the person being asked questions

It is important to observe that we aren't trying to "interview the interviewer". The actual management or technical skills of the interviewer is irrelevant. We are "interviewing the company" and its processes. The assessee serves as proxy for their company.

The idea is to fork this doc for each company I interview for and answer questions inline[^markdown_form_support]. Sections can be filled out piecemeal during the "Q&A" stage of an interview but the assessor should note the assesee's job role (IC, manager, etc).

[^markdown_form_support]: Markdown doesn't have great form input support

The company characteristics examined:

1. Work Culture: What company-wide mechanisms exist to ensure a non-toxic workplace.
2. Engineering Culture: Measured by reviewing tech-infrastructure decisions and employee attitudes towards tech-debt.
3. Management Culture: Employee engagement with management and management transparency with employees
4. Leadership Culture: What mechanisms exists to ensure leaders produce healthy orgs.
5. (Experimental) Company Ethics: Whether the company acts with a consistent set of ethical principles.
6. (Unfinished) Personal Ethics: Whether the company is compatible with my own set of ethics.

## Work Culture

> [!IMPORTANT]
> Only managers should answer this section
>
> Manager's [headcount](^manager_ratio).
>
> - [ ] O(1)
> - [ ] O(10)
> - [ ] O(100)
> - [ ] Director

[^manager_ratio]: O(10^X) headcount chosen because manager to employee ratio in tech usually sits at about 1:10

_Definition_: We use the term ["jerks"](https://en.wikipedia.org/wiki/The_No_Asshole_Rule) as shorthand indicating employees who create a toxic workplace.

Each subsection describes a known mechanism commonly used to control for jerks. The goal of each subsection is to see if the company uses those mechanisms and understands their weaknesses.

> [!NOTE]
> These questions have no perfect [solutions](#no-solve-problem). Consider giving the assesee a pre-amble stating this.

**Question**: "How do you filter our jerks during the interview process?"

_Background_

Situational interviews (e.g. [STAR](https://capd.mit.edu/resources/the-star-method-for-behavioral-interviews/)) have a proven track records in interviews. There is little evidence however around their efficacy in removing jerks despite heavy use for exactly that in the tech industry [citation needed].

Studies [suggests](https://pmc.ncbi.nlm.nih.gov/articles/PMC4856718/) that the reason for their efficacy is that it selects for individuals "Knowing How You Should Behave" rather than "How You Would Behave". My experience is that most toxicity in a tech workplace stems from workplace [chameleons](https://newworkplace.wordpress.com/2016/01/25/beware-the-workplace-chameleon/) with self-serving adaptability. Situational interviews selects for these individuals and in fact they are usually [promoted](https://www.researchgate.net/publication/350589033_How_So_Many_Toxic_Employees_Ascend_to_Leadership).

- [ ] Process is in use
- [ ] Complexities understood
- [ ] Additional novelty present. <_Describe Them_>

**Question**: "What mechanisms exists to ensure jerks are selected out in the promotion process?"

_Background_

Strictly speaking, this does not remove jerks. It only ensures they aren't placed in positions of power where toxicity spreads further. Common mechanisms are to use peer feedback as artifacts informing the promotion process. The weaknesses in this mechanisms is that this enforcement is typically at the candidate's manager discretion; and managers are disincentivized to block a promotion if they want to keep their reports happy.

- [ ] Process is in use.
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>

**Question**: "In what circumstances will HR intervene to remove a jerk?"

_Background_

This typically happens if enough HR complaints are levied. I've only seen this happen for gross violations of explicit HR rules. This leaves a lot of leeway where toxicity can spread especially given that HR has little day-to-day interaction with an employee.

- [ ] Process is in use.
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>

**Question**: "Have you ever [managed out](https://medium.com/@janetkahr/the-managing-out-process-d60f94704564) out an employee? What rationale and methods did you use?"

_Background_

Typically hiring and firing is an HR prerogative. "Mangaging out" is the primary way for a manager to remove an toxic or lower-performing employee. The weakness of this approach is that "managing out" usually typically results in an employee leaving for a different team -- which from a company perspective is just a lateral move.

The reason that managers can't easily fire employees is for ["separation of powers"](https://www.investopedia.com/terms/s/separation-powers.asp). Without a separation of powers, you'd see manager favoritism and nepotism abound. By separating the organization that creates HR policies and the organization that executes those policies, no individual can arbitrarily hire/fire people and objectivity is maintained in both.

- [ ] Process is in use.
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>

**Question**: "What is the purpose of the technical hiearchy at the company? Do mechanisms exist to avoid promoting jerks?"

_Background_

Power has a [corrupting effect](https://pmc.ncbi.nlm.nih.gov/articles/PMC10461512/) on orgs. Care must be taken when creating power structures to minimize those effects. For example, not creating hierachy in the first place is one the reasons why [flatter orgs](https://www.tandfonline.com/doi/full/10.1080/00221309.2024.2317247) tend to be less corrupt than taller ones -- though don't mistake cause for effect in that case. While management requires a hierarchy for [compartmentalization](<https://en.wikipedia.org/wiki/Compartmentalization_(information_security)>) reasons, this is less justifiable in a technical hiearachy. The goal of this section is to assess whether a tech hiearachy is in a way that does not select jerks.

_Common answers_:

- Projects are delivered top-down. Project leads are assigned to those at appropriate tech levels.
  - Weakness: Requires people to ascend the tech hiearachy in order to work on fun problems. Difficulty is also determined by management and smart engineers can exploit this. e.g. sandbagging
- Promotion requires delivering value to a company. Seniority is incentive for employees to work on projects more valuable to the company.
  - Weakness: Requires HR to be able to align tech skills with business needs and so is likely to promote people with better tech skills.
- Tech hierarchy is meritocratic. Higher level indicates higher technical skill. Tech leads are involved in the promo process.
  - Weakness: Less alignment with business needs. Hard to determine what "technical skill" implies.
- Promotion level has no actual power (implicit or otherwise)

  - Weakness: How do technical disagreements get resolved?

- [ ] One or multiple of answers above were given. <_List answers_>
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>

## Engineering Culture

> [!IMPORTANT]
> Only ICs should answer.
>
> Some of these might be too technical. Because we are evaluating the company and not the IC, allow the IC to choose a (yet-unanswered) section.

_Background_

In my experience, good engineering culture can be inferred from the state of a company's technical infrastructure. Soundness in technical infrastructure decisions can often be judged objectively (especially retrospectively). However, it is often unclear whether a lack of good infrastructure stems from a legitimate need. Example: In order to deliver a product on time, a startup uses [JNI](https://en.wikipedia.org/wiki/Java_Native_Interface) to link in existing legacy code.

This ultimately creates varying forms of tech debt. The difference in a healthy engineering culture is that people understand why such tech-debt was created and why it persists.

### Source Code Eco-System

- Repo choice. Example: Mono vs distributed repo
  - Examples: Git, perforce, etc
- Front-end code-viewing support.
  - Examples: Github, Code search
- Code-review support.
  - Examples: Ferrit, critique.
- IDEs
  - Examples: Visual Studio, Intellij, etc.
- Code Symbol search support.
  - Note: Typically requires some tight between build and IDE (or code-search) tools
- Coding standards
  - Additional tools: [Auto-formatting]((https://github.com/google/yapf). Presubmit checks for coding standards. [Example])
- Functional vs Systems vs Integration testing, code-coverage requirements, etc
  - Informational: Are all tests run on every build or is there pruning?
- Code Analysis tools
  - Examples: Code-coverage, race-conditions code-analysis, memory leak code-analysis
  - Presubmit checks on this?
    
- [ ] No Red Flags
- [ ] Red Flags. <_List them_>

**Follow Up**

- [ ] Valid reason given for tech-debt creation
- [ ] Plan for removal
- [ ] Rationale for continuing tech-debt provided
- [ ] None of the above

### Build and Deployment

- CI/CD
  - Examples: jenkins, travis, bazel, github actions, etc
- Code Execution environment
  - Examples: VMs, containers, bare-metal, lambdas
- Build reproducibility.
  - Follow up: Can you build code shipped 10 years ago? Are the build tools themselves compilable from source?
- Build to source-code trackability.
  - Examples: Can you tell which source code file and version was in a build.
- Dynamically linked libraries vs static compiled.
  - Background: DLLs more annoying for debugging and produces limits compiler optimization.
- _Bonus points_:

  - Verifiable builds and provenance. Can build tools me built from source?
  - How do you bisect changes in order to root-cause a bug?

- [ ] No Red Flags
- [ ] Red Flags. <_List them_>

**Follow Up**

- [ ] Valid reason given for tech-debt creation
- [ ] Plan for removal
- [ ] Rationale for continuing tech-debt provided
- [ ] None of the above

### Production Tools

- SLO/SLAs
- On-call rotation.
  - Additiona tools: Pager tools
  - Follow up: Compensation?
- Production monitoring.
  - Examples: [Prometheus](<https://en.wikipedia.org/wiki/Prometheus_(software)>), [Grafana](https://grafana.com/)
- Production logging, collection and aggregation.
  - Examples: [Syslog-ng](https://en.wikipedia.org/wiki/Syslog-ng)
- Customer log/core collection

- [ ] No Red Flags
- [ ] Red Flags. <_List them_>

**Follow Up**

- [ ] Valid reason given for tech-debt creation
- [ ] Plan for removal
- [ ] Rationale for continuing tech-debt provided
- [ ] None of the above

### Debugging Tools

- Core Dump analysis tools
- CPU-level perf tools.
  - Additional tools: perf cli, perf counters
- Network debugging tools.
  - Additional tools: ip cli, traceroute. Are they present in execution environment?
- Cross-server request tracing.
  - Example: rpctrace
- Kernel debugging.

  - Examples: strace, tcpdump, eBPF program

- [ ] No Red Flags
- [ ] Red Flags. <_List them_>

**Follow Up**

- [ ] Valid reason given for tech-debt creation
- [ ] Plan for removal
- [ ] Rationale for continuing tech-debt provided
- [ ] None of the above


### Security

**Question**: "Suppose an SRE wants perform a command on service X could either fix (or cause) an outage.  How does the company make this safe?"

Common Answers:
  - X authenticates SRE before allowing the command to run.  Weaknesses: Any adhoc authentication means that if authentication service is down so is the company.  It's typically better for the SRE to present a time-stamped certificate.  This method also doen't work well if the command itself goes through multiple other services before actually accessing X.  Also note this still isn't sufficient because while the SRE's identity can be established it still needs to be checked against something (e.g. an ACL) before one can know it's safe.
  - Multi-party authentication.  Weakensses: Do this too often and you run into AviD's Rule of Usability: "Security at the expense of usability comes at the expense of security"
  - Server sits inside a physical/virtual network. Weaknesses: The first case is pretty safe but inconvenient. The second case means you need to use a VPN which is less secure.  Both are coarse-grained solutions.  Once you're inside the network you have everything.  It's also easy to do things like spoof source-addresses once inside the network.

**Follow Up**

- [ ] Valid reason given for tech-debt creation
- [ ] Plan for removal
- [ ] Rationale for continuing tech-debt provided
- [ ] None of the above



## Management Culture

> [!IMPORTANT]
> Only ICs should answer

### Employee engagement with management

**Question**: "What are your company's core values? Either implicit or explicit."

_Background_

This question assumes that an workforce engaged with leadership ought to know the answer to these questions.

- [ ] Core values all given
- [ ] Some Core values given
- [ ] No Core values given
- [ ] Company does not have core values
- [ ] Assesee states company is too small to have core values

**Follow Up**: "Can you give an example of how you (or your management) employed these values in the past?"

- [ ] Concrete example given
- [ ] Vague example given
- [ ] Assesee cannot recall
- [ ] N/A

**Question**: "Does your company do Q&As?. If not, why not?"

- [ ] Yes
- [ ] No. Reason: <_insert text_>

**Follow Up**: "Can you give an example of an Q&A that resulted in an action taken by management."

- [ ] Assesee provides a concrete example
- [ ] Assesee provides a vague answer
- [ ] Assesee cannot recall
- [ ] N/A

### Management transparency with employees

**Question**: "Does your company do exit interviews? If not why not?"

_Background_

Giving negative feedback can only have negative consequences on working relationships. Therefore I've found that the only time you can elicit honest feedback is when an employee leave a company. This is true for both an attritioning employee giving feedback about management; and for other employees giving feedback on an attritioning employee.

Most companies don't do exit-interviews for legal [reasons](https://www.law.com/thelegalintelligencer/2019/04/29/exit-interviews-do-the-benefits-outweigh-the-risks/?slreturn=20250806172058) as any exit interview records would subject to discovery for employment lawsuits. Thus a company that chooses to perform exit-interviews makes a conscious decision to trade honest feedback for legal liabilities.

- [ ] Company does exit interviews with record.
- [ ] Company does exit interview with records.
- [ ] Company provides credible reason for not doing exit-interview. <_State reason_>
- [ ] Company does not do exit interview.

**Question**: "Have you ever stronglydisagreed with a management decision? Preferably one that ultimately you had to agree to disagree."

_Background_

The goal of this question is to figure out of how if employees are reluctant to approach leadership about concerns. The actual concern is mostly irrelevant but can be provided if deemed important.

- [ ] Yes
- [ ] No

**Follow Up**: "What did you do about it?"

- [ ] Assesee did nothing
- [ ] Assesee escalated the issue but was eventually convinced they were wrong
- [ ] Assesee escalated the issue but agreed to disagree
- [ ] Aassese escalated the issue initially but eventually gave up
- [ ] N/A

If the issue was escalated:

**Follow Up**: "How far was the issue eventually escalated?"

- [ ] The issue bubbled up to their manager
- [ ] The issue bubbled up to a skip-level manager
- [ ] The issue bubbled up to a an executive
- [ ] The issue bubbled up to HR
- [ ] N/A

## Leadership Culture

> [!IMPORTANT]
> Only managers should answer the following
>
> Manager's [headcount](^manager_ratio).
>
> - [ ] O(1)
> - [ ] O(10)
> - [ ] O(100)
> - [ ] Director

### Leadership Qualities

> [!NOTE]
> While these questions are useful for anyone, the rubrics scoring would depend on your own persoal preferences

**Question**: "Does your org use agile practices? Which ones and why?"

Background:
Note all orgs tend to use at least some agile practices.  The question is if leadership has a good understanding why they've chosen the practices they have or if teams have the agency to choose which ones to use.

_Common answers_:
  - Teams decides which to use.  Follow up: "How was this decided? Through surveys? How was the decision revisited"
  - Whiever ones that studies show to be effective.  *Follow up*: Are those studies specifically tailored for software engineering? In your problem space?

- [ ] One or multiple answers above were given. <_List answers_>
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>

**Question**: "Does your org use KPI practices? How strictly? Does it directly affect promo?"

_Common answers_:
  - Same as in the above

Background:
- [ ] One or multiple answers above were given. <_List answers_>
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>


### Promoting leaders

Selecting good leaders is often more critical than having good processes because:

> “Good governance never depends upon laws, but upon the personal qualities of those who govern. The machinery of government is always subordinate to the will of those who administer that machinery. The most important element of government, therefore, is the method of choosing leaders." - Frank Hebert

Leader are created from either promotion process, from reorganizations and lost via [attrition](https://www.gartner.com/en/human-resources/glossary/attrition). This section examines these processes to see if they select for good leaders. Specifically leaders that won't produce "jerks".

_Background_

Managers are usually evaluated accounting for excellence org healthiness and strategy execution.  The following stresses the former.

> [!NOTE]
> These questions have no perfect [solutions](#no-solve-problem). Consider giving the assesee a pre-amble stating this.

**Question**: "How does the company measure org health?"

_Common answers_:

- HR complaints
  - Weakness: People are wary to HR because it starts a tit-for-tat war between reporter and reportee
- Org surveys
  - Weakness: There's often pressure from execs to score well
- Manager/report/peer feedback

  - Weakness: If peers are chosen by reviewee then this is often exploited. Report feedback is often non-valuable since it typically easy to figure out who provided an instance of negative feedback.

- [ ] One or multiple answers above were given. <_List answers_>
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>

**Question**: "How does the promotion process account for org health when evaluating managers for promotion? Specifically if a manager executes well but has poor org feedback."

_Common answers_:

- HR set a minimum standard during the promo process share a-priori.
  - Weakness: HR is reluctant to intervene directly since they lack firsthand knowledge
- HR intervenes reaches out to block a promotion.

  - Weakness: Not a transparent maneuver

- [ ] One or multiple answers above were given. <_List answers_>
- [ ] Complexities understood.
- [ ] Additional novelty present. <_Describe Them_>


### Reorganizations

_Background_

Constant reorganizations are known to choose leaders poorly:

> "When power sensitized teams are confronted with organizational change, internal power struggles are a likely consequence. " - [The dysfunctions of power in teams: A review and emergent conflict perspective](https://www.sciencedirect.com/science/article/pii/S0191308517300084)

Therefore re-orgs should be minimized to as little as necessary.  The right number could vary from company to company.  The test here is to see if employees in a re-org understand the reason for that re-org.  If employees do not possess a good rationale for that re-org, then the assumption is that the re-org was likely unhealthy.

**Question**: "How often does the average employee experience a re-org affecting <100 people[^min_reorg]?"

*Background*: 

- [ ] Once a 1 year
- [ ] Once every 2 years
- [ ] Once every 3 years
- [ ] 3+ years

[^min_reorg] Large re-orgs rarely matter to ICs because they'll continue reporting to the same line-manager. Average manager to ratio is about 1:10 so any re-org with more than 100 people won't affect ICs usually.

If too many (3+ years then):

**Follow Up**: "What was the reason for your last reorg?"

- [ ] Assesee could not recall the reason
- [ ] Assesse did recall the reason.
- [ ] N/A

If assesee did recall the reason: 

**Follow Up**: "What was the goal (explicit or implicit) in your last re-org?  

*Background*

Constant re-orgs are a sign of bad management as it indicates that teams were not able to organically self-organize to resolve a problem. Similarly in SREs if a service is constantly failing SLOs an incident is often declared which requires a [blame-free](https://sre.google/sre-book/postmortem-culture/) Post-Mortem.  The same is rarely true for re-orgs or failure-to-deliver in general.  

**Question**: 

Answers:

- [ ] To better align with a business need
- [ ] No explicit goal was stated
- [ ] Implicit goal was inferred <_Provide details_>
- [ ] Other. <_Provide details_>

*if no stated goal*, **Follow up** :  "Did the re-org involve any kind of post-mortem on why the previous organization failed?"

If there was a stated goal, **Follow Up*** : "What were the success criteria to determine if the re-org was successful?"

- [ ] No criteria
- [ ] Qualitative success criteria. <_Provide Details_>
- [ ] Quantifiable success criteria (KPI). <_Provide Details_>

## Company Ethics (Experimental)

> [!IMPORTANT]
> This section is **Experimental** because it is interviewing the assessee's skills rather than company processes. The problem with trying to assess a company ethical principles is that company ethics are often implicit rather than explcit.  There are good reasons for this (see "Don't be evil [lawsuit](https://en.wikipedia.org/wiki/Don%27t_be_evil#Lawsuit)").  Thus the only way to assess a company's implicit ethics are to assess an individual's understanding of it.

> [Hanlon's razor](https://en.wikipedia.org/wiki/Hanlon%27s_razor) does apply here however.  An incorrect answer could just mean that an individual lacks understanding of those ethics.  The only useful control mechanism I can see here, is to require that the assessor be someone high up the company --  as good ethical principles tends to [flow top-down](https://pmc.ncbi.nlm.nih.gov/articles/PMC6180164/)
>
> Manager's [^headcount]:
> ~~[ ] O(1)~~
> - [ ] O(10)
> - [ ] O(100)
> - [ ] Director

Background:

All companies of a certain size will have a published code of conduct. However application of that code is rarely equal nor equitable.  To illustrate compare HR to a goverment judiciary branch.  Both do defer (nominally) to an codified ["supreme" law](https://en.wikipedia.org/wiki/Supremacy_Clause): U.S. Constitution vs Company Code of Ethics.  Both HR and the supreme court are responsible for ruling on that code. However in government, courts **must** resolve any conflicts and set precedents related to the Constitution as matter for public record.  HR however tends to exercise arbitrary (discretion)[https://en.wikipedia.org/wiki/Prosecutorial_discretion] in what ethical violations to pursue -- typically only violations with legal liabilities, e.g. discrimination, sexual harassment -- and leaves no record to set further precedent.

This typically leads to two unfortunate attitudes:

1.  "You can do whatever you want as long as the company doesn't risk a lawsuit" and
2.  "If you do something the company does not like, the lack of public precedent allows the use of the code of ethics as a reason for termination"

This also leads to the average employee knowing nothing about their code of ethics, whereas the average citizen can at least quote some constitutional law.  Understanding the code of ethics has no actual value to the employee, and thus is ineffectual as an ethical control process in the company. 

The only ethical principles that do persist are those implicitly propagated [memetically](https://en.wikipedia.org/wiki/Meme) -- for example consider "do no evil" as a meme that people even outside of that company **do** remember even if they cannot exactly express what it means.  Thus companies exhibit  *explicit ethical principles* that "no-one understands" because there is no judiciary function to regularly [rationalize](https://en.wikipedia.org/wiki/Moral_rationalism) them and *implicit ethical principles* that persists via [social intuitionism](https://en.wikipedia.org/wiki/Social_intuitionism). We assess for the latter mostly.  The former is too rare.

> [!WARNING]
> There's little [rote-memorization](#rote-memorization) resistance here. OTOH, the lack of resistance doesnt' matter much because the "correct" answer heavily depends on my own ethical preferences.  So maybe it doesn't matter. 

The questions are all [no-solve problems](#no-solve-problem). Problems constraints are adjusted to ascertain the moral principles in use.  This is necessary because [social intuitionism](https://en.wikipedia.org/wiki/Social_intuitionism) is common.  At the end of the question the assessee should ideally be able to outline the moral reasoning they used.  This mirrors ["Heinz's Dilemma"](https://en.wikipedia.org/wiki/Heinz_dilemma) style of questions.  If they cannot explain their moral reasoning, there is a good chance to don't exercise moral reasoning often.  For ICs this is fine, for leadership this is concerning.

### [Applied](https://en.wikipedia.org/wiki/Applied_ethics) Ethics

This section infers the set of ethical principles practiced at a company.

> **Question**: "Your report sends you an expense report.  He expenses a phone he uses for oncall work, but you know for a fact that the existing phone he uses is less than 1 years old and works fine."

Common answers and follow up:

- "Ask the report why he needs the phone"
  - Follow up: "He wants to send it back to his poor relative in Vietnam where it's difficult to get electronics"
  - Follow up: "He wants to give it to his friend."
- "I reject the request. It would be immoral to do so because the money belongs to the company.  Use your own money"
  - Follow up: "Do companies have the same inherent moral property rights that humans do?"
  - Follow up: "Reports tell him that doing it on company money actually saves money because it's a non-taxable business expense"
    - Follow up: "That's illegal.... yes... does illegality always imply immorality?"

> *Follow Up*: Explain (e.g. flow-chart) the ethical decision-making you used to derive at your solution.

> **Question**: "You overhead an employee X stating that one of your direct reports underperforms. What do you do?"

Common answers and follow up:
- "Do nothing".  People are entitled to their own opinion.
  - Follow up: "What if instead of underperforming, the gossip is that the report is toxic?"
- "It depends, do I hear this in public? Or accdientally from a supposedly private convo?.  If it's public, I inform my report of that feedback"
- "I contact the gossiper's manager and ask how that employee can improve?"
  - Follow up: "The employee retracts and apologizes for their statement"

> *Follow Up**: Explain (e.g. flow-chart) the ethical decision-making you used to derive at your solution.

**Follow Up**: Same question but you are the report.

**Follow Up**: Same question but you are the manager's manager.

**Follow Up**: Same question but you are X's manager.

### [Normative](https://en.wikipedia.org/wiki/Normative_ethics) Ethics

This section seeks to determine how ethical norms are being decided.

> [!TODO]
> Finish this section. Some ideas:
>
> > "I do not expect leadership to have perfect ethic principles. However, I do expect them to be able articulate those ethical principles." - Unknown Engineer. He was pretty cool though.
>
> Ask about a ["past behavior"](https://pmc.ncbi.nlm.nih.gov/articles/PMC4803420/) ethical problem encountered by the company and ask for the ethical principles used to resolve it.
>
> "All religious stuff aside, the fact is, people who can't kill will always be subject to those who can" - Sergeant Brad "Iceman" Colbert
>
> Similarly people without morals will always be an disadvantage to those without morals -- since an immoral person is bound by strictly fewer rules than a moral one. Thus at the level of the individual, natural selection in social contests tends to [select](https://pmc.ncbi.nlm.nih.gov/articles/PMC10558718/) for the immoral over the moral. The only question then is given a company's processes, how much of an advantage does immorality net you?


## Personal Ethics (Unfinished)

This section isn't putting ethics under a microscope per se, it's assessing whether the company at face value (e.g. it's role in progressing/harming society, charitable initiatives, etc) is compatible with my own set of ethics.  As such there are a lot of [trolly problems](https://en.wikipedia.org/wiki/Trolley_problem) at play.

> [!IMPORTANT]
> This section is unfinished. It remains unfinished because unless I'm interviewing for a particularly "evil" company or one that doesn't pay well (e.g. a charity), this section isn't necessary to fill out. My opinion is that money solves most social problems, therefore the ability to provide money for charities (through donation matching or just large salary) satisfies my personal ethical requirements.
> 
> In terms of ethical preferences, I tend to favor [individualizing moral foundations](https://en.wikipedia.org/wiki/Moral_foundations_theory#Main_five) which explains why [charitable donations](https://journals.sagepub.com/doi/10.1002/per.2256) is important.


## Appendix

### Interview methodology

A lot of the design in these questions take inspiration form existing interviewn methods.  We list common interview strategies below for reference.  Note however because we are evaluating an organization rather than an invidiual, one should not assume that the same reasoning behind their use and measumre is re-used.

#### Resistance to rote memorization {#rote-memorization}

It's important to note that regardless of interviewing method, all good interview methods must be resistance to rote memoriation.  Specifically one could provide the candidate solution to the question being asked before-hand, but even with that solution a candidate without the assessed skills will still be unlikely to pass.  Put another way, studying to pass an the interview ought to guarantee that the candidate has learned the (suitably difficult) skill being assessed for. 

**Examples**

Question with bad rote-memorization resistance: "Can you tell me why a hostname lookup fails?" 
Answer: "nslookup, hostname... TLD DNS servers, etc.  First lookup is usually in /etc/hosts... ".  An AI prompt *will* give you the answer.  

Question with good rote-memorization resistance: "Why is hostname lookup implemented the way it is?  How do you prefer to ipmlement DNS resolution at a company?" 
Answer: "Originally for historical reasons.  Memorizing IP addresses was difficult. However this was when security was not a concern.  Nowadadays control over DNS is a very easy way to DDoS an entire service.  There is technically no reason why you can't roll out your own resolution protocol for internal usage.  Externally however DNS is langua franca and in that case it typically fucntions as a very coarse grained load-balancer.  Only touch it if your public-facing load-balancers are problematic. The bulk of actual load-balancing though is still better left to dedicated servers which reverse-proxy traffic".

To evaluate whether an interview has good rote-memorization resistance consider that a interview process typically involves:

- Perform interview and collect rubrics
- Send rubrics to committee, anonymizing all personal information.
- Comittee uses rubrics to assess performance.  Committee provides a final scoring or pass/fail.

Consequentially, "Rote memorization" resistance can be measured by the following study:

1. Prepare a pool of interview questions.
2. Have a candidate go through the interview process for a randomly chosen question.
3. Gather the rubrics and perform commitee scoreing.  
4. Give the rubrics and comitte scores back to the candidate for study.  Wait X days.
5. Repeat 2.
6. Repeat 3

If the candidate population performs statistically much better the second time around, then we know that the interview process itself is learnable -- which implies the skill we are **actually** testing for is trivially learn-able.  Similarly if we want to confirm that a pool of questions *is* actually testing for a particular skill, simply confirm that candidates passing on the first round also consistentl pass on the second.

*Aside*: The statistical model here is tricky to get right.  If for example question quality is of very high variance then it may skew results.  As such it's important to to ensure that the 1-st round "pass-rates" for all interview questions remain about the same.  Another tweak on this methodlogy is to just repeat interiews until an assesee hits a point of diminishing returns (upper-limit) on pass-rate.  The statical inference here would be for both the upper-limit *and* the number of tries to reach that upper limit.

Note this isn't a novel test for interview validity. See ["Why Do Situational Interviews Predict Performance? Is it Saying How You Would Behave or Knowing How You Should Behave?"](https://pmc.ncbi.nlm.nih.gov/articles/PMC4856718/).  

> **Interviewees’ Ability to Identify Criteria (ATIC) and the Validity of Situational Interviews**
>
>  Recently, Kleinmann et al. (2011) presented another explanation for the criterion-related validity of personnel selection procedures in general, including situational interviews. Their explanation assumes that individuals actively strive to successfully handle the situations that they are faced with during the selection procedures, so as to attain positive evaluations. According to Kleinmann et al., this ATIC refers to whether individuals are able to correctly decipher the situational demand characteristics and use them to guide their behavior. ATIC reflects an ability that not only helps individuals to better read the situational demands in interviews, but also those in work contexts. Thus, situational interviews predict performance because they capture whether interviewees are able to read situational demands—or in other words know how they should behave to master performance-relevant situations—both during the interview and on the job (cf. Ingold et al. 2015; Jansen et al. 2013). Thus, for this explanation, it is relevant that ATIC as a common cause is positively related to both performance in the interview and performance in work-related situations. Thereby, ATIC contributes to the criterion-related validity of situational interviews because these interviews capture interviewees standing on this general ability that helps individuals to better read the situational demands in varying social situations, including selection and job contexts.

#### Programming Puzzle 

This is the most common type of technical interview anbd there exists a [lot](https://www.amazon.com/Cracking-Coding-Interview-Programming-Questions/dp/0984782850) of [material](https://leetcode.com/).  However much of that material are simply enumerations of commonm interview questions, they fail to actuallys state *why* companies ask these questions and rubrics used to measure success.  What I notice is that the majority of companies ask these questions primarily because:

- By asking the *same* questions with the *same* solution, fairness and stability can be maintined in the interview process.  Quality of candidates that pass remain above a certain bar.
- Studies show that candidates that do pass tend to do well at the company

However without an actual stated objective and stated rationale why an interview satisfies that objective, the result still is just a ["cargo-cult"](https://en.wikipedia.org/wiki/Cargo_cult#As_a_metaphor) of what other companies.  As such most companies focus on the "pass-fail" aspect and not establishing explicit rubrics around the questions. "Pass-Fail" is easy to measure, creating "rubrics" to fairly assess desired candidate skills is hard.

There are a handful of companies that I think *do* have an udnerstanding of the objectives.  Simply stated, the objective is to figure out whether:

1.  A candidate has the problem-solving skills to be able to decompose difficult technical problems.
2.  A candiate has the problem-solving skills to be able to teach and prove their correctness of the solution in 1.

Evidence for 1 can be glaned by observing that "Programming Puzzles" "comp sci" questions were preceeded by lateral-thinking "round man-hole" kinds of test.  The former replaced the latter mostly because

> "Methods that had a transparent relationship between test content and job duties, such as interviews, work samples, and reference checks were perceived more favorably,"

However the necesscity to measure problem-solving skills still remained a necessity.  

Similary evidence for 2 has some precedent:

>  "If you want to master something, teach it" - [Richard Feynman](https://en.wikipedia.org/wiki/The_Feynman_Lectures_on_Physics), "the great Explainer". Nobel Prize-winning American theoretical physicist.

Additionally It is unheard for a mathematician to publich a solution without being able to provide a proof for correctness.  The same is true for computer scientists and solutions -- note that there is a [logical proof](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_correspondence) on how "mathematical proofs" and "computer program correctness" are related.

"Cargo-cult"-ers generally only look for 1, whereas good companies will focus on 2.  You'll actually see good companies ask problems with no practical solution (e.g. O(N^2) time) for that reason.  The solution isn't important, the problem-solving process (and being able to explain it) *is* what is important.  Good companeis have rubrics centered around exactly this.

#### No-solve problem {#no-solve-problem}

An example of a [no-**win** scenario](https://en.wikipedia.org/wiki/No-win_situation) is the [Kobayashi Maru](https://en.wikipedia.org/wiki/Kobayashi_Maru) wherein the goal is in "testing the character of cadets rather than their actual skills".

A "no-solve", ["situational"](https://en.wikipedia.org/wiki/Situation,_task,_action,_result) interview is similar except that the goal is still to assess the technical skills of the candidate. They are common in "Large Systems Design" interviews as well as "Systems Debugging" interviews wherein problem constraints are shrunk until the candidate can no longer produce a working solution.

Examples:

**Large System Design**

Example: Design a URL shortener that can return a query in less than 10ms.

- Interview: "Okay no design the system to return an answer in less than a millisecond"
- Candidate: "I'll store data in-memory to get O(micro-second) response times"
- Interviewer: "Okay but note you've lost data durability by doing this. Now pretend like the data set spans millions of names. "
- Candidate: "Okay so it can't fit onto one machine. I partition the data onto multiple servers."
- Interviewer: "Okay but now you've increased the probability of dependent services going down if any single server fails. Can you accommodate for that?"
- Candidate: "Not without violating some [CAP](https://en.wikipedia.org/wiki/CAP_theorem) I think... but maybe if you could give more details?"

**Systems Debugging**

Example: Our service returns a query in >10ms for 1% customer queries. Find out why.

- Candidate: "I check service dashboards to try to figure out which service is slow."
- Interviewer: "Okay. Turns out database service is slow but only for 99th percentile of all requests."
- Candidate: "I take a look at front-end logs or an RPC trace to figure out if a particular back-end server is slow."
- Interviewer: "Yes. The front end sees database requests time out occasionally on a particular host."
- Candidate: "I ping the back-end to figure out if it's a network issue."
- Interviewer: "Okay. Root-cause is a network issue but let's roll-back and pretend like the ping didn't show any issue."
- Candidate: "Okay. I log onto a machine and check its logs to see if it received the request"
- Interviewer: "It did receive a request, but returned it in 10ms."
- Candidate: "Oh so that's probably why it didn't failover. Check logs to see if the database application logs anything interesting errors."
- Interviewer: "It does not."
- Candidate: "Does it call any outside services or anything?"
- Interviewer: "How would you check?"
- Candidate: "strace or maybe tpcdump maybe? Tricky to do but do-able."
- Interviewer: "Let's say there's no other downstream service."""
- Candidate: "Huh interesting. Wonder if it's CPU slowness.. does your threading or RPC library support counting instructions executed?"
- Interviewer: "Huh... I've never heard of that. Tell me more."

Strictly speaking, a solution could exist in these scenarios. However ample human effort has been dedicated to such problems with no solution invented yet. The classic example of this "P == NP" where attempts at a solution has led to many [insights](https://en.wikipedia.org/wiki/P_versus_NP_problem#Results_about_difficulty_of_proof) into mathematics.

These questions can also be used to evaluate companies by asking an employee to run through typical company processes. Examples: promotion, exit-interviews, etc. Same as in systems design/debugging, the goal is to evaluate whether
the candidate company has institutional understands of the common breadth of solutions and if companies have their own novel spin on them. As such it is important for such questions to include "common solutions" to provide a common baseline on what constitutes novelty.

#### Spot the issues

These interviews typically start by giving a candidate a code-base (often ahead of an interview) and ask them to explain all the issues present in that code.  These can be actual bugs in the code or simply just known software [anti-patterns](https://en.wikipedia.org/wiki/Anti-pattern).

For some reason I don't see this used much in FANGG interviews.  I suspect this is mostly because it's hard to get a concensus on "good code" vs "bad code" and even harder to measure the value in having "good coders" at a company.

#### "Homework Assignment" interviews

These interviews typically start by giving a candidate a full specification for a problem.  The problems are not programming-puzzle because looking up a solution would be too easy.  Typically they tend to be real-world problems (e.g. design a banking ledger that tracks debit/credits to account ledgers) and often provide a skeleton code base to use.  Providing a working solution is not hard, the interview relies on the interviewers reviewing the code and asking about certain red-flags or (in rare cases) novelties in the solution.

This type of interview requires a lot of effort on both of the interviewer and candidate.  I don't see it used often.

#### ["Situation, task, action, result"](https://en.wikipedia.org/wiki/Situation,_task,_action,_result)

Putting this here just for reference.  Technically all the questions above *are* situational questions.  In practice I see classical STAR interviews used most often to filter out behavior.  However studies [suggests](https://pmc.ncbi.nlm.nih.gov/articles/PMC4856718/) that the reason for the efficacy of STAR is that it selects for individuals "Knowing How You Should Behave" rather than "How You Would Behave".  This suggests STAR is particularly ill-suited for testing for toxicity and has poor [rote-memorization](#rote-memorization) resistance.  This is why other interview methods outlined above are used for technical interviews.

## Unused Work

Most of these are too difficult to solve or lack good rubrics.

### Organizational building theory

**Question**: "Companies tend to form hierarchies? Why?"

Note: This is a deceptively simple question. Most will observe that companies with hierarchies tend to out-compete those without, but rarely can explain why.

**Follow Up**: "Given hierarchies are necessary, what is the ideal method for deciding how to organize that hierarchy?"

- Common answer: Meritocracy.
  - Weakness: Meritocracy [alone](https://gap.hks.harvard.edu/paradox-meritocracy-organizations) isn't enough. Ask for elaboration on what determines merit.

**Question**: "Companies do not form strict meritorious hierarchies. For example HR is typically silo-ed from the rest of the company. In what situation should we consider creating that kind of vertical silo?"

### Tech Debt Attitudes

#### Production philosophy 

**Question**: "When do you prefer to fail fast or fail open?"

*Common answers*:
- SREs generally should prefer to fail fast because failing early gives less time for an issue to spread
- Failing open should generally only occur if you don't have any failure domains or failover systems to fall back to.  This happens a lot in networking services.  For example updating DNS services should generally fail open.

**Question**: "How does your company use failure domains in production?"

*Common answers*:
- Red/blue push pipelines
- Cloud regions

#### Dev philosophy

**Question**: "Can you list a "favorite" language that you've used often but actually consider another language superior?"

Background: A lot of "dinosaur" languages are popular only because of inertia. There's always new and upcoming languages are better for productivity but tech-debt means they are only used for new projects

*Common answers*:

- C++ is generally regarded as a very "bad" language by purists but is successful because of its legacy integration with C.
- Java is also heavily used in the business sector for similar reasons but has been supplanted by golang in a lot of cases.  The OOP of Java has actually proven detrimental.  People at first preferred to use python in cases where OOP was too restrictive or golang when they needed the performance
- Same is true for Rust vs C++
