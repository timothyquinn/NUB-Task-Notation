# NUB Task Notation

## Introduction

Task management is a critical part of any complex process. When projects go bad, poor task management is often to blame; while no one might remember exactly where a project slipped off the mainline, the cascading failure of incomplete or unacknowledged tasks is an unmistakable sign to stakeholders that things have somehow gone irrevocably wrong.

The problem with most task management systems is that they're easily derailed by unexpected urgencies: misprioritization, politicization, extraneous detail, and things unquantifiable. It's little wonder so many project managers fall backward into the arms of Stephen Covey at the first hint of trouble.

To counteract the pressure to prioritize by urgency, I like to use a lightweight form of structured task notation that I call NUB (non-urgency based) notation. It focuses on capturing a minimum of quantifiable data to assist in the rapid scanning and sorting of tasks. The key word here is "quantifiable" -- if it can't be quantified, it shouldn't influence prioritization.

In my experience, besieged project managers too often prioritize based on whether something is easy ("we'll just knock it off and move onto the next thing"), difficult ("after we crack this one, it's smooth sailing"), politically expedient ("if we can nail this, it'll get executive management off our backs") or a source of irritation ("God, I'm tired of hearing about this; just do it and let's move on"), none of which might be appropriate criteria for assigning priority.

NUB is also completely tool-agnostic; it works as well in a text file as in a more robust project management platform.

## How It Works

In NUB notation, every task is expressed in four parts:

1. stoplights (optional)
2. description
3. status (optional)
4. limiters (optional)

Structurally, this ends up looking like:

<blockquote>stoplights | description | status | limiters</blockquote>

Here's how a relatively simple task might be expressed in NUB notation:

<blockquote>Build fence. -$500 -16h</blockquote>

In other words, we need to build a fence which will cost $500 and require two workdays of labor. Now here's a more complex task:

<blockquote>! ? #8 Normalize production database (25%) 31-Dec-10 +$1000/w -16h &lt;7</blockquote>

This time, we need to continue work on a database (we're a quarter of the way there, with an end of year deadline), which will ultimately save us $1,000 per week. Unfortunately, this task is dependent on another task; we also require input from someone or something else. This particular task is mandatory.

Note that in each example some optional punctuation has been added for visual clarity. Periods and colons and brackets and pipes are all acceptable delimiters that don't impede NUB syntax.

## Stoplights

Stoplights precede tasks and indicate critical meta information about the task. These are the stoplights I use:

| Notation | Description                                                                                                                                                                          |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| !        | The task cannot NOT happen. Declaring a task mandatory must be an explicit declaration, rather than an implicit assumption, which prevents overestimation of criticality.            |
| ?        | The task is waiting on someone or something else. While work on this task might not yet be stalled, it cannot be completed.                                                          |
| ~        | The task requires more thought, and might not even happen. Allowing for this stoplight encourages early notation and prioritization of tasks.                                                                   |
| #        | A number sign denotes a unique identifier or ID for this task which can be referenced either elsewhere in the task list (see predecessor limiter below) or outside of the task list. |

## Description

The task description should be as brief yet precise as possible. Ideally, it should be no longer than 100 characters. The shorter the description, the easier the task list will be to scan. A lengthy task description is a hint that you may not have made your tasks atomic enough.

## Status

If a task has begun but not yet been completed, the approximate percentage of completion should be shown. I tend toward a spectrum of 25%, 50% and 75%. If a task has not yet begun, I leave the percentage indicator out rather than adding the clutter of "0%". Likewise, if a task is complete, and my particular task management tool permits it, I might apply a strikethrough rather than denoting it as "100%".

## Limiters

Limiters are optional but important attributes of a task which allow for efficient prioritization; this is the heart of the NUB system. I use three types of limiter: deadline limiters, value limiters and reference limiters.

#### Deadline Limiter

| Notation  | Description                                                                                                                                                                                                             |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 15&#8209;Jul&#8209;10 | The deadline limiter is simply a date, provided with the least practical amount of granularity (e.g. if a task is due by a specify day, specify so, but if it's due simply by the end of the month, leave off the day). |

#### Value Limiters

| Notation | Description                                                                                                                                                                             |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| +$100/w  | The plus or minus prefix denotes whether the task represents a gain or loss. The amount can be expressed in dollars, dollars per unit, hours or hours per unit.                         |
| q        | Because there are tasks whose value cannot be expressed in money or time, a "q" indicates a quality of life gain.                                                                       |
| p        | If a task improves the quality of life of others, there's a separate limiter for that because it's often preferable to help multiple other people rather than just ourselves.           |
| i        | Sometimes tasks are just plain interesting, and this limiter lets you factor that into prioritization, although use it judiciously to avoid negating the whole purpose of NUB notation. |

#### Reference Limiters

| Notation | Description                                                                                                                                                                                                                                    |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &lt;1    | The predecessor limiter points at another task which has the specified indicator or ID, denoting that this task is dependent on that predecessor task. If you've ever used Microsoft Project, this will be a familiar element of notation.     |
| &gt; 1   | Similarly, the successor limiter points at a task which must happen after the current task. While less frequently used, a successor is important for identifying a follow-up task without which the effort of the predecessor would be wasted. |

## The Anatomy of a Task

Using the above, we can now express the abstract structure of a task more completely as:

<blockquote>(mandatory) (waiting) (vague) (ID) description (status) (+-money/unit) (+-time/unit) (quality of life) (philanthropy) (interest) (predecessor)</blockquote>

Although in this form the structure appears complex, it will become second nature after you've done it a few times, and it encourages creating tasks as early as possible and then refining them over time.

Like many project managers, I often apply a higher level of structure by grouping tasks into discrete lists. Lists can be assembled based on category, location, business unit, project, or any other form of aggregation desired -- but shouldn't be structured around attributes which exist down at the task level (e.g. "things to do this month").

As with any other platform- or industry-agnostic methodology, the benefits of NUB task notation are limited by the uniqueness of the environment. I wouldn't, for instance, want to use it to land 747s. (I have a $20 Amazon gift certificate for the first air traffic controller to demonstrate its applicability in the tower. But I will never, ever fly in or out of your city.)

For project managers with a broad selection of problem-sets, NUB task notation offers a means of quantifying the relative value of disparate tasks without having to resort to life balance worksheets and urgency matrices.
