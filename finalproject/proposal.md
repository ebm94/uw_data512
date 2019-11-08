# DATA 512 Project Proposal

**Motivation**  
Analyzing data of college majors and their graduates would definitely give a peak into the trends. It can possibly help future returning students make informed choices about the careers they will most likely be performing for their whole life. This does not take into consideration other factors that may change trends in future and what disciplines may turn out to be more in demand then. These datasets can help analyze both discipline and gender trends in terms of both salary and major adoption. Analyzing them can also help to find any anomalies and busting myths. It would also be interesting to see if any kind of bias can creep into the analysis and being mindful of not letting that happen.

**Data**  
These datasets are coming from American Community Survey 2010-2012 Public Use Microdata Series (PUMS) of US Census Bureau. The data falls under the open data series as mentioned here: [https://www.census.gov/about/policies/open-gov/open-data.html](https://www.census.gov/about/policies/open-gov/open-data.html)

Link to the data: [http://www.census.gov/programs-surveys/acs/data/pums.html](http://www.census.gov/programs-surveys/acs/data/pums.html)

There are three main data files with information on wages, gender and type of job.  
all-ages.csv: Employment statistics for all majors (174 majors) for all ages  
recent-grads.csv: For ages <28, it gives major-wise, how many men and women in that field.  
grad-students.csv: Grad vs non-grad comparison of majors

majors-list.csv: The list of the 174 majors along with major codes  
women-stem.csv: men vs women in stem majors along with median salary information. This dataset is derived from the above recent-grads.csv file.

The privacy concerns with Census data are taken care of due to the deidentification measure incorporated by US Census Bureau to preserve user privacy. In addition, the data set is at an aggregated level of majors which leads to blurring out data at an individual level.

**Dependencies**
I will not hesitate to add in any new dataset into the analysis if I feel that can make the story more powerful. Other than that, the size of the datasets and accessibility has already been accessed and does not look like there would be any hardware resource constraints.

