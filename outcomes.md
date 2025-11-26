---
title: Outcomes
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
*This page intersperses the syllabus with learning outcomes, activities and rationales.* 


# History with AI - Course Syllabus

{% include alert.html 
class="info"
title="Enduring Understandings for the Course"
text="At the end of the course, the students will understand that:
- If you use them carefully, AI provocations can enhance your critical thinking skills.
- Summaries can diminish human thinking while lenses can enhance human thinking.
- AI generates content limited by the normativizing pressures from their training sets.
- Writing History with AI is both a journey and a construction project.
"
%}


HIST 300-009 <br style="clear: both">
Instructor: Jonathan Seyfried <br style="clear: both">
Office: Amaranth Digital Humanities Studio, Mesa Vista Hall 2068 <br style="clear: both">
email: jseyfried@unm.edu 

## Introductory Material

**Land Acknowledgement:** Founded in 1889, the University of New Mexico sits on the traditional homelands of the Pueblo of Sandia. The original peoples of New Mexico Pueblo, Navajo, and Apache since time immemorial, have deep connections to the land and have made significant contributions to the broader community statewide. We honor the land itself and those who remain stewards of this land throughout the generations and also acknowledge our committed relationship to Indigenous peoples. We gratefully recognize our history.

**Citizenship and Immigration Status:** All students are welcome in this class regardless of citizenship, residency, or immigration status. Your professor will respect your privacy if you choose to disclose your status. UNM as an institution has made a core commitment to the success of all our students, including members of our undocumented community. The Administration’s welcome is found on [our website](http://undocumented.unm.edu).

**Course Description:** This course explores the ways that the new technology of generative Artificial Intelligence (AI) might influence History in the near and distant future. The course will introduce students to the capabilities and limitations of AI chatbots as tools for creating and influencing historical narratives. Using an experiential and workshop approach, students will use AI chatbots during each class meeting and as tools to enhance their thinking for long term assignments. Writing History with AI is both a journey and a construction project; at first you might get lost or use tools inefficiently. Eventually, though, History with AI will help you access new ways of thinking of the past.

{% include alert.html 
class="info"
title="Rationale for the Course"
text="When it comes to AI chatbots and higher education, there is no way to put the genie back in the bottle. Even if there is no improvement over current models, current AI chatbots possess an immense capability to innovate the way we think of history. At the same time, great risks abound for those who attempt to outsource thinking to AI and accept its answers without critique. This course will help students to develop tools for using AI chatbots for knowledge work, not just for the writing of history but for any type of narrative or exposition.
"
%}

**Student Learning Outcomes:** <br style="clear: both">
By the end of this course you will be able to:
- carefully use AI provocations to enhance your critical thinking skills
- distinguish between summaries that limit human thinking and lenses that enhance human thinking
- recognized the tendency for AI chatbots to provide information limited by the normativizing pressures of their training sets
- write History with AI while thinking of it as a journey and as a construction project

{% include alert.html 
class="info"
title="Rationale for the Learning Outcomes"
text="Looking at the [AI statement](https://www.historians.org/resource/guiding-principles-for-artificial-intelligence-in-history-education/) published by the American Historical Association, the emphasis lies in using AI critically. That's great, but the AHA neglects to provide even a few illustrative examples of how to do that. The learning outcomes for the course fill this gap by using key vocabulary to direct students' attention to the particular critical thinking challenges of using AI chatbots for knowledge work. By focusing on *provocations*, *lenses*, and *normativizing pressures*, consistently throughout the semester, the instructor will instill in the students a deep understanding of how to interact with AI chatbots thoughtfully.[^sarkar]

[^sarkar]:I am indebted to [Advait Sarkar](https://www.ted.com/talks/advait_sarkar_how_to_stop_ai_from_killing_your_critical_thinking/transcript) for his use of *provocations* and *lenses* to describe critical thinking uses of AI-generated content.

The metaphors of journey and construction project will hopefully stick in the students' long-term memories when thinking about AI.
- **Journey:** When you go on a journey, you might have a map ahead of time or at least some preconceptions about what you might encounter. You might follow the paths recommended by others or invent whole new detours. Traditional scholarship has its own pathways, such as citation chasing. AI chatbots take you through pathways based on pattern-matching. Sometimes an AI chatbot will mimic expert citation chasing but often it comes up with very different paths through the information landscape. Whether you take your journey on the route of traditional scholarship or using an AI chatbot, you will be exposed to useful ideas and research leads. There are advantages and disadvantages to both methods of travel. Throughout the semester we will compare the results of each type of travel to see what is emphasized and what is missing.
- **Construction Project:** To accomplish actual historical thinking with AI chatbots, you cannot submit just one prompt or ask just one question. If you want to get more than simplistic answers, you need to practice *multi-shot prompting* and give the AI chatbot a chance to build on its earlier results. For complex analytical tasks such as writing high quality historical narrative, you must think of using AI like you would a crane in a construction project for a skyscraper. You have a powerful tool at your disposal but you have to know how to use it effectively.
"
%}

**Required Readings:** All required readings will be posted to Canvas either as PDFs or links. The links will be to content available at no cost to you, either because they are on free websites or paid for by UNM Libraries.

## Attendance and Participation
Success in a workshop-style course such as this one depends on regular attendance and infrequent absences. A sign-in roll sheet will circulate each class and students with two or more unexcused/undocumented absences will be dropped from the course. To document your absence, contact me through email and I will help you to make up what you missed. In-class participation is 20% of the course grade because workshopping your interactions with AI in a group setting provides you with an uncomparable opportunity to learn and hone this skill. 

## Course Schedule
{% include alert.html 
class="info"
text=" **Note: Following a workshop model, each class meeting includes a significant amount of time for testing out an AI chatbot for at least one historical question or topic. Students will need to bring a laptop to each class and, if they don't already have one, they can check one out from UNM IT for the semester.**
"
%}
### Unit 1: What It Is and What We Do (Weeks 1-4) <br style="clear: both">
***Week 1*** <br style="clear: both">
**Day 1:** What to expect from this course <br style="clear: both">
▪ No assignment due <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the parameters of the course.
- Activity: Mix of lecture and Syllabus Scavenger Hunt
- Activity: Ask an AI chatbot what would be most important to include in a syllabus on History with AI
"
%}
**Day 2:** Definitions of AI and History <br style="clear: both">
▪ Assignment due on Day 2: Chapter 1 of *Rethinking History* by Keith **Jenkins** | 'Wine, Cheese and ChatGPT: Ladies’ Night in San Francisco.' by Rachel **Levin**, *The New York Times*, October 20, 2025. 
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the definitions of AI and History.
- Activity: Methodology lecture
- Activity: Group Discussion then whole class debrief on the question *what do you think AI chatbots' strengths and weaknesses are for creating history?*
"
%}

