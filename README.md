# visualization-activity

In this activity, we have hypothetically joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer. Given the dataset from a recent study of 249 mice and their responses to the drug over the course of 45 days, we were tasked with comparing the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

In this repo you will find the raw data from the study as well as my full code to both determine values of interest and build data frames and plots that demonstrate various trends and comparisons in the data. Please find my analysis copied below for ease of access.

<h2>Coding Help</h2>

I had to consult documentation a handful of times to remember exact steps. 

I could not figure out how to drop the duplicate rows for the one mouse that had them so I had to consult the internet here:
https://saturncloud.io/blog/how-to-find-all-duplicate-rows-in-a-pandas-dataframe/#:~:text=To%20find%20duplicate%20rows%20in%20a%20pandas%20dataframe%2C%20we%20can,get%20all%20the%20duplicate%20rows.

I also could not remember how to get the color and marker of a boxplot outlier to change so I had to look this up as well:
https://matplotlib.org/stable/gallery/statistics/boxplot_demo.html

<h2>Analysis</h2>

- More mice were treated with Ramicane and Capomulin, our drug of interest, than any other drug (with Propriva being the least used drug).

- Ramicane performed better overall than Capomulin, but the difference is small. Both drugs, however, performed significantly better than the placebo, which suggests a real impact made by both drugs. 

- It is possible that other drugs may have performed better on their own given a larger sample size of mice, though I personally doubt it, as Propriva (the smallest sample size) reduced tumor volume on par with Infubinol, a drug that had about as many observed timepoints as the other mid-sample-size drugs.

- There is a relatively strong positive correlation (0.84) between mouse weight and average tumor volume on the Capomulin treatment specifically. This could mean that higher-weight mice don't respond as well to the drug as their lower-weight counterparts. This being said, even the highest weight mouse on the Capomulin regimen had a lower average tumor volume than every other drug's average tumor volume (excluding Ramicane, which worked at about the same level as Capomulin).
