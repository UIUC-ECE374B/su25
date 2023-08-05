---
layout: default
title: Homeworks
---

<table id="customers">
  <tr>
    <th> # </th>
    <th>Topic</th>
    <th>|Problems|</th>
    <th>Assigned</th>
    <th>Due</th>
    <th>Questions</th>
    <th>Solutions</th>
  </tr>
  {% for iteml in site.data.homework %}  
    {% assign item = iteml[1] %}
    <tr>
        <td>{{ item.num }}</td>
        <td> {{ item.topic }} </td>
        <td> {{ item.num-problems }} </td>
        <td> {{ item.assigned-date | date: "%b %d" }} </td>
        <td> {{ item.due-date | date: "%b %d" }} </td>
        <td> 
            {% if item.questions-link %}
            <a href="{{ site.base }}{{ item.questions-link }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Homework {{ item.num }} Questions"
                    title="Homework {{ item.num }} Questions"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
        </td>
        <td> 
            {% if item.solutions-link %}
            <a href="{{ site.base }}{{ item.solutions-link }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Homework {{ item.num }} Questions"
                    title="Homework {{ item.num }} Questions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}
        </td>
    </tr>        


  {% endfor %}

</table>

&nbsp;

Couple things to note about homeworks:
- Each homework is assigned when you have all (or at least most) of the required knowledge to complete it. In two cases, because of scheduling constraints, one or two problems may require knowledge from the lecture/discussion right after assignment. Either way you'll have the knowledge for those problems by Wednesday. This is a long-winded way of saying: **There is zero reason not to start the homework early**
- Each homework will consist of 3 novel problems and 1-2 problems you've seen in the labs. All the problems counts equally toward your final course grade.
- The homework average consists 24% of your final course grade. We will use the highest 34 scores to calculate your final course grade. Since there are expected to be 43 problems, this means that 9 problems will be dropped (~2 homeworks).
- It's a bad idea to skip homeworks. Homeworks and labs are where I get inspiration for exam problems. 

### Homework Logistics: How to submit

- All homework solutions must be submitted electronically via Gradescope. Submit one PDF file for each numbered homework problem. Gradescope will not accept other file formats such as plain text, HTML, LaTeX source, or Microsoft Word (.doc or .docx).
- **Homeworks are due by noon** of their due date. 
- You **should not** use Canvas to keep track of homeworks or any other course policies and logistics. **Canvas is a gradebook, that's all.**  
- You will be registered with Gradescope using your university email address. If you can't access Gradescope let the course staff know. 
- All homework assignments must be completed and submitted indivudally this semester. No group assignments. 
- As error correction, each submitted homework solution should **include the following information in large friendly letters at the top of every page/problem**. 
    - The homework number
    - The problem number
    - Group names+netids
- **We will not accept late homework for any reason.** To offset this rather draconian policy, we have a very generous number of homework drops (compare to other sections/courses). Also remember you can always resubmit a problem to gradescope. There is zero reason to wait until the last minute to submit your work.  

### Homework Grading Policies: 

- **Homeworks** are graded by the entire course staff, within Gradescope. All numbered homework problems are worth the same amount. Under normal circumstances, all homework should be graded within two weeks of submission.
- Partial credit is given for work that is very close to being correct. 
- **We will give zero points for long and tedious solutions** (i.e., solutions that are longer than the official solutions by a significant amount). We reserve the right of not even reading your solution if it exceedingly and unnecessarily long. If your solutions seems too long - rewrite it to be short and precise. 
- This semester I am limiting solutions text to be **300 words long max** per problem. It is incredibly important to be able to convey complex idea as concisely as possible and I think this is good practice. I highly suggest using figures(flowcharts, graphics)/equations(useful for recurrences) to cut down on the word vomit. 
>If I had more time, I would have written a shorter letter. 
><cite> - [Unknown](https://www.lb7.uscourts.gov/documents/314-cv-921.pdf) <cite>


### Regrades

Regrades requests would be open for a week once grades are released (except for final exam). Regrade requests are not intended for arguing about point allocation, or whether or not the grading scale is fair.

Unfortunately, certain students think that they can tire us into giving them point that they did not earn, by keep asking for unjustified regrade requests. As such, superfluous, argumentative and repetitive regrade requests, after an appropriate warning, would results in a zero on the relevant questions - please do not waste our time.

###### Group homeworks
Homeworks can be completed in groups of at most **three students** as discussed in the [homework policies](https://ecealgo.com/homeworks.html). Ideally, the way it should work is that each individual in a group looks at all the problems and comes up with some quick notes on possible solutions. Then the group would come together and attempt to reach a consensus on each problem. Finally, the solution writing and presentation would be divvied up between the members so alleviate some of the presentation burden. However, I personally am conflicted on group work: 

- **Positive:** If done correctly, it can be a powerful way where students learn from and bounce ideas off one-another. That is definitely a good thing. 
- **Negative:** Since this is my sixth time doing this course, I believe about half the groups simply divvy up the problems and don't even look at the problems not assigned to them. I've done a bit of analysis on past semesters where I've had a exam problem that was nearly identical to a homework problem and consistently, there's been about 25-30% of students that clearly have never seen the problem before. 

In summary, I tend to fall of the side of discouraging group work. From what I've seen, the strongest performing individuals are over-represented in the group of students that do the homework solo. Also I have reduced the homework burden compared to past semesters so a single person should be fine doing all the problems themselves. 
But, I won't get rid of group homeworks all together. Like I say a lot, you guys are adults and should know what works best for you. [My job is to encourage behavior that I believe will be optimal for learning, not force it.](https://www.youtube.com/watch?v=QIBMMVJFM4M) 