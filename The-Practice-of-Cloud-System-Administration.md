# The Practice of Cloud System Administration: DevOps and SRE Practices for Web Services, Volume 2
Thomas A. Limoncelli, Strata R. Chalup, and Christina J. Hogan

<img src="https://github.com/jeffjryan/images/blob/master/ThePracticeOfCloudSystemAdministration.jpg" width=200>

Last accessed on Thursday May 3, 2018
213 Highlight(s)

## Location: 654
The system is resilient to failure. Rather than being surprised by failures and treating them as exceptions, the architecture accepts that hardware and software failures are a part of the physics of information technology (IT).
                

## Location: 731
There is a “playbook” of instructions on how to handle every alert that can be generated. Each type of alert is documented with a technical description of what is wrong, what the business impact is, and how to fix the issue. The playbook is continually improved.
                

## Location: 736
All failures have a corresponding countermeasure, whether it is manually or automatically activated. Countermeasures that are activated frequently are always automated.
                

## Location: 739
The less frequently a countermeasure is activated, the less confident we are that it will work the next time it is needed. Therefore infrequently activated countermeasures are periodically and automatically exercised by intentionally causing failures.
                

## Location: 793
In distributed systems, failure is normal. Hardware failures that are rare, when multiplied by thousands of machines, become common. Therefore failures are assumed, designs work around them, and software anticipates them. Failure is an expected part of the landscape.
                

## Location: 807
Systems should export metrics. They should count interesting events, such as how many times a particular API was called, and make these counters accessible.
                

## Location: 973
CAP stands for consistency, availability, and partition resistance. The CAP Principle states that it is not possible to build a distributed system that guarantees consistency, availability, and resistance to partitioning. Any one or two can be achieved but not all three simultaneously. When using such systems you must be aware of which are guaranteed.
                

## Location: 1,097
Sorry, we’re unable to display this type of content.
        

## Location: 1,098
Figure 1.10: Numbers every engineer should know
                

## Location: 1,167
Designing for operations means making sure all the normal operational functions can be done well. Normal operational functions include tasks such as periodic maintenance, updates, and monitoring. These issues must be kept in mind in early stages of planning.
                

## Location: 1,172
The best strategy for providing a highly available service is to build features into the software that enhance one’s ability to perform and automate operational tasks.
                

## Location: 1,179
Configuration • Startup and shutdown • Queue draining • Software upgrades • Backups and restores • Redundancy • Replicated databases • Hot swaps • Toggles for individual features • Graceful degradation • Access controls and rate limits • Data import controls • Monitoring • Auditing • Debug instrumentation • Exception collection
                

## Location: 1,198
Rather than the term “operational requirements,” some organizations use the term “non-functional requirements.” We consider this term misleading.
                

## Location: 1,271
It must be possible for software upgrades to be implemented without taking down the service.
                

## Location: 1,337
Toggles for Individual Features
                

## Location: 1,347
Graceful Degradation
                

## Location: 1,427
Software needs to generate logs that are useful when debugging. Such logs should be both human-readable and machine-parseable. The kind of logging that is appropriate for debugging differs from the kind of logging that is needed for auditing.
                

## Location: 2,817
Threading Data can be processed in different ways to achieve better scale. Simply processing one request at a time has its limits. Threading is a technique that can be used to improve system throughput by processing many requests at the same time.
                

## Location: 2,943
Graceful degradation,
                

## Location: 2,962
Resilient systems continue where predictive strategies leave
                

## Location: 2,966
Resilient systems decouple component failure from user-visible outages.
                

## Location: 2,967
survivable systems,
                

## Location: 2,970
Software Resiliency Beats Hardware Reliability
                

## Location: 2,973
Software solutions are favored for many reasons. First and foremost, they are more economical. Once software is written, it can be applied to many services and many machines with no additional cost (assuming it is home-grown, is open source, or does not require a per-machine license.) Software is also more malleable than hardware. It is easier to fix, upgrade, and replace.
                

## Location: 2,983
Everything Malfunctions Eventually
                

