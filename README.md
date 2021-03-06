<div>
    <img src="media/newspeak_logo.png" alt="Newspeak House" width="250px" style="float: left;" />
    &nbsp;&nbsp;
    <img src="https://pydata.org/london2018/static/images/logo.288981a8dfa8.png" alt="PyData London 2019" width="150px"  style="float: left;">
</div>

# PyData 2019 Democracy Hackathon
Code and resources for the [PyData 2019 Democracy Hackathon](https://pydata.org/london2019/schedule/presentation/59/) (Saturday 13:30-15:45 in the Mortimer Room). Hosted by Newspeak House Fellow [John Sandall](https://twitter.com/john_sandall) and [Richard Chadwick](https://medium.com/@richchad).

- - -

## Description

Data and technology can be powerful tools for understanding and improving the democratic process. Instead of weaponising these tools to produce unfair advantages, driving mistrust and disenfranchisement, the data community can also do the opposite. This hackathon isn't "[The Great Hack](https://www.sciencemuseum.org.uk/see-and-do/great-hack-london-premiere-qa)", but it will be a hack, it will be great, and it will be using data for good.

Why do some people exercise their right to vote whilst others stay at home? In an era of contentious discourse and political scandals, how can we restore democratic faith and trust in our elected representatives?

In this hackathon, hosted by [Newspeak House](https://www.nwspk.com/), we present a series of challenges and datasets compiled by civic tech organisations working to upgrade democracy for the digital age. We will provide working examples, open ended challenges as well as a Kaggle-style prediction competition, and plenty of support if this is your first data hackathon!

> Newspeak House is an independent residential college founded in 2015 to study, nurture and inspire emerging communities of practice across UK public sector and civil society. Find out more [@nwspk](https://twitter.com/nwspk) or come to one our [upcoming events](https://www.nwspk.com/events) in Shoreditch.


## Themes & Prize Categories

- **Machine learning competition.** There will be a Kaggle-style machine learning competition for predicting the turnout of UK general elections. [SixFifty](https://sixfifty.org.uk) has been working hard to source and produce model-ready datasets for solving this problem. All that remains is for someone to solve it!
- **Voter engagement.** For the hack most likely to get more people to turnout.
- **Open data for democracy.** Help improve discoverability and accessibility of open datasets and streamline getting them from raw to model-ready by contributing to [Maven](https://pypi.org/project/maven/). Maven aims to reduce the time data scientists spend on data cleaning and preparation by providing easy access to open datasets in both raw and processed formats.
- **Painless parsing of political PDFs.** A huge amount of civic data is published as tables trapped in PDF prisons. Work towards liberating this information and set it free!
- **Fake news, misinformation & public sentiment.** It's becoming harder to distinguish legitimate news from demonstrably false news, and with a few taps we can instantly share the stories we consume on our phones to our social networks. More news doesn't mean better news, and big tech companies are increasingly having to moderate and filter the content they host. How can we use the vast quantity of information at our fingertips to create tools or insights into improving the quality of the information we receive online?
- **Wildcard prize.** The theme is democracy. The goal is a better world. You define how we get there. Should Parliament move to another city? What would be the perfect voting system? Perhaps we should back to the [wapentake](https://en.wikipedia.org/wiki/Hundred_%28county_division%29#wapentake) or the [Thing](https://en.wikipedia.org/wiki/Thing_%28assembly%29)? Should Parliament delegate constitutionally contentious issues to a citizens assembly? Should we replace all branches of Government with a Superintelligent AI?


## Datasets

You don't have to use these, but they're a good start.

### General
- **[UK Politics Datasets](http://bit.ly/UKPoliticsDatasets):** Crowdsourced document of links to useful datasets & munging tools. Candidates, polling stations, constituencies, parliament voting records, parliament speeches, Hansard, previous election/referendum results, registered financial interests, boundary maps, shapefiles, campaign expenses, registration rates, candidates CVs, constituency stats, GE2017 manifestos…
- **[Democracy Club](https://democracyclub.org.uk/data/):** Election identifiers, candidates' info since 2010 (name, email, photos, social media), polling stations, all [CC-BY-SA](https://creativecommons.org/licenses/by-sa/3.0/).
- **[mySociety](https://www.mysociety.org/democracy/):** mySociety have created a range of tools including [Parliamentary Monitoring](https://www.mysociety.org/projects/parliamentary-monitoring/pombola/), structured data on [every national politician in the world](https://www.mysociety.org/projects/parliamentary-monitoring/everypolitician/), information on [election candidates](https://www.mysociety.org/projects/parliamentary-monitoring/yournextrepresentative/) around the world, how to [contact elected representatives](https://www.mysociety.org/democracy/writeinpublic/), the [constituency/postcode matching tool MapIt](https://www.mysociety.org/projects/parliamentary-monitoring/mapit/), and published [transcripts from all levels of government](https://www.mysociety.org/projects/parliamentary-monitoring/sayit).
- **mySociety Geographic data:** When it comes to building predictive models, geocoded data is quite handy. Official "open" data portals can be [broken](http://webarchive.nationalarchives.gov.uk/20160105160709/https://geoportal.statistics.gov.uk/geoportal/catalog/main/home.page), or the data only available via [mail-order CD](https://data.gov.uk/dataset/lower_layer_super_output_area_lsoa_boundaries), so mySociety's cache of [OS, ONS, and OSNI open geographic data](http://parlvid.mysociety.org/os/) going back to 2010 is a gold mine.

### Turnout modelling competition
- **Start with the [notebook in `turnout_model`](https://github.com/john-sandall/democracy-hackathon/blob/master/turnout_model/GE2017%20-%20Turnout%20model.ipynb)**.
- **[SixFifty Datasets](https://github.com/six50/pipeline):** Model-ready datasets for 2010/2015 elections, EU referendum, [opinion polling at national/regional levels](https://github.com/six50/pipeline/tree/master/data/polls), all available in CSV, JSON and Feather.
- **Opinion polling data:** In 2017 SixFifty created a manually curated set of poll results can be downloaded in [JSON](https://s3-eu-west-1.amazonaws.com/sixfifty/polls.json), [CSV](https://s3-eu-west-1.amazonaws.com/sixfifty/polls.csv) or [Feather](https://s3-eu-west-1.amazonaws.com/sixfifty/polls.feather). See [data/polls/](https://github.com/six50/hackathon/tree/master/data/polls/) for more information including a data dictionary.

### Voter engagement
- **Start with the [README in `voter_engagement`](https://github.com/john-sandall/democracy-hackathon/tree/master/voter_engagement)**.
- To understand what's been tried before, take a look at the tools and projects that were developed for the 2017 General Election. In the **[GE2017 Tech Initiatives Handbook](http://bit.ly/GE2017TechHandbook)** you'll find a collection of resources, datasets, volunteers, existing projects, proposed projects.

### Open data for democracy
- **Start with [Maven](https://pypi.org/project/maven/)**. How can we make commonly used datasets (e.g. those listed in [Newspeak's Politics Datasets](http://bit.ly/UKPoliticsDatasets) or under the "General" heading above) easier to discover, download and process?

### PDF parsing
- **Start with the [README in `pdf_parsing`](https://github.com/john-sandall/democracy-hackathon/tree/master/pdf_parsing)**.

### Fake news, misinformation & public sentiment
- **Start with the [README in `fake_news`](https://github.com/john-sandall/democracy-hackathon/tree/master/fake_news)**.
- **[Political Twitter](https://drive.google.com/open?id=1jJRsDPNrh9JoHGcgWYt_1KyrQwVOLmM7):** [Richard](https://medium.com/@richchad) has scraped a collection of tweets from UK politicians.

### Wildcard prize
- Start with **_[So you want to reform democracy?](https://medium.com/civic-tech-thoughts-from-joshdata/so-you-want-to-reform-democracy-7f3b1ef10597)_**, but don't be disheartened! One thing is for sure, the world in 100 years will be very different.


## Schedule
- **13:30** – Introduction to challenges & datasets.
- **13:50** – Hacking time!
- **15:25** – Presentations & wrapup.
- **15:45** – Event ends.


## Code of Conduct
All attendees are expected to abide by the NumFOCUS Code of Conduct. Please take this opportunity to review it.

Be kind to others. Do not insult or put down others. Behave professionally. Remember that harassment and sexist, racist, or exclusionary jokes and language are not appropriate for PyData. All communication should be appropriate for a professional audience including people of many different backgrounds. Sexual language and imagery is not appropriate. PyData is dedicated to providing a harassment-free event experience for everyone, regardless of gender, sexual orientation, gender identity, and expression, disability, physical appearance, body size, race, or religion. We do not tolerate harassment of participants in any form. Thank you for helping make this a welcoming, friendly community for all.

The full Code of Conduct and additional information can be found [here](https://pydata.org/code-of-conduct/).

If you wish to submit a Code of Conduct report [click here](https://numfocus.typeform.com/to/ynjGdT/).
