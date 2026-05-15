# AI Mathematical Olympiad - Progress Prize 3

## Overview

The goal of this competition is to create open-source algorithms and models that can solve olympiad-level math problems written in LaTeX format. Your participation will help to advance AI models’ mathematical reasoning skills and drive frontier knowledge.

---

## Description

Note: This is the third AIMO Progress Prize competition. It builds upon the first AIMO Progress Prize competition, which was won in July 2024 by Project Numina and the second AIMO Progress Prize competition, which was won in April 2025 by Nvidia’s NemoSkills team. This third competition features a significantly increased problem difficulty, new submission format, expanded prize pool, industry-leading compute resources for participants, new auxiliary prizes to reward community contributions, and updated rules for using open-source LLMs.

The ability to reason mathematically is a critical milestone for AI. Mathematical reasoning is the foundation for solving many complex problems, from engineering marvels to intricate financial models. However, current AI capabilities are limited in this area.

The AI Mathematical Olympiad (AIMO) Prize is a $10mn fund to spur the open development of AI models capable of performing as well as top human participants in the International Mathematical Olympiad (IMO).

Recent breakthroughs demonstrate AI achieving human-level results on IMO problems. Closed-source models achieved gold medal performance at the 2025 IMO, demonstrating that frontier AI systems are now capable of solving the world's most challenging high school mathematics problems. Our "OpenAI x AIMO eval" in March 2025 revealed that commercial models could solve 50/50 AIMO2 public leaderboard problems with sufficient compute—despite the highest Kaggle score being just 34/50. This demonstrates a significant gap between closed-source and open-source models in mathematical reasoning capabilities.

AIMO3 is designed to accelerate open-source progress and close this gap. The competition features 110 problems spanning algebra, combinatorics, geometry, and number theory, ranging from National Olympiad level all the way up to IMO standard—the pinnacle of high school mathematical achievement. All problems are entirely original, created by an international team of problem solvers to ensure zero risk of train-test contamination. They have been carefully designed to be 'AI hard', tested against current open LLMs' capabilities. They require genuine mathematical reasoning to solve, making answer-only testing as robust as possible (see Problem 10 in the Reference Problems PDF for a detailed discussion of this design philosophy).

Every problem is entirely original, ensuring zero risk of data contamination. Using this transparent and fair evaluation framework, the competition will help to strengthen the benchmarks for assessing AI models' mathematical reasoning skills. This latest AIMO Progress Prize competition offers an exciting opportunity to drive innovation in the field of AI for Math, while also fostering healthy competition and supporting open science.

Join us as we work towards a future where AI models’ mathematical reasoning skills are accurately and reliably assessed, driving progress and innovation.

---

## Evaluation

During the submission period, submission notebooks are run only over the public test set and are evaluated by the unnormalized accuracy between their predicted labels and the ground-truth labels (i.e. number of correct answers).

After the submission deadline, submission notebooks will be run twice over the private test set and their predictions concatenated into a single submission file. We then evaluate submissions by a penalized accuracy score, as follows:

If both predicted answers for a problem are correct, the score is 1 for that problem.
If one predicted answer is correct and the other is incorrect, the score is 0.5 for that problem.
If neither predicted answer is correct, the score is 0 for that problem.
A submission's overall score is the sum of its scores for each problem.

![Extra Info](assets\eval_info.png)

---

### Most Important

