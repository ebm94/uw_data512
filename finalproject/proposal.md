**DATA 512 Project Proposal**
**Analyzing college majors and their employment prospects**

**Motivation**  
Analyzing data of college majors  would give a peek into various trends in the education sector. It can help future new and returning students make informed choices regarding careers that they will most likely be performing for their whole life. The trends can be in terms of gender, salary, major adoption and employment prospects. Analyzing them can also help to find any anomalies and to bust myths. It would also be interesting to see if any kind of bias can creep into the analysis and it would be important to be mindful of not letting that happen. This analysis does not take into consideration other factors that may change career trends in future and what disciplines may turn out to be more in demand then.

**Data**  
These datasets are coming from American Community Survey 2010-2012 Public Use Microdata Series (PUMS) of US Census Bureau conducted across US. The data falls under the open data series as mentioned here: [https://www.census.gov/about/policies/open-gov/open-data.html](https://www.census.gov/about/policies/open-gov/open-data.html)

Link to the data: [http://www.census.gov/programs-surveys/acs/data/pums.html](http://www.census.gov/programs-surveys/acs/data/pums.html)

There are three main data files with information on wages, gender and type of job.

* all-ages.csv: Employment statistics for all majors (173 majors) for all ages

* recent-grads.csv: For ages <28, it gives major-wise, how many men and women in that field.

* grad-students.csv: Grad vs non-grad comparison of majors

* majors-list.csv: The list of the 173 majors along with major codes

* women-stem.csv: men vs women in stem majors along with median salary information. This dataset is derived from the above recent-grads.csv file.

The privacy concerns with Census data are taken care of due to the deidentification measure incorporated by US Census Bureau to preserve user privacy. In addition, the datasets are at an aggregated level of majors which leads to blurring out data at an individual level.

**Dependencies**
I will not hesitate to add in any new dataset into the analysis if I feel that can make the story more powerful. Other than that, the size of the datasets and accessibility has already been accessed and does not look like there would be any hardware resource constraints.

**Questions/Hypotheses**  
1. What are the most and least popular majors and major categories? Popularity is defined as no. of students with that major. It would be interesting to see if this is consistent across overall student population, graduate students and non-graduate students.  
2. Total people and Employed trend chart for major categories? Two charts to compare for graduates and overall?  
3. People in which majors are more likely to go to graduate school?  
4. Are there any majors in which people have high employment rate, but low full-time year-round employment rate?  
5. Which majors are those in which graduate student unemployment is higher than non-graduate student unemployment?  
6. In which disciplines, employment chance increase the highest when a student decides to go to graduate school.  
7. What are the majors in which there are >80% men and those with >80% women? It would be interesting to see what is the average of the median salaries in these two buckets.

**Background/Related Work**
We are living in the technology age, when one does not necessarily have to go to school in order to have a successful career. But, time and again there are articles like [this](https://www.nytimes.com/2014/05/27/upshot/is-college-worth-it-clearly-new-data-say.html?hp&_r=1&abt=0002&abg=0) where they say college degree has never been more valuable. These are backed by studies like [this](https://libertystreeteconomics.newyorkfed.org/2014/09/the-value-of-a-college-degree.html#.VA6Uh_mwLwk) one conducted by the Federal Reserve Bank of New York. The same study had found that college students who earn in the lowest quartile are earning less than what half the high school graduates made. Even if students enroll in colleges, many college students don’t even end up graduating and therefore end up with student debt in addition to lack of job. While this is happening there would be high school graduates who would already have been working for 4 years without student debt ([Source](https://www.wsj.com/articles/SB10001424127887324595904578117400943472068)).

Although entities collect data on major enrolments and graduation, they are rarely helpful for students make informed decisions. It is necessary to bring around messages that are loud and clear in the datasets and share them in a manner that is easy to interpret while sharing all the assumptions that went into arriving at those insights.

**Methodology**
The data sources are flat files that can be analyzed locally without need of any special hardware resources. Before starting further analysis, I would go about exploring the distribution of the variables and identifying any outliers or missing values that are present in the data. I would see what all values are lying 3 standard deviations above the mean of that variable and put them as outliers.

I would go about creating effective plots like line charts for trends across majors that convey important messages of my analysis clearly. When there are some differences in certain proportions, it would be of interest to see if the difference is big enough, I would use Welch t-test. The reason why I would use this test is because it would be quite likely that the variance of the two groups would be unequal. In addition, I would also find correlation between quantitative values like median salary for a major and the enrollment in that group. Correlation is a normalized quantity between 0 and 1 and is universally interpretable. Having said that, I would be cautious about any confounding variables that could reflect in the form of high value of correlation and false relationships between variables. I would also create new features from the existing ones by performing bucketing of quantitative variables. Bucketing can help deduce insights that are otherwise lost in granularity.

**Human-centered considerations**
Without any actual numbers that describe career outcomes as it is, students make career decisions on basis of sources like word of mouth or doing what their peers are doing. This analysis would be especially impactful in helping make the right career choices. A very good example will be that there are some majors that have a lot in similar and the interests are also very much similar; only some slight differences in the applications and obviously the name of the major changes. These two majors can have so much difference in employment prospects in future and students need to be aware of such scenarios and pick their majors wisely.