***Week 2*** <br style="clear: both">
**Day 1:** The history of the emergence of generative AI technology and LLMs <br style="clear: both">
▪ Assignment due on Day 1: Chapter 1 of *Atlas of AI: Power, Politics, and the Planetary Costs of Artificial Intelligence* by Kate **Crawford**, Yale University Press, 2021 | Chapter 1 of *AI Snake Oil: What Artificial Intelligence Can Do, What It Can’t, and How to Tell the Difference* by Arvind **Narayana** and Sayash **Kapoor**, Princeton University Press, 2024.<br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will situate the emergence of AI in larger historical context.
- Activity: Short lecture on history of AI
- Activity: In small groups, query AI chatbots on the history of their existence and whole class debrief
"
%}
**Day 2:** The practice of Historical Thinking <br style="clear: both">
▪ Assignment due on Day 2: Chapter 4 of *Why Learn History (When It’s Already on Your Phone)* by Sam **Wineburg**, The University of Chicago Press, 2018 | Chapter 4 of *Co-Intelligence: Living and Working with AI* by Ethan **Mollick**, Portfolio/Penguin, 2024.
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the criteria for historical thinking.
- Activity: 40-minute workshop on the creation of Columbus Day as a national holiday
- Activity: Student choice of historical topic for 20-minute group research
"
%}