## Location: 3,004
Sheltered from the reality of a world full of malfunctions, we enable software developers to continue writing software that assumes a perfect, malfunction-free world (which, of course, does not exist).
                

## Location: 3,017
Distributed computing, in contrast to the traditional approach, embraces components’ failures and malfunctions. It takes a reality-based approach that accepts malfunctions as a fact of life.
                

## Location: 3,788
The three sources of work are life-cycle management, interacting with stake-holders, and process improvement and automation. Life-cycle management is the operational work involved in running the service. Interacting with stakeholders refers to both maintaining the relationship with people who use and depend on the service, and prioritizing and fulfilling their requests. Process improvement and automation is work inspired by the business desire for continuous improvement.
                

## Location: 3,793
Emergency Issues:
                

## Location: 3,796
Normal Requests:
                

## Location: 3,798
Project Work:
                

## Location: 3,821
The team manager should be part of the operational rotation.
                

## Location: 3,831
Meta-work There is also meta-work: meetings, status reports, company functions. These generally eat into project time and should be minimized.
                

## Location: 3,838
developing software that automates or optimizes aspects of the team’s responsibilities.
                

## Location: 3,857
building organizational memory.
                

## Location: 3,879
shift report
                

## Location: 3,885
Every operations team should have a goal of eliminating the need for people to open tickets with them, similar to how there should always be a goal to automate manual processes.
                

## Location: 3,889
Any ticket created by an automated system should have a corresponding playbook entry that explains how to process it, with a link to the bug ID requesting that the automation be improved to eliminate the need to open such tickets.
                

Note | ## Location: 3,893
End of shift report

## Location: 3,899
Theme
                

## Location: 3,907
Toil Reduction
                

## Location: 3,937
7.4.2 Communication Policies Many teams establish a communication agreement that clarifies which methods will be used in which situations. For example, a common agreement is that chat rooms will be the primary communication channel but only for ephemeral discussions. If a decision is made in the chat room or an announcement needs to be made, it will be broadcast via email. Email is for information that needs to carry across oncall shifts or day boundaries. Announcements with lasting effects, such as major policies or design decisions, need to be recorded in the team wiki or other document system (and the creation of said document needs to be announced via email). Establishing this chat–email–document paradigm can go a long way in reducing communication problems.
                

## Location: 3,947
Operations in distributed computing is done at a large scale. Processes that have to be done manually do not scale. Constant process improvement and automation are essential.
                

## Location: 3,949
Operations is responsible for the life cycle of a service: launch, maintenance, upgrades, and decommissioning. Maintenance tasks include emergency and non-emergency response. In addition, related projects maintain and evolve the service.
                

## Location: 3,952
Checklists
                

## Location: 3,953
The most productive use of time for operational staff is time spent automating and optimizing processes.
                

## Location: 3,988
In a DevOps organization, software developers and operational engineers work together as one team that shares responsibility for a web site or service.
                

## Location: 3,991
DevOps combines some cultural and attitude shifts with some common-sense processes. Originally based on applying Agile methodology to operations, the result is a streamlined set of principles and processes that can create reliable services.
                

## Location: 3,997
We find that (1) operator error is the largest single cause of failures in two of the three services, (2) operator errors often take a long time to repair, (3) configuration errors are the largest category of operator errors, (4) failures in custom-written front-end software are significant, and (5) more extensive online testing and more thoroughly exposing and detecting component failures would reduce failure rates in at least one service.
                

## Location: 4,007
DevOps
                

## Location: 4,012
At its most fundamental level, DevOps is about breaking down silos and removing bottlenecks and risks that screw up an organization’s Development to Operations delivery lifecycle. The goal is to enable change to flow quickly and reliably from specification through to running features in a customer-facing environment.
                

## Location: 4,017
operationalism
                

## Location: 4,028
“DevOps is not a technology problem. DevOps is a business problem,” Damon Edwards
                

## Location: 4,044
It is impossible to understand the operational requirements of a system until at least the design is complete, or in many cases until it is deployed and in active use.
                

