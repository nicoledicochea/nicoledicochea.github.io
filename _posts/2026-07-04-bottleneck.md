# The Next Bottleneck in AI Coding Isn't Generation. It's Knowing Where to Look.

AI just handed you 500 lines of new code.

Tests pass. The endpoint works when you hit it locally. The UI looks right.

You still have to read the code. Your name is going on it either way.

---

## The Reality of AI-generated Code

For years, the bottleneck in software was generation — how quickly a human could produce correct code. That bottleneck is mostly gone.

But nothing scaled up to match it. 

When you wrote every line yourself, you already knew where the risk was, because you'd made every decision along the way. When AI writes it, that built-in awareness disappears. You're handed a finished diff and have to reconstruct, after the fact, which five lines actually mattered.

Tests and manual checks confirm the code *works*. They don't tell you which lines you should be reading most carefully, or which ones quietly encode an assumption nobody actually verified. That's a different problem, and it's the one that lands on you personally the moment you hit approve.

---



## Tackling the Problem

Over the past year, I’ve found myself building small prototypes around this exact moment in the development workflow.

**A pre-PR confidence tool** — something that looks at a fresh diff and flags the handful of changes that actually deserve a closer look: unverified assumptions, missing test coverage, risky business logic, or changes that touch shared code. Not a linter. Just a way to help me know where to start reviewing.

**A PR description generator** —  because good code review starts with good context. It gives future me a record of why I made the change, and gives reviewers a place to start before diving into hundreds of lines of code.

Neither prototype was about replacing human review. They were both trying to answer the same question: *Out of everything AI just generated, what should I pay attention to first?*
---



## Where We Go From Here

Most AI-dev-tool energy right now goes toward generation — writing more, faster, with less friction. Most of what's left goes toward the PR stage — bots that review a pull request once it's already open.

Almost nothing goes toward the moment before either of those: a person, alone, staring at a fresh diff, before it's even a commit. If I don't trust what I'm looking at, it doesn't reach a PR at all. It doesn't reach a review bot. It doesn't reach anyone but me.

That's the part of the workflow nobody's really building for. Everyone's optimizing the review that happens after code is already out in the open, and skipping the moment that decides whether it gets there in the first place.

I think that earlier moment deserves more attention than it's getting. It's the part of the workflow I keep finding myself building for, whether or not anyone's asked.

## The Question I'm Interested In

AI will continue generating more code and humans will continue being responsible for what gets shipped, so I don’t think the interesting question anymore is whether AI can write software. I think it’s how we make the **human checkpoint simpler without removing it**.