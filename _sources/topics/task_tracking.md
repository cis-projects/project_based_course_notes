# Task Tracking

Task tracking, also known as task management, is far more than a simple
to-do list. It means tracking tasks from beginning to end, delegating
subtasks to teammates, and setting deadlines to make sure projects are
done on time.

There are several benefits to using task tracking software:

1.  Centralise tasks, increasing team visibility of task progress.
2.  Prioritise tasks as a team.
3.  Improve collaboration, allowing any team member to work across any
    task.
4.  Track team progress.

As discussed in agile methodology, task tracking is an important part of
representing requirements in an agile way.

In this subject, you are required to make use of a task tracking tool.
As a team, you will need to agree on a tool to use. There are a several
tools to choose from (this list is not exhaustive):

| Name                                                                                                                                            | Description                                                                                                   |
|-------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| [Jira](https://www.atlassian.com/software/jira)                                                                                                 | The industry-leading task tracking software. A good tool to learn if you want to enter the software industry. |
| [Trello](https://trello.com/en)                                                                                                                 | A very popular tool. Less feature-rich than Jira but quicker and easier to set up.                            |
| [GitHub Project Board](https://docs.github.com/en/issues/organizing-your-work-with-project-boards/managing-project-boards/about-project-boards) | New, compared to the other tools. Easy to set up as it comes with your repository but lacking many features.  |
| [asana](https://asana.com/?noredirect)                                                                                                          | Like Trello, but a more mobile-friendly application.                                                          |
| [Linear](https://linear.app/)                                                                                                                   | Much like asana.                                                                                              |

## Setting Up Your Team's Task Management

Once your team has decided on a tool to use, the next step is to
populate it.

Regardless of your choice of task tracking tools, all require similar
set-ups and the same level of detail.

### Requirements

As discussed in agile methodology, all requirements of the system must
be translated into epics, user stories, subtasks, etc. in your chosen
task tracking tool.

```{note}
Please see the chapter on requirements elicitation to understand how to elicit requirements from a client.
```

### Backlog

The backlog contains all pieces of work for the semester. Any work
completed by the development team should have an associated task in the
tracking tool. At the beginning of the semester, the Product Owner
should populate the backlog with all requirements received from the
initial client meeting.

The backlog will look like this once populated:

```{figure} resources/backlog.png
---
name: backlog
---
```

Once the backlog is populated, the Product Owner and client should
jointly determine the priority of each task. The priorities of tasks
help the development team determine what task to pick up next. It is
expected the development team will work on high priority tasks first
before moving on to lower priority tasks.

By default, all tasks are created with medium priority:

```{figure} resources/priority_1.png
---
name: priority_1
---
```

However, the priority can be changed to any of the below by editing the
task:

```{figure} resources/priority_2.png
---
name: priority_2
---
```

The priority of all user stories in the backlog should reflect the
prioritisation given by the client (please see the chapter on
requirements elicitation).

Over the course of the year, the development team then uses the backlog
as its single source of truth for work, and as the project progresses,
work should be added and removed from the backlog.

### Workflow

As a team, you should have a defined flow that all work must follow. A
workflow covers all steps that must be done for work to be considered
"ready for development" and then subsequently "ready for review" and
then "complete". Creating a workflow ensures that all team members
understand and follow the same process, thus ensuring a high quality of
work completed with far less oversight necessary. As workload increases,
having a defined workflow ensures that the team's processes are
scalable.

#### Defining a Workflow

When defining a workflow, it can be tempting to make it complicated -
avoid this temptation. Most important when creating a workflow is that
it is understood by the team and highly repeatable.

1.  All tasks that are created are first created in the backlog. Tasks
    that are selected for development are then moved into the upcoming
    sprint.

2.  Once a developer commences work on an issue, the issue is moved to
    the next status.

3.  Once development work has finished, the task should be moved to the
    next status for review by teammate(s). The task must be reviewed by
    another team member (not the one who completed the work).

4.  If the review passes successfully (no bugs are found), the task
    should be moved to a completed status. If it fails review, it should
    be moved backwards to the prior status so the developer can address
    the bugs found.

#### An Example Workflow

The following is just one example of a workflow, and you are welcome to
define your own that best suits your team - this is by no means the best
workflow.

```{figure} resources/workflow.png
---
name: workflow
---
{cite:p}`AtlassianWorkflow`
```

Status: Open

This is the status that is assigned to all newly created tasks in the
current sprint. For a task to be able to be moved from status open to in
progress, it must have a definition of ready (DoR). A task with a
definition of ready means it can be picked up by any developer and that
developer can begin work immediately.

It is up to your team to decide on the definition of ready, however, a
few examples of what might be required for a task to be considered ready
for development can include (but is not limited to) the following:

1.  The story should be written exactly in the 'user story' format and
    added to the User Stories page in the document repository. If it is
    not a user story, then it does not need to follow this format nor be
    added to the document repository.
2.  The story should be created in the appropriate epic in the task
    tracking tool and added to the backlog.
3.  It must have acceptance criteria written and added to the Acceptance
    Criteria page in the team's document repository.
4.  The acceptance criteria must be understood and agreed to by the team
    *(we will discuss the acceptance criteria in status: in progress
    below)*.
5.  The team must estimate the story during a sprint planning meeting.
6.  The task must have an assignee.
7.  The task must have a due date.

The following is an example of a well populated user story in Jira. It
has a title in the form of a user story, acceptance criteria, priority,
and, as it is still open, it is correctly still in the backlog.

```{figure} resources/story_open.png
---
name: story_open
---
```

Status: In Progress

This status indicates that development work has commenced. For a task to
be properly in progress, it must abide by the following:

1.  It should have a single assignee. If more than one developer is
    completing the work, then the task is too big, and should be broken
    down into smaller, iterative tasks.
2.  It should have an estimation of story points.
3.  It should have a deadline when development is expected to be
    completed.
4.  It should be contained in a sprint.

The following is an example of a well populated user story in Jira. It
has a title in the form of a user story, acceptance criteria, priority,
assignee, due date, and, as the story is in progress, it is assigned to
the current sprint.

```{figure} resources/story_in_progress.png
---
name: story_in_progress
---
```

Status: In Review

There are several methods that can be used to review work done
by team members.

1.  Manual review: reviewers pick up tasks that have status: in review
    and review the code manually. This involves reading the code
    line-by-line, running tests, etc.
2.  Peer programming: Two or more developers work together on a task,
    then one commits the code, and the other developers approve the code
    as reviewed. This is by far the fastest way to review work and
    recommended.
3.  Walk-through: As a substitute for the regular review process, a
    developer can walk through their task with other teammates as part
    of a collaborative process where teammates can ask questions. The
    whole team is not required to be present - your team should decide
    on a quorum required to receive approval.

The following is an example of a well populated user story in Jira. It
has a title in the form of a user story, acceptance criteria, priority,
assignee, reviewer, due date, and, as the story is in review, it is
assigned to the current sprint.

```{figure} resources/story_in_review.png
---
name: story_in_review
---
```

Status: Done

As well as a definition of ready, the team should have a definition of
done (DoD). The definition of done stipulates what is required before a
task can be moved to status: done.

It is up to your team to decide on the definition of done, however, a
few examples of what might be required for a task to be considered done
can include (but is not limited to) the following:

1.  Code is peer-reviewed.
2.  Code is commented.
3.  Code is checked in to trunk.
4.  Code is deployed to test environment.
5.  Code passes all testing listed in the team's document repository.
6.  End-user documentation is updated (for example, how-to guides).
7.  Code is live on the production server.

The following is an example of a well populated user story in Jira. It
has a title in the form of a user story, acceptance criteria, priority,
assignee, reviewer, due date, and, as the story is complete, it is
assigned to the current sprint. It also has comments from the reviewer
showing the task was reviewed with no issues found.

```{figure} resources/story_done.png
---
name: story_done
---
```

### Good Hygiene

Task tracking tools are common spaces shared by the entire team. They
are where teammates go to understand the status of an issue or what to
work on next, supervisors use it to monitor team progress, product
owners use it to communicate progress to the client, etc. It is
therefore imperative that they are kept in good shape:

-   Make sure that issues are updated frequently as coding continues.
-   Add comments to describe the status of an issue as you progress it.
-   Update the deadline if it is pushed back- or forward.
-   Move the issue between statuses as necessary.

:::{admonition} Extra Resources
:class: tip
| Link                                                                                                 | Description                                                                               |
|------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| [Jira best practices](https://www.atlassian.com/software/jira/guides/getting-started/best-practices) | Best practices to follow throughout the semester. It covers creating issues, sprint, etc. |
| [Jira scrum board template](https://www.atlassian.com/software/jira/templates/scrum)                 | A template that might inspire you.                                                        |
| [Trello board template](https://trello.com/templates/engineering/agile-sprint-board-ZqN99gGN)        | A template that might inspire you.                                                        |
:::
