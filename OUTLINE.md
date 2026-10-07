# Workshop outline

2:30 to 5:00 pm, for Biology and BCB graduate students, with experience ranging from none to advanced. About half the time is hands-on.

Main goal: show students how agentic coding can help them build their own website. MindRouter is the layer that connects AI tools (Vandal Chat, coding harnesses, students' own code) to models on University of Idaho GPUs; it accepts OpenAI, Anthropic, and Ollama request formats, so it works with any of the harnesses. Students work in **MindRouter** and **Vandal Chat**, set up one of the six coding harnesses from the [MindRouter agents guide](https://mindrouter.uidaho.edu/blog/running-ai-agents-with-mindrouter), and use it to build and publish a personal academic website. Vandalizer appears only in the appendix list of tools.

| Time | Block | Mode | Min |
|---|---|---|---|
| 2:30 | Welcome | Talk | 5 |
| **Part 1** | **What AI is, and your tools** | | |
| 2:35 | What AI is: next-token prediction, confident fabrication, inconsistency. Overton's slides, biology examples; run the "Inconsistent" prompt live in Vandal Chat. Ends on "Both of these are true": it is an inconsistent, bullshitting next-token predictor, *and* you should use it well (treat it like a lab instrument: calibrate, run controls, replicate) | Talk + demo | 12 |
| 2:47 | **Activity 1: Meet your tools.** Every student signed in to MindRouter (with an API key) and Vandal Chat; end with a checkpoint | Hands-on | 25 |
| **Part 2** | **Agentic coding** | | |
| 3:12 | Chatbot vs. agent: who does the work; agent = model + tools + a loop ("same model, different harness"); what changes when it can act; why a website is a project, not an answer | Talk | 8 |
| 3:20 | **Live demo:** an agent on MindRouter builds a one-page academic website from a plain-language prompt | Demo | 7 |
| 3:27 | **Activity 2: Set up your agent.** Pick one of six harnesses, connect it to MindRouter, test it in an empty my-website folder; safety habits; checkpoint | Hands-on | 12 |
| 3:39 | *Break* (fix any setup problems) | | 10 |
| **Part 3** | **Rules of the road** | | |
| 3:49 | The frontier is jagged, and it moves: Dell'Acqua et al. 2023 (758 BCG consultants, GPT-4). Inside the frontier: 12.2% more tasks, 25.1% faster, 40%+ higher quality; outside: 19 points less likely to be correct. Abilities are "expanding, but uneven," so re-test on your own tasks | Talk | 4 |
| 3:53 | Test the ceiling and the floor: skeptics test AI only on what they and a few experts can do, then dismiss it. Test both: your ceiling (where it fails; you judge best) and your floor (where it lifts you; check harder). Each person's ceiling and floor differ. Same study: below-average performers +43%, above-average +17%. AI raises the floor for everybody | Talk | 3 |
| 3:56 | Judgment and good questions are worth more now: what AI made cheaper vs. what is worth more (choosing the question, knowing whether a result is right, putting your name on it) | Talk | 3 |
| 3:59 | Integrity and disclosure: university, funder, and journal rules; authorship; disclosure statements; talking with your advisor | Talk | 5 |
| 4:04 | Data and IRB: on campus does not mean anything goes. Human-subjects data, unpublished data, manuscripts under review, student work | Talk | 4 |
| 4:08 | **Activity 3: Green, yellow, red.** Pairs sort grad-student scenarios, then debrief disagreements | Hands-on | 7 |
| **Part 4** | **Working well** | | |
| 4:15 | TaMPER in practice: Overton's TaMPER build and prompt walkthrough (fellowship Broader Impacts example), then the revise-and-repeat loop. Sets up the Activity 4 prompt | Talk | 8 |
| **Part 5** | **AI in your research** | | |
| 4:23 | Literature: Vandal Chat Deep Research, from the [MindRouter blog post](https://mindrouter.uidaho.edu/blog/introducing-vandalchat-deep-research). How to start one (telescope button, campus network or VPN, 30–60 min, PDF by email); the pipeline (agents checked by code: quotes verified on downloaded pages, writers see only verified evidence, every sentence fact-checked); one real run (263 drafted statements: 192 confirmed, 15 revised, 56 removed); what's okay and not, framed by Part 3's five rule-setters (instructor, advisor and committee, university, funder, journal); what it can and cannot check. Live spot-check of a report run before class (eDNA fish monitoring question); students start their own run, PDF arrives by email after the workshop | Talk + demo | 7 |
| 4:30 | **Activity 4: Build your own website** with the agent from Activity 2; publish free with GitHub Pages | Hands-on | 20 |
| **Close** | | | |
| 4:50 | **Exit ticket:** draft your own AI-use disclosure statement | Hands-on | 5 |
| 4:55 | Takeaways and where to go next with these tools | Talk | 5 |

## Activity 1: Meet your tools (25 min)

Goal: everyone leaves this activity signed in to MindRouter and Vandal Chat, with a MindRouter API key saved. Every later activity depends on it.

| Min | Tool | Students do | Judgment skill |
|---|---|---|---|
| 8 | MindRouter | Live status page; sign in; note one small and one large model; create an API key (shown once; treat it like a password) | Choosing a model; where your data goes |
| 12 | Vandal Chat | Same question, two models, compare with a neighbor. Ask for three papers on your thesis topic; check one DOI | Answers vary between models; sources get invented |
| 5 | Summary and setup check | What each tool does; three-item check (MindRouter sign-in, API key saved, Vandal Chat answers). Anyone missing one flags it now | |

## Activity 2: Set up your agent (12 min)

Follows the [MindRouter agents guide](https://mindrouter.uidaho.edu/blog/running-ai-agents-with-mindrouter). Each harness name on the slide links to its section of the guide.

- **Pick one harness.** Never opened a terminal: a desktop app (Goose, OpenCode, or Codex inside the ChatGPT desktop app). Comfortable in a terminal: Claude Code (terminal version only; its desktop app cannot use MindRouter), Pi, or ForgeCode.
- **Connect it** with three values: host `https://mindrouter.uidaho.edu` (some tools want `/v1`), the `mr2_` key from Activity 1, model `default-agent`.
- **Already have a Claude or ChatGPT account?** Claude Code (including its desktop app) works with a Claude account and Codex with a ChatGPT account; sign in with it and skip the MindRouter connection. Prompts then go to Anthropic or OpenAI rather than staying on campus: fine for a public website, not for research data.
- **Test it** in an empty folder called my-website: "What files are in this folder?"
- **Seatbelts on** (from the guide's security section): one folder, read before you approve, no secrets in the chat, outside content is untrusted (prompt injection), never skip permissions, keep a way to undo.
- **Checkpoint** before the break; stragglers get help during it.

## Activity 4: Build your own website (20 min)

Goal: every student leaves with a one-page academic website built by their agent, and a felt sense of the difference between chatbot and agentic coding.

| Min | Step | What students do |
|---|---|---|
| 12 | Build | Open the agent in my-website; paste the prompt; read the plan before approving; ask for one change. Fallback if the agent is not working: same prompt in Vandal Chat, save the HTML by hand |
| 5 | Publish | GitHub: new public repo named yourusername.github.io, upload index.html; live in a minute or two. Comfortable with git: have the agent commit and push |
| 3 | Debrief | Decisions made, permissions granted, anything invented about you |

The prompt is on the slide with a Copy button. It uses the Part 4 components (task, context, instructions, output format), asks for a plan first, and tells the model to leave placeholders rather than invent details. Students include only what belongs on a public web page.

## Appendix

- **Tools we've built:** MindRouter, Vandal Chat, and Vandalizer, with links to each tool, its guide or manual, and GitHub. Public tools only; add others as needed.

## Open items

- Which harness to use for the Part 2 live demo.
- Vandal Chat steps on the Activity 1 slides were written without seeing the signed-in interface; check them against the real UI.
- Slides still to write: the exit ticket and takeaways.
- Part 5's Deep Research block has six slides for seven minutes; trim if needed ("How it works" and "How much to trust it" are the easiest to compress).
- Not verified for Part 3: UI IRB guidance on AI (none found) and the text of the Graduate School's AI policy for academic writing.
