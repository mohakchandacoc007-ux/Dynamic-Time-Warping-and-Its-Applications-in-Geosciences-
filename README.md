# Dynamic-Time-Warping-and-Its-Applications-in-Geosciences-
Application of Dynamic Time Warping (DTW) for similarity analysis and alignment of well-log data using Python.

## Overview

This project explores the use of **Dynamic Time Warping (DTW)** for measuring similarity and aligning two time-series signals, with an application to **well-log data**.

Well-log responses may show similar geological patterns at different depths. Direct point-by-point comparison can therefore be inadequate when corresponding features are shifted or stretched along the depth axis. DTW addresses this by finding an optimal alignment path between two sequences while allowing local stretching and compression.

The project demonstrates DTW using both **synthetic signals** and a larger **well-log dataset**.

---

## Objectives

The main objectives of this project are:

- Understand the principle of Dynamic Time Warping.
- Measure the similarity between two well-log signals.
- Calculate the DTW distance between two sequences.
- Determine the optimal alignment path.
- Construct and visualize the pairwise distance matrix.
- Align two well-log signals using the DTW path.
- Compare well logs before and after DTW alignment.
- Apply the method to real well-log data.

---

## What is Dynamic Time Warping?

Dynamic Time Warping is an algorithm used to determine the similarity between two sequences by finding an **optimal alignment** between them.

Unlike conventional point-by-point comparison, DTW allows the sequences to be locally stretched or compressed. This makes it possible to compare signals that have similar patterns but are not perfectly synchronized.

The optimal alignment is obtained by minimizing a predefined cumulative distance or cost between corresponding points.

---

## Methodology

The project follows the workflow:

```text
Well Log Signals
       |
       v
Data Preparation
       |
       v
Pairwise Distance Matrix
       |
       v
Dynamic Time Warping
       |
       +------------------+
       |                  |
       v                  v
DTW Distance       Optimal Path
       |                  |
       +--------+---------+
                |
                v
        Signal Alignment
                |
                v
       Visualization and
       Before/After Comparison
