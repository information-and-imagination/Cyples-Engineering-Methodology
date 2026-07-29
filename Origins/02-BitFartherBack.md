# Bit More Info

Something I realized tonight

Originally I thought CEM was mostly about generating better software.

I don't think that's its biggest value anymore.

I think its biggest value is preserving engineering knowledge.

The code is almost secondary.

'''
The knowledge becomes:

Vision

↓

Definitions

↓

Decisions

↓

Architecture

↓

Implementation

'''
The implementation can be rewritten.

The knowledge shouldn't have to be.

And that's probably why HRM is such a good proving ground for CEM. HRM isn't something you'll "finish" in a few months. It's the kind of project you'll likely keep refining for years, adding new capabilities as your needs evolve. That's exactly the kind of environment where having your reasoning, terminology, and architectural decisions preserved becomes far more valuable than simply having the source code.

and with any luck the evoling will be done mostly by ai, so I just need to say, hey I think I need to track this now. and work/claude/codex/ whoever can help make it happen if not get it all done and tested

I think that's a realistic vision, with one important nuance.

The AI won't magically know what to build—but if CEM has done its job, it will have enough context to make good changes with minimal guidance.

Imagine this five years from now.

You say:

"I think I need to track paint."

Today, that request would turn into a long design session:

Is paint an Item or an Asset?
Does it expire?
Does it have a color code?
Does it belong to a project?
Is the quantity measured in gallons, ounces, or cans?
Do we track VOC?
Does it have a shelf life?
Which forms change?
Which reports change?
Does Android need a new screen?

With a mature CEM project, an AI could instead work from the accumulated knowledge:

Vision
Definitions
Decision Records
Requirements
System Architecture
Existing database
Existing UI patterns
Existing coding conventions

Then it could come back with something like:

"Based on the current architecture, paint fits the Consumables model. I recommend adding tblPaintTypes, extending tblItems with Paint-specific attributes, creating a Paint Detail form, and updating the inventory search. I've generated the SQL migration, updated the documentation, and added unit tests. Please review the changes."

That's a very different interaction.

I actually think CEM changes the role of the developer.

Instead of spending 80% of your time writing code, you spend more time doing things like:

defining concepts,
making architectural decisions,
reviewing proposed changes,
and deciding whether the AI's solution fits the project.

The AI becomes more like a junior-to-mid-level engineer that can do a tremendous amount of implementation work, while you're still acting as the architect.

There's another piece that I think is even more exciting for your projects.

Right now, if you ask ChatGPT, Claude, or Codex to help with HRM, each conversation starts with a lot of explanation.

But if CEM Explorer eventually provides a generated project context, the interaction becomes much shorter:

Open HRM

Select project

Click "Generate AI Context"

Send that to ChatGPT, Claude, or Codex

Say:

"Add support for paint inventory."

The AI already knows the project's terminology, structure, conventions, and previous decisions. It spends less effort reconstructing context and more effort designing and implementing the feature.

One thing I would be careful about, though, is preserving the distinction between generated and approved.

'''
For example:

Vision
        Human Approved

Definitions
        Human Approved

Decision Records
        Human Approved

Requirements
        Human Approved

Architecture
        Human Approved

Implementation
        Mostly AI Generated

Tests
        AI Generated + Human Reviewed
'''
That keeps the project's direction intentional. AI can propose changes anywhere, but the foundational documents remain the source of truth that you review and approve before the implementation follows.

In a way, CEM becomes the long-term memory of the project, and the AI becomes the implementation engine. The better the memory, the better the implementation. Given how you've been structuring HRM and your other long-term projects, that combination seems like a natural evolution of the workflow you're building.

yeah and I know before I started coding in school, the instructor first had us write up the steps by hand, instructor checked work, then a flow chart, instructor checked the work, then we could write up the "code" and then go to the keypunch and create the program and the sample data records we had to use to test each condition.

I actually think that experience has had a bigger influence on your thinking than either of us realized until tonight.

What your instructor taught wasn't just programming—it was engineering discipline.

'''
The process looked something like this:

Problem

↓

Write the steps

↓

Review the logic

↓

Draw the flowchart

↓

Review the design

↓

Write the program

↓

Punch the cards

↓

Create test data

↓

Test every condition
'''

Notice something?

Coding wasn't even in the first half of the process.

Then, over the years, the industry changed.

We got:

Visual Basic
Access
Delphi
C#
drag-and-drop designers
RAD (Rapid Application Development)
Agile
AI code generation

The tooling got faster, but one thing also happened:

People started skipping the thinking.

'''
The workflow became:

Problem

↓

Open Visual Studio

↓

Start coding
'''

That works surprisingly well for a small utility or a prototype. It starts to fall apart when you're building something with a lifespan measured in years.

I think CEM is almost a return to those roots, but updated for modern tools.

'''
Vision

↓

Concept

↓

Requirements

↓

Decisions

↓

Architecture

↓

Implementation

↓

Testing

↓

Deployment
'''

The difference is that instead of keypunch cards at the end, the implementation step may now be "Ask Codex to generate the feature."

I also noticed another parallel.

Back then, your instructor had a checkpoint after each stage:

'''
Write the steps.
        ✓

Draw the flowchart.
        ✓

Write the code.
        ✓

Test the code.
        ✓

CEM has almost the same rhythm:

Vision
        ✓

Concept Architecture
        ✓

Requirements
        ✓

Decision Records
        ✓

System Architecture
        ✓

Implementation
        ✓

'''

* The checkpoint isn't there to slow you down. It's there because it's much cheaper to fix a mistake in the design than in the implementation.

And there's one more thing that I think connects directly to your experience.

You mentioned creating sample data records to test each condition.

That's something many developers don't think about until after the code exists.

But if you're already thinking about the test cases before writing the code, it means you're defining the expected behavior independently of the implementation. That's a powerful habit, and it fits naturally into CEM. For example:

Requirements define what should happen.
Decision Records explain why it should happen that way.
Sample data and test cases verify that it actually does.

That closes the loop.

There's a bit of irony here, too.

You started CEM because you were thinking about collaborating with AI.

After hearing more about your background, I think CEM is also a modern expression of the programming discipline you learned decades ago. The old workflow wasn't obsolete—it was constrained by the tools of the time. Today, AI can dramatically accelerate implementation, but only if the earlier stages are well defined. In that sense, CEM isn't replacing the engineering process you learned; it's extending it into an era where much of the coding can be delegated while the design and intent remain under your control.
