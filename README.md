# Discovering-Pattern-Associations-in-Hang-Seng-Index-Constituent-Stocks

## Background

This project is to appreciate the work done by my research teammates back in the days where AI, Big Data and Machine Learning were not very hot in the industry.

They attempted to tackle a problem of finding patterns in financial time series. Instead of using systematic observations, statistical analysis or artificial intelligence techniques on the discovery of patterns in data, they focus on understanding association relationships between the discovered patterns.

## Objective

I aim at implementing the proposed approach using Python in a Jupyter Notebook for this study.

## Approach

The methodology suggested is for discovering probabilistic patterns in time series data, specifically in the context of financial data. The approach is based on determining association relationships between patterns. Here's a breakdown of the key concepts and steps:

1. Probabilistic Patterns: Patterns that do not appear deterministically in a time series are referred to as probabilistic patterns. These patterns are discovered using the proposed approach.

2. Determining Inter-Dependencies: The goal is to determine if certain events in a sequence of events are inter-dependent. For example, in financial data, the relationship between the stock values at time t and t+n (a time lag later) is examined.

3. Adjusted Residual: The adjusted residual is calculated using the observed and expected frequencies of occurrence of specific events. The adjusted residual helps quantify the strength of the association relationship between events.

4. Maximum Absolute Adjusted Residual (MAAR): MAAR is the maximum absolute adjusted residual among all possible associations. If the MAAR exceeds a threshold value (1.96 in this case), it indicates a statistically significant association relationship.

5. Symbolic Sequence and Contingency Table: The time series data is transformed into a symbolic sequence using predefined symbols (e.g., "U" for up, "D" for down). A contingency table is constructed based on the symbolic sequence to facilitate the calculation of adjusted residuals.

6. Atomic Pattern Construction: Atomic patterns are basic building blocks constructed from a set of simple elements. An evolutionary algorithm is used to generate atomic patterns iteratively. The fitness of a pattern is determined by its frequency and length.

7. Association Relationship Discovery: The atomic patterns are used to transform the symbolic sequence into an atomic-pattern sequence. The MAAR is then calculated for the atomic-pattern sequence to identify association relationships.

8. Time Lagging and Adjusted Residuals: Time lagging is introduced to examine the association between events at different time points. Adjusted residuals are calculated using contingency tables constructed from the atomic-pattern sequence.

## A general framework for implementation

1. Symbolic Sequence Generation:

- Convert your time series data into a symbolic sequence using predefined symbols. For example, you can assign "U" for an upward movement and "D" for a downward movement.

2. Contingency Table Construction:

- Create a contingency table based on the symbolic sequence. The table should count the occurrences of different combinations of symbols at different time lags.

3. Adjusted Residual Calculation:

- Calculate the adjusted residuals using the observed and expected frequencies obtained from the contingency table. You can use statistical methods or libraries to perform this calculation.

4. Maximum Absolute Adjusted Residual (MAAR):

- Determine the MAAR by finding the maximum absolute adjusted residual value among all the associations.

5. Atomic Pattern Construction:

- Define the set of simple elements that can be combined to form atomic patterns.
- Use an evolutionary algorithm or any suitable method to generate atomic patterns iteratively based on their frequency and length.

6. Association Relationship Discovery:

- Transform the symbolic sequence into an atomic-pattern sequence based on the generated atomic patterns.
- Calculate the MAAR for the atomic-pattern sequence to identify significant association relationships.



## Reference
Lui, Kim & Hu, Lun & Chan, Keith. (2009). Discovering Pattern Associations in Hang Seng Index Constituent Stocks. International Journal of Economics and Finance. 2. 10.5539/ijef.v2n2p43. 