## Location: 4,072
In a DevOps environment, developers and sysadmins share the responsibility for meeting uptime requirements, so much so that both share oncall duties.
                

## Location: 4,077
There is no concept of “them,” as in “hand off to them”; there is only “us”—the team working on the product.
                

## Location: 4,081
mandating that operations, development, and business departments work together,
                

## Location: 4,084
The Three Ways of DevOps”
                

## Location: 4,128
The third way involves creating a culture where everyone is encouraged to try new things.
                

## Location: 4,142
Another principle of DevOps is that small batches are better.
                

## Location: 4,150
Velocity is how many times you ship in a month. High velocity and low latency are realized through releasing small batches.
                

Blue highlight | ## Location: 4,156
The first step in adopting the Three Ways is to identify the team’s value streams—processes done for the business, or requested by the business.
                
Note:Value Stream

Blue highlight | ## Location: 4,162
Collect measurements on the length, frequency, and failure rate of the steps.
                

## Location: 4,164
Find the steps that are the most error prone, unreliable, or slow. Replace them, improve them, or eliminate them. The two biggest inefficiencies are rework (fixing mistakes) and redundant work (duplicate effort that can be consolidated).
                

## Location: 4,166
The most beneficial place to put energy into improvement is at the bottleneck.
                

## Location: 4,170
Making all of this happen requires a culture of innovation and a willingness to take risks.
                

## Location: 4,186
adherence to some of the basic Agile principles is definitely required.
                

## Location: 4,196
DevOps can be viewed as system administration reinvented by sysadmins who finally had management support to do it the right way.
                

## Location: 4,199
Site Reliability Engineer (SRE)
                

## Location: 4,204
The tools are engineered to make operations self-service for developers.
                
Note:Need to develop common monitoring and automation tools, that cross applications.

## Location: 4,212
Relationships • Integration • Automation • Continuous improvement
                

## Location: 4,219
“People over process over tools.” Once the right people are performing the right process consistently, only then does one create a tool to automate the function.
                

## Location: 4,220
One of the key defining principles of DevOps is the focus on people and process over writing a script and then figuring out who should run it and when.
                

## Location: 4,229
DevOps strives for simplicity and repeatability. Configurations and scripts are handled as source code and kept under version control.
                

## Location: 4,240
Treat your processes like applications and build error handling into them.
                

## Location: 4,260
Game Day Exercises: Sometimes known as “fire drills,
                

Pink highlight | ## Location: 4,264
Striving for perfection discourages innovation, but too much innovation means taking on too much risk.
                

## Location: 4,265
Google’s Error Budgets
                

## Location: 4,270
Common Technical DevOps Practices
                

## Location: 4,304
Release engineering is the process of taking software in source form, building it, packaging it, testing it, and deploying it into the field.
                

## Location: 4,349
Ideally, get development and operations under one management team, the same vice president, or something similar. Also try to colocate
                

## Location: 4,569
As fear of change increases, innovation declines.
                

Note | ## Location: 4,595
metrics to consider

## Location: 4,829
The two major strategies for configuration are called convergent orchestration and direct orchestration. Convergent orchestration takes a description of how the environment should be configured, and the configuration management system then makes individual changes that lead to the entire system converging on that desired state. If
                

## Location: 4,966
Baked versus Fried Configuration management
                

## Location: 4,975
Different Files for Different Environments
                

## Location: 4,983
The problem with using environment-specific packages is that these files have, essentially, bypassed the testing process. For that reason it is best to keep the use of this mechanism to an absolute minimum, preferably restricting it to files that are low risk or files that can be tested other ways, such as via pre-submit checks.
                

## Location: 4,994
Infrastructure as Code
                

## Location: 5,099
The canary process is a special form of the rolling upgrade that is more appropriate when large numbers of elements need to be upgraded.
                

Pink highlight | ## Location: 5,119
Canarying is an insurance policy against accidental bad releases, not a way to detect bad releases.
                

## Location: 5,161
Blue-Green Deployment
                

## Location: 5,173
Feature toggling is one way to implement the general principle of decoupling deployment and release. Deployment is putting a package into an environment. Release is making a feature available to users.
                

