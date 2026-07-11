---
layout: article
title: "The Workflow Nobody Redesigned For"
date: 2026-07-11
---

Most conversations about AI in software focus on what the AI can do — generate code, write tests, open PRs, review diffs.

Much less gets said about what happens to the engineer standing next to all of it.

---

## The part that gets skipped

I've built a fair number of tools to make reviewing AI-generated code easier, but I'm not attached to that being the answer. If a team would rather automate the whole process with reviewer agents, solid CI, and a real rollback plan, I'm completely on board. 

I'm not fighting this shift. Because that's not the real problem.

What frustrates me is when an organization adopts AI generation and stops there, without changing anything around it.

The expectation quietly becomes: generate more code, ship faster, still personally own every decision, and figure out your own review process while you're at it. The speed is mandated. The system to support the speed is not.

At that point the burden doesn't disappear. It just shifts — from the organization to the individual engineer.

---

## Invisible work, multiplied

When nobody redesigns the workflow, every engineer ends up quietly inventing their own: their own prompting style, their own review strategy, their own way of pulling in context, their own private threshold for when code feels trustworthy enough to commit.

None of that work is visible. All of it consumes attention. And because it's happening individually, it happens dozens of times over, slightly differently each time, with nothing shared and nothing standardized.

That's the hidden cost of "just use AI more" — it looks like acceleration, but a lot of it is just cost moved off the org's books and onto each engineer's.

---

## What changing the workflow actually looks like

The teams getting this right aren't the ones just telling engineers to use AI more. They're the ones treating the workflow itself as the thing that needs redesigning — specialized reviewer agents, CI you can actually trust, routing based on how much a change could break, deployment and rollback built into the safety model, metrics to keep improving the process.

Whether that specific setup is the "right" one or not isn't really the point. The point is that someone decided the workflow had to evolve alongside the tooling, instead of leaving that to each person to solve alone.

---

## Where do humans fit now?

As AI produces more of the work, organizations have to actually decide where humans sit in the new system.

Maybe humans review less. Maybe agents verify more. Maybe deployment strategy changes. Maybe what "ownership" means changes.

I don't think there's one correct answer. But I'm fairly sure of the wrong one: expecting engineers to silently absorb all the new cognitive load while the workflow around them stays exactly the same.

AI doesn't just change how we write code. It changes how an engineering organization has to operate — and that part can't be left as homework for each engineer to figure out alone.