# Prompt-Engineering-Studio
Prompt Engineering Internship Tasks
# Prompt Engineering Internship – Tasks 01 to 04

This repository contains the work completed for the Prompt Engineering Internship. The tasks demonstrate how prompt structure, context, tone, examples, automation, and conversational design can be used to guide AI models effectively.

---

## TASK 01 – Writing Better Prompts

### Objective
Understand how prompt clarity, context, audience, tone, and output format influence the quality of AI-generated responses.

### Task
Create and compare different prompts for the same topic: **Climate Change**.

### Prompt 1 – Vague Prompt
"Tell me about climate change."

### Prompt 2 – Specific Prompt
"Explain climate change to a high-school student in simple language. Cover its main causes, effects, and two practical ways students can help reduce its impact. Use short paragraphs and bullet points."

### Comparison
The vague prompt produces a general response because it provides very little context or direction.

The specific prompt produces a more focused response because it clearly defines:
- The topic
- The target audience
- The required information
- The tone and complexity
- The expected output format

### Conclusion
A well-structured prompt generally produces more relevant and useful results. Important elements include:
- Clarity
- Context
- Audience
- Tone
- Output format
- Specific requirements

---

# TASK 02 – Prompting for Creativity

## Objective
Explore how prompt structure, tone, examples, and few-shot prompting influence creative AI outputs.

## Task
Design prompts that generate creative startup ideas and compare multiple generated variations.

### Base Prompt

"Generate a creative startup idea for college students. Include:
1. Startup name
2. Problem being solved
3. Target users
4. Main features
5. Revenue model
6. Why the idea is useful

Keep the idea practical and suitable for students."

### Few-Shot Prompt

"Here are examples of the expected style:

Example 1:
Startup: StudySync
Problem: Students struggle to coordinate group study sessions.
Solution: A platform that helps students create study groups, schedule sessions, share notes, and track progress.

Example 2:
Startup: LeftoverLink
Problem: Restaurants and hostels waste excess food.
Solution: A platform connecting food providers with nearby organizations or people who can use surplus food.

Example 3:
Startup: SkillSwap
Problem: Students want to learn skills but cannot always afford courses.
Solution: A peer-to-peer platform where students exchange skills and knowledge.

Now generate 3 new startup ideas using the same level of creativity, practicality, and detail."

### Expected Output
Generate multiple creative startup concepts while maintaining the style and level of detail demonstrated in the examples.

### Comparison Criteria
Compare the generated ideas based on:
- Creativity
- Practicality
- Level of detail
- Relevance to college students
- Clarity
- Uniqueness

### Conclusion
Few-shot prompting helps guide the model by showing examples of the desired style and structure. The examples provide a pattern that the model can follow while still generating new and creative outputs.

---

# TASK 03 – Prompting for Task Automation

## Objective
Use prompt engineering to make an AI model perform a structured information-extraction task and return consistent JSON output.

## Task
Extract the following information from a student description:

- Name
- Age
- Department
- Semester
- Skills

If any information is missing, return `null`.

### Prompt

"You are an information extraction assistant.

Extract the following fields from the given student information:

- name
- age
- department
- semester
- skills

Return ONLY valid JSON.

Rules:
1. Do not add extra fields.
2. If a value is missing, use null.
3. Skills must be returned as an array.
4. Preserve the information provided by the user.
5. Do not include explanations outside the JSON."

### Example 1

Input:
"Ananya is 20 years old and studies Computer Science and Engineering. She is currently in her 6th semester and knows Python, Java, and SQL."

Output:

{
  "name": "Ananya",
  "age": 20,
  "department": "Computer Science and Engineering",
  "semester": 6,
  "skills": ["Python", "Java", "SQL"]
}

### Example 2

Input:
"Rahul is a 21-year-old student from the Information Science department. He is in the 5th semester and has skills in JavaScript and React."

Output:

{
  "name": "Rahul",
  "age": 21,
  "department": "Information Science",
  "semester": 5,
  "skills": ["JavaScript", "React"]
}

### Example 3

Input:
"Priya is studying Computer Science. She knows Python and C++."

Output:

{
  "name": "Priya",
  "age": null,
  "department": "Computer Science",
  "semester": null,
  "skills": ["Python", "C++"]
}

### Conclusion
Structured prompting makes AI output more predictable and useful for automation. Clearly defining the required fields, rules, and output format helps ensure consistent JSON responses.

---

# TASK 04 – Simulating an Assistant

## Objective
Design a conversational AI assistant that can understand a student's request, ask relevant questions, provide a solution, and follow up.

## Assistant Persona

You are a **College Student Support Assistant**.

Your responsibilities are:
1. Greet the student.
2. Understand the student's request.
3. Ask relevant questions when information is missing.
4. Provide a clear and practical solution.
5. Ask a follow-up question or offer additional help.

## Conversation Flow

Student → Greeting  
Assistant → Understand the request  
Assistant → Ask clarification questions if necessary  
Assistant → Provide solution  
Assistant → Follow-up

---

## Scenario 1 – Study Planning

Student:
"I have exams coming up and I don't know how to plan."

Assistant:
"I can help you create a study plan. When are your exams, how many subjects do you have, and how many hours can you study each day?"

After receiving the details, the assistant should create a realistic timetable based on the student's available time.

---

## Scenario 2 – Assignment Help

Student:
"I have an assignment due tomorrow and I don't know how to start."

Assistant:
"Sure, I can help. What is the subject, what is the assignment topic, and are there any specific formatting or page requirements?"

After receiving the information, the assistant should:
- Break the assignment into smaller sections
- Explain what should be included
- Provide a logical structure
- Help the student complete each section

---

## Scenario 3 – Programming Debugging

Student:
"My Python program is not working."

Assistant:
"I can help debug it. Please share the code, the error message you're getting, and tell me what you expected the program to do."

The assistant should then:
1. Identify the error.
2. Explain the cause in simple language.
3. Provide the corrected code.
4. Explain the correction.
5. Ask whether the student wants help understanding the concept.

---

# Overall Learning Outcomes

Through these four tasks, the project demonstrates:

1. **Better Prompt Writing** – Creating clear and specific prompts.
2. **Creative Prompting** – Using structured and few-shot prompts to influence style and creativity.
3. **Task Automation** – Extracting information and producing structured JSON output.
4. **Conversational AI** – Designing an assistant that follows a structured conversation flow.

## Conclusion

These tasks demonstrate how prompt engineering can improve AI performance across different use cases. By providing clear instructions, context, examples, constraints, and expected output formats, AI models can generate more relevant, consistent, creative, and structured responses.
