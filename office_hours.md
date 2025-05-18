---
layout: default
title: Course Schedules
---
{% if site.archived == true %}
Obviously this course isn't active and there aren't any discussion sections or office hours. But I left a bunch of sample data in the repo to show how the backend works when you need to display a weekly schedule (in this case OHs). It was tricky to get working at the time but I built everything so that you only need to set the time(s) in the people.yml file and everything is beautifully displayed on the schedule table. Super helpful since staff needs to change OH times frequently throughout the semester and all you need to do on your end is to change a few values in the .yml file instead of futzing with a bunch of HTML.   
{% endif %}


#### Synchronous sessions

<table id="customers">
  <tr>
    <th> Section </th>
    <th> Tuesdays and Thursdays at </th>
    <th> Who </th>
    <th> Location </th>
  </tr>
  <tr>
    <td> AL1/OL1 </td>
    <td> 10:00AM - 11:20AM </td>
    <td> Kani </td>
    <td> 2015 ECEB and <a href="https://illinois.zoom.us/j/5828330103?pwd=UkJLNjBpWXFnSytWTHJsVXU4dU1idz09">Zoom</a>
  </td>
  </tr>
</table>
&nbsp;

#### Office hours
Office hours will be conducted by the instructor(s), TAs and CAs. Office hours are not a place to check if your homework solutions are correct (the CAs do not even have access to the homework solutions). Office hours are meant to help you master the course concepts and assist you in working through any assignments when you are stuck. **No office hours the first week of classes. OHs will begin Monday, September 2.**

{% include OHs_table.html %}