***Week 3*** <br style="clear: both">
**Day 1:** How to recognize a historian's expertise <br style="clear: both">
▪ Assignment due on Day 1: Chapter 1 of *A Medieval Life: Cecilia Penifader and the World of English Peasants before the Plague* by Judith M. **Bennet**, Revised edition. University of Pennsylvania Press, 2021. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand what differentiates historians' expertise.
- Activity: Continue group research from last class
- Activity: Group task on practicing Bennett's methodology
"
%}
**Day 2:** How to recognize silences and active silencing in the historical record <br style="clear: both">
▪ Assignment due on Day 2: Chapter 1 of *Silencing the Past: Power and the Production of History* by Michel-Rolph **Trouillot**, Beacon Press, 2015 | 'Building Ignorance by Disseminating ‘Evidence’: An Agnotological Look into the Digital Archives of the Islamic Republic of Iran,' by Natalia **Pashkeeva**, *Archival Science* 24, no. 3 (2024): 455–79. 
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand historical silencing.
- Activity: Exercise on historical silencing
- Activity: Visit to the National Archives of Iran
"
%}


***Week 4*** <br style="clear: both">
**Day 1:** How methods of using evidence connect to definitions of expertise <br style="clear: both">
▪ Assignment due on Day 1: No assignment due today but you should be working on Report 1 <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will connect uses of evidence to definitions of expertise.
- Activity: In-class work time for Report 1
- Activity: Share out of progress on Report 1
"
%}
**Day 2:** Debrief of Report 1 and predictions for what will come next <br style="clear: both">
▪ Assignment due on Day 2: Report 1
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will draw conclusions about how AI Chatbots interact with historical expertise.
- Activity: Group task on debrief for Report 1
- Activity: Refreshing memories of what is on the syllabus for this course
"
%}

### Unit 2: Creating (Weeks 5-8)
***Week 5*** <br style="clear: both">
**Day 1:** Case studies in the opportunities and problems of AI-generated history <br style="clear: both">
▪ Assignment due on Day 1: Chapters 11 & 12 of *Searches: Selfhood in the Digital Age* by Vauhini **Vara**, Pantheon Books, 2025. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the problems and opportunities of AI generated historical reenactments.
- Activity: Drawing on your completed AI Reading Summary Critiques (the homework due today), assemble evidence for a presentation to high school students about the dangers of using AI image generation for historical reenactments.
"
%}
**Day 2:** The effect of the prompt <br style="clear: both">
▪ Assignment due on Day 2: 'Google Has a Striking History of Bias Against Black Girls,' by Safiya **Noble**, *TIME*, March 26, 2018. | 'Prompt Engineering: A Comparative Study of Prompting Techniques in AI Language Models,' by Jothan **Almeida**, *2025 IEEE Integrated STEM Education Conference (ISEC)*, March 2025, 1–4. | 'Integrating AI into Art Education: Reimagining Classical Styles with Microsoft Copilot,' by Muwaffaq **Abdulmajid**, *International Journal of Education & the Arts* 26, nos. 23–27 (2025): 1–33. 
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the effects of complex prompts for AI chatbot content.
- Activity: In small groups, experiment with multi-shot prompting through planning out prompts ahead of time and seeing what they generate.
"
%}

***Week 6*** <br style="clear: both">
**Day 1:** Compare the gaps in AI-generated history to gaps in traditional scholarship <br style="clear: both">
▪ Assignment due on Day 1: 'Mussolini and ChatGPT. Examining the Risks of AI Writing Historical Narratives on Fascism,' by Fabio **De Ninno** and Michele **Lacriola**, *Journal of Modern Italian Studies*, 30:2 (2025), 187-209. | 'The Transgender Turn: Eleanor Rykener Speaks Back,' by M.W. **Bychowski** in *Trans Historical: Gender Plurality before the Modern*, edited by Greta LaFleur, Masha Raskolnikov, and Anna Kłosowska. Cornell University Press, 2021. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the need to recognize gaps in any historical narrative.
- Activity: In pairs, work with your AI Reading Summary Critiques (the homework due today) to understand how much the AI chatbot resolves gaps in traditional scholarship. Guiding question: *What evidence is there that ChatGPT does better now at prompts about Mussolini versus how it did a year ago?* 
"
%}
**Day 2:** Citation chasing <br style="clear: both">
▪ Assignment due on Day 2: Pages ix-32 of *The Cheese and the Worms: The Cosmos of a Sixteenth-Century Miller* by Carlo **Ginzburg**, translated by John A. Tedeschi and Anne Tedeschi. Johns Hopkins University Press, 1992.
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the process of citation chasing.
- Activity: Small groups work together to replicate Ginzburg's process of citation chasing to reconstruct Menocchio's reading list.
"
%}

