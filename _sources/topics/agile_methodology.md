# Agile Methodology

In this subject, you will form teams and operate according to the agile
methodology. This chapter will help familiarise students with the agile
framework for project management and software development.

## Software Development Lifecycles (SDLCs)

Software development lifecycles (SDLCs) refer to a process for planning,
developing, testing, and deploying a software system. There are two main
types of SDLCs: formal and Agile.

| SDLC                                                                                                                                                | Type   |
|-----------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| [Waterfall](https://www.workfront.com/project-management/methodologies/waterfall)                                                                   | Formal |
| [Incremental](https://www.guru99.com/what-is-incremental-model-in-sdlc-advantages-disadvantages.html)                                               | Formal |
| [V-Model](https://www.tutorialspoint.com/sdlc/sdlc_v_model.htm#:~:text=The%20V%2Dmodel%20is%20an,for%20each%20corresponding%20development%20stage.) | Formal |
| [Kanban](https://www.atlassian.com/agile/kanban)                                                                                                    | Agile  |
| [Scrum](#scrum)                                                                                                                                     | Agile  |
| [Extreme Programming](http://www.extremeprogramming.org/)                                                                                           | Agile  |

```{attention}
You do not need to learn these SDLC methodologies - you will only make
use of Scrum. Links have been provided to the others in case you want to
learn more.
```

Agile was formed after teams were frustrated by the rigidity of formal
methods, and their inability to adapt to change easily without exceeding
cost and time constraints. For example, in Waterfall, teams complete all
the requirements work before moving to design and subsequently
development. If the requirements changed during the development phase,
the team would need to start over, costing significant time and money,
something that is not feasible in many situations.

## Agile Manifesto

Agile, much like its name, focuses on being able to adapt to change
rapidly through developing software incrementally. The agile manifesto
explains the core values and principles that are the basis of Agile:

- Individuals and interactions over processes and tools.
- Working software over comprehensive documentation.
- Customer collaboration over contract negotiation.
- Responding to change over following a plan.

## Scrum Framework

For this subject, you will work in agile teams following the Scrum
framework.

### What is Scrum?

Scrum is a framework used to implement an Agile mindset. It focuses on ensuring teams 
work together, embodying the values from the agile manifesto. Scrum is based on teams
working iteratively, in time-boxed sprints (typically 2-4 weeks), with a predetermined
set of tasks. During sprint planning, the team decides which tasks to work on during 
the upcoming sprint, to ensure they maximise value to their client. If requirements 
change, the teams can easily adapt as sprints are short, and the subsequent sprints 
planning can re-prioritise the changed requirements.

### Sprints

Sprints are a short time-boxed period in which a scrum team endeavours to complete a set 
amount of work. The duration of sprints can be determined by teams, but typically duration 
is between 2-4 weeks. As sprints have several [ceremonies](#scrum-ceremonies) that must be 
completed, teams should determine what works best for them.

### Scrum Roles

Scrum teams have three key roles: product owner, scrum master, and development team members

#### Product Owner

The product owner ensures the team delivers the most value to the client. They have a strong 
understanding of the project, which is used to prioritise user stories in upcoming sprints.

```{figure} resources/product_owner.png
---
name: product_owner
---
{cite:p}`AtlassianScrumRoles`
```

Product owners are required to maintain close ties with the client and
seek their validation and input. They are also the conduit for
communication with the client - all emails, meeting invites, etc. from
the team should be guided through the product owners to reach the
client.

#### Scrum Master

The scrum master is responsible for ensuring that the Scrum framework is
followed. Unlike a manager, the scrum master coaches the team rather
than leading them - scrum masters are **servant leaders**. They have no
authority to act as a manager in the traditional sense of being able to
allocate tasks. Instead, it is their responsibility to ensure that they
oversee how the project is tracking, and work to unblock developers to
continue meeting objectives.

```{figure} resources/scrum_master.png
---
name: scrum_master
---
{cite:p}`AtlassianScrumRoles`
```

#### Development Team

The development team refers to the team members who are implementing the
system. In your project, **all team members** must be a part of the
development team (including the Scrum master and product owner).

```{figure} resources/development_team.png
---
name: development_team
---
{cite:p}`AtlassianScrumRoles`
```

There are several other roles that teams may benefit from using. Please
note that these are not Scrum roles:

- Quality Assurance/Testing lead: Monitors testing other initiatives
    to ensure the system is built to a high quality. Often, they are
    responsible for creating a testing plan and ensuring the testing
    objectives are met
- Frontend lead: Oversees the frontend development of the project and
    is typically responsible for setting up and configuring the frontend
    codebase. Additionally, plays a key role in any decision-making
    about frontend architecture.
- Backend lead: Oversees the backend development of the project and is
    typically responsible for setting up and configuring the backend
    codebase. Additionally, plays a key role in any decision-making
    about backend architecture.

### Scrum Artefacts

Managing work in a scrum team involves the use of two artefacts:

- Product backlog: Primary list of work that needs to be done which is
    maintained by the product owner.
- Sprint backlog: The list of work that needs to be completed in the
    current sprint.

### Scrum Ceremonies

Scrum ceremonies refer to a set of meetings that are used to manage the
development of a project. These ceremonies are important in facilitating
team communication and reducing the feedback loop. The table below shows
the key details of the Scrum ceremonies.

```{figure} resources/scrum_ceremonies.svg
---
name: scrum_ceremonies
---
{cite:p}`AtlassianSprints`
```

| Ceremony             | When                 | Who                             | Preparation                                             | Duration                                                              | Process                                                                                                                                                                                                                                                                                              | Outcome                                                         |
|----------------------|----------------------|---------------------------------|---------------------------------------------------------|-----------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| Sprint planning      | Start of each sprint | Development team                | Product owner should have a prioritised product backlog | 1 hour per week of sprint. E.g., 2-week sprints have a 2-hour session | 1. Product owner presents product backlog<br/>2. Discussions with team about high priority features, which are then broken down into smaller tasks<br/>3. Estimate the effort required for tasks.<br/>4. Team agrees on the tasks set out for the sprint, and tasks are moved to the sprint backlog. | Populated sprint backlog in the team’s task tracking tool.      |
| Stand-up             | Weekly               | Development team and supervisor | None                                                    | <15 minutes                                                           | Each team member says what they have done, what they will be working on and any blockers.                                                                                                                                                                                                            |                                                                 |
| Sprint review        | End of each sprint   | Development team and client     | None                                                    | 1 hour                                                                | Product owner presents the work completed in previous sprint and seeks feedback.                                                                                                                                                                                                                     | Populated sprint review page in the team’s document repository. |
| Sprint retrospective | End of each sprint   | Development team                | None                                                    | 20 mins                                                               | Scrum master facilitates session to establish what the team thought went well, what did not work and what actions the team could do to improve.                                                                                                                                                      | Populated retrospective page in the team’s document repository. |

We have outlined how the scrum framework can assist teams in following
the agile manifesto. Now we will discuss how development requirements
can be represented.

