# European-League-Football

# European Football League Analysis (20/21 – 24/25)

This project investigates the long-standing debate: Is the Premier League really the “best league in the world,” or are other top European leagues unfairly dismissed as “farmers' leagues”?


## Data Scope

Leagues covered: Bundesliga, EPL, La Liga, Ligue 1, Serie A

Seasons analysed: 2020/21 – 2024/25

---
## Key Insights and Metrics used

### ⚡ Match Intensity

The intensity metric was constructed as a weighted aggregate of fouls committed, yellow cards, and red cards per match, normalised across leagues to ensure comparability. Intensity captures the physical engagement in matches — leagues where players are more often fouled or booked suggest tighter defensive play or less tolerance for skilful dribblers.

Statistically, this captures the rate of disciplinary actions per 90 minutes as a proxy for physicality and aggressiveness in play. 
La Liga’s significantly higher intensity score (36.16 vs. EPL’s 29.12) reveals a stronger central tendency toward fouls and bookings, suggesting higher variance in match disruption. This contradicts the popular narrative of the Premier League being “the most physical”, as the data indicate La Liga systematically generates more stoppages and disciplinary incidents. 

A possible explanation, from a statistical bias perspective, is that flair and technical dribbling in La Liga induce defenders to commit fouls, inflating intensity values relative to leagues where play is more direct.

### 🎯 Match Quality

Quality was measured through a weighted index that incorporated average goals per game, Shots on target, and shot conversion rate. 

The Bundesliga’s highest score (29.23) reflects both high offensive production (3.14 goals per match mean, with a relatively low variance in scoring outcomes) and attacking efficiency. A higher composite score indicates an environment that fosters high-scoring and entertaining football.

From a statistical standpoint, this points to a distribution skewed toward goal-rich environments, where kurtosis is lower (i.e., fewer low-scoring outliers). La Liga’s lower score (25.53) contrasts its reputation for technical brilliance, suggesting that while it excels in intensity, 
it lags in measurable scoring efficiency relative to peers. The finding underscores the importance of distinguishing between qualitative perceptions of “beautiful football” and quantifiable offensive output.


### 🏆 Top 5 Teams’ Win Share 

This metric was calculated as the proportion of total league wins accounted for by the top five teams over the period analysed, effectively a concentration ratio. It measures dominance and competitive balance at the top. A higher value indicates concentration of success in elite teams, while lower values reflect a more distributed competition.

$$
\text{Win Share} = \frac{\text{Wins by Top 5 Teams}}{\text{Total Wins in League}}
$$

The Premier League’s dominance score (0.53) demonstrates a higher level of win concentration than La Liga (0.50) or Ligue 1 (0.49). The Premier League recorded the highest win share (0.53), meaning the "big clubs" dominate more heavily compared to La Liga (0.50) and Ligue 1 (0.49). This suggests the EPL’s appeal may hinge on top-heavy rivalries, though competitiveness outside the top 5 might be weaker. 

However, the framing around “Top 5” may bias results in favour of leagues with deeper competitive depth (e.g., EPL) rather than those with extreme dominance by a top one or two teams (e.g., PSG in Ligue 1, Real/Barça in La Liga, Bayern in Bundesliga, although in recent years, Man City have dominated the EPL, winning 4 titles in the last 5 years and 6 in the last 8 years).


### ⚽ Competitiveness

Competitiveness was assessed via the standard deviation of win percentages across all teams in each league, a robust measure of dispersion around the mean. Lower values suggest tighter clustering, i.e., higher parity. 

$$
\sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}\left(p_i - \bar{p}\right)^2}
\quad\
$$

Where $$\bar{p}$$ = League Average, and

$$p_i$$  = Win Percentage of each Team

The Bundesliga and Ligue 1 both record 0.13, which reflects a more homogeneous distribution of team performance, whereas the EPL’s 0.14 indicates slightly higher variance, translating into greater disparity between its best and worst teams. From an inferential perspective, this variance difference, though numerically small, is statistically meaningful in shaping perceptions of league unpredictability. 

A tighter standard deviation implies a flatter distribution where outcomes are less predictable, increasing competitive balance. By contrast, a higher deviation in the EPL supports the perception of top-team dominance but also makes mid-table variance more pronounced.


### Other Metrics used include:
* Average Goals Per Match
* Home/Away Wins
* Win Percentage
* Draw Percentage

---


## ✅ Conclusion

The data reveals that the Premier League is not superior across all metrics. Instead:

* La Liga = intensity & physical battles
* Bundesliga = goals & attacking quality
* Ligue 1 = balanced competition
* EPL = global dominance & top-team strength

This project demonstrates how perceptions differ from reality and invites fans to appreciate the unique value each league brings to European football.

