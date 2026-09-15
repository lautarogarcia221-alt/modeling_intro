# Modeling Intro

Welcome to the first coding repository for CMSE 802.

At first glance, this repository appears to be about drawing a colorful triangle. In practice, it is about something more important: **how research software evolves**.

![Example Barycentric Triangle](./Example.png)


The triangle gives us a small visual example we can understand completely. Because the example is simple, we can focus on software design instead of getting lost in domain details.

Across three notebooks, you will start with a working script and gradually transform it into a reusable software tool.

## Recommended: Fork This Repository

If you have a GitHub account, consider creating a fork of this repository before starting.

Working in your own fork allows you to:

- save your work to GitHub
- keep your edits after the course
- build a portfolio of examples and projects

You are welcome to work directly from a local clone, but many students find that maintaining a personal fork is a useful habit for long-term project development.

## A model of models

Throughout this course, we will discuss three common components found in computational models:

- Analytical
- Physical
- Data-Driven

These are not separate categories. Most real research projects contain a mixture of all three.

We can represent that idea mathematically:

$$A + P + D = 1$$

where:

$A =$ Analytical contribution    
$P =$ Physical contribution  
$D =$ Data-Driven contribution   

and all three values are nonnegative.

## Why a Triangle?

A triangle provides a convenient way to visualize mixtures of three components.

In this repository we use color as a visual metaphor:

* Red   -> Analytical
* Green -> Physical
* Blue  -> Data-Driven

Every location inside the triangle represents a different component mixture.

We will introduce many modeling methods later in the semester. The triangle modle helps us discuss where methods and projects may fall in that space.


## Why Start Here?

Many students enter graduate school with programming experience, but less experience treating software as an evolving artifact.

A common pattern in research looks something like:

    Idea
      ↓
    Quick Script
      ↓
    Working Script
      ↓
    Reusable Functions
      ↓
    Library
      ↓
    Research Tool

This repository follows that progression.

Rather than building a large project from scratch, we will use a small example to practice the habits that support high-quality research software.

## Scientific Software Engineering Principles

Throughout CMSE 802 we will revisit five qualities of scientific software:

- Safe
- Portable
- Reproducible
- Robust
- Literate

You do not need to master all of these ideas immediately.

Instead, use them as a lens when evaluating software and making design decisions.

When you modify code, ask:

- Does this make the code safer?
- Does this make the code easier to move to another machine?
- Does this make results easier to reproduce?
- Does this make the software more robust?
- Does this make the code easier for another person to understand?

The exercises in this repository make those questions concrete.

## Learning Goals

By the end of this repository, you should be able to:

- run and inspect existing code
- make small improvements without breaking functionality
- replace magic numbers with meaningful variables
- refactor a script into reusable functions
- design useful function arguments and defaults
- move functionality into a Python module
- import and reuse code from multiple notebooks
- use Git to track software evolution
- improve code quality using automated tools
- explain how software engineering supports scientific research

## Repository Structure

## Notebook 01: Model Triangle

Start with a working script that generates a barycentric RGB triangle. You will explore the code, make modifications, and practice improving an existing program.

## Notebook 02: Building a Library

Refactor the original script into a reusable Python module.

Topics include functions, imports, code reuse, and organization.

## Notebook 03: Improving Software

Introduce tools that help improve software quality.

Topics include Git, Ruff, formatting, and software improvement workflows.

## Suggested Learning Flow

Work through the notebooks in order.

1. Run and modify a working script.
2. Transform the script into a reusable library.
3. Improve the library using software engineering tools.
4. Use the same habits when moving into more physical and data-driven modeling repositories.

Each notebook builds on the work completed in the previous notebook.

This repository still connects directly to the later course sequence:

- it emphasizes notebook-to-script transitions,
- it reinforces reusable function design,
- it introduces linting and quality checks,
- it prepares students for the more physical and data-driven repositories that follow.

## Optional Quick Start

An `environment.yml` file is included for a reproducible setup. The environment contains Python, NumPy, Matplotlib, JupyterLab, and Ruff.

If your local setup already works, using this environment is optional. Otherwise, create it with:

```bash
conda env create --prefix=./.envs --file environment.yml
```

Activate it with:

```bash
conda activate ./.envs
```

If you need Ruff only, you can also install it directly:

```bash
pip install ruff
```

## Notes for Students

As you work through the repository:

- Keep changes small.
- Test frequently.
- Run your code after each modification.
- Use Git commits to capture important milestones.
- Focus on understanding why a change is useful, not just how to make it.
- Discuss design decisions with your teammates.

Most importantly:

- Start with code that works.
- Improve it in small steps.
- Preserve behavior while improving readability, reuse, and portability.

# Help Improve this repository

This repository is part of an ongoing open educational resource project.

If you find:

- a typo
- a bug
- an error in the instructions
- a confusing explanation
- a missing step
- an idea for improvement

please consider opening a GitHub Issue.

Professional software projects improve through feedback, and submitting issues is an important software engineering skill.

You do not need to know how to fix a problem in order to report it.

In fact, identifying and clearly describing problems is often one of the most valuable contributions a user can make.

Throughout the semester, feel free to submit issues to any course repository.

Your feedback helps improve the materials for future students.