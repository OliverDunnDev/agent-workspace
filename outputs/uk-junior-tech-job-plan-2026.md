# Your UK Junior Tech Job Plan: Autumn 2026

Written 7 October 2026 for: junior full-stack developer (.NET, Python, JavaScript, React), open to AI engineer, frontend and web design roles. Remote, hybrid, or on-site in Hull or Manchester.

> **Do this first (5 minutes):** this file lives on your Tribal OneDrive and your access ends **Tue 13 Oct**. Copy the whole `agent-workspace` folder to a personal drive or a private GitHub repo today. Also export your LinkedIn contacts and ask 2-3 colleagues for LinkedIn recommendations before you leave.

---

## 1. The honest picture

Be realistic. It will make your effort better aimed.

- UK entry-level tech hiring has contracted sharply. Sources put the 2024 drop in entry-level tech roles at around 46%, with some projections nearer 53% by the end of 2026. Treat the exact numbers as indicative, since they come from blogs and recruiter commentary rather than official statistics. The direction is consistent across sources.
- The **work** juniors used to be given (boilerplate, simple endpoints, basic tests) is what AI does fastest. So employers now want juniors who show **judgement**: reading code critically, testing, debugging, and explaining decisions.
- It is **not** the end of junior roles. Demand has moved towards people who can work *with* AI tools and prove they understand what they ship.

**Analogy:** AI is a very fast but overconfident new hire. Employers no longer need someone to type faster than it. They need someone who can *review its work, catch its mistakes, and take responsibility for the result*. Everything below is built around becoming that person, and being able to prove it.

**Your advantages:** a real commercial job on your CV, an edtech domain (Tribal), a mainstream stack (.NET and React are still widely used in UK enterprise, public sector and regional employers), and being willing to be hybrid or on-site in Hull or Manchester.

---

## 2. The skills, in priority order

### Tier 1: Fundamentals (you probably have most of these; sharpen them)
These let you *judge* AI-generated code.
- **Read and debug code you didn't write.** Use the debugger, logs and stack traces. Never just paste the error back into AI.
- **Git properly:** branches, pull requests, resolving conflicts, readable commit messages.
- **Testing:** unit tests (xUnit or NUnit for .NET, pytest, Jest or Vitest) and API testing. Be able to say what makes a test *good*.
- **SQL and data modelling:** still asked in almost every full-stack interview.
- **HTTP/REST, auth basics, and security basics** (OWASP Top 10: injection, broken auth, secrets in code). AI-generated code gets these wrong often, so this is a visible differentiator.
- **Core .NET/C# and TypeScript/React.** Be able to explain state, hooks, async/await, dependency injection.

