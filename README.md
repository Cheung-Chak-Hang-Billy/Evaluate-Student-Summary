## Evaluate Student Summaries
Automatically assess summaries written by students in grades 3-12

## Overview
### Goal of the Project
The goal of this project is to assess the quality of summaries written by students in grades 3-12. The model builds to evaluates how well a student represents the main idea and details of a source text, as well as the clarity, precision, and fluency of the language used in the summary. 

This project will assist teachers in evaluating the quality of student work and also help learning platforms provide immediate feedback to students.

### Context
Summary writing is an important skill for learners of all ages. Summarization enhances reading comprehension, particularly among second language learners and students with learning disabilities. Summary writing also promotes critical thinking, and it’s one of the most effective ways to improve writing abilities. However, students rarely have enough opportunities to practice this skill, as evaluating and providing feedback on summaries can be a time-intensive process for teachers. Innovative technology like large language models (LLMs) could help change this, as teachers could employ these solutions to assess summaries quickly.

There have been advancements in the automated evaluation of student writing, including automated scoring for argumentative or narrative writing. However, these existing techniques don't translate well to summary writing. Evaluating summaries introduces an added layer of complexity, where models must consider both the student writing and a single, longer source text. Although there are a handful of current techniques for summary evaluation, these models have often focused on assessing automatically-generated summaries rather than real student writing, as there has historically been a lack of these types of datasets.

### Project Website
This project is from a competition organized by CommonLit in Kaggle.
Details can be found from the following website
https://www.kaggle.com/competitions/commonlit-evaluate-student-summaries

## Dataset 
The dataset comprises about 24,000 summaries written by students in grades 3-12 of passages on a variety of topics and genres. These summaries have been assigned scores for both content and wording. The goal of the project is to predict content and wording scores for summaries on unseen topics.

### File and Field Information
summaries_train.csv - Summaries in the training set.
* student_id - The ID of the student writer.
* prompt_id - The ID of the prompt which links to the prompt file.
* text - The full text of the student's summary.
* content - The content score for the summary. The first target.
* wording - The wording score for the summary. The second target.

summaries_test.csv - Summaries in the test set. Contains all fields above except content and wording.
prompts_train.csv - The four training set prompts. Each prompt comprises the complete summarization assignment given to students.
* prompt_id - The ID of the prompt which links to the summaries file.
* prompt_question - The specific question the students are asked to respond to.
* prompt_title - A short-hand title for the prompt.
* prompt_text - The full prompt text.

prompts_test.csv - The test set prompts. Contains the same fields as above. The prompts here are only an example. The full test set has a large number of prompts. The train / public test / private test splits do not share any prompts.


