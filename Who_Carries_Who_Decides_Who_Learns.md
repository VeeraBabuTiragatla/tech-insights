---
layout: default
title: "Who Carries, Who Decides, Who Learns?"
subtitle: "What Eight Frontier AI Companies Reveal About the Journey from Intelligence to Enterprise Action"
permalink: /who-carries-who-decides-who-learns/
description: "A strategic framework for comparing how eight frontier AI companies allocate the work, decision rights and learning involved in turning intelligence into enterprise action."
image: /assets/images/who-carries-who-decides-who-learns-framework.jpg
image_width: 1536
image_height: 1024
date: 2026-08-30
series: "Technology Landscape"
---

# Who Carries, Who Decides, Who Learns?

<p class="article-deck">What Eight Frontier AI Companies Reveal About the Journey from Intelligence to Enterprise Action</p>

<p class="article-meta">Veera Babu Tiragatla &middot; Technology Landscape</p>

In my previous article, [**“Why Enterprise AI Is Becoming Harder to Compare,”**](/why-enterprise-ai-is-becoming-harder-to-compare/) I argued that much of the confusion around enterprise AI comes from comparing products that occupy different parts of the technology stack.

But there is another problem with the stack metaphor.

A stack tells us **where things sit**.

It tells us much less about what has to happen **between them**.

That distinction is becoming more important as AI moves from answering questions to actually doing work.

A model can understand a request. An agent can develop a plan. A protocol can expose tools. An enterprise system can execute a transaction.

But between:

> **“Resolve this customer's problem”**

and

> **the customer's account actually changing**

lies a surprisingly large amount of hidden work.

Someone has to translate intention into a plan.

Someone has to connect that plan to the right capabilities.

Someone has to establish which data represents the current state of the business.

Someone has to decide what the agent is authorised to do.

Someone has to turn a probabilistic AI decision into a deterministic system change.

And, after all of that, someone has to determine whether the action actually produced a good outcome.

This led me to a different way of looking at the frontier AI competition.

Instead of asking:

> **Who has the smartest model?**

or even:

> **Who owns the largest part of the AI stack?**

I think enterprises increasingly need to ask three different questions:

### Who carries the work?  
### Who retains the decision rights?  
### Who gets close enough to the outcome to learn?

Those three questions reveal very different strategies across today's frontier AI companies.

---

## From intelligence to action

For this analysis, I use a simple seven-stage journey:

> **Model → Interface → Agent → Connection → Context → Control → Execution**

This is not intended as a universal taxonomy of enterprise AI.

It is simply a way of following intelligence as it moves toward organisational consequence.

At the **model** stage, intelligence exists as capability.

The **interface** turns that capability into something a person or system can direct.

The **agent** converts an objective into a sequence of decisions.

The **connection** layer gives that agent access to external capabilities.

**Context** tells it what those capabilities and data mean inside a particular organisation.

**Control** determines what may actually be done.

And **execution** changes the state of a real system.

Then something important happens:

### there is an outcome.

A refund either resolves the complaint or doesn't.

A price change either improves margins or damages demand.

A deployed code change either works or creates an incident.

An automated procurement decision either saves money or creates a supply problem.

So the complete journey is really:

> **Intelligence → Action → Outcome → Learning**

And every movement along that journey requires translation.

<figure class="article-figure article-figure-wide">
  <img src="/assets/images/who-carries-who-decides-who-learns-framework.jpg" alt="Seven-stage journey from model intelligence to enterprise execution and outcome, analysed through Translation Load, Decision Rights and Outcome-Loop Position.">
  <figcaption>The journey from model intelligence to enterprise action reveals who carries the translation work, who retains decision rights and who can connect outcomes back to future decisions.</figcaption>
</figure>

---

## The hidden work of enterprise AI

Imagine an agent receives this instruction:

> **“Resolve the issue with this supplier invoice.”**

The model may understand the English perfectly.

But what is an *issue*?

