# Task 03 – Task Automation

## Objective

Use prompt engineering to extract information from unstructured text and convert it into structured JSON.

---

## Prompt

You are an information extraction assistant.

Extract the following fields:

- name
- age
- department
- semester
- skills

Return ONLY valid JSON.

Rules:

1. Do not add extra fields.
2. If information is missing, use null.
3. Skills must be returned as an array.
4. Preserve the information provided by the user.
5. Do not include explanations outside the JSON.

---

## Input

Ananya is 20 years old and studies Computer Science and Engineering. She is currently in her 6th semester and knows Python, Java, and SQL.

---

## Output

```json
{
  "name": "Chaithra",
  "age": 20,
  "department": "Computer Science and Engineering",
  "semester": 7,
  "skills": [
    "Python",
    "Java",
    "SQL"
  ]
}
