# Fall 2025 Data Challenge Instructions

## Foreword:

This event provides an opportunity for students to gain practice in working with real data and communicating the analysis results clearly and concisely. Positive outcomes of this data challenge will be rewarded based on an in-person presentation and a short one or two-page executive report. 

This Data Challenge is judged on the final report, presentation, and model accuracy. The emphasis of this Data Challenge is on clear explanations of the conclusions and the underlying methodology. Your presentation may also include any exploratory analysis of the dataset, potential weaknesses of your model or methodology, and/or future improvements you would make to your work.

## Important Dates:

**October 6, 2025**: Help Session at 6:00pm, 2532 Mordgridge Hall


**October 13, 2024**: Midpoint Checkpoint - Submit your code for a small point boost.

**October 24, 2024**: Report, and Code are due by 11:59pm

> **Note:** Unlike previous semsters we are **not** requiring you to submit your presentations before hand.

**October 27, 2024**: Oral presentations before a panel of judges at 6:00pm, 2532 Mordgridge Hall


---
GROUPS MAY HAVE UP TO 4 MEMBERS . . .  NO MORE
---

## Relevant Variable Explanation

**Commodity:** This column lists a commodity or commodity group and its corresponding North American Industry Classification System (NAICS) code used by North American (Canada, US, and Mexico) federal statistics agencies. Note that some codes refer to broad classifications of commodities while others refer to specific commodities. It may be useful (but not required) to familiarize yourself with the NAICS, which you can do with this document: [link](https://www.census.gov/naics/reference_files_tools/2022_NAICS_Manual.pdf). 

**Month:** This column lists the month of analysis.

**Year:** This column lists the year of analysis.

**Country:** This column lists the country of analysis.

**Total Exports Value ($US):** This column contains the value of US exports, expressed in **nominal** USD ($). See this [link](https://usatrade.census.gov/data/Perspective60/Browse/SummarySpawned.aspx?SummaryType=DimensionSummary&userId=225891&DimensionIndex=3&Language=en&SummaryReportId=7028&SummaryCubeId=17) for further details. 

**Customs Import Value (Gen) ($US):** This column contains the value of US imports, in **nominal** USD ($), excluding tariffs and other factors which influence the value of imported goods. See this [link](https://usatrade.census.gov/data/Perspective60/Browse/SummarySpawned.aspx?SummaryType=DimensionSummary&userId=225891&DimensionIndex=3&Language=en&SummaryReportId=7028&SummaryCubeId=17) for further details.

**CPI_Annual:** This column contains the US's average annual CPI-U for each year. The CPI-U is the Consumer Price Index for Urban Consumers. It can be used to calculate **price inflation**, or at least a good and commonly-referenced estimate of inflation. It may be useful to familiarize yourself with the CPI and how to use it to calculate inflation. Here is a good starting point: [link](https://en.wikipedia.org/wiki/Consumer_price_index_in_the_United_States). 

**GDP_Current_USD:** This column contains the US's nominal Gross Domestic Product (GDP) in USD ($) for each year. It may be useful to familiarize yourself with GDP and its relevance to interpreting US trade data.

## Introduction to the Data Challenge

The topic of this Data Challenge is international trade. Trade flows - imports, exports, and balances of goods and services - sit at the heart of how countries interact with one another. From fueling domestic industries to influencing global alliances, patterns of trade shape the economic and political order of the world. Today, trade disputes, tariff battles, and supply chain disruptions underscore just how powerful these flows are. Understanding them is not only a matter of economics but also of geopolitics and strategy.

The goal of this Data Challenge, then, is to explore patterns in global trade using U.S. Census Bureau data. By analyzing trade volumes, substitution effects, correlations across goods, or the consistency of relationships between countries, you will develop insights into how nations and industries navigate this ever-changing landscape. Rather than producing a single “right answer,” your task is to ask sharp, research-like questions and explore them through statistical methods.

You are given a dataset sourced from the U.S. Census Bureau, which contains detailed information on imports and exports across goods, services, and trading partners over time. It is important to note that not every variable (column) is equally useful—part of your challenge will be to decide what is most relevant for your chosen question. Some questions may require aggregating categories of goods, others may focus on time-series dynamics, and still others may compare relationships across countries.

It would also be smart to do some preliminary research on the terms used in the dataset and the broader economic context. For example, what distinguishes a tariff from a trade barrier? Why do certain industries, like semiconductors or pharmaceuticals, carry disproportionate weight in trade discussions? And what might it mean for a relationship between two countries to be “stable” or “unstable”?

**IMPORTANT:** Note that both U.S. GDP and the CPI have increased steadily over the selected time period, and that all export and import values are expressed in nominal terms. Without adjustment, a rise in dollar values might reflect nothing more than general price inflation or the natural expansion of the overall economy. To isolate genuine shifts in trade behavior, it is essential to deflate nominal trade flows with a price index and to consider them relative to GDP. Accounting for inflation and economic growth allows you to distinguish real changes in the quantity and significance of trade from mere monetary effects, giving your analysis a sound economic foundation.

## Data Challenge Questions: 


Contrary to how we have done things in the past, you are in **NO WAY** expected to answer each of the questions below, nor are you expected to follow the *Example Methods*.  
The list of questions is meant to encourage you to form **one or more research-like questions** that allow your group the freedom to explore something of interest.  
The questions are intended to be open-ended but not vague. If you are confused, please reach out to the Vice President [Spencer Venancio](mailto:svenancio@wisc.edu) or any of the other board members (contacts below).

#### Question 1  
When tariff rate increases are applied unevenly across goods and countries, do we observe substitution?  
- Geographic substitution (countries shifting partners or sourcing from new regions)  
- Product substitution (importers/exporters shifting away from certain goods toward others)  
What broad trade trends emerge as a result?  

> **Example Methods:**  
> - Correlation matrices or heatmaps of trade flows  
> - Regression models testing substitution effects  
> 
---

#### Question 2  
Which goods and services show strong correlations in their trade flows?  
Do changes in imports/exports of one good systematically move with others?  

> **Example Methods:**  
> - Network analysis of goods based on co-movement  
> - Principal Component Analysis (PCA) to identify shared drivers  
> 
> ---

#### Question 3  
How do trade volumes differ across countries?  
Consider factors such as geography, development status, and population.  

> **Example Methods:**  
> - Mixed-effects regression models (countries as random effects, sectors as fixed effects)  
> - Hypothesis testing of mean balances across regions  
> 
---

#### Question 4  
Which countries have the most consistent trade relationships, and which have unstable ones?  

> **Example Methods:**  
> - Time-series analysis of bilateral trade stability  
> - Clustering methods to group countries by volatility patterns  
> 
---

#### Question 5  
Which industries drive changes in U.S. exports and imports?  
Focus on categories such as capital goods, semiconductors, pharmaceuticals, and autos.  

> **Example Methods:**  
> - ANOVA / MANOVA comparing export/import values across industries  
> - Cluster analysis (k-means or hierarchical) to group industries with similar trade patterns  


## Awards:
Certificates will be given for the following categories:
- Best Oral Presentation
- Best Written Report
- Most Accurate Model
- Best Visualizations
- Best Overall Project

Teams will be judged by department faculty and graduate students. You will receive official certificates for the awards, and your team photos will be shared on our club’s social media pages. The team that wins **Best Overall Project** will earn spots on the UW–Madison team for MUDAC, a regional statistical analysis competition held in the spring, with full travel funding provided.

## Presentations:
Your group will prepare a three to five minute presentation of your data analysis, followed by questions from the audience. The goal of the presentation is to practice presenting statistical findings in a concise and clear manner. The presentation should include key evidence (e.g. plots, tables, inferential methods, etc.) that support your findings. Your presentation must be clear and precise enough so that the audience will be able to understand which statistical analyses you used and how you have reached your conclusions.

The requirements for the presentation are as follows:
-  Due to time constraints, the five-minute time limit will be strictly enforced.  While we will provide time cards and warnings for you during the presentation, it is ultimately your responsibility to rehearse your presentation so that it stays under five minutes. 
-  Each member of your group must speak for at least 1 minute during the five-minute presentation. 
- All members of the group must work on the presentation and be prepared to answer 1-3 short questions about the presentation from the audience (including the judges and other participants).

The exact time of your group’s presentation will be determined randomly on the day of the presentation.

## Written Report:

Your group must submit a one to two page report of the data analysis. In particular, the report should include (1) your **overall findings**, (2) relevant and important **evidence** for your findings (e.g. plots, tables), and (3) important **details of your statistical analysis** (e.g. type of model used, inferential quantities, outliers, leverage points, modeling assumptions, etc.). Your report should be detailed enough that any data scientist can read it and replicate your analysis.

The requirements for the executive report are as follows: 

- Typed in 12-inch Times New Roman or Arial, single-spaced, 1-inch margins 
- Include all relevant figures/tables, equations, and references 
- Must be legible 
- Must not exceed two pages 
- You may follow any reasonable guidelines for formatting the references (Ex. MLA, APA, Chicago Manual of Style, etc.)

## Submission

### Checkpoint  
> Submit a zipped folder containing your exploratory data analysis code.  
> Email the folder with the subject line **`Data Challenge Checkpoint`** to [Spencer](mailto:svenancio@wisc.edu) by **October 13, 2024**.  

### Final  
> Submit a zipped folder labeled with your team name. This folder should include:  
> - Slides for your presentation (PPT or PDF)  
> - Executive report (PDF)  
> - Code used for analysis  
>   
> Email the folder with the subject line **`Data Challenge Submission`** to [Spencer](mailto:svenancio@wisc.edu) by **11:59 PM on October 24, 2024**.  



# Data Challenge Rubric (Fall 2025)

| Category            | Criteria | Description | Points |
|---------------------|----------|-------------|--------|
| **Write-up / Model** (25 pts) | W1 | Introduces the dataset, context, and purpose of the analysis. Includes a well-defined thesis or research question. | 5 |
|                     | W2 | Justifies the choice of data analysis methods or predictive techniques, explaining why they fit the problem or dataset. | 5 |
|                     | W3 | Explains key findings clearly and concisely, including parameter estimates (if applicable) and their significance. Avoids unnecessary output. Interprets results in accessible terms. | 5 |
|                     | W4 | Assesses strengths and weaknesses of chosen methods, checking assumptions and diagnostics (e.g., overfitting, bias-variance, validation performance). | 5 |
|                     | W5 | Evaluates predictive or explanatory accuracy using appropriate metrics and validation. | 5 |
| **Presentation** (25 pts) | P1 | Communicates key messages and conclusions clearly, leaving the audience with a strong understanding of the findings. | 5 |
|                     | P2 | Uses visuals (plots, charts, tables) that are clear, relevant, and easy to follow. Explanations are concise and accessible. | 5 |
|                     | P3 | Demonstrates that methods are statistically sound; addresses strengths and weaknesses. Interprets results correctly and highlights insights. | 5 |
|                     | P4 | Provides strong evidence and logical reasoning to support conclusions. Connects analysis to findings effectively. | 5 |
|                     | P5 | Delivers the presentation clearly and engagingly. Maintains audience understanding throughout. | 5 |

**Total: 50 points**



## Rules and Academic Integrity

Each student assumes the responsibilities of an active participant in UW–Madison’s community of scholars. All academic work and behavior are held to the highest standards of integrity. Academic misconduct compromises the integrity of the university. Examples of misconduct include cheating, fabrication, plagiarism, sabotaging other groups’ work, unauthorized collaboration, and helping others commit these acts.

---

### Specific Guidelines

- **No copying, plagiarizing, or stealing** deliverables from other groups, students outside of the club, or the Internet.  
- You may ask other groups about general ideas or questions. However, **you cannot** ask them for help cleaning, analyzing, or interpreting the dataset.  
- **Directly copying, paraphrasing, or using existing analyses** of the competition dataset is prohibited. Examples include:  
  - Online course materials  
  - Blog posts or published notebooks  
  - Pre-written scripts or APIs that automatically perform analysis (e.g., sentiment analysis tools)  
- You are **encouraged** to browse for background information. Using external resources to provide context is acceptable as long as you give proper attribution and ensure the analysis itself is your own work.  
- Your team’s analysis must be **original** and reflect your own effort. In industry terms: *do not steal others’ intellectual property*.  
- You may not ask anyone outside your group to perform any part of the analysis on your behalf.  

---

### Use of AI Tools

AI tools (e.g., ChatGPT, Copilot) are permitted under **standard academic integrity policies**. We want participants to gain *real-world experience*, where the use of AI is increasingly common.  

However:  
- If AI is used, your team must still be able to **explain, justify, and defend** all decisions made in your analysis.  
- Failure to demonstrate understanding of your own work because of overreliance on AI will be considered a **serious penalty**. It will heavily impact the quality assessment of your project.  

---
### External Research and Data

We highly encourage students to develop at least a basic domain knowledge in **macroeconomics** and related areas. Statistics is an applied discipline, and meaningful analysis often requires some understanding of the subject matter.  

Using external resources is allowed and encouraged, but it comes with important responsibilities:  

- **Cite your sources.** Any external materials, whether academic papers, chatbots, websites, or data repositories, must be properly attributed.  
- **Use external data carefully.** It is fine to bring in outside data to complement the provided dataset, but the majority of your analysis should remain grounded in the official competition data.  
- **Balance your work.** If your analysis relies too heavily on outside sources, or if external data begins to overshadow the provided resources, your project may stray too far from the challenge’s intent. Some extension is acceptable, but the focus should stay connected to the given dataset.  
- **Proceed with caution.** Background knowledge is meant to enrich your analysis, not replace it. The strongest projects will combine domain knowledge with careful statistical reasoning.  

---

**Bottom line:** Use resources responsibly, give credit where it is due, and make sure you fully understand and can explain every part of your team’s work.  