Which invoice?

Which supplier record is authoritative?

Does “resolve” mean contact the supplier, modify the invoice, approve payment, raise an exception or escalate to finance?

Is the employee who delegated the task allowed to approve the amount involved?

Can that authority be delegated to an AI agent?

If the ERP and procurement system disagree, which one represents organisational truth?

And if the agent takes action, what evidence later tells us whether its decision was correct?

None of these are simply model-intelligence problems.

They are **translation problems**.

That translation can be performed by the AI platform, the enterprise itself, application vendors, systems integrators, protocols, cloud infrastructure—or some combination of them.

And that creates the first question.

---

## 1. Who carries?

I call this **Translation Load**.

Translation load is the technical and organisational work required to convert AI capability into something compatible with actual enterprise operations.

It includes things such as:

- connecting applications;
- mapping schemas and terminology;
- resolving system state;
- establishing identities;
- defining permissions;
- reconciling conflicting data;
- orchestrating tools;
- implementing approvals;
- monitoring actions;
- handling failures and exceptions.

A platform that absorbs more of this work can make enterprise AI substantially easier to deploy.

But the work does not simply disappear.

It moves.

This distinction becomes useful when looking at MCP.

---

## MCP reduces translation work—but does not eliminate organisational translation

The **Model Context Protocol** is important because it standardises significant parts of how AI applications can discover and interact with external tools and data.

Anthropic originally created MCP and later donated it to the Agentic AI Foundation under the Linux Foundation. Anthropic says MCP has grown into a broad ecosystem and has been adopted across multiple AI products and developer environments.

Instead of building a different custom AI integration for every application, a shared protocol can reduce some of the work required to expose capabilities to agents.

But connectivity is not the same thing as organisational understanding.

An MCP tool can tell an agent:

> `issue_refund`

It cannot, by protocol alone, determine:

> whether issuing a refund is the appropriate organisational response to this particular customer under this employee's delegated authority.

That requires context and governance beyond simple tool discovery.

So the interesting question is not whether MCP “solves enterprise integration.”

It is:

> **Which translation work does MCP standardise, and which translation work remains with the enterprise and surrounding architecture?**

Anthropic's own strategy increasingly reflects both sides of this equation. MCP promotes open interoperability, while Claude itself is moving deeper into workflows through connectors, enterprise tools and managed-agent capabilities.

MCP therefore illustrates something larger.

Enterprise AI architecture is partly a decision about **where translation work should live**.

**Primary sources:**  
- Anthropic MCP documentation: https://docs.anthropic.com/en/docs/mcp  
- MCP project/specification: https://modelcontextprotocol.io/  
- Anthropic MCP / Agentic AI Foundation announcement: https://www.anthropic.com/news/donating-the-model-context-protocol-and-establishing-of-the-agentic-ai-foundation

---

## 2. Who decides?

Reducing translation load introduces a second question that may ultimately matter more.

### **Decision Rights**

Suppose an AI platform makes integration beautifully simple.

It understands the company's documents.

It knows the customer record.

It can see available tools.

It has an agent identity.

It knows the workflow.

It can execute an action.

That sounds desirable.

But then we need to ask:

> **Who defines what those things actually mean?**

Who determines which customer record is authoritative?

Who decides what constitutes a high-risk transaction?

Who sets the threshold at which an agent must stop and ask a human?

Who determines which tools the agent may discover?

Who controls whether a sub-agent inherits authority?

Who defines the difference between an ordinary exception and something requiring executive approval?

These are not merely configuration choices.

They are **organisational decision rights expressed through software**.

The distinction is subtle but important:

> **Permission asks whether an agent can perform an action.**

Governance additionally asks:

> **whether that agent should exercise that capability for this objective, in this context, under this delegated mandate.**

As agents become more autonomous, this distinction becomes harder to ignore.

Google's enterprise agent infrastructure makes the issue particularly visible. Its Agent Gateway can assign trackable agent identities, enforce granular policies, govern access to tools and produce observability data across agent interactions.