***Week 7*** <br style="clear: both">
**Day 1:** How to recognize outsourced thinking <br style="clear: both">
▪ Assignment due on Day 1: 'AI and the Death of Student Writing,' by Lisa Lieberman, *The Chronicle of Higher Education*, June 7, 2024. | 'The Impact of Generative AI on Critical Thinking: Self-Reported Reductions in Cognitive Effort and Confidence Effects From a Survey of Knowledge Workers,' by Hao-Ping (Hank) **Lee**, Advait Sarkar, Lev Tankelevitch, et al. *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems*, ACM, April 26, 2025, 1–22. | 'Now the Humanities Can Disrupt ‘AI.’' by Lauren M.E. **Goodlad** and Samuel **Baker**, *Public Books*, February 20, 2023. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will develop a sharp awareness of the signs of outsourced thinking.
- Activity: In groups of four or six, students go through a [Structured Academic Controversy](https://serc.carleton.edu/sp/library/sac/index.html) on the topic of Generative AI's effect on the critical thinking mission of higher education. 
"
%}
**Day 2:** Normativizing pressures on AI-generated content <br style="clear: both">
▪ Assignment due on Day 2: Chapter 1 of *UFO Crash at Roswell: The Genesis of a Modern Myth*, by Benson **Saler**, Charles A. Ziegler, and Charles B. Moore. Smithsonian Institution Press, 1997. | Chapter 1 of *UFO Crash at Roswell*, by Kevin D. **Randle** and Donald R. **Schmitt**. Avon Books, 1991.
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the role of normativizing pressure in AI generated content.
- Activity: Working individually, students will attempt to manipulate an AI chatbot into admitting the possibility of an alien crash landing near Roswell in 1947. Whoever gets the chatbot furthest into conspiracy theory wins.
- Whole-class discussion on the question: *what are the benefits and drawbacks to the normativizing pressure programmed into AI chatbots?*
"
%}


***Week 8*** <br style="clear: both">
**Day 1:** A deeper understanding of the opportunities and problems of AI-generated history <br style="clear: both">
▪ Assignment due on Day 1: No assignment due today but you should be working on Historical Narrative 1 <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will experience the challenges and opportunities of creating history with AI
- Activity: In-class workshopping of Historical Narrative 1
"
%}
**Day 2:** Honing the skill of critiquing AI-generated historical content <br style="clear: both">
▪ Assignment due on Day 2: Historical Narrative 1
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will deepen their skills in critiquing AI generated historical content.
- Activity: Debrief Historical Narrative 1
- Activity: Optional extra credit presentations on Historical Narrative 1
"
%}

### Unit 3: Experiments (Weeks 9-12)
***Week 9*** <br style="clear: both">
**Day 1:** Revisiting historical reenactment and introducing critical fabulation <br style="clear: both">
▪ Assignment due on Day 1: 'Venus in Two Acts,' by Saidiya **Hartman**, *Small Axe: A Caribbean Journal of Criticism* 12, no. 2 (2008): 1–14. | 'Diaspora, Indigeneity, Queer Critique: Tracey Moffatt’s Aesthetics of Dwelling in Displacement,' by Gayatri **Gopinath** in *Women and Migration: Responses in Art and History*, Open Book Publishers, 2019, 345–62. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will re-evaluate their earlier conclusions about AI for historical reenactment.
- Activity: In small groups, use AI chatbots to imagine, with detail, the queer and/or subaltern archive that does not exist for a specific time and place for which we lack such an archive.
"
%}
**Day 2:** Practice critical fabulation <br style="clear: both">
▪ Assignment due on Day 2: Excerpt from the Code of **Hammurabi** | Chapter 1 of *Sins against Nature: Sex and Archives in Colonial New Spain* by Zeb **Tortorici**, Duke University Press, 2018. 
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will practice critical fabulation.
- Activity: Group task using AI chatbots to carry out critical fabulation for silenced historical subjects in Ancient Mesopotamia and Colonial New Spain.
- Activity: Create guidelines for best practices of AI co-authoring for narrative reconstructions of historical subjects.
"
%}
 