[AIMO - Models](https://www.kaggle.com/competitions/ai-mathematical-olympiad-progress-prize-3/models)

## Submitting

You must submit to this competition using the provided Python evaluation API, which serves test set instances one-by-one in random order for the public leaderboard, and uses fixed, random order for the private leaderboard. To use the API, follow the template in this notebook.

---

## Timeline

November 20, 2025 - Start Date.
April 8, 2026 - Entry Deadline. You must accept the competition rules before this date in order to compete.
April 8, 2026 - Team Merger Deadline. This is the last day participants may join or merge teams.
April 15, 2026 - Final Submission Deadline.

As noted in the Evaluation section, selected submissions will be run against the private test set after the Submission deadline. Final results will be available shortly thereafter.

All deadlines are at 11:59 PM UTC on the corresponding day unless otherwise noted. The competition organizers reserve the right to update the contest timeline if they deem it necessary.

---

## Code Requirements

Submissions to this competition must be made through Notebooks. In order for the "Submit" button to be active after a commit, the following conditions must be met:

CPU Notebook <= 9 hours run-time
GPU Notebook <= 5 hours run-time
Internet access disabled
Freely & publicly available external data is allowed, including pre-trained models
Submission file must be generated by the API.
Submission runtimes have been obfuscated. If you repeat the exact same submission you will see up to 30 minutes of variance in the time before you receive your score.

Please see the Code Competition FAQ for more information on how to submit. And review the code debugging doc if you are encountering submission errors.

---

## Upgraded Kaggle Hardware

We're excited to announce that we've added powerful new H100 machines to the AIMO hardware pool! See this page for more on these machines.

What you need to know:

AIMO 3 Only - H100 are only available for notebooks attached to this competition, use of H100s for any other activity could result in moderation action (e.g. site suspension or account ban).
No Internet - To help ensure these machines are reserved for competition use, all H100 sessions must have internet disabled.

---

## Note on Language and Notation

All problems are text-only with mathematical notation in LaTeX. The following conventions are observed:

---

## Partnerships and Additional Resources

The Hosts' aim is not just to run a competition, but to provide an ecosystem for it.

We thus have partnered with the Fields Model Initiative (supported by two organizations: the LLMC from the National Institute of Informatics in Tokyo and Benchmarks+Baselines from Vienna) and with Thinking Machines, which makes the Tinker service available.

These partnerships provide compute and API credits, respectively, to help contestants train/fine-tune their models. AIMO is the first large-scale Kaggle reasoning competition to provide significant support in this direction, enabling competitors to have a streamlined experience for training and competing with their models.

This addresses a significant pain point from previous AIMO competitions and a persistent issue of any large-scale competitions that focus on computationally expensive AI models, such as LLMs, as previous competitions were 1) skewed towards large labs with significant resources having an edge, and 2) skewed towards teams with strong engineering know-how, putting mathematicians keen on competing at a disadvantage.

Our partnerships solve both problems. AIMO3 levels the playing field by providing access to 128 H100 GPUs via the Fields Model Initiative (applications for more will be considered on a case-by-case basis), totaling hundreds of thousands of hours of compute we can offer to teams, and up to $400 in API credit for Tinker. Tinker abstracts away much of the engineering knowledge, making it particularly beneficial for mathematicians.

Because demand may exceed supply, an application process will be in place for both of these services, and applications will open later in December, with precise details outlined in the Kaggle Discussion forum. Because it is our goal to make these resources available to teams with the greatest promise to devise a strong reasoning model, factors beyond application time may be considered.

## About the Hosts

XTX Markets is a leading algorithmic trading company and has over 200 employees based in London, Paris, New York, Mumbai, Yerevan and Singapore. XTX provides liquidity in the Equity, FX, Fixed Income and Commodity markets and trades over $250bn a day across markets.

XTX Markets' expansive research cluster contains 100,000 cores and 20,000 A/V100 GPUs and is growing. It also has 390 petabytes of usable storage and 7.5 petabytes of RAM. Alongside rich datasets and advanced technological infrastructure we are at the forefront of the crossover of finance and technology.

XTX Markets’ philanthropy focuses on maths and science education and research, alongside other areas such as academic sanctuaries, carbon removal and an employee matching programme. Since 2017, XTX Markets has donated over £100mn to charities and good causes, establishing it as a major donor in the UK and globally.

---

## Citation

Simon Frieder, Sam Bealing, Philip Vonderlind, Sida Li, Arsenii Nikolaiev, Geoff C. Smith, Kevin Buzzard, Timothy Gowers, Peter J. Liu, Po-Shen Loh, Lester Mackey, Leonardo de Moura, Dan Roberts, D. Sculley, Terence Tao, David Balduzzi, Simon Coyle, Alex Gerko, Ryan Holbrook, Addison Howard, and XTX Markets. [AI Mathematical Olympiad - Progress Prize 3](https://kaggle.com/competitions/ai-mathematical-olympiad-progress-prize-3), 2025. Kaggle.
