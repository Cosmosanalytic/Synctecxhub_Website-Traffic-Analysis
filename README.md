WEBSITE TRAFFIC ANALYSIS
Power BI Dashboard —Project


1.  Project Introduction

This project presents a comprehensive analysis of website traffic data using Microsoft Power BI Desktop. The dashboard was developed as part of a structured data analytics training programme, designed to demonstrate professional-grade skills in data modelling, DAX calculation, and business intelligence reporting.
The dataset originates from Google Analytics 4 (GA4) exports and covers user acquisition and engagement metrics segmented by session channel group, enabling a clear view of which marketing channels drive the most traffic and the highest-quality user engagement.

2.  Project Overview

The project centers on a single Power BI data model built from a GA4 website traffic export table. Seven DAX measures were engineered to quantify user volume, session quality, and engagement behavior, while a custom calculated column, Channel Group Performance Tier, was developed to automatically classify each row by its channel’s performance rank, embedding the actual channel name and star rating into the label.

Dataset At a Glance
Table:  Website Traffic   │   Rows: Multi-date, multi-channel   │   Source: Google Analytics 4 (GA4)

Columns in the dataset:
•	Session Channel Group — marketing acquisition channel
•	Date — daily session date
•	Sessions, Users, Engaged Sessions, Event Count
•	Average Engagement Time Per Session, Engagement Rate, Events Per Session, Engaged Sessions Per User

3.  Tools & Technologies Used


Tool / Technology	Category	Purpose
Microsoft Power BI Desktop	Business Intelligence	Dashboard design, DAX modelling, data visualization
DAX (Data Analysis Expressions)	Query & Calculation Language	KPI measures, calculated columns, and time intelligence
Power BI MCP Integration	AI-Assisted Development	AI-powered model operations via Claude MCP connector
Google Analytics 4 (GA4)	Data Source	Raw website traffic & user engagement export
Microsoft Excel / CSV	Data Preparation	Raw data staging and initial review

4.  Business Question

“Which website traffic source channels are driving the highest volume of sessions and the strongest user engagement, and how can this knowledge shape smarter marketing investment decisions?”

Supporting analytical questions explored in this project include:
•	Which channel groups generate the highest total sessions and unique users?
•	Which channels produce the most engaged sessions and the lowest bounce behavior?
•	Where is the average engagement time per session highest across channels?
•	How do top-performing channels compare against lower-tier channels in event generation?
•	Which channels represent the best return on traffic investment?

5.  Business Problem Solved

Marketing and digital teams often struggle to evaluate channel performance beyond surface-level session counts. Without a structured analytical view, budget allocation decisions risk favoring high-volume but low-quality channels over those generating genuinely engaged users who are more likely to convert.
This project addresses that gap by building a data model that goes beyond raw traffic numbers to surface engagement quality metrics, enabling stakeholders to identify not just where traffic is coming from, but which channels are delivering meaningful user experiences. The automated Channel Group Performance Tier column further eliminates the need for manual channel classification in every report.

6.  Key KPIs


162,895
Total Sessions
Across all channels	133,440
Total Unique Users
Distinct visitors	90,132
Total Engaged Sessions
Active engagements

770,911
Total Event Count
User interaction events	50.3%
Overall Engagement Rate
Avg across all channels	66.6s
Avg Engagement Time
Per session average

DAX Measures Developed
•	Total Sessions — SUM of all recorded sessions
•	Total Users — SUM of unique users
•	Total Engaged Sessions — SUM of engagement-qualified sessions
•	Engagement Rate — Engaged Sessions / Total Sessions × 100
•	Avg Engagement Time Per Session — Weighted average engagement time in seconds
•	Total Event Count — SUM of all tracked user events
•	Engaged Sessions Per User — Total Engaged Sessions / Total Users

 
7.  Key Insights


Channel Group	Sessions	Users	Engaged Sessions	Event Count	Eng. Rate	Avg Eng. Time (s)
#1 Organic Social	60,627	47,572	32,697	296,631	54.1%	53.5s
#2 Direct	37,203	30,042	17,243	156,318	45.6%	45.5s
#3 Organic Search	33,372	28,387	19,425	136,957	57.9%	47.0s
Referral	30,990	26,774	20,653	177,992	66.1%	92.7s
Organic Video	141	123	109	1,071	76.0%	180.4s
Unassigned	559	540	4	1,932	0.75%	79.0s
Email	3	2	1	10	33.3%	72.7s

