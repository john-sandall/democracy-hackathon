<img src="https://pydata.org/london2018/static/images/logo.288981a8dfa8.png" alt="PyData London 2019" width="150px"  style="float: left;">


# PyData 2019 Democracy Hackathon: PDF Parsing Challenge


## Description
The goal of this challenge is to extract useful data and information from PDF's containing civic data. This can be a difficult task, but even the slightest progress can have a big impact. We have a few ideas to get you started, but any civic data not already in a usable format is fair game!



## Candidate data
[The Democracy Club](https://democracyclub.org.uk/) collects data on every candidate standing for election in the UK. The official source of candidate information comes from a “Statement of Persons Nominated” (SOPN) published by each local authority that is managing an election. The statement is normally published as a PDF on each local authority’s website.

At the moment, with the help of thousands of crowdsourcers, they collect the links to all the PDFs on the day they’re published. Then manually enter the information [(sometimes as SOPN parties)](https://docs.google.com/document/d/1uTnqugmUuhUQQrl_lA8I_MIX86KPK_Iw8FiZrCXiUOk/edit#) into a structured format using their [crowdsourcing website](https://candidates.democracyclub.org.uk/).

Can we automate or speed up this work?

[Sym Roe's](https://twitter.com/symroe) ['Machine learning to help elections'](https://democracyclub.org.uk/blog/2018/03/12/machine-learning-help-elections/) contains information about how the data is structured in the PDF's and a link to download a few thousand SOPN's (1.3gb if the internet is slow we can air drop them to you).

You can dive straight into the PDF's and try to extract the data, or work on some of the articles suggested hybrid approaches that can speed up the manual processing of SOPN's. These SOPN's have already been processed, so we're aiming to develop tools for future elections.





## Polls
Polls are more varied in their design and more challenging. A number of organisations aim to aggregate polling data, but like the good people at The Democracy Club, they also manually process it.

Each pollster has a different design, so choose your battle wisely. A few of the more prominent pollsters who release in PDF format are [IPSOS MORI](https://www.ipsos.com/sites/default/files/2017-06/pm-election-2017-final-tables.pdf),
[YouGov](https://d25d2506sfb94s.cloudfront.net/cumulus_uploads/document/o8pit1boew/TheTimes_190703_VI_Trackers_w.pdf), and [Survation](https://survation.com/wp-content/uploads/2017/06/Survation-GE2017-Final-Poll-2d7l9l8.pdf).

#### Links to get you started
- [Links to recent polls - Wikipedia](https://en.wikipedia.org/wiki/Opinion_polling_for_the_next_United_Kingdom_general_election#2019)
- [Links to 2017 polls - Six Fifty](https://sixfifty.org.uk/polls)
- [On building an automated polling pipeline](https://sixfifty.org.uk/2017/05/21/building-sixfiftys-election-tracker/)
- [How polling works](https://sixfifty.org.uk/2017/04/29/how-polling-works/)

