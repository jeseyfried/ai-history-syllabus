---
title: Syllabus
layout: base
---

<div class="scroll-spy-wrapper">
  <nav class="scroll-spy-nav" id="scrollSpyNav" aria-label="Section navigation">
    <h4>Jump to</h4>
    <div class="nav nav-pills flex-column"></div>
  </nav>

  <div id="pageContent" class="page-content" markdown="1">
<script>
document.addEventListener('DOMContentLoaded', () => {
  const container = document.querySelector('#pageContent');
  const nav = document.querySelector('#scrollSpyNav .nav');
  if (!container || !nav) return;
  const headings = container.querySelectorAll('h2');
  headings.forEach(h => {
    let id = h.id;
    if (!id) {
      id = h.textContent.trim().toLowerCase()
        .replace(/[^\w]+/g, '-')
        .replace(/^-+|-+$/g, '');
      h.id = id;
    }
    const a = document.createElement('a');
    a.className = 'nav-link';
    a.href = '#' + id;
    a.textContent = h.textContent;
    nav.appendChild(a);
  });
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        nav.querySelectorAll('.nav-link').forEach(l => l.classList.remove('active'));
        const active = nav.querySelector('[href="#' + entry.target.id + '"]');
        if (active) active.classList.add('active');
      }
    });
  }, { rootMargin: '0px 0px -70% 0px', threshold: 1 });
  headings.forEach(h => observer.observe(h));
});
</script>


<br style="clear: both">
*This is the syllabus that the students receive.*

# History with AI - Course Syllabus
HIST 300-009 <br style="clear: both">
Instructor: Jonathan Seyfried <br style="clear: both">
Office: Amaranth Digital Humanities Studio, Mesa Vista Hall 2068 <br style="clear: both">
email: jseyfried@unm.edu 

## Introductory Material

**Land Acknowledgement:** Founded in 1889, the University of New Mexico sits on the traditional homelands of the Pueblo of Sandia. The original peoples of New Mexico Pueblo, Navajo, and Apache since time immemorial, have deep connections to the land and have made significant contributions to the broader community statewide. We honor the land itself and those who remain stewards of this land throughout the generations and also acknowledge our committed relationship to Indigenous peoples. We gratefully recognize our history.