## Location: 5,237
“Gatekeeper”
                

## Location: 5,237
dark launches:
                

## Location: 5,253
database views.
                

## Location: 5,254
This decouples software upgrades from schema changes. Now when the schema changes, each view’s code must change to provide the same abstraction to the new schema. The change in schema and the upgrade of view code happen atomically, enabling smooth upgrades.
                

## Location: 5,261
McHenry Technique.
                

## Location: 5,429
Progressive improvement beats delayed perfection. —Mark Twain
                

## Location: 5,433
We should not make changes to the system; rather, we should instruct the automation to make those changes.
                

## Location: 5,438
modern system administrators must be software developers.
                

## Location: 5,441
System administrators who can write code are more valuable to an employer.
                

## Location: 5,442
However, automation should not be approached as simply developing faster, more predictable functional replacements for the tasks that people perform. The human–computer system needs to be viewed as a whole.
                

## Location: 5,466
Also bear in mind that eliminating a task, whether it is easy, difficult, frequent, or rare, is beneficial because it becomes one less thing to know, do, or maintain. If you can eliminate the task, rather than automating it, that will be the most efficient approach.
                

## Location: 5,475
Sorry, we’re unable to display this type of content.
        

## Location: 5,479
Tasks classified as rare/easy can remain manual. If they are easy, anyone should be able to do them successfully. A team’s culture will influence if the person does the right thing. • Tasks classified as rare/difficult should be documented and tools should be created to assist the process. Documentation and better tools will make it easier to do the tasks correctly and consistently. This quadrant includes troubleshooting and recovery tasks that cannot be automated. However, good documentation can assist the process and good tools can remove the burden of repetition or human error. • Tasks classified as frequent/easy should be automated. The return on investment is obvious. Interestingly enough, once something is documented, it becomes easier to do, thus sliding it toward this quadrant. • Tasks classified as frequent/difficult should be automated, but it may be best to acquire that automation rather than write it yourself. Purchasing
                

## Location: 5,487
commercial software or using free or open source projects leverages the skills and knowledge of hundreds or thousands of other people.
                

## Location: 5,554
When designing automation, ask yourself which view of the human component is being assumed by this automation. Are people a bottleneck, a source of unwanted variability, or a resource? If people are a bottleneck, can you remove the bottleneck without removing their visibility into what the system is doing, and without making it impossible for them to adjust how the system works, when necessary? If people are a source of unwanted variability, then you are constraining the environment and inputs of the automation to make it more reliable. What effect does that have on the people running the automation? How does it constrain their work?
                

## Location: 5,561
The long-term operation of a system can be broken down into four stages: tracking, regulating, monitoring, and targeting. Tracking covers event detection and short-term control in response to inputs or detected events. Automation typically starts at this level. Regulation covers long-term control, such as managing transition between states.
                

## Location: 5,615
There is a popular misconception that the goal of automation is to do tasks faster than they could be done manually. That is just one of the goals. Other goals include the following: • Help scaling. Automation is a workforce multiplier. It permits one person to do the work of many. • Improve accuracy. Automation is less error prone than people are. Automation does not get distracted or lose interest, nor does it get sloppy over time. Over time software is improved to handle more edge cases and error situations. Unlike hardware, software gets stronger over time (Spolsky 2004, p. 183). • Increase repeatability. Software is more consistent than humans when doing tasks. Consistency is part of a well-controlled environment. • Improve reliability. Once a process is automated, it is easier to collect statistics and metrics about the process. These data can then be used to identify problems and improve reliability. • Save time. There is never enough time to do all the work that needs to be done. An automated task should require less SA time than a manual one. • Make processes faster. Manual processes are slower because they involve thinking and typing. Both are error prone and correcting mistakes often has a large time penalty itself. • Enable more safeguards. Adding additional pre- and post-checks to an automated process is easy. Doing so incurs a one-time cost, but improves the automation for all future iterations of the process. Adding more checks to a manual process adds a burden and creates temptation for the person to skip them. • Empower users. Automation often makes it possible for a non-SA to do a task. Automation turns a task that only an expert can do into one that an end user can do using a self-service tool. In the example in Section 12.2.3, someone from the human resources department is now able to provision new accounts without the involvement of system administrators. Delegation saves time and resources. • Reduce user wait time. Manual processes can be done only when an SA is available. Automation can be running all day and all night, and will usually have completed a task before an SA would have been available to start it. Even if automation were slower than a person doing the same task, the net user wait time would likely be shorter. • Reduce system administrator wait time. Many manual processes involve doing one step, then waiting some time before the next step can proceed—for example, waiting for new data to propagate through a system or waiting for a machine to reboot. A process like this is said be full of “hurry up and wait” steps. If the wait is long, an SA may be able to fill the time with other work. However, this is often inefficient. All too often, we start working on something else, get distracted, and forget to return to the first task or lose context. Computers are better at waiting than people are.
                
