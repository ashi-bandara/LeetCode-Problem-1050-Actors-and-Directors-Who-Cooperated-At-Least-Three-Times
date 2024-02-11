
# LeetCode Challenge D50

## Overview

Welcome to my LeetCode solution repository! This project addresses the coding challenge presented by [1050. Actors and Directors Who Cooperated At Least Three Times](https://leetcode.com/problems/actors-and-directors-who-cooperated-at-least-three-times/). Below, you'll find details about the problem, my approach to solving it, and the implemented solution.

## Problem Statement

Write a solution to find all the pairs  `(actor_id, director_id)`  where the actor has cooperated with the director at least three times.

Return the result table in  **any order**.

The result format is in the following example.

**Example**
>**Input:**
>
| actor_id | director_id | timestamp |
|:--------:|:-----------:|:---------:|
|     1    |      1      |     0     |
|     1    |      1      |     1     |
|     1    |      1      |     2     |
|     1    |      2      |     3     |
|     1    |      2      |     4     |
|     2    |      1      |     5     |
|     2    |      1      |     6     |

>**Ouptut:**
>
| actor_id | director_id |
|:--------:|:-----------:|
|     1    |      1      |

>
>**Explanation:** The only pair is (1, 1) where they cooperated exactly 3 times.

**Language Used**
> MySQL

**Difficulty**
> Easy

## Solution Overview
The solution finds pairs of actors and directors who have worked together on at least three projects. It does this by looking at a table that records each time an actor and director team up. The solution groups these records by actor and director pairs and counts how many times they've worked together. Then, it filters out pairs that haven't collaborated at least three times. This helps identify actor-director duos with a strong history of working together, which is useful for understanding their successful partnerships in the movie industry.