**Citizenship and Immigration Status:** All students are welcome in this class regardless of citizenship, residency, or immigration status. Your professor will respect your privacy if you choose to disclose your status. UNM as an institution has made a core commitment to the success of all our students, including members of our undocumented community. The Administration’s welcome is found on [our website](http://undocumented.unm.edu).

**Course Description:** This course explores the ways that the new technology of generative Artificial Intelligence (AI) might influence History in the near and distant future. The course will introduce students to the capabilities and limitations of AI chatbots as tools for creating and influencing historical narratives. Using an experiential and workshop approach, students will use AI chatbots during each class meeting and as tools to enhance their thinking for long term assignments. Writing History with AI is both a journey and a construction project; at first you might get lost or use tools inefficiently. Eventually, though, History with AI will help you access new ways of thinking of the past.

**Student Learning Outcomes:** <br style="clear: both">
By the end of this course you will be able to:
- carefully use AI provocations to enhance your critical thinking skills
- distinguish between summaries that limit human thinking and lenses that enhance human thinking
- recognized the tendency for AI chatbots to provide information limited by the normativizing pressures of their training sets
- write History with AI while thinking of it as a journey and as a construction project

**Required Readings:** All required readings will be posted to Canvas either as PDFs or links. The links will be to content available at no cost to you, either because they are on free websites or paid for by UNM Libraries.

## Attendance and Participation
Success in a workshop-style course such as this one depends on regular attendance and infrequent absences. A sign-in roll sheet will circulate each class and students with two or more unexcused/undocumented absences will be dropped from the course. To document your absence, contact me through email and I will help you to make up what you missed. In-class participation is 20% of the course grade because workshopping your interactions with AI in a group setting provides you with an uncomparable opportunity to learn and hone this skill. 

## Course Schedule
### Unit 1: What It Is and What We Do (Weeks 1-4) <br style="clear: both">
***Week 1*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ No assignment due <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: Chapter 1 of *Rethinking History* by Keith **Jenkins** | 'Wine, Cheese and ChatGPT: Ladies’ Night in San Francisco.' by Rachel **Levin**, *The New York Times*, October 20, 2025. 

***Week 2*** <br style="clear: both">
**Day 1:** The history of the emergence of generative AI technology and LLMs <br style="clear: both">
▪ Assignment due on Day 1: Chapter 1 of *Atlas of AI: Power, Politics, and the Planetary Costs of Artificial Intelligence* by Kate **Crawford**, Yale University Press, 2021 | Chapter 1 of *AI Snake Oil: What Artificial Intelligence Can Do, What It Can’t, and How to Tell the Difference* by Arvind **Narayana** and Sayash **Kapoor**, Princeton University Press, 2024.<br style="clear: both">
**Day 2:** The practice of Historical Thinking <br style="clear: both">
▪ Assignment due on Day 2: Chapter 4 of *Why Learn History (When It’s Already on Your Phone)* by Sam **Wineburg**, The University of Chicago Press, 2018 | Chapter 4 of *Co-Intelligence: Living and Working with AI* by Ethan **Mollick**, Portfolio/Penguin, 2024.

***Week 3*** <br style="clear: both">
**Day 1:** How to recognize a historian's expertise <br style="clear: both">
▪ Assignment due on Day 1: Chapter 1 of *A Medieval Life: Cecilia Penifader and the World of English Peasants before the Plague* by Judith M. **Bennet**, Revised edition. University of Pennsylvania Press, 2021. <br style="clear: both">
**Day 2:** How to recognize silences and active silencing in the historical record <br style="clear: both">
▪ Assignment due on Day 2: Chapter 1 of *Silencing the Past: Power and the Production of History* by Michel-Rolph **Trouillot**, Beacon Press, 2015 | 'Building Ignorance by Disseminating ‘Evidence’: An Agnotological Look into the Digital Archives of the Islamic Republic of Iran,' by Natalia **Pashkeeva**, *Archival Science* 24, no. 3 (2024): 455–79. 

***Week 4*** <br style="clear: both">
**Day 1:** How methods of using evidence connect to definitions of expertise <br style="clear: both">
▪ Assignment due on Day 1: No assignment due today but you should be working on Report 1 <br style="clear: both">
**Day 2:** Debrief of Report 1 and predictions for what will come next <br style="clear: both">
▪ Assignment due on Day 2: Report 1

### Unit 2: Creating (Weeks 5-8)
***Week 5*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 6*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 7*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 8*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

### Unit 3: Experiments (Weeks 9-12)
***Week 9*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 10*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 11*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 12*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

### Unit 4: Boundaries (Weeks 13-14)
***Week 13*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 14*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

### Unit 5: Writing History with AI (Weeks 15-18)
***Week 15*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 16*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 17*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ Assignment due on Day 1: <br style="clear: both">
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: 

***Week 18: Exam Week*** <br style="clear: both">
**Day 1:** Complete Historical Narrative 2 <br style="clear: both">
▪ Assignment due on Day 1: Historical Narrative 2<br style="clear: both">


## Assignments
In addition to the descriptions below, you will receive specific assignment instructions for the Reports and Historical Narratives. <br style="clear: both">
- **Critiques of AI Reading Summaries:** You must complete this assignment for every class that a reading is assigned. For one of the assigned readings, you will turn in an AI-generated summary along with your critique of it. For days with more than one reading assigned, you choose one. To generate the summary, you can choose whether to prompt the AI chatbot to produce a simple summary or to challenge the chatbot to a higher level analysis of the reading. The next step is the **most important part**: write at least ten thoughtful comments on what the chatbot created for that reading, evaluating the strengths and weaknesses of the chatbot's analysis compared to the understanding you developed from the assigned reading. <br style="clear: both">
- **Report 1:** For this first report, you will evaluate the historical work of an AI chatbot of your choice on a topic of your choice. You will give the chatbot a series of prompts that you have workshopped in class about the history of your topic. After the chatbot generates an answer for you, or a series of answers, that add up to at least fifteen pages, you will report on the quality of historical thinking demonstrated in the chatbot's answer. You will also conduct your own research on the topic in order to ascertain what relevant historical evidence the chatbot might have excluded in its answer. <br style="clear: both">
- **Historical Narrative 1:** After several practice rounds in class, you will use at least two AI chatbots to write a historical narrative on a topic of your choice. You will work with the chatbot as a co-intelligence and not as a replacement for your own thinking. The historical narrative will be assessed based on the quality of the historical analysis according to standards for historical writing in peer-reviewed scholarly publications. These criteria include: quality of evidence selected to support an argument, the significance of the evidence makes sense for the narrative's thesis statement, and the causal explanation includes all relevant historical conditions/events. <br style="clear: both">
- **Report 2:** You will work on this report about halfway through the course. By that time you will have experience with the capabilities and limitations of AI chatbots for constructing historical narrative. In this report, you will carry out experiments in radical new forms for presenting historical content. Based on the work you do in Weeks 9-12 of the course, you will pick two radical new approaches to historical narrative to present to your classmates in this report. Everyone in the class will have access to what everyone else writes for Report 2. <br style="clear: both">
- **Historical Narrative 2:** This is the culminating product for the class. You can think of this as a repeat of the process for Historical Narrative 1, but this time with additional new flavors that emerged from the work carried out by you and your classmates for Report 2. Based on a new historical topic of your choice you will write another narrative with the co-intelligence of at least two AI chatbots. Your historical narrative will be assessed according to the criteria used for the first one, and also based on how successful you were with the innovations that you chose to include from the experiments profiled in the Report 2 submissions from your classmates.<br style="clear: both">

## Grading Scale
Grades will be assigned on a +/- scale <br style="clear: both">
| A 94-100   | A- 90-93   | B+ 87-89   | B 84-86    | B- 80-83   | C+ 77-79    | C 74-76    | C- 70-73 | D 60-69   | F 0-59    |


## Grade Components <br style="clear: both">
In-Class Participation: 20% <br style="clear: both">
Reading Summary Critiques: 20% <br style="clear: both">
Report 1: 10% <br style="clear: both">
Historical Narrative 1: 10% <br style="clear: both">
Report 2: 15% <br style="clear: both">
Historical Narrative 2: 25% <br style="clear: both">



</div>
</div>


