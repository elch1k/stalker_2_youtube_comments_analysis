# STALKER 2 trailer's YouTube marketing campaign analysis
![stalker_main_image](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_2_main_image.jpg)
*Short word:* This project was intended for release much earlier, as I initiated it prior to the game's release, immediately following the completion of my NLP course. However, after finishing the core analysis, I lacked the time to prepare a GitHub release and compile the necessary README file.
**Project goals:** Track audience sentiment throughout the Stalker 2 release cycle, documenting its evolution. Assess the impact of GSC Game World's policies on the Russian audience, and determine if this impact was detectable on platforms like YouTube in comments section. Analyze the level of support for the game from the Ukrainian audience, and investigate how GSC Game World's policies influenced the English-speaking audience. Examine the dynamic changes in both sentiment and default YouTube statistics and also identify the dominant discussion topics associated with each trailer.

*Additional information:* you can find YouTube comment scraper [here](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/youtube_comment_parse.ipynb) and first comment preprocessing [here](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/youtube_comment_preprocessing.ipynb).

EDA of Simple YouTube Statistics
---
The plots illustrate the changes in YouTube statistics (views, likes, and comments) over time. Notably, the Stalker 2 trailer's marketing campaign spanned nearly four years, a considerable duration, which was significantly impacted by the war.
![first_eda_youtube_stat_plot](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_1.png)
![second_eda_youtube_stat_plot](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_2.png)

Let's examine the overall language distribution of comments from the Stalker 2 trailers.

![third_eda_plot](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_3.png)

We can also compare the language distribution of comments between the first trailer (S.T.A.L.K.E.R. 2 – Trailer #1) and the latest (S.T.A.L.K.E.R. 2: Heart of Chornobyl — Gone Gold).

![fourth_eda_plot](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_4.png)

Sentiment Analysis
---
A key challenge in this analysis was the multilingual nature of the comments. After research ([here](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/youtube_comment_analysis.ipynb)), I decided to analyze sentiments using only the three predominant languages in the comments: Ukrainian, English, and Russian.
![sentiment_analysis_plot_1](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_5.png)

Detailed sentiment distribution by language is shown below.
![sentiment_analysis_plot_2](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_6.png)

It would also be beneficial to observe sentiment distribution by language over time (across video trailers).
![sentiment_analysis_plot_3](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_7.png)

Topic Modeling
---
Further details on this section of the project can be found via this [link](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/youtube_comment_analysis.ipynb) in the concluding portion. The image below presents the main topics from the 11th video (S.T.A.L.K.E.R. 2: Серце Чорнобиля — Developer Deep Dive). As demonstrated, the topic modeling reveals primary topic sentiments (happiness, excitement, politics). However, it's noticeable that certain words appear across multiple topics, possibly due to English words being written using non-English characters, which may be a translator issue (which I need to solve).
![topic_modeling_image](https://github.com/elch1k/stalker_2_youtube_comments_analysis/blob/main/images/stalker_project_plot_8.png)
