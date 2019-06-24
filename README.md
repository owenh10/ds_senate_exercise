# Texas Senate Race
The 2018 US Senate race between Republican Senator Ted Cruz and Democratic Congressman Beto O'Rourke was one of the most hotly contested political contests of the election. This poll was a collaboration between the New York Times and Siena College in New York. It asked 800 Texans about who they were planning on voting for, along with demographic information like age, sex, and race. Despite Texas being a heavily Republican state, Beto O'Rourke came close to upsetting Cruz with a final share of 48.33% of the vote. The race was made more exciting by polls like the one from the New York Times, which helped to put on display the closeness of the race and the share of undecided voters who could potentially swing the election. Despite the fact that Cruz avoided an upset, the election also displayed political trends that will remain relevant going into the 2020 election. We're going to examine some of those trends within the race using our new data science and visualization skills.

### Release 0: Set Up Your Environment
Using today's lecture notes as a guide, set up your virtual environment and install jupyter and seaborn. Then, create a new jupyter notebook using the `python3` kernel.

### Release 1: Clean the Data
Take a look in the `txsen-2.csv` file and observe the formatting of the data. How can we clean this up?
* We mostly care about the first five columns (party response, age, education, race, and gender). In addition to these, we would like to be able to look at the region where a voter is located. Read these columns into a pandas dataframe.
* Some of our column names aren't descriptive. For example, the party a voter has chosen to vote for is marked as response. Rename this column to be "party_response".
* Some voters chose not to answer some questions, so data is missing for these rows. Remove the voters for whom this is the case.

### Release 2: Simple Description
Answer these questions by querying your dataframe and saving the queries and their results in a Jupyter notebook.
* If all of Texas voted like the respondents in this poll, who would win the race?
* For each category, what response was most common for those surveyed? That is, which race holds the majority in the election?, What sex?, What level of education?, Etc...
* What percentage of those surveyed were undecided?
* Out of all of our voters, how many did we have to remove from our dataframe because they didn't answer part of the survey?
* Create a histogram showing where voters lived. Which region was most populous among those surveyed?
* Create a histogram showing voter age. What age was most common among those surveyed?
* Create a histogram showing voter education. What eductation level was the most common?
* Create a histogram showing voter sex. What sex was more represented in the survey?
* Create a histogram showing voter race. What race was best represented in the survey?

### Release 3: Finding Trends
Answer the following questions based on the data from our poll. When coloring these visualizations, red should represent votes for Cruz and blue should represent votes for O'Rourke.
* Who would win if only men voted? If only women voted? Create a pie chart to show the percentages for each.
* Create a histogram of education level by party response (there should be two sets of five columns--one set describes republican voters and one describes democratic voters). What education level is the most common for each party? Answer the question numerically with queries, then graph the data.
* Who would win if only city voters (major OR minor) voted? Show a graph of responses by region. Which candidate did rural voters prefer? What about urban? (it might be useful to add value labels to your graphs here--for example, show counts for each group so you can compare directly). Answer the question with queries, then graph the data.
* Which age/sex combination (e.g. men 18-34) had the largest margin between the two candidates--in other words, which group agrees the most in their choice? Answer the question numerically with queries, then graph the data.
* Which age/sex combination was the least decided as a group (i.e. which group is closest to a 50/50 split)? Answer the question with queries, then graph the data.

### Release 4: Pairplot
Create a pairplot like the one from our lecture, coloring points by how each voter voted. Try to identify which graph from the pairplot display a strong seperation between red points and blue points. Which two variables does it map? You will likely have to manipulate your graph to make individual points more visible or otherwise find some way to group them. The seaborn documentation will be very helpful here!
