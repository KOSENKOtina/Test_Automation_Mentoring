<h3>Task 1 answer</h3>
<n>
 I am currently a part of the team working for a client, who has been outsourcing their work to EPAM for 12+ years. This means, the applications we develop and support appear to be huge systems, which consist of lots of services. It would be near to impossible to manage the releases without test automation, or would require enormous number of manual testers to do “monkey job” rerunning same test cases over and over again, let alone writing them. That is one of two main reasons we use automation broadly, trying to cover as much as possible, even including edge cases, if we have capacity to do so.
<br></n>The second main reason we have automation is to have fast feedback on newly developed code.<br> It is a very common situation when our tests catch bugs just after new build of the application becomes available. Moreover, if written clearly, developers might run them locally before even trying to merge their code to master branch. However, I hardly ever seen such devs, they’re like unicorns😊
It is very important to have balance in the Test Automation Framework(TAF), so that there’s not too many and not too little tests. Apart from Unit-tests(which are usually written by developers), the first thing that has to be automated is application’s services or APIs. 
<br></n>First, we need healthchecks, also known as smoke checks. These are fast tests, which run as often as the budget permits. It’s important to use an effective alerting system for them. After that, it is helpful to have some complicated API tests. They will show, if a piece of functionality was broken or impacted. The last chunk of tests we might add to API suits consists of some e2e user scenarios. For example: login->create an event->edit an event-> delete an event -> logout.
<br></n>Regarding UI tests, the builds to run should have nearly same structure as API. One crucial thing they have to have in common is independency. The more independent the suits are – the better. Nevertheless, we should always remember to mimic end user’s workflow to get relevant fast feedback from our tests.

<h3>Task 2 answer</h3>
Let the project be in active development and support for 6 years. Average time required for manual testing is 80 hours per week. <br> 
C_M = 80 man-hours * 52 weeks * 6 years = 24960 <br>
 Considering only first 2 years are dedicated to active development and other 4 to change requests, bug fixes  and support, we will need 120 man-hours per week for the first half a year to implement TAF, a year and a half  to write scripts spending 80 hours per week. It will take 20 hours per week for executing, analyzing results and supporting test for the rest 4 years <br>
FW + S+ E+ R = 120 * 52 * 0.5 + 80 * 2 * 1.5 + 20 * 52 * 4 = 13520
This takes us to ROI <br>
(C_M - I)/I*100% = (24960 - 13520)/13520 * 100% = 85% <br>
Reviewing these calculations, it can be easily understood that there’s a huge benefit of test automation in a long run even if it might be more expensive in the first two years.
