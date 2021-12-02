This document outlines what that means to be a Project leader at Koan, along with some helpful hints to get things off on the right foot. There's also a rubric aligned to each phase of the project to help quantify otherwise-qualitative expectations and measure progress.

[Project Rubric](project-rubric.md)

## Expectations

As the tech lead, you're the project's de-facto subject matter expert. You're also a bridge between a project's stakeholders and the implementation team. Connecting both sides is both an important part of the job and a significant factor in whether it succeeds or fails.

At the start of the project, you'll be deeply involved in project planning. As the focus shifts to implementation, you'll communicate project status, negotiate change orders as needed, and orchestrate work with the team. Finally, you'll help coordinate the eventual release.

### Planning

- **Project definition**. We don't need a traditional Product Requirements Document (PRD) to get started, but we do need a clear sense of what we're going to build, communicated in terms that a reasonably informed person can understand.
  1.  **Customer requirements**. These set expectations around what is and isn't important to the project's customers. They should be clear, concrete, and easily assessed. Even if the customer arrives waving a neatly-written list of requirements, they're still worth a review and discussion. Implementation has a way of wandering into gaps that may not have been obvious on paper!
  2.  **Acceptance criteria**. These describe the scope and "done" state of the project. User stories ("_[Actor] does [Action] to [Achieve Result]_") are a familiar, reasonably complete way to express what a feature is expected to do. They're relatable outside the dev team, and they make for nice headlines on test cases, too. And don't forget that some criteria ("implements UI as designed") are implicit. Use good judgment!
  3.  **Milestones**. Most projects will start with a time-boxed "research" phase to uncover unknowns, work out the technical plan, and queue up the remaining work. That's the first milestone. As soon as possible afterwards, you'll want to work with stakeholders to outline the scope and order of all the other milestones needed to see the project through. Remember: the further something is in the future, the fuzzier it gets. Set expectations accordingly.
- **Tech specs**. New projects will likely require new development. As the tech lead, you're not necessarily on the hook to play architect (teammates can help with this)—but you'll want at least a loose map of how data models, API contracts, and infrastructure will need to shift around to make space for the new project.
  - Don't forget instrumentation for observability, diagnostics, and analytics

In devising the plan, be mindful of the trade-offs between quality, urgency, and risk. Strapping an engine on a bicycle adds customer value faster than building an entire motorbike. If a customer requirement mentions a freeway, though, you'll want to think long and hard about how small of a shippable unit we can really get away with.

### Implementation

As the project enters implementation, you'll take on two new responsibilities: orchestrating work and communicating status.

- **Orchestrating work.** Leading a project doesn't mean implementing it yourself. Breaking work down into units that can be distributed across the entire team makes for a much more pleasant, collaborative project experience—and as that the tech lead, that breakdown starts in your corner. To make it happen, you'll want to:

  - **Create an epic for the project** or an immediate milestone. For one example of how this
  - **Write an initial set of tickets** that provide clear goals and adequate context. "Context" is subjective, but try to anticipate likely follow-up questions that might block the ticket and answer them in the ticket description.

    Links to relevant specs or designs can also be very helpful, but be careful—links to stale documents are worse than no links at all. When in doubt, link to the project's root page in Notion or Figma rather than a specific, likely-to-change element deeper inside.

    You're not on the hook to write every ticket (team members can and will add their own as new tasks turn up), but a good set of starter issues will help get things rolling.

  - **Prioritize work**. Tackling highest-priority work first helps ensure it gets done. Check in with stakeholders often—at least once per week—to understand what's most important to them and update priorities as needed. If "everything's equally important," inject a measure of reality of your own. However the call gets made, priority is crucial to making sure feelings won't be hurt when the cut-line lands towards the end of the project.
  - **Make sure blockers are resolved**. There will be obstacles along the way. You'll head off what you can, but you won't anticipate everything. Keep an eye out for features that are hung up in code review or architectural decisions that aren't working out. You don't need to resolve everything yourself, but you do need to call attention to problems as they happen—and follow up until they're solved.
  - **Have the answers**. Not all team members will have the complete context or mental map of the project in their head; as the tech lead, you'll be called on to provide both. Know the requirements. Know the plan. Be ready to share both, early and often.

    If you _don't_ have the answer, find one. Somebody probably asked a good question!