***Week 10*** <br style="clear: both">
**Day 1:** Contextualization as an exploration of systems of meaning in past societies <br style="clear: both">
▪ Assignment due on Day 1: 'On the Concept of History,' by Walter **Benjamin** in *Walter Benjamin: Selected Writings, Vol. 4 1938-1940*, translated by Edmund Jephcott and Others, edited by Howard Eiland and Michael W. Jennings, Harvard University Press, 2003. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand contextualization as a description of systems of meaning in past societies.
- Activity: Individual effort, then compare in groups, for use of AI to elucidate the context-bound ideas of Walter Benjamin and the elements of transhistorical philosophy of history in his piece *On the Concept of History*.
"
%}
**Day 2:** On the blending of mythology, oral tradition, and history <br style="clear: both">
▪ Assignment due on Day 2: Pages 1-50 of *The Book of Chilam Balam of Chumayel*, translated by Ralph L. Roys, Carnegie Institution, 1933.
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will practice blending mythology, oral tradition, and history.
- Activity: As a group task, create a guidance document for high school students writing history dependent on the use of mythological texts with the help of AI
"
%}

***Week 11*** <br style="clear: both">
**Day 1:** Classical Chinese historiography <br style="clear: both">
▪ Assignment due on Day 1: 'The Story of the Rebel Xiang Yu' by Sima Qian in *The First Emperor: Selections from the Historical Records* by **Sima Qian**, translated by Raymond Dawson, Oxford University Press, 2007. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will assess AI chatbots skill in reproducing Classical Chinese Historiography.
- Activity: Group task with each group assigned a different AI chatbot to produce history in the style of Sima Qian.
"
%}
**Day 2:** Case studies in regional and temporal biases in AI training sets <br style="clear: both">
▪ Assignment due on Day 2: 'Iyoba, the Queen Mother of Benin: Images and Ambiguity in Gender and Sex Roles in Court Art,' by Flora Edowaye **Kaplan**, *Art History* 16, no. 3 (1993): 386–407. 
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will attempt to overcome the regional and temporal biases of AI training sets.
- Activity: Create guidance for high school students researching premodern history of regions of Africa
"
%}

***Week 12*** <br style="clear: both">
**Day 1:** Understanding versus pattern-matching <br style="clear: both">
▪ Assignment due on Day 1: No assignment due today but you should be working on Report 2 <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the difference between pattern matching and understanding.
- Activity: In-class workshopping of Report 2
"
%}
**Day 2:** When a historical narrative achieves a transformative reframing <br style="clear: both">
▪ Assignment due on Day 2: Report 2
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will recognize when a historical narrative achieves a transformative reframing.
- Activity: Shareout of Report 2 conclusions
"
%}

### Unit 4: Boundaries (Weeks 13-14)
***Week 13*** <br style="clear: both">
**Day 1:** Going deeper with filter bubbles <br style="clear: both">
▪ Assignment due on Day 1: Chapter 3 of *Co-Intelligence: Living and Working with AI* by Ethan **Mollick**, Portfolio/Penguin, 2024. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will fully describe the limitations imposed by filter bubbles.
- Activity: Groups draft guidelines and practices for how to account for filter bubbles when working with AI chatbots to create historical narratives
"
%}
**Day 2:** Determining ethical constraints for AI-generated historical narratives <br style="clear: both">
▪ Assignment due on Day 2: Chapters 15 & 16 of *Searches: Selfhood in the Digital Age* by Vauhini **Vara**, Pantheon Books, 2025 | Excerpt from *On Diplomatics* by Jean **Mabillon**, Chapter 8 of *Historians at Work: Volume II* edited by Peter Gay and Victor G. Wexler, Harper & Row, 1972.
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will decide on ethical constraints for AI generated historical narratives.
- Activity: In small groups, with whole-class debrief at the end, create comparison charts for Vara and Mabillon
"
%}

***Week 14*** <br style="clear: both">
**Day 1:** The outer limits of AI-generated historical narratives <br style="clear: both">
▪ Assignment due on Day 1: no assignment due for today but you should be working on Historical Narrative 2<br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will describe the outer limits of AI generated historical narratives.
- Activity: Workshop initial stages of Historical Narrative 2
"
%}
**Day 2:** Evaluating our experiments in narrative and planning for Historical Narrative 2 <br style="clear: both">
▪ Assignment due on Day 2: Report 2 results from classmates
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will connect the results of their experiments to their planning of their second Historical Narrative.
- Activity: Rotation activity in which students share their Report 2 results with each other and do their best to incorporate their classmates' Report 2 results into an experimental element in their own Historical Narrative 2.
"
%}

