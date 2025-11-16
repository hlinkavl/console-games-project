# Project Background 🖼️
Recently, companies worldwide across various industries have been discovering marketing opportunities in video games and esports. From content creator partnerships and fan events like Red Bull Solo Q to digital in-game branding—such as Adidas banners in FIFA or Barack Obama’s campaign billboards in Madden NFL—the gaming sector offers unique avenues for audience engagement. Before entering the ecosystem of video games as an advertiser or strategic partner, it is essential to consider key areas like:

- **Market Size and Growth**
- **Video Game Popularity (Sales) by Title & Console**
- **Popular Genres in the Region**

The original dataset can be found on [Kaggle](https://www.kaggle.com/datasets/asaniczka/video-game-sales-2024).

The Excel spreadsheet containing transformed dataset & ad hoc analysis can be found [here](data_pivot_tables.xlsx).

Power BI file used to report and explore sales trends can be found [here](vg_sales_dashboard.pbix).



# Data Structure & Initial Checks ✔️

The original dataset provides information about game title, genre, device, critic score, total sales, sales in Europe/North America/Japan/Other. After removing rows with incomplete records and adding an index column, the dataset was transformed – columns containing regional sales were unpivoted and then filtered, so only the top 100 games were left. The original table was split into 2 fact tables and 1 dimensional as you can see below:

![Data model](relationship_diagram.png)



# Executive Summary 🔑

### Overview of Findings

The console video game market is primarily led by major franchises such as Call of Duty in the shooter genre and Grand Theft Auto in the action genre. Sales are almost balanced between PlayStation and Xbox, with major titles usually available on both platforms. While Europe and North America exhibit similar genre preferences, Japan demonstrates a strong inclination towards role-playing games. Annual sales by region fluctuate based on the popularity of new releases.

![Dashboard screenshot](dashb.png)



# Insights Deep Dive 🔎
### Market Size & Growth:

Between 2009 and 2011, the console video game market saw significantly high revenue, largely due to the popularity of the Call of Duty series, which dominated sales at the time. After 2014, revenues began a gradual decline, likely influenced by the rise of PC games based on microtransaction models. Unlike traditional console games, which require players to purchase the game upfront, many PC games with microtransactions are freely available to download, allowing players to gradually spend smaller amounts within the game. This model has been particularly appealing as it reduces the barrier to entry and enables flexible spending, drawing some players away from console titles. Looking ahead, the console gaming market is expected to stabilize or slightly decline, with occasional revenue spikes likely when particularly popular titles are released. With the modern trend of multi-platform releases—including games that support crossplay on both PC and consoles—a steady revenue stream for consoles is likely, though still lower than for PC gaming.


### Genres and Titles by Region:

Player preferences in North America and Europe are generally similar, with both regions favoring action and shooter genres. The primary difference lies in the popularity of sports games. In Europe, the FIFA series leads the sports genre due to the region’s strong cultural affinity for soccer, while in North America, Madden NFL holds the top spot in sports. However, sports games in North America do not achieve the same level of sales as other popular genres. Meanwhile, role-playing games (RPGs) such as Skyrim and the Fallout series enjoy higher sales in North America, a preference that is even more pronounced in Japan, where the RPG genre is particularly strong, driven by the enduring popularity of the Final Fantasy series.


### Regional Market Share Trends:

Over the years, regional market shares in console gaming have undergone noticeable changes. For many years, North America led with a substantial share, peaking in 2010 when it accounted for as much as 60% of global console gaming revenue. However, these regional disparities have gradually diminished, and an eventual shift occurred where Europe surpassed North America in market share. This shift was largely driven by the consistent popularity of Grand Theft Auto in Europe and the annual release cycle of the FIFA series.

![market shares](shares.png)
  


# Recommendations 📋

Based on the insights and findings above, I would recommend any organization willing to enter the gaming ecosystem to consider the following: 

### Focus on the Sports Genre in Europe for Long-term Growth
The sports genre has shown steady revenue growth in Europe over the long term, a trend that sets this market apart from the U.S. and Japan, where revenues in the genre have declined. This stability in Europe makes sports games a strong choice for sustained investment in the region. By associating with popular sports titles, a commercial partner can leverage the consistent demand for sports-related content to build a loyal customer base.

### Strategic Positioning in the U.S. with Proven Genres and Titles
In the U.S., proven genres like shooters offer a clear path to high engagement and revenue potential. However, associating with shooters may not align with every brand’s image. In that case, a better strategy could be to back new or unique action titles that frequently experience major marketing success. Titles such as Uncharted, Red Dead, and the Batman series have illustrated that non mainstream action games can achieve impressive reach and resonance with American audiences. Investing in the action genre allows partners to capitalize on impactful marketing while exploring unique narratives that align with their brand identity.

### Tap into Nostalgia to Reach Gamers with Spending Power
The nostalgia factor is a powerful tool to capture the interest of gamers who grew up with classic consoles and now have the means to invest in their hobbies. Many players who enjoyed titles from the ’90s and early 2000s, such as Mario Kart, Street Fighter, or the original Final Fantasy games, are now more likely to spend on experiences that rekindle fond memories.

By partnering on remakes, exclusive retro merchandise, or revamped editions of these iconic games, brands can create campaigns that appeal to both sentiment and spending power. This approach taps into an audience ready to invest in products that evoke the cherished gaming experiences of their past while exploring new, enhanced versions of these classics.



# Assumptions and Caveats ⚠️

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* The analysis considers only the top 100 most popular unique games; games with the same title released on multiple platforms are counted separately
  
* To simplify data interpretation, it is assumed that all sales (sum of sales) per game were made during the game's release year
  

