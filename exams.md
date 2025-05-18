---
layout: default
title: Exams
---

<table id="customers">
  <tr>
    <th> # </th>
    <th>Topic</th>
    <th>Date</th>
    <th>Skillset</th>
    <th>Cheat Sheet</th>
    <th>Sample 1</th>
    <th>Sample 2</th>
    <th>Exam & Solutions</th>
  </tr>
  {% for iteml in site.data.exam %}  
    {% assign item = iteml[1] %}
    <tr>
        <td>{{ item.num }}</td>
        <td> {{ item.topic }} </td>
        <td> {{ item.date | date: "%b %d" }} </td>
        <td> 
        <!-- Skillset  -->
            {% if item.skillset %}
            <a href="{{ site.base }}{{ item.skillset }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} skillset"
                    title="{{ iteml[0] }} skillset"
                    src="{{ site.base }}/img/icons/notes.png" />
            </a>
            {% endif %}
        </td>
        <td> 
        <!-- Cheatsheet  -->
            {% if item.cheat_sheet %}
            <a href="{{ site.base }}{{ item.cheat_sheet }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} cheat sheet"
                    title="{{ iteml[0] }} cheat sheet"
                    src="{{ site.base }}/img/icons/cheat_sheet_icon.png" />
            </a>
            {% endif %}
        </td>
        <td> 
        <!-- Sample Exam 1 -->
            {% if item.samp_exam1 %}
            <a href="{{ site.base }}{{ item.samp_exam1 }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} sample exam"
                    title="{{ iteml[0] }} sample exam"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
            {% if item.samp_exam2_sol %}
            <a href="{{ site.base }}{{ item.samp_exam1_sol }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam solutions"
                    title="{{ iteml[0] }} exam solutions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}              
        </td>
        <td>
        <!-- Sample Exam 2 -->
            {% if item.samp_exam2 %}
            <a href="{{ site.base }}{{ item.samp_exam2 }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} sample exam"
                    title="{{ iteml[0] }} sample exam"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
            {% if item.samp_exam2_sol %}
            <a href="{{ site.base }}{{ item.samp_exam2_sol }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam solutions"
                    title="{{ iteml[0] }} exam solutions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}            
        </td>        
        <td> 
            {% if item.exam_questions %}
            <a href="{{ site.base }}{{ item.exam_questions }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam questions"
                    title="{{ iteml[0] }} exam questions"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
            {% if item.exam_solutions %}
            <a href="{{ site.base }}{{ item.exam_solutions }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="{{ iteml[0] }} exam solutions"
                    title="{{ iteml[0] }} exam solutions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}
        </td>
    </tr>        


  {% endfor %}

</table>



&nbsp;

Couple things to note about exams:
- All the midterms will be administered during lecture time in the usual lecture room. 
- The final will be conducted according to the registrar's schedule. 

### Exam Policies

Besides the obvious "don't cheat" exam policies outlined in the [policies page](/policies/cheating) you should know about the following exam procedures: 

#### Exam redemption

**Exam redemption replaces conflict exams.** As per the grading policy, we have included one more exam than normal so that students can miss or "retake" one exam grade each semester. If you miss any of the midterms, the final exam grade will replace the midterm grade you missed. If you complete all the midterms but feel that one (or more) of the midterm grades is not reflective of your mastery of the material, you may take the final and the final grade will replace your lowest midterm score. Note that this is a slight departure from prior years where the final itself could be dropped. After considerable data over the years, I realized that students the vast majority of students would yolo the final and make it difficult for the staff to accurately set a curve that equalized all the exam distributions. Hence, this new modification to the policy is simply to ensure that if you take an exam, you are serious about performing well and if you are already satisfied with your grade, you go and focus on other thigns without guilt.  

This exam redemption has the same purpose as the HW drop - to give students a buffer for those times when life gets in the way. **Should you get sick or maybe have a moment of panic** during one of the exams, you now have a an opportunity for redemption so that one grade won't sink you.  

One critique of this policy is "what if you missed two exams?" I have taught this course more than ~10 times and I have yet to meet someone that missed two exams but had mastered the material. In the past several years that I have taught the course, every case of a student missing two or more exams is accompanied by the student performing in the bottom 10% of the exams they did take. This makes sense when you think about. Missing two exams is indicative of being absent for the majority of the semester which would in turn mean that the material was probably not mastered. 

However, I will make a deal with anyone that is still worried about this. If you miss two exams due to *documented* emergencies but score in the top 20th percentile on the other two exams, I will substitute the lower completed exam grade for one of the missed exams. Note: you must have documentation of the emergency circumstances that required you to miss the two exams. You can email me about the specific requirements for this documentation.  

#### Cheatsheet

I've wrestled with the concept of cheatsheets a lot in past semesters. Ideally, what a cheatsheet is for is to help you memorize tedious equations or details that are easy to forget. However, I like to give exam questions that are very similar to the HWs/labs. In prior semesters, I noticed that cheat sheets didn't contain definitions/algorithms. Instead, they contained copied questions and solutions of HW/lab problems. Basically cheat sheets had become a "guess what Kani might put on the exam"-sheet. Worse, many, many people simply copied the cheatsheet solutions and were frustrated when they learned that those solutions didn't apply to the exam problems. This leaves me with two options: 

- Make sure that the exam problems are changed up so that copying from a HW/lab problem would hurt more than help. 
- Eliminate cheatsheets altogether. 

I think I've come up with a solution that'd help everyone. Over the course of several semesters, we've constructed a communal cheat sheet for each of the exams. These cheat sheets will be posted on the website well in advance of the exam and will be attached to the back of the exam. 

This lets me use problems that many of you have seen before but know that the people answering those problems are doing so because they actually mastered the material. 

#### Use pen

The exams will be scanned and uploaded to Gradescope where they will be graded by the TAs. Unfortunately, last semester we had a problem with a number of individuals that used a pencil with a light touch causing the exam to be illegible. Therefore, we're banning pencils. I'm not going to go around confiscating pencils like some weird pen nazi, but if we see an exam that is difficult to read, we will take off points. Just use pen, if you need to change something you can always cross out the previous answer and make a note for the grader to look at the scratch page.  


### Regrades

Regrades requests would be open for a week once grades are released (except for final exam). Regrade requests are not intended for arguing about point allocation, or whether the grading scale is fair.

Unfortunately, certain students think that they can tire us into giving them point that they did not earn, by keep asking for unjustified regrade requests. This is especially true in the case of exams. I have had students that would submit a grade request for **every single exam problem** hoping for more points. That's not cool. As such, superfluous, argumentative and repetitive regrade requests, after an appropriate warning, would results in a zero on the relevant questions - please do not waste our time.

Again, you should not fear submitting regrades if you have a question that you're confused and didn't gain any insight from the exam solutions (**please check the solutions first**). It's just that in any large group, there will be a few individuals that view teaching as an adversarial relationship and I have to make this stupid announcement for them. I hate it as much as you do. 
 
### DRES
- If you have a DRES accommodation, please email the course staff directly (not sure if sending documents over Piazza is compliant with EHR policies or not, but why risk it). Make sure I respond that I've recorded your accommodation! If I don't respond email again.
- Because of the limited staff, DRES students will take the exams at the [TAC](https://www.disability.illinois.edu/academic-accommodations-and-supports/academic-accommodations/testing-accommodations) synchronously with the rest of the class. We'll hammer out the details closer to MT1. 
- Best thing you can do is to schedule the exams with TAC **now**. That way there is no chance on forgetting to schedule a slot and missing out on your accommodations.  