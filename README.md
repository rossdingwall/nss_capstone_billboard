# nss_capstone_billboard
“Billboard Hot 100: Historical Trends in Popular Music”
	
	This project will look at trends in the Billboard Hot 100 between 1958-2019. I want to use methods learned in this class to quantitatively analyze trends in popular music. My two main data questions are “How has chart composition changed over time?” and “How has the chart movement of hit songs changed over time?” I will be using a dataset from data.world. I have some assumptions and challenges listed later in this document, but I think this project is feasible. 
 
edit: this is still mostly the same. 


Motivation


I wanted to pick a topic that I was familiar with, and do things that I haven’t seen before. My first data-related love was sports statistics, and we don’t really talk about music the way we talk about sports. I think this is an interesting way to look at popular culture through an unbiased quantitative analysis. 
	
Little questions that made me think about this topic:

-why are there fewer  "one hit wonders"  in the 2000s and 2010s than previous decades? In the digital age, is the fame of a single hit enough to almost ensure subsequent hits?    

-I listen to the radio in the car, and I get sick of overplayed songs on pop and hip-hop radio. My Suzuki is a prison, and Drake is a merciless warden. Was heavy saturation as significant in previous eras?

-Everyone makes fun of Nickleback now, but they have a really impressive Billboard career. I’m not really going to look at genres or do any other measures of popularity, but Nickleback is an interesting case for me. 

-Looking at Billboard's records and achievements list, there clearly are some generational things happening. “Biggest drop from the #1 spot” is all songs from the 70s. “Most consecutive #1 hits” and “Most consecutive years with a #1 hit” are led by previous generations, but “Most Top 10 debuts” and “Most consecutive weeks on Hot 100” are dominated by 21st century artists. These are just cherry-picked observations, but there are probably some broader trends that can be identified.

edit: this is still mostly the same 

Data Question
 
I address two research questions: chart composition and movement of individual songs. 
 
Chart composition: I’m interested in looking at the “diversity” of charts over time. The concept I imagined is a sort of Gini coefficient: looking at “market share” over time. Once I figure out how to make a functioning ‘Gini analysis’ (or some other analysis of statistical dispersion), I can look at it in two ways: how  “market share dispersion” has changed over time for individual artists, and how “market share dispersion” has changed over time for individual songs. 
 
Edit: I did this. It’s a fun metric to have, but I need to “walk people into it” with more straightforward explanations of the data


Changes in individual song behavior over time. 
 
 
Schedule (through 1/9/2020)
 
Note: I’m just estimating deadlines, so I’ll add some notes to elaborate. I’m happy to change these dates based on your recommendations. 
Get the Data (Main Dataset is currently downloaded. If we decide to add later months via webscraping, we can try it out ASAP, and wait until the end of November or end of December to tack on the final months.)
Clean & Explore the Data (December 17th? I’ve done a good amount of exploring already. I need help with a regex to properly count artist names, and some discussion of how to organize the data by artist/by song. )
Create Presentation of your Analysis (12/28)
I intend on presenting a slideshow and having a cleaned-up Jupyter Notebook for GitHub. 
Internal demos (1/4/2020. Since I don’t anticipate presenting anything beyond a slideshow, I don’t think I need any special arrangements/equipment.)
Demo Day!! (1/9/2020)
 
Data Sources
Main dataset is from data.world: https://data.world/kcmillersean/billboard-hot-100-1958-2017.


Known Issues and Challenges

This is ordinal data- all we have is information about historical chart position. I’m planning on using an inverse scale: a song gets 100 points for being in the #1 position, and 1 point for being in the #100 position. This has some basis in Billboard's history. There are some assumptions in using an inverse scale, but I think it’s an ok way to handle the data and accomplish my goals. I’m open to suggestions if there are other methods for handling ordinal data. 







The things that I’m envisioning are currently Python-based. I haven’t really thought of ways to incorporate Excel and SQL. Python is the language that I’ve really grown to enjoy, but I’m not sure if it’ll be perceived poorly to have a single-language project. I think it’s ok as long as I have strong work examples of Excel and SQL in my GitHub.
 
Analyses I’ve Done:
Weeks on Chart by Artist- distribution
Weeks on Chart by Song- distribution
instances per song (Christmas)
% of features by year (can build upon with market share of feature vs non-feature)
“Chart-points” - overview, boxplots by artist + by song
Unique Songs per year + unique songs per performer time-series, unique songs vs unique performers 
per performer, distinct songs vs distinct weeks on chart or distinct years on chart (Glee)
Performer weeks per song: boxplot, scatter vs # of unique songs (Neon Trees)
Gini: overview, time-series of gini by performer and by song
Unique years per performer (lifespan): scatter, mean by year, median by year. 
Unique weeks per performer (lifespan): 
Similarity index (set operations): boxplot, weekly plot, by-year means (12/5/98)
 “Differential”: chart-points vs chart position (“country effect”)
 
To-Do List:
re-run analysis with “feature artist” splits
is it useful to keep pre-split data for any observations (ie comparing unique performers) 

Things I've thought about that I haven't been able to capture:

-"album effect" (Beyonce/Pusha T/ Kids See Ghosts)
-"country effect" (festival posters)
	-movement of songs ("cat ear" graphs)
- gini trend of mid-90s to early 2000s: what's going on here? 
- main artist vs features: set operations? 