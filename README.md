# Cookie_Cats_AB_Analysis

This repository contains the code and data for analyzing an AB-test conducted on the game Cookie Cats to investigate the impact of moving the first gate from level 30 to level 40 on player retention. The analysis was performed using Python and various data analysis libraries.

## Dataset

The dataset used in this analysis consists of data from 90,189 players who installed the game during the AB-test period. The variables included in the dataset are:

- `userid`: A unique identifier for each player.
- `version`: The AB-group to which the player was assigned, either "gate_30" or "gate_40".
- `sum_gamerounds`: The number of game rounds played by the player during the first 14 days after installation.
- `retention_1`: Whether the player came back and played 1 day after installing.
- `retention_7`: Whether the player came back and played 7 days after installing.

## Analysis Steps

1. **Understanding the Data**: Load the dataset using pandas and examine its structure by displaying the first few rows.

2. **Distribution of Game Rounds**: Visualize the distribution of the number of game rounds played by players during their first week using a histogram.

3. **1-day Retention Analysis**: Calculate and compare the overall 1-day retention rate and the 1-day retention rate for each AB-group. 

4. **Bootstrapping Analysis**: Assess the uncertainty of the retention numbers using bootstrapping. Perform 500 bootstrap replications by resampling the dataset and calculating the 1-day retention rate for each sample. Visualize the bootstrap distributions using Kernel Density Estimate (KDE) plots.

5. **Probability of a Difference**: Determine the probability that 1-day retention is greater when the gate is at level 30 compared to level 40.

6. **7-day Retention Analysis**: Calculate and compare the overall 7-day retention rate and the 7-day retention rate for each AB-group.

7. **Bootstrap Analysis of 7-day Retention**: Perform bootstrapping to analyze the difference in 7-day retention between the AB-groups. Visualize the bootstrap distribution and calculate the probability of a difference.

8. **Conclusion**: Summarize the findings of the analysis, emphasizing the impact of gate placement on player retention and making a recommendation based on the results.

