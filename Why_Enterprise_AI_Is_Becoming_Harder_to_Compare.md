---
layout: default
title: "Why Enterprise AI Is Becoming Harder to Compare"
permalink: /why-enterprise-ai-is-becoming-harder-to-compare/
description: "A practical guide to models, agents, MCP, A2A, enterprise context, and the platforms competing around them."
image: /assets/images/enterprise-ai-comparison-map.jpg
date: 2026-08-23
---

# Why Enterprise AI Is Becoming Harder to Compare

<p class="article-deck">A practical guide to models, agents, MCP, A2A, enterprise context, and the platforms competing around them</p>

<p class="article-meta">Veera Babu Tiragatla &middot; 15-minute read &middot; Technology Landscape</p>

<figure class="article-figure article-figure-wide">
  <img src="/assets/images/enterprise-ai-comparison-map.jpg" alt="Enterprise AI comparison map showing frontier AI labs moving outward from intelligence and enterprise incumbents moving inward from process and context toward a shared execution stack">
  <figcaption>Frontier AI providers and enterprise incumbents begin from different positions, but increasingly converge around the same enterprise execution environment.</figcaption>
</figure>

I started noticing the change at technology meetups in Melbourne.

A year or two ago, conversations about generative AI could quickly turn into comparisons between models. Which one reasoned better? Which one generated better code? Which one handled more context? Which benchmark had moved?

Those conversations have not disappeared. But increasingly, the questions I hear are different.

People are talking about agents, MCP servers, enterprise context, tool access, identity boundaries, orchestration, agent-to-agent communication, observability, and runtime policy.

And the interesting questions often begin *after* a model has already been selected:

- What can the agent actually access?
- Can it read from an enterprise system but not write to it?
- Whose identity is it operating under?
- What happens when it invokes another tool—or another agent?
- Where is policy enforced?
- And if something goes wrong, can we reconstruct what actually happened?

That shift in technical dialogue helps explain why the enterprise AI market has become surprisingly difficult to evaluate.

Follow the industry today and we encounter what looks like an increasingly chaotic collection of products: OpenAI has the Responses API and Agents SDK for building agents that execute across tools and systems. Microsoft spans Copilot Studio, Microsoft Foundry, Microsoft 365 Copilot, and Agent 365. AWS builds Amazon Bedrock AgentCore around agent runtime and supporting services. Google helped introduce A2A for agent interoperability. Anthropic introduced MCP. SAP embeds Joule and agents into business processes. Salesforce continues to develop Agentforce.

At first glance, these products can appear to be contestants in one giant AI race.

**They are not.**

They occupy different positions in the same emerging enterprise AI environment.

The strategic question is becoming less:

> **Which company has the best AI?**

And more:

> **Which part of the enterprise AI architecture is each company actually trying to occupy?**

---

## 1. They Are Not All Competing at the Same Layer

I find six simple questions useful when trying to make sense of an enterprise AI product.

This is not intended as a rigid academic taxonomy. Real platforms overlap constantly. It is simply a practical lens for making the market easier to read.

### 1. Intelligence — Which model reasons?

This is the part of the market we have spent most of the generative-AI era watching.

The model provides reasoning, language, multimodal capability, and increasingly sophisticated problem solving.

Breakthroughs here continue to matter enormously. But as capable models become available from several providers, raw model performance may become less decisive on its own as an enterprise differentiator.

The next question becomes:

**What happens around the intelligence?**

### 2. Interface — Where do we begin?

The interface might be a chat application, a coding environment, Microsoft 365 Copilot, or an assistant embedded inside an ERP, CRM, service-management platform, or industry application.

This matters because the interface is often where human intention first enters the AI environment.

It can influence which model receives the request, what organisational context becomes available, which tools are exposed, and which agents are invoked downstream.

Enterprise technology becomes particularly powerful when we stop consciously deciding to use it and simply begin our work there.

### 3. Context — What does the AI know about our organisation?

Context grounds general reasoning in organisational reality.

That can include semantic definitions, transactional history, supplier status, master data, process state, permissions, business rules, and organisational structure.

A frontier model may know an extraordinary amount about the world.

It does not automatically know what *our organisation* means by:

“approved supplier”

“credit hold”

“priority order”

“material status”

or “exception approval.”

Without context, an intelligent model is still something like a **well-read stranger**.

Capable. Articulate. Potentially very useful.

But unfamiliar with the particular operational reality in which our organisation works.

### 4. Agency — What can plan and pursue the task?

Answering a question is one thing.

Pursuing an objective is another.

An agent may break a goal into steps, retrieve information, invoke a tool, inspect the result, adjust its plan, prepare an action, execute it, or hand part of the work to another agent.

This is where AI begins to move from:

**help us understand the work**

toward:

**help us perform the work.**

