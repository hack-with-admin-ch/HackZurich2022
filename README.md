# Make climate change tangible with Swiss open data

Welcome to “Hack with Admin CH”. In this repository, you will find all the information and tools you need to master our challenge. You can find more information about the challenge, our partners and us at <http://bit.ly/3kJVNzK>.

Before you read any further, please note that this documentation is still a work in progress; we will continue to update the repository until the start of the event. If you want to stay up to date, we’d suggest you “watch” the repository.

**We will add some Python Jupyter notebooks showing how to access the data.**

If you have any questions or further commentary regarding the documentation and provided code, feel free to get in touch with us by participating in discussions, creating issues or pull requests.
**You can also reach us in Discord [Channel #18-foitt-fso](https://discord.com/channels/987004253711245342/1011653890585927724).**

## Challenge description

While recent events let us have a glimpse at what our future in a world of rising global temperatures and increasingly hot and dry summers might look like, climate change and its impact on our everyday lives is a complex issue. While both historical data and official scenarios are available to us, truly grasping the scope, the "feel" of climate change remains difficult.

That's where our challenge comes in: **help us make climate change more tangible by developing a solution that allows citizens to access and comprehend the information provided by the federal administration in an innovative way!**

### You can tackle the challenge from different angles

- **Adopt a historical perspective:**
Based on historical data, how has climate change changed our lives and our environment in recent years?  
[For example, this is how annual mean temperatures betwen 1864 and 2017 have evolved](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/swiss-climate-change-scenarios/observed-climate-change-in-switzerland/_jcr_content/par/slideshow/images/190_1540816017406/image.imagespooler.png/1540918023575/Jahresmitteltemperatur%201864-2017_V01.png)

- **Adopt a forward-looking perspective:**
Based on the official CH2018 climate scenarios, what’s our future going to «feel» like?  
[For example, deglaciation in the Alps is accelerating](https://twitter.com/matthias_huss/status/1567110247910674432?t=85bJlouRU7A57Mm2aWKEyQ&s=03)

From a "simple" visualisation to innovative infographics, from an AR / VR solution to a game, surprise us!
**Can you think of innovative solutions that inform citizens and help lower the «low sense of urgency» barrier?**

## Background

As stated in the [sixth assessment report of the IPCC](https://www.ipcc.ch/assessment-report/ar6/), global temperatures have already risen to 1.1°C above pre-industrial levels, affecting both natural and human systems in Europe. After this past summer, it's become quite clear that the impacts of compound heatwaves and droughts have become more frequent, with largely negative impacts projected for southern regions. Rising temperatures, loss of biodiversity and an increased frequency of extreme weather events – recent years seem to support what a lot of scientific data shows: the climate has changed, and climate change is accelerating. As an Alpine country, [Switzerland is particularly impacted by these changes](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/swiss-climate-change-scenarios/observed-climate-change-in-switzerland.html).

![observed changes](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/swiss-climate-change-scenarios/observed-climate-change-in-switzerland/_jcr_content/par/image/image.imagespooler.png/1540829704666/infografik_obs_change_V01.png)
For instance, already today, Switzerland has experienced a long-term **warming around two times higher** than the global average. As a consequence, [snow cover has diminished](https://tc.copernicus.org/preprints/tc-2020-289/tc-2020-289.pdf), hot days and heavy precipitation have become more frequent and more intense, the vegetation period has been extended and the [zero-degree line has risen](https://rmets.onlinelibrary.wiley.com/doi/10.1002/joc.7228). And most strikingly, a very recent study has shown that the volume of the [**Alpine glaciers has shrunk by about 50 percent**](https://tc.copernicus.org/articles/16/3249/2022/) since 1931.  

The official Swiss CH2018 [Climate Change Scenarios](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/swiss-climate-change-scenarios.html) show where and how climate change affects Switzerland. The expected consequences of unchecked climate change for Switzerland include more hot days, dry summers, heavy precipitation and winters with little snow. How drastic these changes will be depending on global efforts to mitigate climate change by curbing CO2 emissions.

Possible scenario in **2060**, without mitigation: The average near-surface air temperature in Switzerland through June, July and August is about **4.5 °C warmer** than today. At the same time, there is up to **a quarter less rainfall**, and the **longest dry period without precipitation in summer lasts about 20 days instead of 11**. 

For example, in the hottest days in summer, temperatures could shoot up 5.5 °C higher than we are accustomed to now. Hot summers such as in the record year of 2003 have become the norm. Very hot days – with temperatures that used to occur only once in a year – are now occurring on average 18 times per year. [Cities are particularly vulnerable](https://www.nccs.admin.ch/dam/nccs/fr/dokumente/website/sektoren/gesundheit/hitze_staedte_2018_bafu.pdf.download.pdf/2018_OFEV_ARE_quand%20la%20ville%20surchauffe.pdf) to heat stress due to the formation of heat islands, with [effects on health](https://www.nccs.admin.ch/dam/nccs/de/dokumente/website/sektoren/gesundheit/ofev-la-canicule-et-la-secheresse-2018.pdf.download.pdf/OFEV_La%20canicule%20et%20la%20s%C3%A9cheresse%20de%20l%27%C3%A9t%C3%A9%202018%20(2019).pdf).

The official Swiss Hydro-CH2018 hydrological scenarios further indicate that climate change will also [greatly affect water availability](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/schweizer-hydroszenarien/key-messages.html) over the course of the year, with implications for our forests, agriculture, hydropower and biodiversity.

## Data

Have a look at the [Jupyter notebook `loading_datasets_example.ipynb`](loading_datasets_example.ipynb) to find examples of how to use the following datasets.

- [Swiss CH2018 Climate Change Scenarios](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/swiss-climate-change-scenarios.html)
  - With the following links, you can access the datasets. The first link will lead you to the curated list, containing the projection `MPICSC-REMO1_MPIESM_EUR11`. The second one will allow you to access the complete datasets.
    - [curated](listing_tree_curated.md)
    - [complete](listing_tree_source.md)
  - [Jupyter notebook `intro_climate_data.ipynb`](intro_climate_data.ipynb) shows how to work with that data.
- [Homogeneous data series since 1864, temp and precipitation, per month/year](https://www.meteoswiss.admin.ch/home/climate/swiss-climate-in-detail/homogeneous-data-series-since-1864.html?region=Table)
- [Klimamessnetz **Tageswerte** seit Messbeginn](https://opendata.swiss/de/dataset/klimamessnetz-tageswerte) Download gives you a text file with metadata and link to download a list of links... :-)
- [Klimamessnetz **Monatswerte**](https://opendata.swiss/de/dataset/klimamessnetz-monatswerte)
- [Climate normals precipitation 1961-1990 spatial analysis](https://opendata.swiss/de/dataset/klimanormwerte-niederschlag-1961-1990)
- [Climate normals temperature 1961-1990 spatial analysis](https://opendata.swiss/de/dataset/klimanormwerte-temperatur-1981-2010)
- [Phenological data](https://opendata.swiss/de/dataset/klimanormwerte-temperatur-1981-2010)
- [Hydro-CH2018 datasets](https://www.nccs.admin.ch/nccs/en/home/data-and-media-library/data/hydro-ch2018-datasets.html)
- [Data on lakes](https://www.datalakes-eawag.ch/)
- [Hydrological data](https://www.bafu.admin.ch/bafu/en/home/topics/water/state/data/obtaining-monitoring-data-on-the-topic-of-water/hydrological-data-service-for-watercourses-and-lakes/hydrological-data-service--products-available--with-examples-.html)
- [Glaciers monitoring](https://glamos.ch/)
- [Environmental research data](https://www.envidat.ch/#/)
- [Swisstopo lo-res LIDAR data](https://www.swisstopo.admin.ch/en/geodata/height/surface3d.html)
  - see [Jupyter notebook `lidar-processing.ipynb`](lidar-processing.ipynb) for samples on how to use that data
- [FSO STAT-TAB for direct download of px files](https://www.pxweb.bfs.admin.ch/pxweb/de/) for example [population scenarios](https://www.viz.bfs.admin.ch/assets/01/ga-01.03.01/de/index.html) by canton
- [population scenarios data links on opendata.swiss](https://opendata.swiss/de/dataset/szenarien-zur-bevolkerungsentwicklung-der-schweiz-2020-2050-bevolkerung-und-bewegungen-nach-sze)
- [greenhouse gas emissions in CH 1990-2022](https://www.bafu.admin.ch/bafu/en/home/topics/climate/state/data/greenhouse-gas-inventory.html)
- [geoportal of Federal Office for the Environment, with some historical data series](http://map.bafu.admin.ch/?lang=en&topic=bafu&X=190000.00&Y=660000.00&zoom=1&bgLayer=ch.swisstopo.pixelkarte-farbe)

## Ideas and examples

- Nice infographics: [Seven things to know about climate change in The National Geographic](https://www.nationalgeographic.com/magazine/graphics/seven-things-to-know-about-climate-change)
- [The power of visual communication and of engaging with our senses](https://www.bloomberg.com/news/features/2022-07-30/how-ai-is-giving-real-world-streets-a-virtual-makeover?s=03)
- [#Show your stripes at the University of Reading: climate stripe visualisations](https://showyourstripes.info/s/globe)
- [A similar example of climate stripes, and average temperature change visualisation in Germany](https://www.zeit.de/wissen/umwelt/2019-12/klimawandel-globale-erwaermung-warming-stripes-wohnort)
- [A nice example of heat danger visualisation from the US](https://firststreet.org/research-lab/published-research/article-highlights-from-hazardous-heat/)
- [Climate opinion factsheets: an example of climate communication from Yale University](https://climatecommunication.yale.edu/visualizations-data/factsheets/)
- [A global climate dashboard](https://climatedata.imf.org/pages/climatechange-data)
- [Seville names and categorizes heat waves](https://www.fastcompany.com/90763832/seville-is-the-first-city-to-name-and-categorize-heatwaves-like-hurricanes)

## Publications and resources

- [Swiss National Center for Climate Services, NCCS](https://www.nccs.admin.ch/nccs/en/home.html)
- [Swiss climate change scenarios, CH2018](https://www.meteoswiss.admin.ch/home/climate/climate-change-in-switzerland/climate-change-scenarios.html)
- [Swiss water bodies in a changing climate](https://www.nccs.admin.ch/nccs/en/home/climate-change-and-impacts/schweizer-hydroszenarien.html)
- [Swiss glacier monitoring, Glamos](https://www.glamos.ch/)
- [Living with heat: heat is killing more people than ever](https://www.science.org/content/article/heat-killing-more-people-ever-scientists-are-looking-ways-lower-risk?adobe_mc=MCMID%3D38579558465394467738169735892311986110%7CMCORGID%3D242B6472541199F70A4C98A6%2540AdobeOrg%7CTS%3D1656591528)
- [Impact of the warm summer 2015 on emergency hospital admissions in Switzerland](https://ehjournal.biomedcentral.com/articles/10.1186/s12940-019-0507-1)
- [Canicule de 2018: rapport de l'OFEV](https://www.nccs.admin.ch/dam/nccs/de/dokumente/website/sektoren/gesundheit/ofev-la-canicule-et-la-secheresse-2018.pdf.download.pdf/OFEV_La%20canicule%20et%20la%20s%C3%A9cheresse%20de%20l%27%C3%A9t%C3%A9%202018%20(2019).pdf)
- [Cooling in a warming world: special issue of Science](https://www.science.org/doi/10.1126/science.abf1931?adobe_mc=MCMID%3D38579558465394467738169735892311986110%7CMCORGID%3D242B6472541199F70A4C98A6%2540AdobeOrg%7CTS%3D1656591571)
- [This report collates numerous examples that show how the heat island effect can be mitigated.](https://www.nccs.admin.ch/dam/nccs/fr/dokumente/website/sektoren/gesundheit/hitze_staedte_2018_bafu.pdf.download.pdf/2018_OFEV_ARE_quand%20la%20ville%20surchauffe.pdf)
- [Trees can help reduce heat islands](https://www.epa.gov/heatislands/using-trees-and-vegetation-reduce-heat-islands)
- [MeteoSwiss blog post on climate change in the Alps: in German, but there is a link to the scientific publication in English](https://www.meteoschweiz.admin.ch/home/aktuell/meteoschweiz-blog.subpage.html/de/data/blogs/2022/5/die-alpen-_-ein-hotspot-im-klimawandel.html)
- [The Swiss alpine zero degree line](https://www.meteoschweiz.admin.ch/home/aktuell/meteoschweiz-blog/meteoschweiz-blog.subpage.html/de/data/blogs/2021/6/die-schweizer-nullgradgrenze-in-den-letzten-150-ja.html)
- [What is global warming, explained: a 2019 article in The National Geographic](https://www.nationalgeographic.com/environment/article/global-warming-overview)
- [Climate change heat impact and prevention](http://www.climatechip.org/)
- [How long draughts make heatwaves worse, in WIRED](https://www.wired.com/story/drought-causing-floods/)
- [A Twitter post that went viral, about how dry ground is "impermeable" to water](https://twitter.com/UniofReading/status/1557350976725581824?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E1557350976725581824%7Ctwgr%5E67a32a5cd950311cd24eaeb786e8526801d31cf9%7Ctwcon%5Es1_&ref_url=https%3A%2F%2Fconfluence.bit.admin.ch%2Fdisplay%2FHACKZURICH%2FLinks2022)
- [The effect of heat waves on people with chronic diseases](https://www.statnews.com/2022/07/19/heat-waves-risk-to-people-with-chronic-illness/?utm_source=STAT+Newsletters&utm_campaign=4924a383e7-Daily_Recap&utm_medium=email&utm_term=0_8cab1d7961-4924a383e7-152497145)
- [Climate change is taking a large toll on our health, in The National Geographic](https://www.nationalgeographic.co.uk/environment-and-conservation/2022/02/major-un-report-says-climate-change-is-taking-a-large-toll-on-our-health)
- [Living with heat](https://www.science.org/content/article/heat-killing-more-people-ever-scientists-are-looking-ways-lower-risk?adobe_mc=MCMID%3D38579558465394467738169735892311986110%7CMCORGID%3D242B6472541199F70A4C98A6%2540AdobeOrg%7CTS%3D1656591528)
- [IPCC 6th assessment report](https://www.ipcc.ch/report/ar6/wg2/)

### A few definitions

#### **Reference periods**

Reference periods are usually *30 years long*, to account for intrinsic climate variability.
The Climate Scenarios CH2018 each describe an average level of climatic conditions over a period of three decades, grouped around the years **2035, 2060 and 2085**. When the text refers to the “middle of this century” or 2060, this refers to the period from 2045 to 2074. Similarly, a reference to the “end of the century” means 2070 to 2099.
Reference period for the climate scenarios CH2018 and Hydro-CH2018: **1981 – 2010**.
Usual reference for publications after 2021: **1991 – 2020**.
For some historical comparisons, reference is often 1961 – 1990 (or even earlier, sometimes pre-industrial).
**!! Be aware of the reference, since changes (in temperature, precipitations etc.) are usually presented as relative to a reference !!**

#### **Greenhouse gas-emissions**

**Representative Concentration Pathways (RCP)**

- RCP2.6: with concerted climated change mitigation
- RCP4.5: middle-of-the-road scenario with limited climate change mitigation
- RCP8.5: no climate change mitigation

### Judging criteria

- **Value:** Does your solution make a difference to citizens? Does it facilitate informed decision-making in our democracy?
- **Creativity:** Does your solution convey information in an innovative / striking way? Thinking outside the box is encouraged!
- **Execution:** Is your solution well designed? Is it usable in its current state? Does everything appear to work?
- **Trustworthiness:** Is your solution well documented? Have you acknowledged data sources? **If assumptions were made, have you clearly stated them?**
