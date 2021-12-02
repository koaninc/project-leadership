| Name                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Project Definition - 1 | We have a few feature requests from customers through support channels, or a brand new idea, but little in the way of vetting or documentation beyond a bulleted list                                                                                                                                                                                                                                                                                                                      |
| Project Definition - 2 | We have insights from customers about what they value, and we've identified the problems that the feature solves for our users. We have meeting notes and bullet points about those insights, any draft milestones, and research spikes. We're iterating on those notes as we work toward a real plan.                                                                                                                                                                                     |
| Project Definition - 3 | We have a real plan, broken down into targets we can use to prioritize features and scope. Most targets are covered by user stories or other acceptance criteria that can be translated into a set of tickets later. Not all stories are fleshed out enough to allow anyone to pick it up without context, but most are understandable and intelligible                                                                                                                                    |
| Project Definition - 4 | We have a solid list of customer requirements, possibly even backed by metrics. We've probably passed some milestones, and we have our key deliverables (implementation, documentation, test plan, etc.) written down. All the work that we know about has a ticket and solid acceptance criteria. Tickets have links to documentation and design.                                                                                                                                         |
| Implementation - 1     | We have a rough idea of the work involved, and we might have surveyed the code to gauge level of effort. Informal, initial talks have begun between product and engineering. Priorities are still in the "unknown unknowns" stage. We have more questions than answers.                                                                                                                                                                                                                    |
| Implementation - 2     | We have a Jira epic, a project section in Notion, and a project channel in Slack. We might have had a project kickoff We have tickets for spikes and some broad sets of work. By now we should have a sense of the effort required for our targets. Those targets are at least roughly prioritized.                                                                                                                                                                                        |
| Implementation - 3     | Work has begun. Tickets are prioritized, and we're having sync ups at least every week to keep those priorities updated. By now we have a strong mental model of the work that needs to be done and there are more answers than questions in terms of how the features will be implemented and the level of effort involved.                                                                                                                                                               |
| Implementation - 4     | Code is in a launchable state. There maybe non-blocking tickets in the backlog still, but we've hit our milestones. We might have a follow on epic for post-launch work.                                                                                                                                                                                                                                                                                                                   |
| QA - 1                 | We have an idea of how things should work, and we've sketched out the basic constraints the feature needs to conform to                                                                                                                                                                                                                                                                                                                                                                    |
| QA - 2                 | We know enough about corner cases and possible boundary conditions to be able to hit most of those during testing. A mental checklist has started to form, but no formal test script yet.                                                                                                                                                                                                                                                                                                  |
| QA - 3                 | We have a more formal test script written down, specific enough to hit happy paths and corner cases, general enough to allow testers to try clicking around and find new and interesting bugs.                                                                                                                                                                                                                                                                                             |
| QA - 4                 | The test script is thorough enough to inspire confidence in Growth and Product that if the script is green, the project is shippable. We've used what we've learned from testing to implement more automated tests, both to keep confidence high in the future and to reduce QA burden.                                                                                                                                                                                                    |
| Release Plan - 1       | We know that there will be a launch. We probably have a good idea about feature flags we'll need. We might have an idea about what metrics we'll want to measure. Growth at least knows the project exists.                                                                                                                                                                                                                                                                                |
| Release Plan - 2       | We've had a project kickoff with growth present. They at least know the direction we're headed and enough about what's changing to be able to form opinions on the work that needs to be done on their side. Feature flags are in place, we're aware of any data migrations that will need to happen as the project goes on.                                                                                                                                                               |
| Release Plan - 3       | Growth is looped in on the status of the project, especially when designs or scope change. We're being proactive about helping with any KB articles, training materials, customer communications, and beta releases that will need to happen for launch. We probably have an idea of when we want to launch (+/- a few days). Work has settled enough that we know what failure states to be on the lookout for, data migrations to be run on launch.                                      |
| Release Plan - 4       | We have a thorough plan for the order of launch items: migrations, deploys, feature flag flips, etc. We know what error states to be on the look out for, how to do a manual check that everything is working in prod, and the on-call engineer knows enough about the project to feel comfortable responding to issues. Growth is comfortable with their preparations. At this point they probably even have the launch keys (metaphorically) in hand, to give the go when they're ready. |
| Post Launch - 1        | The project is launched, we're staying on top of issues as they come up, responding to any alerts or support queue items.                                                                                                                                                                                                                                                                                                                                                                  |
| Post Launch - 2        | Any support fires have settled. Bugs, follow-on epics are being prioritized and worked.                                                                                                                                                                                                                                                                                                                                                                                                    |
| Post Launch - 3        | Feature flags have been removed. The final determination on follow up work cutoff has been made. A retro has been planned.                                                                                                                                                                                                                                                                                                                                                                 |
| Post Launch - 4        | We've had a project retro and come away with learnings about what went well and what didn't go so well. Tickets after the cutoff have either been closed or deferred in priority. We're all done!                                                                                                                                                                                                                                                                                          |