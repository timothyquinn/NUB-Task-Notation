# NUB Task Notation

## Introduction

Task management is a critical part of any complex process. When projects go bad, poor task management is often to blame; while no one might remember exactly where a project slipped off the mainline, the cascading failure of incomplete or unacknowledged tasks is an unmistakable sign to stakeholders that things have somehow gone irrevocably wrong.

The problem with most task management systems is that they're easily derailed by unexpected urgencies: misprioritization, politicization, extraneous detail, and things unquantifiable. It's little wonder so many project managers fall backward into the arms of Stephen Covey at the first hint of trouble.

To counteract the pressure to prioritize by urgency, I like to use a lightweight form of structured task notation that I call NUB (Non-Urgency Based) notation. It focuses on capturing a minimum of quantifiable data to assist in the rapid scanning and sorting of tasks. The key word here is "quantifiable" -- if it can't be quantified, it shouldn't influence prioritization.

In my experience, besieged project managers too often prioritize based on whether something is easy ("we'll just knock it off and move onto the next thing"), difficult ("after we crack this one, it's smooth sailing"), politically expedient ("if we can nail this, it'll get executive management off our backs") or a source of irritation ("God, I'm tired of hearing about this; just do it and let's move on"), none of which might be appropriate criteria for assigning priority.

NUB is also completely tool-agnostic; it works as well in a text file as in a more robust project management platform. (Pro tip: it works particularly well in free, markdown-based Obsidian.)

Please take a moment to review How It Works below before clicking through to individual versions.

## Versions

Versions are incremental, and later versions replace earlier versions. In general, an integer increment is not backwards-compatible, while a decimal increment is.

- [2.0](versions/1-0.md) (latest)
- [1.0](versions/1-0.md)

## How It Works

In NUB notation, every task is expressed in four parts:

1. stoplights (optional)
2. description
3. attributes (optional)

Structurally, this ends up looking like:

<blockquote>stoplights | description | attributes</blockquote>

Here's how a relatively simple task might be expressed in NUB notation:

<blockquote>Build fence | -$500 -16h</blockquote>

In other words, we need to build a fence which will cost $500 and require two workdays of labor. Now here's a more complex task:

<blockquote>! ? Normalize production database | 25% 31-Dec-10 +$1000/w -16h #8 &lt;7</blockquote>

This time, we need to continue work on a database (we're a quarter of the way there, with an end of year deadline), which will ultimately save us $1,000 per week. Unfortunately, this task is dependent on another task; we also require input from someone or something else. This particular task is mandatory. We now have a lot of evaluative prioritization data packed into relatively compressed space.

Note that in each example a pipe (|) has been added for visual clarity. Segment punctuation is of course purely optional; periods and colons and brackets and pipes are all acceptable delimiters that don't impede NUB syntax.

Although in this form the structure appears complex, it will become second nature after you've done it a few times, and it encourages creating tasks as early as possible and then refining them over time.

Like many project managers, I often apply a higher level of structure by grouping tasks into discrete lists. Lists can be assembled based on category, location, business unit, project, or any other form of aggregation desired -- but shouldn't be structured around attributes which exist down at the attribute level (e.g. "things to do this month").

As with any other platform- or industry-agnostic methodology, the benefits of NUB task notation are limited by the uniqueness of the environment. I wouldn't, for instance, want to use it to land 747s. (I have a $20 Amazon gift certificate for the first air traffic controller to demonstrate its applicability in the tower. But I will never, ever fly in or out of your city.)

For project managers with a broad selection of problem-sets, NUB task notation offers a means of quantifying the relative value of disparate tasks without having to resort to life balance worksheets and urgency matrices.