Note:Goals of automation follow

## Location: 5,651
Automation, however, would be applied where each freshly installed machine looks up its hostname in a directory or external database to find its function. It then configures the machine’s OS, installs various packages, configures them, and starts the services the machine is intended to run. The manual steps are eliminated, such that machines come to life on their own.
                

## Location: 5,682
Automation has many benefits, but it requires dedicated time and effort to create. Automation, like any programming, is best created during a block of time where there are no outside interruptions. Sometimes there is so much other work to be done that it is difficult to find a sufficient block of time to focus on creating the automation. You need to deliberately make the time to create the automation, not hope that eventually things will quiet down sufficiently so that you have the time.
                

## Location: 5,728
Apply any and all effort to fix the biggest bottleneck first. There may be multiple areas where automation is needed. Choose the one with the biggest impact first.
                

## Location: 5,741
You can’t automate what you can’t do manually.
                

## Location: 5,838
The automation tools and their support tools such as bug trackers and source code repositories should be a centralized, shared service used by all involved in software development. Such an approach makes it easier to collaborate. For example, moving bugs and other issues between projects is easier if all teams use the same bug tracking system.
                

## Location: 5,907
A VCS should not be used only for source code; that is, configuration files must also be revision controlled. When automation or use of tools involves configuration file changes, you should automate the steps of checking the config file out of version control, modifying it, and then checking it back in. Tools should not be allowed to modify config files outside of the VCS.
                

## Location: 5,917
A style guide is a standard indicating how source code should be formatted and which language features are encouraged, discouraged, or banned.
                

## Location: 5,923
Style Guide Basics
                

## Location: 7,243
The ideal monitoring system makes the operations team omniscient and omnipresent.
                

## Location: 7,276
Many monitoring systems do not track the units of a metric, requring people to guess based on the metric name or other context, and perform conversions manually.
                

## Location: 7,321
information as follows: Operational Health is
                

## Location: 7,343
16.3 What to Monitor
                

## Location: 7,345
The following are some example KPIs:
                

## Location: 7,345
• Availability:
                

## Location: 7,347
• Latency:
                

## Location: 7,348
• Urgent Bug Count:
                

## Location: 7,350
• Urgent Bug Resolution:
                

## Location: 7,351
• Major Bug Resolution:
                

## Location: 7,352
• Backend Server Stability:
                

## Location: 7,354
• User Satisfaction:
                

## Location: 7,355
• Cart Size: The median number of items
                

## Location: 7,356
• Finance:
                

## Location: 7,360
You need to instrument your system enough so that you can see when things are going to fail.
                

## Location: 7,376
The Minimum Monitor Problem A common interview question is “If you could monitor only three aspects of a web server, what would they be?” This is an
                

## Location: 7,377
excellent test of technical knowledge and logical thinking. It requires you to use your technical knowledge to find one metric that can proxy for many possible problems.
                

## Location: 7,409
reduce storage needs is through summarization, or down-sampling. With this technique, recent data is kept at full fidelity but older data is replaced by averages or other form of summarization.
                

## Location: 7,414
Meta-monitoring
                