That is no longer merely “AI connected to an API.”

It is infrastructure for allocating machine-executable decision rights.

**Primary source:**  
- Google Gemini Enterprise Agent Gateway: https://docs.cloud.google.com/gemini-enterprise-agent-platform/govern/gateways/agent-gateway-overview

---

## 3. Who learns?

Then there is a third question.

Suppose the agent successfully acts.

Who sees what happened next?

I call this **Outcome-Loop Position**.

It does **not** mean that the AI provider necessarily receives customer data or trains its foundation model on it.

Those are separate issues.

It means something more architectural:

> **Which part of the system can associate an AI-driven decision with evidence about its eventual consequence?**

Consider:

**Intent**  
→ resolve customer complaint

**Decision**  
→ issue replacement

**Action**  
→ replacement shipped

**Outcome**  
→ customer retained

Now compare that with:

**Intent**  
→ resolve customer complaint

**Decision**  
→ issue refund

**Action**  
→ account refunded

**Outcome**  
→ customer still leaves.

A system that can connect outcomes back to decisions has something more valuable than another interaction log.

It has the beginnings of an **operational learning loop**.

OpenAI makes this increasingly explicit in Frontier. The platform combines enterprise business context, agent execution, individual agent identities and permissions, observability, and evaluation and optimisation loops.

Again, this should not be confused with using enterprise customer data to retrain foundation models.

The strategic point is simply that proximity to execution makes **evaluation of real work** possible.

And that may become an important source of advantage.

**Primary sources:**  
- OpenAI Frontier: https://openai.com/business/frontier/  
- OpenAI business-data controls: https://help.openai.com/en/articles/10306912-sharing-feedback-and-api-inputs-and-outputs-with-openai

---

## Eight companies, three questions

Viewed this way, the eight frontier AI companies begin to look less like participants in one model race and more like experiments in how intelligence should connect to organisational reality.

## OpenAI — absorbing more of the journey

OpenAI's direction is increasingly clear.

Frontier connects agents with business context, systems of record, identity and access management, execution environments, monitoring and evaluation.

Through this lens, OpenAI is absorbing more **translation load**.

The attraction for enterprises is obvious: fewer pieces need to be assembled independently.

The corresponding strategic question is equally obvious:

> As one platform carries more context, orchestration, identity and execution responsibility, **which decision rights should remain firmly under enterprise control?**

OpenAI itself emphasises explicit permissions, boundaries and auditable actions, so this is not an argument that the company is taking those rights away.

It is a broader architectural question created by deeper integration.

Source: https://openai.com/business/frontier/

---

## Anthropic — standardising the journey while increasingly participating in it

Anthropic began with a particularly interesting strategic move: rather than owning every enterprise application, it helped standardise how agents reach external capabilities through MCP.

That lowers part of the translation load without requiring the same company to own the ERP, CRM, database and productivity suite.

But Anthropic is no longer simply a model-and-protocol company.

Claude now works through connectors and increasingly capable enterprise workflows, while Anthropic is building a large partner ecosystem to help organisations integrate Claude into existing operations.

So Anthropic illustrates a hybrid strategy:

> **standardise heterogeneous connectivity while building richer agent workflows above it.**

That may preserve greater architectural composability, but it also means more of the semantic and organisational translation can remain distributed among enterprises and their technology partners.

Sources:  
- https://docs.anthropic.com/en/docs/mcp  
- https://www.anthropic.com/news/claude-partner-network

---

## Google — reducing translation through ecosystem adjacency

Google starts from a very different position.

It does not have to build every surrounding enterprise capability from zero.

Gemini can coexist with Google Cloud, Workspace, enterprise identity infrastructure, data services, agent runtimes and a substantial governance layer.

Gemini Enterprise Agent Platform includes agent identity, registry, gateway, policy enforcement and observability.

That gives Google a potentially powerful form of **adjacency advantage**.

