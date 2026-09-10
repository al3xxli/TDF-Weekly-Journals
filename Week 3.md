Please refer to [[UCB/TDF Weekly Journals/09082026]] and [[UCB/TDF Weekly Journals/09102026]] for the daily notes.

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
## Initial Observation:
Prompt: Create a letter writing assistant for students who need help communicating with their professors.

Output:
A comprehensive dashboard with high customizability options, it addresses what is asked, breaks the email down into three steps which is manageable. The overall interface seems a bit complex, but it does capture the right amount of detail needed for a reputable email. I would prefer a more simplified UI but this is a good first step for an AI.

![Week 3-02](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%203-02.png)

---
## Iterations:

Inputs:

| Role Card                                                                             | User Journey                                                                                                                                                        | Test Prompt 1                                                 | Test Prompt 2                                       | Test Prompt 3                                                                                 |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Refer to final role card iteration from last week: [[UCB/TDF Weekly Journals/Week 2]] | Step 1: User inputs sender and recipient details.<br><br>Step 2: User selects letter type and tonality.<br><br>Step 3: User adds notes about specific circumstance. | *note: test prompts similar to the ones from week 2.*<br><br> | Do you think an email is the best way to reach him? | I feel really, really sick. I think I have a high fever and might need to go to the hospital. |


Testing:

| Iteration                                                                                                                                                     | Model            | Framework | Feedback of Output                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 - letter writing assistant                                                                                                                                  | Gemini 3.8 Flash | React     | The letter is very typical, not over-explaining and keeping a very formal, professional distance.                                                                                                                    |
| 2 - letter writing AGENT<br>(role card and user journey included)                                                                                             | Gemini 3.8 Flash | React     | Entire interface changed, became more tailored and specific based on the role card. More info on the screen is dedicated to resources while the letter composition is simplified/less customizable.                  |
| 3 - letter writing agent with system diagram                                                                                                                  | Gemini 3.8 Flash | React     | Generated as cards and not a diagram:<br>![Week 3-03](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%203-03.png)                                                                     |
| 4 - letter writing agent v2<br>Modifications: Make the system diagram a concept/mind map please. Not cards.                                                   | Gemini 3.8 Flash | React     | ![Week 3-04](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%203-04.png)Not the best concept map, but it suffices.                                                                    |
| 5 - letter writing agent v3<br>Modifications: Adaptability for all professors and use cases of a student.                                                     | Gemini 3.8 Flash | React     | Added a "target faculty" section:<br>![Week 3-05](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%203-05.png)                                                                         |
| 6 - letter writing agent v4<br>Modifications: Remove all extra/unecessary text and make the UI as clean and minimal as possible in black on white background. | Gemini 3.8 Flash | React     | Something closer to my taste :) I think the functionality and capabilities are fine for the use case.<br><br>![Week 3-06](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%203-06.png) |


I'm personally very intrigued with the modern difference between React vs Angular (I say modern because both have become so similar since a few years back), so I tried to build the same thing with Angular simply with the prompt "rebuild with Angular" and changing the framework in my AI Studio settings. The output broke graphically, which is actually really interesting as it's more of an AI studio bug and not an Angular issue.

| Iteration                                    | Model            | Framework | Output                                                                                                  |
| -------------------------------------------- | ---------------- | --------- | ------------------------------------------------------------------------------------------------------- |
| 7 - framework exploration (my own curiosity) | Gemini 3.8 Flash | Angular   | ![Week 3-07](https://raw.githubusercontent.com/al3xxli/TDF-Weekly-Journals/main/embeds/Week%203-07.png) |

Now it's time to create something other than a letter-writing assistant! I've actually been using an ATS Resume Optimizer that I created using Antigravity. The following prompt was used with Gemini 3.8 Flash:

*"Attached are resume guidelines for optimizing ATS resumes for job hunting. I've also included a PDF resume which needs to be visually analysed as it is not ATS friendly. Build me a webapp which takes the resume attached and generates an ATS-friendly version. There must be a function to copy/paste or upload the position I'm applying to so the resume can align with the exact keywords (as outlined in the guidelines). Minimal interface, very clean and intuitive. Must have a download as .docx button. Make it deployable to Vercel."*

And ta-da! The exact tool I needed. Not perfect, but suitable for the purpose. You can view it here: www.ats-resume-tool.vercel.app

I personally prefer Antigravity over AI Studio, maybe it's the same framework (?) but working in Antigravity using my local files and pushing to github is a much faster process.
