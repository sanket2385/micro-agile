Micro Agile
===========

Agile product development for small teams.

## Sprints

Sprints are usually 1-2 weeks in length.

### Sprint Planning Meeting

A 1-2 hour meeting at the start of the sprint. Two, sometimes three parts:

1. Stakeholders & team - discuss the priorities for the sprint
2. Team - discuss how they will go about tasks.
3. Product manager & stakeholders - confirm priorities with stakeholders after team estimations and discussion. This can be a quick 5 minute check-in.

__Estimates:__

Teams can provide estimates to tasks if they wish. Estimates can help to measure a team's velocity (user story points are best for this) and can help with planning and communicating expectations to stakeholders (sometimes time based estimates are useful here).

__Goals & Milestones:__

1. Sprint-goals: span one or multiple sprints (e.g )
2. Team goals: specific goals for team members (e.g learn React.js)
3. Milestones: more major and often time-bound, can tie-in to larger business milestones (e.g launch new homepage and PR campaign)

### Sprint Demo Meeting

The development team present and discuss the latest work to stakeholders and the wider team and can discuss upcoming work. Also a good time for a team retrospective.

## Daily Scrums

Morning time team get-together, 10-20 mins. Say 1) what you did yesterday 2) what you're planning today 3) if anything is blocking you. Discuss outstanding work and how you can help each other, keep it high level. If there are any points of greater discussion, take them outside the meeting.

## Tickets

__Story:__ an outline of some functionality without too much specific detail.
See [Gov.uk/user-stores](https://www.gov.uk/service-manual/agile-delivery/writing-user-stories). Most tickets should ideally be stories. If a story is too large, break it down.

__Task:__ a discrete and already specified task

__Bug:__ something broken with an already deployed

__Design & Research:__ a design task, or a research task.

__Meta Task:__ a list of small tasks (e.g 'high priority homepage issues')

__Epic:__ either 1) a new product feature (e.g 'messaging system v1', blog v3) or 2) a group of general ongoing updates (e.g 'infrastructure', 'frontend', 'login system')

### New Tickets

* Highest priority tickets -> add to this sprint and start ASAP
* High priority tickets -> next sprint
* All other -> backlogs

## Ticket Workflow

__Scrum board columns__

* __Todo:__ to be started
* __In progress:__ started. After finishing -> update ticket with testing info, add pull request when a ticket is complete
* __Ready for testing or deployment__ Someone tests, code reviews, discusses, more work is usually done, and then the developer who worked on the ticket deploys
* __Deployed or complete__

__Typical story workflow:__

1. Create ticket
2. Optional: Research stage
3. Specify acceptance criteria
4. Complete initial Development against acceptance criteria
5. Create / update existing pull request
6. Update ticket with how to test & comments
7. Code review
8. Optional: Repeat 4-7
9. Merge into master & deploy

__Typical design workflow:__

For new products, features or updates to existing areas:

1. Create design ticket
2. Do research
3. Develop prototypes
4. Optional: UX testing (we sometimes leave this until after MVP has been built)
5. Other team members review
6. Move to __deployed__ if integration is complete
7. Alternatively, create new __story ticket(s)__ for other team members to start with development (e.g MVP development for new features or integration for updates)
8. Prototypes are used as a point of reference, rather than for pixel-perfect implementation

## Backlogs

1. __Current sprint:__ all tasks currently in development
2. __Sprint backlog:__ ready for development soon(ish)
3. __Backlog:__ ideas, will need more specification and discussion before development

## Team Roles

* Developer: executes the development tasks
* Product Manager: guides the team, sets challenges for the team, manages meetings and backlogs
* Stakeholder: defines the higher-level business objectives

## Code Management

* All code should be stored in a Git repo which should be for code only (no database dumps or static files).
* The [git-flow branching model](http://nvie.com/posts/a-successful-git-branching-model/) is good for managing new feature development. The [git-flow Git extension](https://github.com/nvie/gitflow) is useful for efficient development using git-flow.
* __Release branches and versions are not used__ in continuous product development.
* Feature branches should be named after their ticket name / number, e.g ```git checkout -b feature/PROJ-123```
* Git commits should contain one specific thing, rather than several features or unrelated tidy-ups in one commit. This makes commits and PRs simpler for others to review.

## Product Roadmaps

Group product feature epics into 'short-term', 'medium-term' and 'future'.

TODO: Provide visual example.

## Notes

TODO: Incorporate these notes into this guide.

* Testing: automated tests, manual tests, testing procedure before deploying
* Continuous integration and dev->stage->production workflow
* Research & ideation: use Google Docs to list future ideas, always remember to think about the value generated for the user
* Use brainstorming sessions for product development plans and ideas
* UX & design: lean user testing & tools to help, design & architecture spikes
* Coding standards: use linters and code sniffers aggressively and document coding standards
* Feedback: group into: business value / user value + critical / future

## Useful Reading

* [Manifesto for Agile Software Development](http://agilemanifesto.org/)