When model, identity, context, governance and execution infrastructure already coexist within the same ecosystem, some translation work can occur inside existing relationships rather than across new organisational boundaries.

The trade-off is familiar:

> integration coherence can increase at the same time as platform dependence.

Sources:  
- https://cloud.google.com/gemini-enterprise/agents  
- https://docs.cloud.google.com/gemini-enterprise-agent-platform/govern/gateways/agent-gateway-overview

---

## Meta — making intelligence portable and letting others determine the architecture

Meta's strategy has historically placed much greater weight on open distribution.

Llama has been positioned as something businesses, developers, cloud providers and partners can use to build their own systems.

That moves more translation load toward cloud providers, application vendors, developers, systems integrators, and enterprises themselves.

But it can also give those deployers greater choice over where context, governance and outcome data reside.

The strategic proposition is therefore different:

> **Make intelligence portable enough that the surrounding ecosystem decides how it becomes enterprise action.**

Sources:  
- https://ai.meta.com/opensourceAI/  
- https://ai.meta.com/blog/llamacon-llama-news/

---

## Mistral — moving intelligence toward organisational context

Mistral exposes another possibility.

Perhaps the enterprise should not always move more data, context and control toward a central AI platform.

Perhaps intelligence can instead move toward the enterprise.

Mistral Forge supports models grounded in proprietary datasets, ontologies, decision frameworks and institutional knowledge, with deployment available across private cloud, on-premises infrastructure or Mistral-managed environments.

That can relocate part of the translation problem.

Instead of repeatedly translating organisational reality into an external platform environment, the organisation can place more intelligence inside an environment it already governs.

This does not eliminate integration work.

In some cases, it may increase the engineering responsibility retained by the enterprise.

But it changes **where the work and decision rights live**.

Sources:  
- https://mistral.ai/news/forge/  
- https://mistral.ai/services/

---

## DeepSeek — making the intelligence layer easier to substitute

DeepSeek is particularly interesting because its strategic effect may be larger than its enterprise application footprint.

Its APIs support tool calling and compatibility patterns that make DeepSeek relatively easy to place behind existing agent frameworks and developer tooling.

That suggests a different future.

If capable model intelligence becomes increasingly easy to substitute through compatible interfaces, then some enterprise value may migrate away from the model layer toward:

**context**

**governance**

**workflow**

**identity**

**execution**

and

**outcome evaluation**.

DeepSeek therefore raises a useful strategic question:

> **What becomes scarce if model intelligence becomes easier to swap?**

Organisational reality may be one answer.

Source: https://api-docs.deepseek.com/guides/function_calling

---

## xAI — rapidly moving from world context toward enterprise action

xAI is the company where earlier assumptions can become outdated quickly.

Its proximity to X makes it tempting to characterise Grok mainly around real-time external information.

But xAI has also been moving into enterprise connectors and persistent agent capabilities.

This makes xAI interesting because its architecture is moving across **both sides of reality**:

external world state through X and the web,

and

internal organisational state through enterprise tools and agent execution.

The question is no longer simply whether xAI can enter enterprise workflows.

It is how quickly it can build the governance, trust and operational depth required around that execution.

Sources:  
- https://x.ai/news/grok-connectors  
- https://x.ai/news/introducing-grok-bot

---

## Moonshot AI — putting more agency close to the user's machine

Moonshot's Kimi trajectory points in yet another direction.

Kimi Work is a local agent capable of interacting with files, browsers, code, scheduled tasks and tools on the user's own computer, while Moonshot has also been developing increasingly capable multi-agent execution.

That architecture is strategically interesting because execution does not always have to occur inside a central cloud control plane.

Some intelligence can operate much closer to the user's immediate computing environment.

This potentially relocates execution, permissions, local state and parts of the translation load toward the endpoint itself.

It also creates new governance questions.

If increasingly capable agents operate locally, enterprises will need to govern not just central AI platforms but **distributed machine-level agency**.