### Unit 5: Writing History with AI (Weeks 15-18)
***Week 15*** <br style="clear: both">
**Day 1:** The new and changing potential for writing history with AI <br style="clear: both">
▪ Assignment due on Day 1: 'The Leading AI Models Are Now Good Historians,' by Benjamin **Breen**, Substack newsletter. *Res Obscura*, January 22, 2025. <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the current potential for writing history with AI.
- Activity: Whole-class discussion on how Breen's observations will affect the process for creating Historical Narrative 2
- Activity: Workshop outlines for Historical Narrative 2
"
%}
**Day 2:** The old, the new, and the changing definitions of expertise <br style="clear: both">
▪ Assignment due on Day 2: Last two chapters and epilogue of *Co-Intelligence: Living and Working with AI* by Ethan **Mollick**, Portfolio/Penguin, 2024. 
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the relationship between expertise and AI generated material.
- Activity: Workshop on recognizing expertise and recognizing the lack of expertise
- Activity: Pair work to help determine what expertise looks like for the topics the students have chosen for Historical Narrative 2
"
%}

***Week 16*** <br style="clear: both">
**Day 1:** Mastery level application of historical thinking to AI-generated content <br style="clear: both">
▪ Assignment due on Day 1: no assignment due for today but you should be working on Historical Narrative 2 <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the importance of applying historical thinking to AI generated material.
- Activity: Workshop results of multi-prompt AI-generated historical content for topics chosen for Historical Narrative 2
"
%}
**Day 2:** One last round of ethical questions <br style="clear: both">
▪ Assignment due on Day 2: First check-in for Historical Narrative 2
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will evaluate the ethics of using AI to write history.
- Activity: Peer edits for Historical Narrative 2
"
%}

***Week 17*** <br style="clear: both">
**Day 1:** What further innovations will AI bring to us in the next five years? <br style="clear: both">
▪ Assignment due on Day 1: no assignment due for today but you should be working on Historical Narrative 2 <br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand the potentialities for AI-generated historical content in the next five years.
- Activity: Optional presentations on Historical Narrative 2
- Activity: In-class time to work on Historical Narrative 2
"
%}
**Day 2:** A final review of the opportunities and problems of writing history with AI <br style="clear: both">
▪ Assignment due on Day 2: Second check-in for Historical Narrative 2
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will understand all the major pitfalls of using AI to write history.
- Activity: Optional presentations on Historical Narrative 2
- Activity: In-class time to work on Historical Narrative 2
"
%}

***Week 18: Exam Week*** <br style="clear: both">
**Day 1:** Complete Historical Narrative 2 <br style="clear: both">
▪ Assignment due on Day 1: Historical Narrative 2<br style="clear: both">
{% include alert.html 
class="info"
text="
- Learning Outcome: Students will use AI to create a historical narrative and to create a metacognitive report on the process.
- Activity: Turn in Historical Narrative 2
"
%}