### 5. Connection — What systems and capabilities can it reach?

An agent becomes substantially more useful when it can interact with the systems around it.

That can mean databases, APIs, business applications, tools, external services, or other agents.

This is where protocols such as MCP and A2A become relevant.

### 6. Control — How is its behaviour governed and audited?

Once agents can act, control moves closer to execution.

Identity, permissions, policy enforcement, guardrails, logging, observability, and lifecycle governance become part of the production environment rather than something added afterwards.

---

## 2. Enterprise Systems Accumulate Operating Memory

This is where my background around SAP and complex enterprise-platform implementations makes me particularly cautious about comparing enterprise AI only through model benchmarks.

Years around enterprise software taught me that these systems accumulate far more than raw data.

They accumulate what I think of as **operating memory**.

A finance rule gets configured.

An approval threshold changes.

A warehouse process becomes integrated with another system.

Security roles evolve.

Master-data conventions become established.

Reports begin depending on particular structures.

Another application gets connected.

An exception process develops.

Someone discovers a workaround.

Years later, new employees may not even know *why* part of the process works the way it does.

Yet the organisation continues to operate around it.

That accumulated history creates a kind of pull.

I think of that pull as **process gravity**.

Not because an established platform is impossible to replace.

But because replacing mature enterprise technology rarely means replacing software alone.

We are changing relationships between data, processes, roles, integrations, controls, habits, and people.

AI is arriving inside that environment.

**It is not arriving on a blank page.**

---

## 3. Why a Smart Model Is Not Yet an Enterprise Worker

Consider something that sounds straightforward:

> **Resolve this supply-chain exception.**

To a general reasoning system, that looks like a problem to analyse.

Inside an enterprise, however, the instruction may imply much more.

Which plant is affected?

What inventory is available elsewhere?

Is the supplier approved?

Is there a contractual restriction?

What is the purchase-order status?

Does changing the supplier trigger another approval?

Who has authority to approve the exception?

Are there regional tax or compliance implications?

Is the relevant information in SAP, another database, an email, a planning tool, or somebody's operational knowledge?

This is where the difference between **reasoning** and **enterprise execution** becomes visible.

A model may be intelligent enough to propose a solution.

But useful enterprise AI also requires access to the context and capabilities needed to determine whether that solution is appropriate—and, where permitted, to do something about it.

**Intelligence matters enormously. But so does everything intelligence must pass through before it becomes enterprise action.**

---

## 4. Why Vendors Are Approaching From Opposite Directions

Once we separate these functions, the vendor landscape becomes easier to read.

Different providers begin from very different positions.

### Frontier AI providers: moving outward

Companies such as OpenAI and Anthropic begin primarily with **intelligence**.

Their core strength is the reasoning engine.

From there, they can move outward into developer environments, agent frameworks, connectivity, orchestration, enterprise integrations, governance, and execution.

A simplified direction looks like:

**Intelligence → Interface → Agents → Connections → Enterprise Work**

### Enterprise incumbents: moving inward

Companies such as SAP, Salesforce, and ServiceNow begin much closer to **process and context**.

They already sit near business rules, transactional history, user permissions, organisational workflows, and operational systems.

Their direction looks more like:

**Process + Context → Agents → Intelligence**

They do not necessarily need to build the world's most capable foundation model themselves.

They can bring increasingly capable intelligence into environments where work is already happening.

<figure class="article-figure article-figure-wide">
  <img src="/assets/images/enterprise-ai-execution-stack.png" alt="Two directions toward one enterprise execution stack, comparing frontier AI labs moving outward and enterprise incumbents moving inward across six capability layers and eight evaluation questions">
  <figcaption>Different starting points, one enterprise execution stack: the market is converging around intelligence, interface, context, agency, connection and control.</figcaption>
</figure>

---

## 5. Process Position Is an Advantage — Not an Automatic Victory

Enterprise incumbents possess something strategically important.

They already occupy many of the environments where operational work happens.

Existing users.

Existing data.

Existing permissions.

Existing workflows.

Existing integration points.

That gives them what I would describe as **process position**.

But it does not mean incumbents automatically win.

Legacy complexity can slow them down.

Enterprises may prefer external models.

Open protocols can reduce integration barriers.

Specialised tools may outperform functions embedded inside broad platforms.

And many organisations may deliberately operate multi-model and multi-platform environments.

The result is not simply a battle between “AI companies” and traditional enterprise software.

It is a convergence.

Model providers are moving closer to enterprise execution.

Enterprise platforms are moving closer to intelligence.

Hyperscalers increasingly span several functions at once.

And open standards are making some boundaries more permeable.

---

## 6. Where MCP and A2A Actually Fit

Much of the current industry conversation revolves around protocols such as MCP and A2A.