Source: https://www.kimi.com/en/help/kimi-work/overview

---

## What the comparison reveals

The eight companies do not divide neatly into permanent categories.

That is actually the point.

Their strategies are converging in some places and diverging in others.

OpenAI is expanding toward enterprise infrastructure.

Anthropic combines interoperability with increasingly capable workflows.

Google can build on an existing enterprise ecosystem.

Meta continues to emphasise portability and ecosystem deployment.

Mistral offers greater choice about where intelligence physically and operationally resides.

DeepSeek increases model substitutability.

xAI is moving rapidly into persistent agents and enterprise connectors.

Moonshot is experimenting with powerful local and multi-agent execution.

So perhaps the more useful enterprise comparison is not:

> **Which one has the best model?**

It is:

| Question | What enterprises should examine |
|---|---|
| **Who carries?** | How much integration, semantic mapping, orchestration and operational engineering does the vendor absorb? |
| **Who decides?** | Where do identity, permissions, policy, business meaning and approval authority remain? |
| **Who learns?** | Who can connect agent actions with outcomes, evaluations and subsequent improvement? |

These questions reveal something benchmark tables cannot.

---

<figure class="article-figure article-figure-wide">
  <img src="/assets/images/organisational-reality-frontier-ai-strategies.png" alt="Eight frontier AI companies approaching the scarce core of organisational reality, including context, identity, business rules, authority, execution, outcomes and institutional memory.">
  <figcaption>Different AI strategies approach the same scarce enterprise core: organisational meaning, authority, execution, outcomes and institutional memory.</figcaption>
</figure>

## What does an enterprise surrender when integration becomes easy?

This may be the hardest question.

The best AI platform may eventually make enterprise integration almost invisible.

It may understand employees, customers, applications, permissions, documents, workflows, business terminology, past decisions, and increasingly the outcomes of work.

That could be enormously valuable.

But enterprises should recognise that integration architecture is not neutral.

When a platform absorbs translation work, it may become more deeply embedded in how the organisation:

**represents reality**

**allocates authority**

and

**learns from action**.

The appropriate response is not necessarily to avoid integrated platforms.

Nor is it to insist on building everything internally.

It is to become much more deliberate about what is being outsourced.

An enterprise might happily outsource connector maintenance.

It might welcome a standard protocol for tool discovery.

It may want a vendor to operate complex agent infrastructure.

But it may decide that definitions of authoritative business state, approval thresholds, delegated authority or strategic outcome data must remain under its own governance.

The question is therefore no longer simply:

> **open versus closed**

or

> **build versus buy**.

It becomes:

> **Which translation burdens are worth outsourcing—and which decision rights and learning loops are too important to surrender?**

---

## Intelligence may become abundant. Organisational reality will not.

Frontier models will continue improving.

Prices will change.

Benchmarks will change.

Today's leader may not be tomorrow's leader.

Protocols will become more standard.

Agents will gain access to more tools.

But every enterprise possesses something far harder to commoditise:

its own operational reality.

The meaning hidden inside years of workflows.

The exceptions nobody documented.

The difference between what policy says and how work actually happens.

The relationships between people and systems.

Its risk appetite.

Its institutional memory.

Its authority structure.

And ultimately, the consequences of its decisions.

That suggests a different way to think about the next phase of enterprise AI.

The competitive advantage may not belong simply to the company that produces the most intelligent model.

It may belong to architectures that can move intelligence toward action while answering three questions convincingly:

> **Who carries the work?**

> **Who retains the right to decide?**

> **And when the action meets reality—who gets to learn?**

Because once AI moves from generating answers to changing organisations, intelligence is only the beginning.

### **The real system begins where intelligence meets consequence.**

---

## Source note

The company analysis is intentionally based primarily on first-party product and technical documentation. Vendor descriptions are used to establish current product direction; the strategic interpretation in this article is the author's analysis rather than a claim made by the vendors themselves.
