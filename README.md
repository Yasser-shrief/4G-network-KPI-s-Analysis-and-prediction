# 4G-network-KPI-s-Analysis-regression
4G network KPI's Analysis &amp; regression including Dashboard 

A typical 4G network consists of several nodes connected to each other, where each node serves users in the surrounding area. While users are accessing network services, their mobile phones record Key Performance Indicators (KPI’s) which can help network operators in assessing their quality of service.<br>
There are many KPI’s which evaluate different aspects of the network. For example, RSRP (Reference Signals Received Power) is a KPI which measures the network coverage in the user’s location. Traffic Volume is another KPI which measures how much data has been consumed by the user.

For this challenge, I have two crowdsourced datasets: RSRP and Traffic Volume. Each dataset has the corresponding KPI measurements collected from mobile phones of different users over a week. It also includes the user’s location, operator, phone model and other information. Note that the data is in its raw format <br>

The **dashboard** MUST include these 4 charts:
1. A time-lapse of a density map showing how users move during the hours of the day. You should see the density on the map changing according to people’s activities every hour. Use the locations in RSRP dataset.<br>
2. A heat map of user locations for a selected operator colored by RSRP value with a dropdown menu to choose the operator.<br>

3. A bubble map showing the areas with high downlink traffic for each operator. Each bubble represents an area on the map and the area covered by this bubble can be controlled with a slider. In this chart, the bubble size depends on the sum of the Traffic Volume of all users in this area and it’s colored per operator.<br>
4. A Bar chart of RSRP per device type per operator with an option to choose the aggregation method of RSRP (avg, min, max and 90th Percentile). Add a slider to control the minimum number of users of each device

Assume that the target audience is one of the operators in the dataset. What do you think this data uncovered for them?
Examples of these findings can be:<br>
• Areas having good or poor coverage compared to competitors <br>
• Certain mobile phones that suffer from poor performance <br>
• Traffic hotspots for operators

The dashboard [here](https://datastudio.google.com/u/0/reporting/ed6fce84-afb4-4ae8-88a8-4f455fde60b0/page/iLVVC)

## Part2: Machine learning

Imagine you are running a conversation with one of the operators whose data is in the dataset provided. The discussion is referring to any polygon of your choice that’s at least **10km x 10km** size and has enough data samples. Can you help the operator to answer the questions below?<br>

1. Assuming that the coverage next week will improve in that polygon compared to competition (i.e., RSRP will get better than other operators). What would be the impact on downlink and uplink traffic volumes?<br>
2. Samsung devices are the main handsets in our network. Can you predict the traffic volume growth, uplink and downlink, over time for these devices and compare it to the competitors?