## Location: 7,415
Monitoring the monitoring system is called meta-monitoring. How do you know if the reason you haven’t been alerted today is because everything is fine or because the monitoring system has failed?
                

## Location: 7,420
The accuracy and precision of collected data should be monitored; one should monitor how often an attempt to collect a measurement fails.
                

## Location: 7,474
Monitoring is the primary way we gain visibility into the systems we run.
                

## Location: 7,477
The goal of monitoring is to detect problems before they turn into outages, not to detect outages. If we simply detect outages, then our operating process has downtime “baked in.”
                

## Location: 7,479
A measurement is a data point.
                

## Location: 7,481
Identify the business’s key performance indicators (KPIs) and then determine which metrics can be collected to create those KPIs.
                

## Location: 7,502
Sorry, we’re unable to display this type of content.
        

## Location: 7,513
Sensing and Measurement
                

## Location: 7,514
The sensing and measurement component gathers the measurements. Measurements can be categorized as blackbox or whitebox, depending on the amount of knowledge of the internals that is used.
                

## Location: 7,520
Blackbox monitoring means that measurements try to emulate a user.
                

## Location: 7,523
Doing an HTTPS GET of a web site’s main page is an example of blackbox monitoring.
                

## Location: 7,526
Blackbox testing includes monitoring that attempts to do multi-step processes as a user, such as verifying that the purchasing process is working.
                

## Location: 7,533
A whitebox measurement has the benefit of internal knowledge because it is a lower level of abstraction. For example, such a measure might monitor raw counters of the number of times a particular API call was made, the number of outstanding items waiting in a queue, or latency information of internal processes.
                

## Location: 7,538
Direct versus Synthesized Measurements
                

## Location: 7,539
Some measurements are direct, whereas others are synthesized. For example, if every time a purchase is made the system sends a metric of the total money collected to the monitoring system, this is a direct measurement. Alternatively, if every 5 minutes the monitoring system tallies the total money collected so far, this is a synthesized metric.
                

## Location: 7,548
Rate versus Capability Monitoring
                

## Location: 7,549
Event frequency determines what to monitor.
                

## Location: 7,550
The rate at which purchases happen determines which of these to monitor.
                

## Location: 7,553
In short, rate metrics are more important when event frequency is high and there are smooth, predictable trends.
                

## Location: 7,554
When there is low event frequency or an uneven rate, capability metrics are more important.
                

## Location: 7,555
never collect rates directly.
                

## Location: 7,574
A counter is a measurement that only increases—for example, a count of the number of API calls received by a service or the count of the number of packets transmitted on a network interface.
                

## Location: 7,596
Collection Once we have a measurement, we must transmit it to the storage system.
                

## Location: 7,703
Escalation Chain: The escalation chain is who to contact, and who to contact if that person does not respond. Generally, one or two chains are defined for each service or group of services. • Suggested Resolution: Concise instructions of what to do to resolve this issue. This is best done with a link to the playbook entry related to this alert, as described in Section 14.2.5. The last two items may be difficult to write at the time the alert rule is created.
                

## Location: 7,719
Having the ability to negatively acknowledge (“NAK”) the alert saves time during escalations.

## Location: 7,785
The only thing we dislike more than pie charts are averages, or the mathematical mean. Averages can be misleading in ways that encourage you to make bad decisions.
                

## Location: 7,790
That said, averages aren’t inherently misleading and have a place in your statistical toolbox. Like other statistical functions they need to be used wisely.
                

## Location: 7,911
There are two major objectives of capacity planning. First, we want to prevent service interruptions due to lack of capacity. Second, we want to preserve capital investment by adding only the capacity required at any given time.
                

## Location: 7,923
Terms to Know QPS: Queries per second. Usually how many web hits or API calls received per second. Active Users: The number of users who have accessed the service in the specified timeframe. MAU: Monthly active users. The number of users who have accessed the service in the last month. Engagement: How many times on average an active user performs a particular transaction. Primary Resource: The one system-level resource that is the main limiting factor for the service. Capacity Limit: The point at which performance starts to degrade rapidly or become unpredictable. Core Driver: A factor that strongly drives demand for a primary resource. Time Series: A sequence of data points measured at equally spaced time intervals. For example, data from monitoring systems.
                

