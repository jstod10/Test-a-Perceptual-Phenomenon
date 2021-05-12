### Background Information

In a Stroop task, participants are presented with a list of words, with each word displayed in a color of ink. The participant’s task is to say out loud the color of the ink in which the word is printed. The task has two conditions: a congruent words condition, and an incongruent words condition. 

In the congruent words condition, the words being displayed are color words whose names match the colors in which they are printed. 

In the incongruent words condition, the words displayed are color words whose names do not match the colors in which they are printed. 

In each case, we measure the time it takes to name the ink colors in equally-sized lists. Each participant will go through and record a time from each condition.

### Purpose of Task

Investigate a classic phenomenon from experimental psychology called the Stroop Effect using inferential statistics.  Outline the statistical investigation from start to finish and report findings along the way.  Provide justifications for reasonings that support findings. 

### Variable Identification

* Independent Variable - 'Congruent' or 'Incongruent' condition
* Dependent Variable - Time it takes to write the word

### Hypotheses

*The incongruent task will take longer than the congruent task because the combinations are not natural and, therefore, the taker requires more response time to process the information.*

* Null Hypothesis (H0) - No change in time between completion of both tasks
* Alternate Hypothesis (H1) - The incongruent task will take longer

#### Calculation Methods

* H0 = μi ≤ μc (μi - population mean of incongruent values, μc - population mean of congruent values)
* H1 = μi > μc (μi - population mean of incongruent values, μc - population mean of congruent values)

### Statistical Test

A t-score was calculated to test my alternate hypothesis against the null hypothesis.  The critical value of the null hypothesis was calculated to use as a baseline for comparison (using a confidence level of 95% and a degree of freedom of 23).  

I chose the *t-score for dependent means (paired t-test)* because the provided dataset contained fewer than 30 records, the data values were paired measurements, and the population standard deviation was unknown.  Both sets of values were also (mostly) normally distributed.

* Standard deviation of differences between 'Congruent' and 'Incongruent' datasets: 4.8
* Mean of differences between 'Congruent' and 'Incongruent' datasets: 7.97

I calculated the t-score by first finding the standard deviation of the difference between 'Congruent' and 'Incongruent' results.  Then, I calculated the mean of the difference between both data sets.  Finally, I created a script to replicate the formula to calculate the t-stat score using those values. 

#### Formula for creation of t-score

* t_stat = mean_dif/(std_dif/math.sqrt(df.shape[0]))

### Results

* Critical Value of null hypothesis - 1.71
* t-score value of alternate hypothesis - 8.02

#### Interpretation

The t-score of 8.02 is significantly higher than the 1.71 critical value of the null hypothesis.  This difference allows for the *rejection of the null hypothesis*, as the results clearly align with my initial hypothesis that 'Incongruent' times would be longer on average than 'Congruent' baselines.  

It makes both hypothetical and logical sense that interpreting unnatural relationships would require the human brain to take more time to process the information.  Thus, the Stroop test is clearly an effective measurement of how quickly an individual can process information.  

There is a well-defined relationship between the 'Congruent' and 'Incongruent' results, as 'Incongruent' tests repeatedly took longer.  Also, the relative word condition clearly has as influence on the test, as 'Incongruent' values were interpreted more slowly and with greater variance (as represented by the slightly skewed distribution of 'Incongruent' data highlighted in the histogram).

In conclusion, the results absolutely matched my expectations coming in to the exercise.  There was a tangible difference in data sets and a pattern emerged that showed the 'Incongruent' tests would take significantly longer on average than 'Congruent' testing.
