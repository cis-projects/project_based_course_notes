# User Stories

## Representing Requirements the Agile Way

Product requirements are a way of defining a product's purpose,
features, functionality, and behaviour. It serves as a common place to
develop and guide understanding for the technical team (the developers)
and the client to help build the product.

These requirements are then represented as initiatives, epics, tasks,
and subtasks.

```{figure} resources/requirements.png
---
name: requirements
---
{cite:p}`AtlassianUserStories`
```

### Initiatives

In this subject you will only have one concurrent project, so the
project will count as the initiative. In a larger business where there
might be 2 or more applications under development simultaneously, there
would be 2 or more initiatives to cover each development.

### Epics

An epic refers to a large body of work that can be broken down into user
stories. Epics cluster user stories that have a similar higher-level
objective.

Epics are a useful way to organise and create a hierarchy out of the
work. The goal of breaking down epics into user stories is to reduce the
amount of work required for the project into small, incremental tasks so
that value is delivered throughout the life of the project through the
completion of these smaller tasks. For client-based projects, this means
that you can deliver incremental progress and demonstrate value much
easier than if the tasks remained large pieces of work.

Epics generally have a duration greater than one sprint. As the team
progresses through the project and develops a better understanding of
the project and its requirements, user stories will naturally be added
and removed from an epic. This is exactly what we want in an epic
following agile methodology: a flexible scope that changes based on
client feedback and team progress.

### User Stories

A user story is the smallest unit of work in the agile framework. A user
story may have one or many subtasks, but user stories are considered the
smallest piece of work that constitutes an end goal from a user's
perspective. A user story is an end goal, not a feature, expressed from
the perspective of the software user.

As discussed, user stories refer to a way of writing requirements from
the perspective of the end-user. By doing this, requirements follow the
agile methodology and are focused on the value delivered to the
end-user.

A key component of agile software development is putting people first,
and a user story puts end-users at the centre of the conversation. User
stories use non-technical language to provide context for the
development team. From reading a user story, the developer doing the
work required for that user story knows what they are building, why they
are building, for whom they are building it, and what value it creates.

#### How to Write a User Story

When first created, user stories consist of only one sentence in simple
language meant to outline the desired outcome - they don't go into
detail. User stories are expanded upon later and more details are added
to the user story, as agreed by the team, as work begins on the issue.

User stories are written to be non-technical following the format:

As a \[role\], I want to \[goal\], so that I can \[benefit\].

As an example, a company like Facebook might create a user story for new
functionality for their website with the following format:\
*As an individual user, I want to upload a photo to my profile picture,
so that people who search for my name can see a photo of me.*

#### Story Points: User Story Estimation Metric

As user stories reflect requirements that a developer must implement,
they should have a corresponding estimate for the effort required to
develop the functionality. This is necessary for time-boxed projects to
estimate the time to delivery for new functionality. However,
estimations in the Agile world are not based on time, but instead use
**story points**.

Story points estimate a task by considering the amount of work that
needs to be done, the difficulty of the task and any potential risk or
uncertainty involved. This is a better estimate as using the time taken
to complete a task can vary from developer to developer depending on
their level of experience.

Various scales can be used for story points. Two common methods used
are:

- Fibonacci sequence (1, 2, 3, 5, 8...)
- T-shirt sizing (XS, S, M, L, XL)

Regardless of which estimation technique your team chooses to use, you
should have the estimation technique documented in your team's document
repository.

#### Estimation Process

The estimation process occurs during [sprint
planning](#scrum-ceremonies). There are several ways to estimate the
story points of a user story - we will look at planning poker today:

1. All members are given cards that have a story point value. If using
    Fibonacci sequence, would have cards for 0, 1, 2, 3, 5, 8, 13...
2. Product owner reads out a user story and clarifies details if anyone
    has any questions.
3. Team discusses how they will handle the task and what skills are
    required to understand the approach.
4. Each member picks a card with a story point value they feel matches
    the user story just discussed, and places it face-down.
5. Once all team members have chosen a card, the team turns over all
    the cards and discusses.
6. Once the team reaches a consensus on the user story's estimate, the
    product owner notes down the value.
7. Repeat until all user stories product owner has prepared are
    complete.

The estimates should be added to your chosen task tracking tool.

:::{admonition} Extra Resources
:class: tip

| Link                                             | Description                            |
|--------------------------------------------------|----------------------------------------|
| [Planning Poker](https://www.planningpoker.com/) | A free tool that gamifies the process. |
:::

#### User Story Prioritisation

To deliver greater value to your client, you will want to invest your
efforts in tasks that are of importance first. The importance of tasks
is decided in discussions with the client (it **is not** up to the
development team to decide priority). One method of displaying the
priority of a task is the MoSCoW task prioritisation method. Priorities
are broken down into different levels of priority:

- *Must have:* features that must be delivered or the software will not
    create the expected value for the client;
- *Should have:* features that have significant value to the client and
    should be delivered, but not considered crucial;
- *Could have:* features that the client considers nice to have but will
    not have a material impact to value, if not delivered; and
- *Won't have:* out-of-scope features; useful as next steps for your
    project as potential improvements for future releases.

:::{admonition} Extra Resources
:class: tip

| Link                                                                                                         | Description                                      |
|--------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| [MoSCoW method](https://en.wikipedia.org/wiki/MoSCoW_method)                                                 | Further discussion of the MoSCoW method.         |
| [Scrum Guide](https://www.atlassian.com/agile/scrum)                                                         | Comprehensive Scrum guide.                       |
| [Sprint planning meeting](https://www.mountaingoatsoftware.com/agile/scrum/meetings/sprint-planning-meeting) | Details on running your sprint planning meeting. |
:::

Once written, these stories should be documented centrally in the team's
document repository:

```{figure} resources/confluence.png
---
name: confluence
---
```

#### User Story Mapping

User story maps are intended to spark collaboration across agile team members, while providing them 
with the bigger picture of how the backlog stories fit together into a larger vision of the product your team 
is building. In agile team, product work exists as discrete backlog tasks and so visual tools are extremely helpful
in communicating deadlines, goals, and the final product to developers in the team, as well as the client.
This guarantees everyone is working towards the same ultimate goal.

Once created, the Product Owner is responsible for driving the creation of the user story map. However, it is
a group exercise and should be done by the entire team. Once created, it should then be communicated to the client.

##### When to Create User Story Maps

The user story map can be created before or after user story prioritisation. Sometimes it can help to visualise
user stories when prioritising them.

This is an example of a user story map:

```{figure} resources/user_story_map
---
name: user-story-map
---
```

:::{admonition} Extra Resources
:class: tip

To aid you in creating a user story map, you can make use of templates.

- [Miro template](https://miro.com/templates/user-story-map/) 
- [LucidChart template](https://www.lucidchart.com/blog/how-to-create-a-user-story-map)
- [A Complete Beginner's Guide to Usability Testing](https://maze.co/guides/usability-testing/)
:::

```{admonition} What's Next
Now that your team has elicited the requirements - it is time to start designing the application.
```