## Location: 7,963
Future Resources = Current Usage × (1 + Normal Growth + Planned Growth) + Headroom
                

## Location: 8,019
Another component in determining how much headroom is needed is the amount of time it takes to have additional resources deployed into production from the moment that someone realizes that additional resources are required.
                

## Location: 8,080
Core drivers are factors that strongly drive demand for a primary resource.
                

## Location: 8,086
holidays. A more accurate representation of users may be how many were active in the last 7 or 30 days.
                

## Location: 8,173
moving average convergence/divergence (MACD) metric. MACD measures the difference between a long-period (e.g., 3 months) and a short-period (e.g., 1 month) moving average.
                

## Location: 8,215
Resource Regression A resource regression is a calculation of the difference in resource usage between one release or version and another.
                

## Location: 8,233
How many database calls? A single transaction may touch many services within your system infrastructure, and those service resources must be assessed as well and scaled appropriately along with the transaction server scaling.
                

## Location: 8,308
Standard capacity planing is sufficient for small sites, sites that grow slowly, and sites with simple needs. It is insufficient for large, rapidly growing sites. They require more advanced techniques.
                

## Location: 8,309
Advanced capacity planning is based on core drivers, capacity limits of individual resources, and sophisticated data analysis such as correlation, regression analysis, and statistical models for forecasting.
                

## Location: 8,345
Measurement affects behavior. People change their behavior when they know they are being measured.
                

## Location: 8,346
People tend to find the shortest path to meeting a goal. This creates unintended side effects.
                

## Location: 8,349
Setting KPIs is quite possibly the most important thing that a manager does.
                

## Location: 8,350
It is often said that a manager has two responsibilities: setting priorities and providing the resources to get those priorities done.
                

## Location: 8,355
A key performance indicator is a type of performance measurement used to evaluate the success of an organization or a particular activity.
                

## Location: 8,357
KPIs should be directly tied to the organization’s strategy, vision, or mission.
                

## Location: 8,359
A well-defined KPI follows the SMART criteria: Specific, Measurable, Achievable, Relevant, and Time-phrased.
                

## Location: 8,368
Fewer than 10 “severity 1” open bugs.
                

## Location: 8,380
OKRs, which stands for “objectives and key results.”
                

## Location: 8,395
Step 1: Envision the Ideal
                

## Location: 8,395
Pause to imagine what the world would be like if this goal was met perfectly.
                

## Location: 8,402
Step 2: Quantify Distance to the Ideal
                

## Location: 8,410
Imagine How Behavior Will Change
                

## Location: 8,411
What are all the ways that people could behave but still match the incentive? How could a person maximize his or her personal gain?
                

## Location: 8,421
engineers will examine the KPIs given and follow them as stated. Again, this is not “gaming the system,” but simply following the rules.
                

## Location: 8,426
Revise and Select
                

## Location: 8,427
we revise the KPI. We may select one KPI over another or loop back to Step 1 and start over.
                

## Location: 8,428
Seek confirming and non-confirming data.
                

## Location: 8,450
Deploy the KPI
                

## Location: 8,451
or institute it as policy. This is mostly a communication function.
                

## Location: 8,453
Deploying the KPI means making people aware of it as well as putting into place mechanisms to measure the KPI.
                

## Location: 8,456
the process should not require human intervention.
                

## Location: 8,526
Step 5 deploys the KPI. The KPI is communicated to key stakeholders. Measurements required to calculate the KPI plus the computation itself should be automated and presented in a dashboard.
                

## Location: 8,530
Evaluating the KPI A few weeks after deployment, the initial results should be audited for unintended negative side effects.
                

## Location: 8,543
Error Budget Benjamin Treynor Sloss, Vice President of Engineering at Google, revealed a highly successful KPI called Google Error Budget.
                

## Location: 8,569
When the budget is exhausted, all launches stop. An exception is made for high-priority security fixes.
                