Their names can make the landscape seem more complicated than it needs to be.

In practical terms, I think of them this way.

### MCP — Model Context Protocol

MCP primarily helps AI applications and agents discover and use external tools, resources, and capabilities.

It helps address a basic question:

> **How does the AI reach things outside itself?**

That might include data sources, services, APIs, enterprise systems, or specialised tools.

### A2A — Agent-to-Agent

A2A focuses more directly on interoperability between independent agents.

A useful mental shortcut is:

**MCP → AI application/agent ↔ capabilities and resources**

**A2A → agent ↔ agent**

But this should not be treated as a permanent architectural law.

Both areas are evolving.

And open protocols do not automatically make an entire enterprise environment portable.

Data models, workflow definitions, runtime dependencies, identity systems, proprietary APIs, and governance arrangements can still create substantial switching costs.

---

## 7. Control May Become One of the Most Important Layers

Control is not the most glamorous part of AI.

It may become one of the most important.

When an AI produces a paragraph, governance can remain relatively distant from execution.

When an agent can call an API, modify a record, invoke another service, communicate externally, or initiate a transaction, governance enters the execution path.

We need to ask:

Which identity is the agent using?

Which resources can it access?

How are permissions scoped?

What happens when it delegates?

Which policies apply?

Are tool calls visible?

Can security teams identify which agents exist?

Can we reconstruct what happened after an incident?

The model is only one part of the production system.

As AI moves from generating information toward performing work, **control becomes infrastructure**.

---

## 8. What We Should Actually Compare

This is why I would not evaluate enterprise AI using a single model leaderboard.

We should ask at least eight questions.

| Evaluation dimension | Question we should ask |
| --- | --- |
| **1. Model flexibility** | Can we use or replace underlying reasoning models as capability, economics, or requirements change? |
| **2. Context depth** | How naturally can the system work with our master data, business semantics, transaction history, and permissions? |
| **3. Integration breadth** | How easily can it reach the systems and capabilities we already use? |
| **4. Agent capability** | Can it reliably perform multi-step work, or is “agent” mainly a label around a conversational experience? |
| **5. Identity & security** | How is the agent identified? Whose permissions does it inherit? Can permissions be independently scoped? |
| **6. Observability** | Can we trace inputs, outputs, tool invocations, policy decisions, and system modifications after execution? |
| **7. Portability** | If we change providers, what moves with us—prompts, agent definitions, tools, workflow logic, or evaluation data? |
| **8. Switching cost** | Which parts of our operating logic are becoming dependent on a vendor-specific runtime, identity system, data layer, or workflow environment? |

Those questions tell us much more than:

> **Which model scored highest this month?**

---

## 9. Platform Convenience vs. Architectural Portability

There is no universally correct architecture.

A deeply integrated environment can be extremely attractive.

Identity may already exist.

Security tooling may already be deployed.

Logging may already be centralised.

Support relationships already exist.

Employees already know the interface.

Using more of the same ecosystem can reduce friction considerably.

But convenience creates dependency.

The more functions one provider occupies, the more difficult replacement can become.

A composable architecture offers another route.

Different models.

Different tools.

Independent agents.

Open protocols.

Separate data platforms.

Potentially greater choice.

But composability has a cost too.

Every boundary introduces another integration.

Another authentication relationship.

Another policy boundary.

Another operational dependency.

Another thing that can fail.

The useful question is therefore not:

> **Open or closed?**

It is:

> **Where is portability valuable enough to justify the additional complexity?**

---

## What to Remember

The enterprise AI market becomes easier to understand when we stop asking which product is simply **“the best AI.”**

The products are not all doing the same job.

Some compete on intelligence.

Some control important interfaces.

Some sit closest to enterprise data and process context.

Some are building agents.

Some are building connections between agents and enterprise capabilities.

Others are building the identity, governance, and control infrastructure needed to let those agents operate.

And increasingly, the same companies are trying to occupy several of these positions at once.

Model leadership can change quickly.

Enterprise position usually changes much more slowly.

The next phase of enterprise AI competition may therefore be shaped as much by who becomes embedded in organisational context, workflows, identity, and control as by who leads the next benchmark.

For enterprise leaders, that leaves a question more durable than another model comparison:

> **Which parts of the architecture around intelligence do we want to remain easy to replace—and which parts are we comfortable allowing to become deeply embedded?**

---

### Author Note

**Veera Babu Tiragatla** writes about enterprise technology, AI, data systems, and the changing relationship between intelligent systems and organisational decision-making. His perspective draws on years working around SAP, enterprise data, business intelligence, and complex technology environments, alongside his continuing exploration of modern AI and data platforms.

---

### Publication Series

**Technology Landscape**

Practical perspectives on the technologies, architectures, and competitive shifts reshaping enterprise systems.
