# Kuli Singh

AI Platform Engineer. I build cognitive intelligence pipelines, agentic backend systems, and developer tooling that makes AI useful in production rather than impressive in demos.

By day I'm leading platform and AI engineering on a large-scale financial services programme, working across 24 domain squads. Most of my recent work lives at the intersection of LLM pipeline architecture, trust design, and developer experience: how do you build AI systems that teams can actually rely on, audit, and understand?

Outside of that, I build things for myself.

## Personal Projects

### Renaissance

An agentic personal intelligence loop I use every day.

Voice input on mobile is transcribed server-side, split into structured thoughts, classified, embedded, and stored in Supabase. Thoughts can become commitments with progress tracking. A backend agent, NanoClaw, runs on cron, reads the accumulated memory, reasons over open commitments, values-action gaps, and behavioural drift, then writes its output back into the same database.

The mobile app renders the result: a Morning Mirror, a Focus feed, a Spirit Animal, a Values Mirror, and a commitment surface.

The loop is closed. The agent is not triggered by me. It runs whether I open the app or not.

Expo / React Native, TypeScript, Supabase, NanoClaw backend agent

### Hercules

A voice-first gym logger that actually understands what you said.

Gym shorthand is compressed and context-dependent. "Same weight for six" or "set three, five reps" only resolves correctly if the system knows what exercise block is active and what the last set weighed. Hercules treats this as a structured inference problem, not a transcription problem. The parser holds the current workout block context, fills the gaps, and surfaces its assumptions before writing anything to the database. You can correct before it saves.

I use it during every session, talking through sets in real time.

The workout data lands in the same Supabase database as Renaissance. NanoClaw has access to both. The agent reasons across my thoughts, commitments, and training history together, then writes its output back into the database: morning and evening nudges that surface directly in the app. My training becomes part of the same intelligence loop as my life plans, not siloed into a fitness app that never talks to anything else.

Expo / React Native, TypeScript, Supabase

### Socialiser

A multi-user, values-led social planning platform and personal CRM.

Most social plans die in the gap between "we should do something" and an actual event. Socialiser is built to close that gap. It treats social life as a system: values, relationship context, friendship groups, reusable event templates, saved locations, invitations, RSVPs, and follow-through.

The unusual product decision is where it starts. Socialiser does not begin with a blank calendar event or a contact list. It starts from values: what kind of life are you trying to live, who do you want to spend time with, and what patterns of gathering are worth repeating? From there, you can create activity templates, connect them to values, select friends or groups, reuse common locations, and turn a rough intention into a real scheduled event.

The Gemini layer is workflow-native rather than decorative. It can take a prompt like "something low-key outdoors this weekend" and reason over the user's saved values, preferences, locations, activity templates, and social context to produce structured event suggestions that map back into the domain model. The output is not just advice; it is something the app can convert into an event instance with venue, timing, capacity, invite policy, and RSVP flow.

The invite system is the key real-world design choice. Socialiser separates host power from guest friction. The organiser gets the full authenticated planning system: personal CRM, values, templates, saved locations, headcount, and guest management. Guests do not need an account. Invited friends receive personalised URLs backed by unique invite tokens; external guests can use a public event page when allowed. They can view the event, RSVP, and be counted without logging in or joining the platform.

It also handles practical guest mechanics: capacity limits, host attendance, invited vs confirmed vs pending counts, external guest tracking, invite-only vs open guest policies, and optional guest list visibility. This makes it usable for real gatherings rather than just elegant as a planning concept.

Next.js, TypeScript, Prisma, PostgreSQL, NextAuth, Gemini, Vercel

## What I Work With

**AI and Agentic Systems:** LLM pipeline architecture, AWS Bedrock, Claude Sonnet, Haiku, Titan Embeddings, multi-model systems, context engineering, agentic workflows, trust architecture, human-in-the-loop design, prompt engineering, anti-hallucination by design.

**Platform and Infrastructure:** AWS, Azure, Terraform, GitHub Actions, GitHub Apps, IaC, developer experience tooling, specification-driven workflow automation.

**Languages and Frameworks:** TypeScript, Python, React Native, Expo/EAS, Next.js, Node.js.

**Data and Storage:** Supabase, PostgreSQL, Prisma, vector embeddings, semantic retrieval.

## Currently

Building production AI systems, shipping personal projects, and selectively taking on senior AI Platform Engineering contracts where the problem is genuinely interesting.

If you're working on something in agentic systems, cognitive pipelines, or AI developer experience and want to talk through the architecture, feel free to reach out.

[Email](mailto:kuli.singh@gmail.com) | [LinkedIn](https://www.linkedin.com/in/kulisingh/)
