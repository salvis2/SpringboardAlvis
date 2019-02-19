## League of Legends Item Balancing
This is the repository for my first capstone project: League of Legends Item Balancing, part of my SpringBoard Data Science Career Track curriculum.

### About this project
This project was born out of a love for data science and League of Legends.
I have seen many websites that suggest various characters and items for players in a game of League of Legends, so I didn't want this project to follow suit. Instead, I took a stab at a problem from a developer standpoint. 
My overarching question was: As a developer for League of Legends, how do I know when I need to change an item? Can I develop a method or metrics to help with this? (Note that while there are roughly 237 items in LoL, I only analyzed 80. More on that in the notebooks)

I developed two metrics, one through statistical analysis and one through machine learning.

This first metric was gathering statistics on how often each item won, including the average win rate, and finding items that were unlikely to have the average win rate as their true win rate. This produced two lists of items: items that won too often, and items that didn't win often enough.

The second metric was the feature coefficients of a logistic regression. I took the top and bottom 10 coefficients and considered those to be unusually strong or weak predictors of game result.

The intersections of the statistical anomalies and feature coefficient anomalies are strong candidates for rebalancing. Most of the items in either anomalies list are decent candidates for rebalancing. For a full list of recommendations, see the final report or presentation.

### About this repository
This repository contains the data files and the Jupyter notebooks for each of the steps in my project's analysis.

The documentation is in the following 
<a href='https://drive.google.com/drive/u/0/folders/1txlu0tMy173O6N7p61SgwsUZjI-_ApZK'>
  Google Drive folder
</a>.

<a href='https://docs.google.com/document/d/1VuyZARXjh_g1gKjVY1xix4kJ32gM3IULC4Q9lpZzl6U/edit?usp=sharing'>
  Original Project Proposals
</a>
<br>
<a href='https://docs.google.com/document/d/1UpmTvFLnK358bkCElF-5BBpu8rGkTa4aa47KeYMUc3k/edit?usp=sharing'>
  Final Project Proposal
</a>

#### Capstone Project Process

The process for this capstone project is as follows:
Data is acquired and exported to csv in the data wrangling 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_1/capstone_project_1_data_wrangling_test.ipynb'>
  notebook
</a>.<br>
<a href='https://docs.google.com/document/d/1ZEtG8J5OLgc7ZrKy63zEYGR_Sx5nVMUxgOtI1KCwl-M/edit?usp=sharing'>
  The Data Wrangling Explained
</a>

Data is visualized and explained in the data storytelling 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_1/capstone_project_1_data_storytelling.ipynb'>
  notebook
</a>.

Data is analyzed statistically in the exploratory data analysis (EDA) 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_1/capstone_project_1_EDA.ipynb'>
  notebook
</a>.<br>
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_1/capstone_project_1_eda_report.pdf'>
  The EDA Explained
</a>

Data is analyzed with machine learning in the in-depth analysis (IDA) 
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_1/capstone_project_1_ida.ipynb'>
  notebook
</a>.
  

<a href='https://docs.google.com/document/d/1R3gYKpOdeu2fklTPPRNTi-4Tso-tiKHORYBUdV8Dl_E/edit?usp=sharing'>
  Final report
</a>
<br>
<a href='https://github.com/salvis2/SpringboardAlvis/blob/master/capstone_project_1/capstone_project_1_presentation.pptx'>
  Final Presentation
</a>

#### Running the Notebooks

If you wish to run the first notebook, you will first need to go to https://developer.riotgames.com/ and get a development API key. You log in with your League of Legends account, if you have one. If not, you need to create one. There is a spot in the data wrangling notebook where you can place the API key, and then the notebook should function correctly.

If you just want to take the data files as they are, you can skip the first notebook and go to the data storytelling.

Running the notebooks in order (wrangling, storytelling, EDA, IDA) should generate all of the data files you see in this repository. It will also generate the various figures that you can find in the presentation.

If you want to suggest comments or changes, feel free to email me at sebialvis@gmail.com