### Tier 2: AI-era engineering (the new junior baseline)
- **Using an AI coding agent well:** plan first, small tasks, review every diff, run tests, commit often. (You've already started this with Claude Code and CLAUDE.md.)
- **LLM API basics:** calling a model from .NET or Python, system prompts, structured JSON output, streaming, token costs and limits.
- **Tool use / function calling and MCP** (Model Context Protocol): how an AI model is given safe access to tools and data.
- **RAG (retrieval-augmented generation):** chunking documents, embeddings, a vector store, retrieving context, and citing sources. This appears in nearly every junior AI-engineer ad.
- **Evaluation:** building a small test set to measure whether your AI feature actually works. This is the strongest "I'm not just vibe coding" signal. Few juniors do it.
- **AI risks:** hallucination, prompt injection, data privacy, cost. Be able to talk about them calmly.

### Tier 3: Differentiators
- **Deployment:** Docker basics, a CI pipeline (GitHub Actions), one cloud (Azure fits .NET best).
- **Domain knowledge:** edtech or education data, student records, accessibility (WCAG). Your Tribal experience counts.
- **Frontend polish and accessibility**, if you aim at frontend or web design roles.

**What to skip for now:** training models from scratch, deep maths or ML theory, and learning a new language. Roles asking for PyTorch and a master's are mostly not aimed at you. Target "AI engineer (applied/LLM)" roles instead.

---

## 3. Learning plan

### Phase A: Claude sprint (Wed 7 to Tue 13 Oct, while you have access)
Goal: leave with the *habits*, a finished portfolio project skeleton, and saved notes. Use Claude for building and reviewing, and treat every output as something you must understand.

| Day | Focus | "Done when..." |
|---|---|---|
| **Wed 7** | Back up this folder. Sign up (free, email only) at Anthropic Academy and start **Claude Code 101** (Explore, Plan, Code, Commit). Choose your portfolio project (section 4). | Folder copied out. Course 1 finished. One-paragraph project spec written. |
| **Thu 8** | Anthropic Academy: **Building with the Claude API**. Make a small .NET (or Python) console app that calls the API with a system prompt and returns structured JSON. | App runs. You can explain every line. |
| **Fri 9** | **RAG**: add document chunking, embeddings and retrieval to a small API. Have Claude plan it, then *you* write the key parts and ask Claude to review them. | Questions about a small document set return answers with sources. |
| **Sat 10** | **Evaluation + tests**: write 20 question/answer pairs and a script that scores your system. Add unit tests. Deliberately find 3 cases where the AI was wrong. | Eval script runs. A `WHAT_AI_GOT_WRONG.md` lists 3 failures and how you caught them. |
| **Sun 11** | **React frontend** for the project (chat/search UI, loading and error states, accessibility check). Learn **MCP** and **subagents** in the Academy. | Working UI talking to your API. |
| **Mon 12** | **Deploy** (Azure free tier or similar), add a README with architecture diagram and decision log. Do the **AI Capabilities and Limitations** course. | Public URL works. README explains *why*, not just *what*. |
| **Tue 13** | Save everything: export your notes, prompts, CLAUDE.md pattern, and project to your personal GitHub. Write a "how I work with AI agents" page (section 5). Final LinkedIn and CV update. | Everything exists outside Tribal and Claude. |

Throughout the sprint, keep a **running log** of prompts that worked, mistakes the AI made, and what you learned. It becomes interview material.

### Phase B: After 13 Oct (about 4 to 6 weeks, mostly free)
- **Keep using AI tools for free:** Anthropic Academy courses stay free with just an email. Claude, ChatGPT, Gemini and GitHub Copilot all have free tiers with limits. Check current limits yourself, as they change.
- **Daily rhythm (target 4 to 5 hours of learning, 2 to 3 hours of applications):**
  - Morning: one learning block (algorithms and SQL practice, or extend the project).
  - Midday: applications and networking.
  - Afternoon: build, write up, or interview practice.
- **Resources worth your time (all free or cheap):**
  - [Anthropic Academy](https://anthropic.skilljar.com) for Claude Code, API, MCP, agent skills.
  - Microsoft Learn for .NET, Azure and the Azure OpenAI/AI Foundry paths. Microsoft certifications such as AZ-900 and AI-900 are cheap and recognised by UK .NET employers.
  - DeepLearning.AI short courses (RAG, agents, evaluation) and Hugging Face's free courses.
  - freeCodeCamp, The Odin Project, and Exercism (C#, Python, TypeScript) for practice.
  - NeetCode or LeetCode (easy and medium only) for the interview-style problems still used by many employers.
  - OWASP Top 10 and PortSwigger Web Security Academy (free) for security.
- **Second project (weeks 3 to 5):** a smaller, *non-AI* project that shows fundamentals: a .NET API with authentication, a SQL database, tests and CI. Employers want to see you can build without AI at the centre.

---

## 4. Portfolio: one flagship project, done properly

**Suggested project: "Policy/Docs Assistant with evaluation"**
- Takes a public document set (for example UK government education guidance or a public technical manual), answers questions with **citations**, and says "I don't know" when it can't find an answer.
- **Stack:** .NET minimal API (or Python FastAPI) + React frontend + vector search (pgvector, Azure AI Search, or SQLite plus embeddings).
- **Why this one:** it shows RAG, evaluation, security awareness (prompt injection) and your edtech angle, using the stack you already know.

**What makes it credible rather than "vibe-coded":**
1. **A README that explains decisions**: why this chunk size, why this database, what you rejected.
2. **An evaluation harness** with results: "Answers were correct on 16 of 20 test questions; here are the 4 failures and what I changed."
3. **Tests that run in CI** (green badge).
4. **`WHAT_AI_GOT_WRONG.md`**: 3 to 5 real examples of AI-generated bugs or bad suggestions, and how you spotted and fixed them. Employers love this.
5. **Small, readable commit history** and pull requests with descriptions.
6. **A live demo link and a 2-minute screen recording** walking through the code.
7. **Security notes**: how you handle secrets, user input, and prompt injection.

**The litmus test:** could you spend 30 minutes on a call explaining any file in the repo, and live-change it? If not, simplify the project until you could.

---

## 5. How to stand out beyond GitHub

1. **Be the person who can explain it.** In interviews, expect "walk me through this code" and "what would you do if the AI gave you this?" Rehearse out loud. Record yourself.
2. **Write a short public post per project** (LinkedIn or a simple blog): problem, approach, what went wrong, what you'd do next. Two or three honest posts beat ten polished repos.
3. **Publish a "How I work with AI" page** (one page): your plan, build, review, test loop. Based on your CLAUDE.md workflow, it shows maturity most juniors lack.
4. **Show review skill:** pick a small open-source project, find a "good first issue", and submit one genuine pull request. Even a documentation or test fix counts.
5. **Tailor every application** to 2 or 3 lines of the job ad. Mention a specific thing about the company. Generic applications are the quickest ones to ignore, especially now that recruiters receive floods of AI-written ones.
6. **Referrals and people:** most UK junior hires still come from conversations. Message 5 people a week (ex-colleagues, local developers, hiring managers): "I'm a junior full-stack developer in Hull/Manchester, recently redundant. Could I ask two quick questions about your team?" Don't ask for a job in the first message.
7. **Meetups:** attend in Manchester (find current tech meetups on Meetup.com and Luma) and look for developer or digital groups in Hull and Yorkshire. Check who is active now rather than relying on old lists.
8. **Use your redundancy story simply:** "My role was made redundant in October. I've used the time to build X and learn Y." Calm and specific.
9. **Certifications as tie-breakers only** (AZ-900, AI-900, Anthropic Academy certificates). They help filters, but the project and your explanation do the real work.

---

## 6. Where to find roles in the UK

### Main places to search (set daily alerts on all)
- **LinkedIn Jobs**: biggest source. Set alerts and turn on "Easy Apply" filters, but always add a tailored message. Also search *people* (hiring managers, engineers) at target firms.
- **Indeed** and **Reed**: strong for regional (Hull, Yorkshire) and SME roles.
- **CWJobs**, **Technojobs**, **Totaljobs**: IT-specific boards with many recruiters.
- **ITJobsWatch**: not a job board as such. It shows salary and demand trends per skill and region, useful for checking what a "Junior .NET" role pays in Hull versus Manchester. Recent figures suggest medians around £30,000 for junior .NET in Hull and Yorkshire, and Manchester graduate/junior .NET roles advertised higher (roughly £25k to £45k depending on employer). Treat these as rough guides.
- **Wellfound** (start-ups) and **Welcome to the Jungle** (formerly Otta): good for start-ups with clear salary and culture info.
- **Gradcracker** and graduate scheme pages: even without a recent degree, some "graduate/junior" roles accept career-changers. Read each ad.
- **Find an Apprenticeship (gov.uk)**: there's no upper age limit and some degree-level and software apprenticeships exist. Pay is lower but a route in with training. Check the employer is genuine.
- **Civil Service Jobs, NHS Jobs, and local councils/universities**: Digital, Data & Technology roles. .NET is common in public sector, and these employers are more stable and open to juniors.
- **Direct company career pages** for your area: search "software developer" plus Hull, Manchester, or Yorkshire, then browse employers' own sites. Local firms often advertise only there.

### Role titles to search
- Junior Software Developer, Junior Full Stack Developer, Graduate Software Developer, Associate Software Engineer
- Junior .NET Developer, C# Developer (junior), Junior Python Developer
- Junior/Applied AI Engineer, AI Engineer (graduate), LLM Engineer (junior), Prompt/AI Automation Developer
- Frontend Developer (junior), React Developer (junior), Web Developer, Web Designer, UI Developer
- Technical Support Engineer, Implementation Consultant, QA/Test Engineer, Software Tester (these are common stepping stones into development)

### Recruitment agencies and "train then place" schemes
- Register with 5 to 8 tech recruiters covering the North (search "technology recruitment Hull/Leeds/Manchester"). Call them, don't just upload a CV.
- **Caution on "hire-train-deploy" schemes** (such as Sparta Global or similar consultancy programmes). They can be a genuine way in, but **read the contract**: look for training bonds, clawback fees, minimum terms, low starting pay, and placement outside your area. Ask them directly.

### Local note (Hull/Manchester)
- Hull: expect a smaller market, with a mix of local software houses, NHS/public sector, and larger firms with Hull sites. One advertised example during my research was a Hull-based Junior Software Developer (.NET / Power Platform) role around £26,660 to £32,000. Verify any listing yourself, since I couldn't confirm which employers are currently hiring.
- Manchester: the biggest tech hub in the North, with many more roles, and hybrid is common. Use it as your main target for volume, and consider remote roles based elsewhere.
- Remote junior roles are very competitive, so don't make them your only route.

---

## 7. Weekly job-hunt routine (from 14 Oct)

| Per week | Target |
|---|---|
| Tailored applications | 10 to 15 (quality over quantity) |
| People messaged | 5 |
| Recruiters called | 2 to 3 |
| Learning/project hours | 20+ |
| Interview practice (out loud) | 3 sessions |
| Written/public post | 1 every 1 to 2 weeks |

Track everything in a simple spreadsheet: company, role, date applied, contact, status, follow-up date. Follow up after 7 days.

**Interview prep checklist:** explain your flagship project end to end; a live-coding warm-up (FizzBuzz-level to easy LeetCode); SQL joins and indexes; REST and auth basics; React hooks and state; one story each about a bug you fixed, a disagreement, and something you learned; "how do you use AI in your work, and how do you check it?"

---

## 8. Tailoring your CV and LinkedIn
- Headline: "Junior Full-Stack Developer (.NET, React, Python) | Building LLM/RAG applications".
- Top of CV: 3 lines of summary, then **your flagship project with measurable results** (e.g. "evaluation suite, 20 test cases, 80% correct, failures documented"), then your Tribal experience with outcomes.
- Keep it to 1 to 2 pages, plain formatting (it must survive automated parsing), and match keywords from each ad honestly.
- Don't claim skills you can't discuss. Interviewers probe.

---

## 9. Your biggest risks, and what to do about them
- **Collecting tutorials instead of building.** Fix: every learning block must end with something you built or wrote.
- **Spending all day applying.** Fix: cap applications and spend time on referrals, which convert far better.
- **Over-trusting AI output.** Fix: never merge anything you can't explain.
- **Money pressure.** Fix: also apply for adjacent stepping-stone roles (support engineer, QA, implementation). A foot in the door beats waiting for a perfect title.
- **Confidence dips.** A tough market means rejections, so treat them as data, not a verdict.

---

## Sources (market research done 7 Oct 2026; secondary sources, verify specifics)
- [Are AI Tools Changing Entry-Level IT Jobs in the UK?](https://www.itjobboard.co.uk/blog/418/are-ai-tools-changing-entry-level-it-jobs-in-the-uk)
- [Are Junior Developers Still in Demand in 2026? (Thoughtgears)](https://thoughtgears.co.uk/blog/are-junior-developers-in-demand-2026/)
- [AI shrinks computer science graduate hiring, UK data shows](https://www.hererockhill.com/2026/09/14/ai-cs-graduates-uk-jobs-fall/)
- [AI Job Market 2026: A Junior Engineer's Survival Guide](https://www.transparent.tech/ai-job-market-junior-engineer-survival-guide-2026/)
- [Junior AI/agentic engineering jobs, UK](https://agentic-engineering-jobs.com/jobs/junior/united-kingdom)
- [Junior AI Engineer example advert (ITJobsWatch)](https://www.itjobswatch.co.uk/jv/Intellect-Group/Junior-Artificial-Intelligence-Engineer-Job-London-UK-4vek9t)
- [Junior .NET Software Developer trends in Hull (ITJobsWatch)](https://www.itjobswatch.co.uk/jobs/hull/junior%20.net%20software%20developer.do)
- [Junior .NET Software Developer trends in Yorkshire (ITJobsWatch)](https://www.itjobswatch.co.uk/jobs/yorkshire/junior%20.net%20software%20developer.do)
- [Junior Software Developer (.NET / Power Platform), Hull example](https://www.itjobboard.co.uk/job/16819735/junior-software-developer-net-power-platform/)
- [Python developer jobs in Manchester, 2026 guide](https://www.itjobboard.co.uk/blog/396/python-developer-jobs-manchester-|-2026-salary-&-guide/)
- [Anthropic Academy overview](https://pasqualepillitteri.it/en/news/371/anthropic-academy-free-courses-claude)
- [Tech job boards in the UK](https://www.manatal.com/blog/tech-job-boards-uk)