## Location: 8,605
Remember that the KPI should be achievable.
                

## Location: 8,637
High-performing organizations have smooth operations, well-designed policies and practices, and discipline in what they do. They meet or exceed the needs of their customers and delight them with innovations that meet future needs often before such needs ever surface. The organization is transparent about how it plans, operates, provides services, and handles costs or charge-backs to customers. The vast majority of customers are happy customers. Even dissatisfied customers feel they have a voice, are heard, and have a channel to escalate their issues. Everyone feels the operations organization moves the company forward. Its funding reflects a reasonable budget for the work the organization does. The organization makes its successes visible and, more importantly, is honest and forthright when it comes to discussing its own faults. The organization is constantly improving. Outages and escalated issues result in action plans that reduce future occurrences of that problem. The world is constantly changing, and the organization incorporates new technologies and techniques to improve its inner workings as well as the services it provides.
                

## Location: 8,676
Operational Responsibilities
                

## Location: 8,680
Regular Tasks (RT):
                

## Location: 8,682
Emergency Response (ER):
                

## Location: 8,685
Monitoring and Metrics (MM):
                

## Location: 8,688
Capacity Planning (CP):
                

## Location: 8,691
Change Management (CM):
                

## Location: 8,693
New Product Introduction and Removal (NPI/NPR):
                

## Location: 8,698
Service Deploy and Decommission (SDD):
                

## Location: 8,702
Performance and Efficiency (PE):
                

## Location: 8,761
look-for’s
                

## Location: 8,761
A look-for is a behavior, indicator, or outcome common to a service or organization at a particular level.
                

## Location: 8,969
A.1 Regular Tasks (RT) Regular Tasks include how normal, non-emergency, operational duties are handled—that is, how work is received, queued, distributed, processed, and verified, plus how periodic tasks are scheduled and performed. All services have some kind of normal, scheduled or unscheduled work that needs to be done. Often web operations teams do not perform direct customer support but there are interteam requests, requests from stakeholders, and escalations from direct customer support teams. These topics are covered in Chapters 12 and 14. Sample Assessment Questions • What are the common and periodic operational tasks and duties? • Is there a playbook for common operational duties? • What is the SLA for regular requests? • How is the need for new playbook entries identified? Who may write new entries? Edit existing ones? • How are requests from users received and tracked? • Is there a playbook for common user requests? • How often are user requests not covered by the playbook? • How do users engage us for support? (online and physical locations) • How do users know how to engage us for support? • How do users know what is supported and what isn’t? • How do we respond to requests for support of the unsupported? • What are the limits of regular support (hours of operation, remote or on-site)? How do users know these limits? • Are different size categories handled differently? How is size determined? • If there is a corporate standard practice for this OR, what is it and how does this service comply with the practice? Level 1: Initial • There is no playbook, or it is out of date and unused. • Results are inconsistent. • Different people do tasks differently. • Two users requesting the same thing usually get different results. • Processes aren’t documented. • The team can’t enumerate all the processes a team does (even at a high level). • Requests get lost or stalled indefinitely. • The organization cannot predict how long common tasks will take to complete. • Operational problems, if reported, don’t get attention. Level 2: Repeatable • There is a finite list of which services are supported by the team. • Each end-to-end process has each step enumerated, with dependencies. • Each end-to-end process has each step’s process documented. • Different people do the tasks the same way. • Sadly, there is some duplication of effort seen in the flow. • Sadly, some information needed by multiple tasks may be re-created by each step that needs it. Level 3: Defined • The team has an SLA defined for most requests, though it may not be adhered to. • Each step has a QA checklist to be completed before handing off to next step. • Teams learn of process changes by other teams ahead of time. • Information or processing needed by multiple steps is created once. • There is no (or minimal) duplication of effort. • The ability to turn up new capacity is a repeatable process. Level 4: Managed • The defined SLA is measured. • There are feedback mechanisms for all…
                Some highlights have been hidden or truncated due to export limits.

## Location: 10,452
http://www.youtube.com/watch?v=Fx8OBeNmaWw
