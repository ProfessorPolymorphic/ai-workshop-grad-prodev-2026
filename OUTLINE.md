# Workshop outline

2:30 to 5:00 pm, for Biology and BCB graduate students, with experience ranging from none to advanced. About half the time is hands-on. Students work in **MindRouter** and **Vandal Chat**. Vandalizer appears only in the appendix list of tools.

Rough balance: skills and judgment first, the research lifecycle second, tools and logistics the rest.

| Time | Block | Mode | Min |
|---|---|---|---|
| 2:30 | Welcome | Talk | 5 |
| **Part 1** | **What AI is, and your tools** | | |
| 2:35 | What AI is: next-token prediction, confident fabrication, inconsistency. Overton's slides, biology examples; run the "Inconsistent" prompt live in Vandal Chat. Ends on "Both of these are true": it is an inconsistent, bullshitting next-token predictor, *and* you should use it well (treat it like a lab instrument: calibrate, run controls, replicate) | Talk + demo | 12 |
| 2:47 | **Activity 1: Meet your tools.** Get every student signed in and working on MindRouter, then Vandal Chat; end with a sign-in checkpoint | Hands-on | 25 |
| **Part 2** | **Agentic coding** | | |
| 3:12 | Chatbot vs. agent: who does the work; agent = model + tools + a loop ("same model, different harness"); what changes when it can act; why a website is a project, not an answer | Talk | 8 |
| 3:20 | **Live demo:** an agent on MindRouter builds a one-page academic website from a plain-language prompt | Demo | 7 |
| 3:27 | *Break* | | 10 |
| **Part 3** | **Rules of the road** | | |
| 3:37 | Integrity and disclosure: university and journal policies, authorship, disclosure statements, talking with your advisor | Talk | 8 |
| 3:45 | Data privacy and IRB: on campus does not mean anything goes. Human-subjects data, unpublished data, manuscripts under review, student work | Talk | 8 |
| 3:53 | **Activity 2: Green, yellow, red.** Pairs sort grad-student scenarios, then debrief disagreements | Hands-on | 10 |
| **Part 4** | **Working well** | | |
| 4:03 | TaMPER in practice: Overton's TaMPER build and prompt walkthrough (fellowship Broader Impacts example), then the revise-and-repeat loop; checking the output; keeping a log | Talk | 8 |
| 4:11 | **Activity 3: Fix a bad prompt** in Vandal Chat | Hands-on | 12 |
| **Part 5** | **AI in your research** | | |
| 4:23 | Literature: a Vandal Chat Deep Research report (run before class), citations spot-checked live | Demo | 7 |
| 4:30 | **Activity 4: Build your own website.** Chat track (Vandal Chat) or agent track (agent on MindRouter), same TaMPER-structured prompt; publish free with GitHub Pages | Hands-on | 20 |
| **Close** | | | |
| 4:50 | **Exit ticket:** draft your own AI-use disclosure statement | Hands-on | 5 |
| 4:55 | Takeaways and where to go next with these tools | Talk | 5 |

## Activity 1: Meet your tools (25 min)

Goal: everyone leaves this activity signed in to MindRouter and Vandal Chat, with both working. Every later activity depends on it.

| Min | Tool | Students do | Judgment skill |
|---|---|---|---|
| 8 | MindRouter | Live status page; sign in; note one small and one large model. Already comfortable: create an API key for Activity 4 | Choosing a model; where your data goes |
| 12 | Vandal Chat | Same question, two models, compare with a neighbor. Ask for three papers on your thesis topic; check one DOI | Answers vary between models; sources get invented |
| 5 | Debrief and checkpoint | Three takeaways; anyone not signed in to both tools flags it now | |

## Activity 4: Build your own website (20 min)

Goal: every student leaves with a one-page academic website, and a felt sense of the difference between chatbot and agentic coding.

| Min | Step | Chat track (anyone) | Agent track (agent already set up) |
|---|---|---|---|
| 12 | Build | Paste the prompt into Vandal Chat, save the HTML as index.html, open it in a browser, ask for one change | Same prompt to an agent in an empty folder; read its plan before approving; have it preview and fix |
| 5 | Publish | GitHub: new public repo named yourusername.github.io, upload index.html; live in a minute or two | Ask the agent to create the repo and publish; read each permission request |
| 3 | Debrief | Who did the work? Copy-paste count vs. decisions made; did it invent anything about you? | |

The prompt is on the slide with a Copy button. It uses the Part 4 components (task, context, instructions, output format) and tells the model to leave placeholders rather than invent details. Students include only what belongs on a public web page.

## Appendix

- **Tools we've built:** MindRouter, Vandal Chat, and Vandalizer, with links to each tool, its guide or manual, and GitHub. Public tools only; add others as needed.

## Open items

- Which agent to use for the Part 2 live demo (Claude Code, Codex, OpenCode, or Goose on MindRouter).
- Activity 4 went from 25 to 20 minutes and the exit ticket from 8 to 5 to make room for Part 2.
- Activity 3 (fix a bad prompt) was planned around the workshop paper, which is paused; it needs a source text.
- Vandal Chat steps on the Activity 1 slides were written without seeing the signed-in interface; check them against the real UI.