## Assignments
In addition to the descriptions below, you will receive specific assignment instructions for the Reports and Historical Narratives. <br style="clear: both">
- **Critiques of AI Reading Summaries:** You must complete this assignment for every class that a reading is assigned. For one of the assigned readings, you will turn in an AI-generated summary along with your critique of it. For days with more than one reading assigned, you choose one. To generate the summary, you can choose whether to prompt the AI chatbot to produce a simple summary or to challenge the chatbot to a higher level analysis of the reading. The next step is the **most important part**: write at least ten thoughtful comments on what the chatbot created for that reading, evaluating the strengths and weaknesses of the chatbot's analysis compared to the understanding you developed from the assigned reading. You will be graded on the extent to which the final product reflects your judgment, your understanding, and your cognitive effort. <br style="clear: both">
{% include alert.html 
class="info"
text=" Rationale: Probably the most important takeaway from the course will be to instill in the students a habit of mind to check what they get when an AI chatbot answers their prompts. Ideally, the regular practice of checking an AI summary will become second-nature by the end of the semester. As I read the critiques of what AI produces, I expect that at the start of the semester, students will not catch all the times that the chatbot skimps on the relevant evidence or fails at logical cohesion. By the end of the semester, the students' comments should reflect growth in understanding of historical thinking as well as familiarity with terms such as *filter bubble* and *pattern-matching*.
"
%}
- **Report 1:** For this first report, you will evaluate the historical work of an AI chatbot of your choice on a topic of your choice. You will give the chatbot a series of prompts that you have workshopped in class about the history of your topic. After the chatbot generates an answer for you, or a series of answers, that add up to at least fifteen pages, you will report on the quality of historical thinking demonstrated in the chatbot's answer. You will also conduct your own research on the topic in order to ascertain what relevant historical evidence the chatbot might have excluded in its answer. You will be graded on the extent to which the final product reflects your judgment, your understanding, and your cognitive effort.  <br style="clear: both">
{% include alert.html 
class="info"
text=" Rationale: This assignment is meant to help students see that AI chatbots can be very useful, if one keeps in mind the pitfalls of using it. This is when the students will start to work with AI generated content as a lens.
"
%}
- **Historical Narrative 1:** After several practice rounds in class, you will use at least two AI chatbots to write a historical narrative on a topic of your choice. You will work with the chatbot as a co-intelligence and not as a replacement for your own thinking. The historical narrative will be assessed based on the quality of the historical analysis according to standards for historical writing in peer-reviewed scholarly publications. These criteria include: quality of evidence selected to support an argument, the significance of the evidence makes sense for the narrative's thesis statement, and the causal explanation includes all relevant historical conditions/events. You will also be graded on the extent to which the final product reflects your judgment, your understanding, and your cognitive effort.  <br style="clear: both">
{% include alert.html 
class="info"
text=" Rationale: This first comprehensive historical narrative will allow students to try their hand at using AI to write history. As they are workshopping this product, I expect to hear students using the metaphors of journey and construction project. The students should be able to talk about what ideas AI has presented to them in terms of provocation, as distinct from simply being a passive recipient of answers. Students will receive a rubric for this assignment that clearly communicates to them that their final grade depends on logical use of relevant evidence to support a causal explanation of past events or past perspectives on events.
"
%}
- **Report 2:** You will work on this report about halfway through the course. By that time you will have experience with the capabilities and limitations of AI chatbots for constructing historical narrative. In this report, you will carry out experiments in radical new forms for presenting historical content. Based on the work you do in Weeks 9-12 of the course, you will pick two radical new approaches to historical narrative to present to your classmates in this report. Everyone in the class will have access to what everyone else writes for Report 2. You will also be graded on the extent to which the final product reflects your judgment, your understanding, and your cognitive effort.  <br style="clear: both">
{% include alert.html 
class="info"
text=" Rationale: This assignment invites surprise for the instructor. The *Experiments* unit will hopefully produce ideas and methodologies that the students originate. For this Report, I will encourage the students to think radically about how to create historical narrative, to speculate about new meanings of history, and to think in bizarre ways. Each student's two new approaches should reflect aspects of their own positionality and perspective.
"
%}
- **Historical Narrative 2:** This is the culminating product for the class. You can think of this as a repeat of the process for Historical Narrative 1, but this time with additional new elements and flavors that emerged from the work carried out by you and your classmates for Report 2. Based on a new historical topic of your choice you will write another narrative with the co-intelligence of at least two AI chatbots. Your historical narrative will be assessed according to the criteria used for the first one, and also based on how successful you were with the innovations that you chose to include from the experiments profiled in the Report 2 submissions from your classmates. You will also be graded on the extent to which the final product reflects your judgment, your understanding, and your cognitive effort. 
{% include alert.html 
class="info"
text=" Rationale: Here is the final journey and last construction project of the course. In this historical narrative, I hope to see the students putting all the different concepts, discussions, provocations, and lenses to good use. In this assignment, the students must *leverage* AI to do new interesting things in the writing of History. 
"
%}
<br style="clear: both">

## Grading
**Scale** <br style="clear: both">
Grades will be assigned on a +/- scale <br style="clear: both">
| A 94-100   | A- 90-93   | B+ 87-89   | B 84-86    | B- 80-83   | C+ 77-79    | C 74-76    | C- 70-73 | D 60-69   | F 0-59    |


**Components** <br style="clear: both">
In-Class Participation: 20% <br style="clear: both">
Reading Summary Critiques: 20% <br style="clear: both">
Report 1: 10% <br style="clear: both">
Historical Narrative 1: 10% <br style="clear: both">
Report 2: 15% <br style="clear: both">
Historical Narrative 2: 25% <br style="clear: both">



</div>
</div>