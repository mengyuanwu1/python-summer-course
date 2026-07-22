# Homework Guidance: How to Get Unstuck

Homework in this course is meant to build your own problem-solving process. The goal is not to find a finished answer quickly; the goal is to learn how to turn a problem statement into small, testable pieces of Python.

## What Help Looks Like

Teaching Fellows can help you understand background concepts, translate the problem statement, plan your approach, read error messages, design tests, and debug partial work.

Teaching Fellows will generally not give full finished code for homework problems. If you ask for help, bring your current attempt, the exact error message, and one sentence describing what you expected the code to do.

## A Good Workflow

1. Restate the problem in plain English.
2. Identify the inputs, outputs, and important variables.
3. Write a tiny example by hand before coding.
4. Break the task into helper functions when possible.
5. Run one small test case before running thousands of simulations or a full dataset.
6. Print intermediate variables when you are confused.
7. Compare your result with what should happen in a small hand-traced case.

## For Simulation Homework

Simulation problems often feel hard because several ideas happen at once: randomness, loops, counters, records, and summaries. Separate them.

Ask yourself:

- What is random in one trial?
- What state changes after each trial?
- When should the loop stop?
- What should be recorded for later analysis?
- What should happen in a very small test case?
- After many repetitions, what pattern do I expect to see?

For an NBA best-of-7 series, for example, do not start by thinking about all 10,000 simulations. First trace one possible series by hand: game number, winner, team A wins, team B wins, and whether the series should stop.

## `np.random` Background

In Assignment 2, NumPy's randomness tools are used to simulate uncertain events:

- `np.random.choice(options, p=probabilities)` chooses one item from `options`.
- The probabilities in `p=[...]` must add to 1.
- `np.random.uniform()` gives a random number between 0 and 1.
- `np.random.seed(...)` makes random output repeatable while debugging.

For `generate_bernoulli(p)`, students should understand the model before memorizing the line of code: output `1` has probability `p`, output `0` has probability `1 - p`, and the two probabilities must match the two possible outcomes `[0, 1]`.

For `single_series(team_A, team_B, p_A)`, students should first design the state variables: `n_games`, `team_A_wins`, `team_B_wins`, `game_record`, and the current game winner.

## Assignment 2 Background Checklist

Before writing code for the NBA simulation questions, make sure you can explain these ideas:

- A Bernoulli random variable represents a win/loss outcome with probability `p`.
- A uniform random variable in `[0, 1]` can be used as a random score or draw.
- A best-of-7 series ends when either team reaches 4 wins.
- A game record should store enough information to reconstruct what happened.
- Repeating a simulation many times lets you estimate patterns such as the distribution of series length.
- A histogram summarizes many simulated outcomes, not one individual game.

## What To Bring To Homework Review

Bring one of these:

- A hand trace for one small example.
- A function skeleton with TODO comments.
- A screenshot or copy of the exact error message.
- A question about which variables should exist at a specific point in the loop.
- A plot or summary statistic that looks suspicious, plus your guess about why.

The best question is not "What is the answer?" but "Here is my model of the problem; which part of the model is wrong?"