Insight 1 — Organic Social is the Traffic Leader
Organic Social generated 60,627 sessions, nearly 37% of total website traffic, making it the single dominant acquisition channel. With 47,572 unique users and 296,631 total events, it drives not only volume but also meaningful user interaction, reflecting a highly active social media presence.
Insight 2 — Referral Delivers the Highest Engagement Quality
Despite ranking 4th in session volume (30,990 sessions), Referral produces the highest average engagement time per session at 92.7 seconds and a 66.1% engagement rate, both the best among all channels. This suggests referral traffic arrives with strong intent, likely driven by trusted third-party sources.
Insight 3 — Organic Search Outperforms Direct in Engagement Quality
Organic Search ranks 3rd in sessions (33,372) but achieves a 57.9% engagement rate, outperforming Direct (45.6%). This indicates that users arriving via search queries are more purposeful and engaged than those navigating directly, a strong signal of effective SEO and relevant content alignment.
Insight 4 — Organic Video Shows Exceptional Engagement per Session
Despite minimal traffic volume (141 sessions, 123 users), Organic Video records the highest average engagement time at 180.4 seconds per session and a 76% engagement rate. This indicates that video-referred audiences, though small, arrive highly motivated and spend significantly more time on-site.
Insight 5 — Direct Traffic Has the Weakest Engagement Rate Among Top Channels
Direct traffic ranks 2nd in volume (37,203 sessions) but records the lowest engagement rate among the top three channels at 45.6%. This may suggest branded traffic that does not always convert to active engagement, or a proportion of bot/automated visits inflating raw session numbers.

8.  Recommendations

Scale Organic Social Investment
As the highest-volume channel with strong event engagement, Organic Social merits increased content investment. Teams should prioritize consistent posting cadence, community interaction, and creative formats proven to drive traffic to maintain and grow this channel’s lead.
Prioritize Referral Partnership Development
Referrals’ quality metrics far exceed its volume, suggesting untapped potential. A targeted strategy to expand referral sources, including guest publishing, influencer partnerships, and industry directory listings, could significantly increase high-intent traffic without inflating ad spend.
Strengthen SEO to Grow Organic Search
Organic Search’s strong engagement rate validates its strategic value. Investing in keyword optimization, long-form content, and technical SEO improvements should be prioritized to increase session volume while maintaining the quality of intent-driven visitors.
Investigate and Improve Direct Traffic Engagement
The relatively low engagement rate of Direct traffic (45.6%) warrants investigation. This could indicate a poor landing page experience for returning visitors or an inflated session count from automated traffic. A/B testing landing pages and filtering bot traffic in GA4 are recommended first steps.
Explore Organic Video as a Growth Channel
The quality signals from Organic Video, 180+ second engagement time, and 76% engagement rate, are exceptional. Scaling video content output and ensuring strategic call-to-action placement within video content could convert this niche channel into a high-value traffic source.

9.  Conclusion

This Website Traffic Analysis project successfully delivers a structured, insight-driven view of digital channel performance using Power BI Desktop. By combining seven engineered DAX measures with a dynamic Channel Group Performance Tier calculated column, the model enables decision-makers to move beyond raw traffic counts and focus on the quality of user engagement each channel delivers.
The analysis reveals that while Organic Social leads in volume, Referral and Organic Search offer superior engagement quality, and Organic Video, despite minimal volume, shows remarkable depth of engagement. These nuanced differences are invisible without structured analytical modelling.
The project demonstrates a professional-grade application of Power BI, DAX, and AI-assisted model development (via MCP integration), and serves as a portfolio-ready artefact illustrating competency in business intelligence, data storytelling, and actionable insight generation.

About the Author

Cosmos Isuru
Data Analyst  │  Power BI Developer  │  Business Intelligence Specialist 
Specializes in data analytics, HSE/Safety analysis, dashboard development, and business intelligence reporting, with a focus on delivering clear, actionable insights from complex datasets using Power BI and DAX.

Project: Website Traffic Analysis   |  Tool: Microsoft Power BI Desktop  | 
