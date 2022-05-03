# Reddit-Analysis
The goal for this project is to conduct a sentiment analysis to classify the posts into different moods. We will explore millions of posts, classify them into different politic topics and then analyze the mood for all the posts under each topic, trying to tell the altitude of these posts.
<table border="0" style="width:100%;">
	<tbody>
	    <tr style="background-color:#FFFFFF;">
			<td colspan="2" style="width: 50%; text-align: right; vertical-align: top; line-height:150%">
			    
			    <h2 style="text-align: left;">SUMMARY</h2>
			    <br />
			    <br />
			    <p style="font-size:150%"><strong>Right Gains a Higher Post Score</strong></p>
			    
			    <p style="font-size:100%">The posts from right related author_flair type tend to have a higher score, no matter whether the posts are from authors of Authoritarian or Libertarian.</p>
			</td>
			<td style="width:50%; text-align: center;"><img alt="" src="/anly502/conclusion/fig1.png" style="width: 700px; height: 570px;" /></td>
		</tr>
		<tr style="background-color:#FFFFFF;">
			<td colspan="2" style="width: 50%; vertical-align: middle; line-height: 150%; text-align: center;">
			    <table align="center" border="0" cellpadding="0" cellspacing="0" style="line-height:10%; font-size:80%;" width="800">
				<tbody>
					<tr height="21">
						<td colspan="5" height="21"><strong>Summary table by topic</strong></td>
					</tr>
					<tr height="21">
						<td height="21" width="150"><strong>Sentiment</strong></td>
						<td align="right" width="85"><strong>Positive</strong></td>
						<td align="right" width="85"><strong>Neutral</strong></td>
						<td align="right" width="85"><strong>Negative</strong></td>
						<td align="right" width="125"><strong>Pos-Neg Ratio</strong></td>
					</tr>
					<tr height="21">
						<td height="21"><strong>Covid</strong></td>
						<td align="right">12548</td>
						<td align="right">1813</td>
						<td align="right">20020</td>
						<td align="right">0.63</td>
					</tr>
					<tr height="21">
						<td height="21"><strong>Election</strong></td>
						<td align="right">20562</td>
						<td align="right">2516</td>
						<td align="right">21120</td>
						<td align="right">0.97</td>
					</tr>
					<tr height="21">
						<td height="21"><strong>Economics</strong></td>
						<td align="right">62773</td>
						<td align="right">4979</td>
						<td align="right">52316</td>
						<td align="right">1.20</td>
					</tr>
					<tr height="21">
						<td height="21"><strong>Finance</strong></td>
						<td align="right">13928</td>
						<td align="right">1517</td>
						<td align="right">13579</td>
						<td align="right">1.03</td>
					</tr>
					<tr height="21">
						<td height="21"><strong>Gender Equality</strong></td>
						<td align="right">43667</td>
						<td align="right">2021</td>
						<td align="right">14229</td>
						<td align="right">3.07</td>
					</tr>
					<tr height="21">
						<td height="21"><strong>Racial Equality</strong></td>
						<td align="right">98744</td>
						<td align="right">15071</td>
						<td align="right">157961</td>
						<td align="right">0.63</td>
					</tr>
				</tbody>
			</table>
			</td>
			<td colspan="1" style="width: 50%; text-align: left; vertical-align: middle; line-height:150%">
			<p style="font-size:150%"><strong>Different Contents, Different Sentiments</strong></p>

			<p style="font-size:100%">COVID and Racial Equality related posts tend to have a larger proportion of negative sentiment, while Economics and Gender Equality related posts are likely to be more positive.</p>
			</td>
		</tr>
		<tr style="background-color:#FFFFFF;">
		    <td colspan="2" style="width:50%; text-align: right; vertical-align: middle; border:0;">
			<p style="font-size:150%">
			<strong>Different Topics, Different Keywords, Different Sentiments</strong></p>

			<p style="font-size:100%">LDA, one of the most famous topic modeling methods was utilized here to define a topic for each post. It can be recognized that some specific topics tend to be more positive, while some are not. Some keywords appear in more than one topic, so those unique words will explain more for the topics. The average Pos-Neg Ratio of all posts is 1.64, while the ratio of Topic 4 (more about accusation) is only 1.13, compared to 3.94 for Topic 3 (more about improvement)</p>
			</td>
		    <td colspan="2" style="width: 50%; text-align: left; vertical-align: middle; line-height:10%">
			    <table align="center" border="0" cellpadding="0" cellspacing="0" style="line-height:100%; font-size:80%;" width="800">
				<tbody>
				    <tr height="21">
						<td colspan="2" height="21"  style="text-align: center;"><strong>Summary Table of Topic (Average Pos-Neg Ratio: 1.64)</strong></td>
					</tr>
					<tr style="background-color:#FFFFFF;border-color:#FFFFFF;">
						<td align="right" style="vertical-align: middle;"><img alt="" src="/anly502/ml/topic_1.png" style="width: 350px; height: 105px;" /></td>
						<td align="left" style="vertical-align: middle;"><strong>Topic 0 <br>Keywords: senator <br> Pos-Neg Ratio: 2.05</strong></td>
					</tr>
					<tr style="background-color:#FFFFFF;border-color:#FFFFFF;">
						<td align="right" style="vertical-align: middle;"><img alt="" src="/anly502/ml/topic_2.png" style="width: 350px; height: 105px;" /></td>
						<td align="left" style="vertical-align: middle;"><strong>Topic 1 <br>Keywords: short, das<br> Pos-Neg Ratio: 1.61</strong></td>
					</tr>
					<tr style="background-color:#FFFFFF;border-color:#FFFFFF;">
						<td align="right" style="vertical-align: middle;"><img alt="" src="/anly502/ml/topic_3.png" style="width: 350px; height: 105px;" /></td>
						<td align="left" style="vertical-align: middle;"><strong>Topic 2 <br>Keywords: integrate, conspiracy<br> Pos-Neg Ratio: 1.46</strong></td>
					</tr>
					<tr style="background-color:#FFFFFF;border-color:#FFFFFF;">
						<td align="right" style="vertical-align: middle;"><img alt="" src="/anly502/ml/topic_4.png" style="width: 350px; height: 105px;" /></td>
						<td align="left" style="vertical-align: middle;"><strong>Topic 3 <br>Keywords: improvement<br> Pos-Neg Ratio: 3.94</strong></td>
					</tr>
					<tr style="background-color:#FFFFFF;border-color:#FFFFFF;">
						<td align="right" style="vertical-align: middle;"><img alt="" src="/anly502/ml/topic_5.png" style="width: 350px; height: 105px;" /></td>
						<td align="left" style="vertical-align: middle;"><strong>Topic 4 <br>Keywords: officer, hillary, accusation<br> Pos-Neg Ratio: 1.13</strong></td>
					</tr>
				</tbody>
			</table>
			</td>
		</tr>
		<tr style="background-color:#FFFFFF;vertical-align: middle;">
		    <td><img alt="" src="/anly502/ml/fig_summary.png" style="width: 650px; height: 568px;" /></td>
		    <td colspan="2" style="width:50%; text-align: left;vertical-align: middle;"> 
		    <p style="font-size:150%"><strong>Posts' Moods Can Indeed Affect Stock Prices</strong></p>
			<p style="font-size:100%">Since political factor is always an essential feature of stock market, these subreddit posts may have an impact on the stock prices. According to the time series plot of Nasdaq Index, the predictions is pretty close to the real close prices. And the best model uses the last 60 days' historical data to make a prediction of the next day price. </p>
			</td>
		</tr>
		<tr style="background-color:#FFFFFF;">
		    <td colspan="2" style="width: 50%; vertical-align: top; text-align: left;">
			    <h2 style="font-size:100%">What's next?</h2>
			    <br />
			    <p style="font-size:100%"><strong>US Elections</strong> are one of the most important and worldwide concerned events, since a different president may thoroughly change the situation in the world. Our topic here is about the subreddit #PoliticalCompassMemes, which is apparently highly related to the US elections. Therefore, we will try to extend this project to conduct some researches about the relationship between the posts and the daily and final results of 2020 US elections. 
			        
			    </p>
			</td>
			<td><img alt="" src="/anly502/conclusion/election.png" style="width: 650px; height: 450px;" /></td>
		</tr>
	</tbody>
</table>