- **Communicating status.** Keeping everyone informed as development progresses and change-orders land is a constant struggle. It also crucial to successful delivery. Over-communicate early and often, including:

  - sharing epic links and Jira filters everywhere
  - frequently grooming/updating "living" planning docs
  - summarizing both progress and updates in your reflection and any relevant Slack channel(s)

  Communication is the key to adaptation. We'll learn new things as we build. We'll shift priorities, people, and project scope to accommodate. Communicating early and often gives both stakeholders and the dev team as much lead time as humanly possible to adapt and respond. Sometimes reality sets in. When it does, share it. Drama's much easier to manage when we can catch it in the open.

### QA

As the tech lead, you're not on the hook to do QA yourself. You won't be good at it anyway—with your head deep in how the project _should_ work, a friendly collaborator from outside the project team is far more likely to get confused and turn up extra cases than you ever would.

You _are_ on the hook to make sure QA happens ahead of a release. Depending on the complexity of the project, you should:

1.  write a thorough (but not too thorough) test script
2.  run it and document/fix any obvious issues
3.  recruit at least one pair of outside eyes to join the fun
4.  repeat until stakeholders are convinced that the project is ready

Note that many issues turned up in QA (and especially close to the shipping date) will not block a release. That's fine. On principle (see [Every Software team Deserves a Charter](https://medium.com/developing-koan/every-software-team-deserves-a-charter-1fcbc2d210ee)) we release _the moment staging is better than production_, and cases of "great" blocking "good" are fine to file and fix in subsequent releases.

### Release prep

There's more to a release than flipping a switch. Collateral and documentation need to be prepared; team members need to be trained; reporters need to be briefed; customers need to be notified. Once again, you aren't on the hook for all of this—but as the tech lead, you need to make sure that it happens.

On the growth side of the house, make sure **_well in advance of the launch date for the project or milestone_** that a written launch list covers the relevant details. These will likely include:

- A [product] marketing plan
- Knowledge Base (KB) articles
- Any demo videos or other training material
- Customer communications/rollout/awareness promotion

You'll be asked (better yet, volunteer) your expertise to inform and review this material. Be generous with your time. Great work barely counts if we aren't in a good place to take credit for it and see our customers find value.

### Flipping the switch

The switch _does_ still need to be flipped, though, and that's on you. You've set clear expectations around the date, but you'll still want a launch list of your own. This will cover things like:

- data migrations that need to be run
- feature flags that need to be flipped
- builds that need to be deployed
- logs to be tailed; analytics to be watched; support queues to be monitored

That sort of thing. You know the drill. We release all the time! But some releases are bigger than others.

### After the launch

Getting the project into customers' hands is cause for celebration. But! The project isn't quite over yet. Even with the initial version out the door, you'll still need to work with the project team and stakeholders to:

- monitor logs, analytics, and inbound feedback for signs of trouble—or new opportunities
- prioritize follow-up issues, then implement or defer
- remove feature flags
- schedule and run a project retrospective

## Don't forget...

We score points for shipping value to customers—not for solo heroics or sudden fits of technical innovation. With that in mind, don't be shy to take advantage of:

- **Your team**. You're leading a meaningful project—something we'd all like to see built—and your teammates are here to help. Beyond implementation, our insights and perspectives may be useful in challenging product plans, splitting up work, or filling in technical details. Let us know how we can help!
- **Existing infrastructure**. Like many teams practicing continuous delivery, we rely heavily on feature flags to keep half-built features out of sight in production. They're cheap to set up and historically not too arduous to tear down (let's keep it that way). Use them!

## Aphorisms & anecdotes

As the latest in a proud line of project leaders at Koan, you're in good company. From teammates who've run the show before...

- _"Every project starts 'red"'_
- "_Do the hard stuff first."_
- _"Work back from the end-user impact"_
- _"Don't sweat the details until delivery's no longer in doubt"_
- _smaller pieces == less scope risk_
- _more communication == less fumble risk_
- _fewer hands (lottery problem notwithstanding) == less comms risk_
