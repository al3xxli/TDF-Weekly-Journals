Please refer to [[UCB/TDF Weekly Journals/09082026]] and xxx for the daily notes.

The main assignment this class is to create a basic app in AI Studio. Something simple with no agents:
1. Create the letter writing assistant (refer to role card exercise) without the role card for initial observation.
2. Then, use the role card and ask AI Studio to build a letter writing agent.
	1. Include design intent
	2. Describe the user journey (ideal user journey/interaction loop)
	3. Provide role card
	4. Test with standardised prompts
	5. Ask the agent to include a system diagram for the app including the agent, add as an info button or "view" button.
	6. Modify the app through conversation with AI Studio
	7. Repeat 3x
3. Try with different design goals (other than a letter writing assistant)
---
Initial Observation:


Inputs:

| Role Card                                                                             | User Journey | Test Prompt 1 | Test Prompt 2 | Test Prompt 3 |
| ------------------------------------------------------------------------------------- | ------------ | ------------- | ------------- | ------------- |
| Refer to final role card iteration from last week: [[UCB/TDF Weekly Journals/Week 2]] |              |               |               |               |


Testing:

| Iteration                                                         | Prompt | Model            | Framework | Output |
| ----------------------------------------------------------------- | ------ | ---------------- | --------- | ------ |
| 1 - letter writing assistant                                      |        | Gemini 3.8 Flash | React     |        |
| 2 - letter writing AGENT<br>(role card and user journey included) |        | Gemini 3.8 Flash | React     |        |
| 3 - letter writing agent with system diagram                      |        | Gemini 3.8 Flash | React     |        |
| 4 - letter writing agent v2<br>Modifications:                     |        | Gemini 3.8 Flash | React     |        |
| 5 - letter writing agent v3<br>Modifications:                     |        | Gemini 3.8 Flash | React     |        |
| 6 - letter writing agent v4<br>Modifications:                     |        | Gemini 3.8 Flash | React     |        |


I'm personally very intrigued with the modern difference between React vs Angular, so I tried to build the same thing with Angular. Key differences are XXX

| Iteration                                    | Prompt | Model            | Framework | Output |
| -------------------------------------------- | ------ | ---------------- | --------- | ------ |
| 7 - framework exploration (my own curiosity) |        | Gemini 3.8 Flash | Angular   |        |

Now it's time to create something other than a letter-writing assistant! I'm currently in the midst of job hunting so an ATS Resume Optimizer would be very helpful to quickly create customized resumes and cover letters. 

| Iteration         | Prompt | Model            | Framework                                       | Output |
| ----------------- | ------ | ---------------- | ----------------------------------------------- | ------ |
| 8 - Alternate use |        | Gemini 3.8 Flash | React/Angular (update based on previous output) |        |

Now, the real question is: **are all these steps even neccessary?**
For learning, yes. For outputs, not really.
Case in point, I've actually been using an ATS Resume Optimizer that I created using Antigravity. The prompt was simply:

*"Attached are resume guidelines for optimizing ATS resumes for job hunting. I've also included a PDF resume which needs to be visually analysed as it is not ATS friendly. Build me a webapp which takes the resume attached and generates an ATS-friendly version. There must be a function to copy/paste or upload the position I'm applying to so the resume can align with the exact keywords (as outlined in the guidelines). Minimal interface, very clean and intuitive. Must have a download as .docx button. Make it deployable to Vercel."*

And ta-da! The exact tool I needed. Not perfect, but suitable for the purpose. You can view it here: