# Five Lectures on FinTech

#### Sanjiv R. Das

This collection of five lectures covers a small selection of topics in FinTech. I will be using slides, readings, referrring to various URLs (web sources) and programming in Python. I will use mostly open source tools, but some in class demos will also use proprietary products. I will host all the materials in *github* at the following repository, from which you may download the needed files (or clone and pull) the repository if you are familiar with using github. See: http://github.com/srdas/IDTF.

The five lectures are described below. The numbering begins from Lecture 6, as there are going to be five lectures preceding this one.

## Lecture 6: Modern Payment Systems

This lecture covers: (i) An introduction to Python in Jupyter notebooks; (ii) Blockchains and Cryptocurrencies; (iii) Payment systems. We will begin with an introduction to Python for Financial Modeling, so that you are able to come up to speed with the main language being used for many applications in FinTech. In order to get a job in the FinTech space, Python is the lingua franca. In preparation for this class, please undertake the following.

#### Python

- Install anaconda, which includes Python and many useful libraries. Download the single install file from here: https://www.anaconda.com/download/. Once you have installed it, use the launcher to start up the Jupyter notebook. I will assume you know how to initiate and use Jupyter notebooks. (By the way, Jupyter is an acronym that the dev team chose as it includes three popular programming languages, Julia, Python, and R.)
- Visit the Jupyter project web site (http://jupyter.org/) and check out the documentation there. See: https://jupyter.readthedocs.io/en/latest/content-quickstart.html.
- Try out the starting notebooks from here: https://try.jupyter.org/
- Especially, if you have not use Python before, then please go through the "Welcome to Python" notebook. Open it in your browser and then execute each cell block, you need to use the command Shoft+Enter (as stated there). Look at the output and then compare it with the code.
- Read the PDF file "Python Tutorial for Absolute Beginners.pdf" in the folder for Lecture 6.
- A good book to get started with Python is "Python for Data Analysis", which I prefer to call **p4da** - it an excellent introduction, and is especially apt because the author WesMcKinney built the Pandas package (Chapter 5) for use at one of the top hedge funds (a good example of a firm that uses FinTech). An older edition is available online: http://www.cin.ufpe.br/~embat/Python%20for%20Data%20Analysis.pdf. I strongly recommend skimming through and learning the first four chapters, and then spending time on chapter 5, giving it a much more careful read. In addition, the best way to learn is to try out lines of code in a Jupyter notebook alongside, as you read.
- I will be using the following notebook in class, which will be provided in advance: **GetStarted_Python_in_Finance.ipynb**. You will find this in the course folder. You do not need to work through this before class, but load it up and bring it on your laptop for class.

#### Blockchains and Payment Systems

- Next, we will move on to a technical exposition of blockchains and related cryptocurrencies. You will have already obtained some familiarity with this topic from earlier lectures.
- The slides for this lectures are in: **6_BlockChains_and_Cryptocurrencies**. Within these slides there will also be links to more readings. This is to incentivize you to go through the slides in advance and follow the links and do some more reading to facilitate discussion in class. This is expected of you.
- Coverage will be on both the business and technical aspects of: distributed ledgers; blockchain; cryptocurrency; bitcoin; transaction flow; hash functions; digital signatures; double spending; proof of work; mining; security; malicious attack; Ethereum; smart contracts; merkle tree; gas; difficulty; Ethereum virtual machine; DAO; initial coin offerings; hyperledger; futures; blockchain infrastructure; payment systems; crypto portfolios (see **CryptoPortfolio.ipynb**).
- Please read all the PDF files in the lecture folder.



## Lecture 7: Textual Analysis for FinTech and RegTech

#### Text Analytics

- In this lecture, we will undertake a somewhat detailed look at why and how text analytics is becoming an important part of the FinTech revolution.
- We will use Python and learn many Python tools for text analytics.
- In the first Python notebook titled **TextMining** we introduce basic text analysis. Please work through this before class.
- The package that is useful is known as **NLTK**, and this stands for "Natural Language Tool Kit". See http://www.nltk.org/book/.
- We will learn how to import textual data from the web using the *requests* package, and also clean it up using the *Beautiful Soup* package. (Note: when you see the "import" command in Python, it is importing a package, and this means that the package needs to be installed. Sometimes the package is already part of the base installation. But it may not be. In such cases when you import the package it will throw an error. Then go ahead and install the package using the "pip install" command followed by the package name.)
- We will learn how to sentiment score text, and discuss how this may be used for financial modeling. For a detailed exposition of text mining in finance, please read the book titled "Text and Context: Language Analytics for Finance" (Das 2014): http://srdas.github.io/Papers/Das_TextAnalyticsInFinance.pdf.
- In the **TwitterAnalysis.ipynb** notebook, we will see how to handle a large collection of tweets. This is a popular input into automated trading strategies. We will also learn how to pull tweets online using the Twitter API, and then sentiment score these tweets.
- In the **IndiaNewsExtractor.ipynb** notebook, we will see how to pull news topics from the Economic Times. Here we will learn how to use CSS selectors. We will also learn various text analytics operations such as removing punctuation, numbers, stopwords, stemming, etc. We will consider the notion of a Corpus. The basic text data structure is a "Term Document Matrix" which we will construct from real data, and see why it is a fundamental starting point for textual analysis. We will also use this to construct Wordclouds.
- We will use a large Reuters data set of news articles to demonstrate advanced topics in financial text analysis, such as: topic modeling; word2vec; t-SNE representations. Again, this will be done using the NLTK package.

#### RegTech

- In RegTech we discuss how technology enables new opportunities in financial regulation.
- As a example we will look at how emails may be used as an early warning indicator of financial failure. The paper titled "Zero-Revelation RegTech: Detecting Risk through Linguistic Analysis of Corporate Emails and News" (Das, Kim, Kothari 2017) will be discussed, and you may download the paper here: http://srdas.github.io/Papers/EnronZeroRev.pdf. The slides to accompany this part of the class are in **7_Enron_Text_Analytics**.
- Also come prepared to discuss how RegTech may be implemented in India.



## Lecture 8: New Technologies for Wealth Management, Risk Management, Trading

This entire lecture deals with financial automation in three separate areas of finance. As we will see, automation that is supported by theoretical modeling is a powerful disruptive force in FinTech.

#### Goal-Based Asset Management with Robo(t) Advisors

- A discussion of goal-based wealth management products that are now being widely used by "robo" advisors.
- The theoretical modeling for goal based wealth management will be discussed. Read the paper titled "Portfolio Optimization with Mental Accounts," (Sanjiv Das, Harry Markowitz, Jonathan Scheid, and Meir Statman, 2010), PDF in the lecture folder. The companion practitioner version of the paper is also provided in Das, Markowitz, Scheid, and Statman, 2011.
- The Python program implementation for this is in the following Jupyter notebook: **Markowitz_MeanVariance_Optimization_BPT.ipynb**.
- The slides for this segment are in **8_GoalBasedAssetMgmt_BPT_RoboAdvising**.
- We also examine how derivatives are used in this portfolio approach. See the paper **JEDC_OptionsStructuredProducts_BPT.pdf**.
- The original work by Markowitz is also available in the following PDFs in the folder: **markowitz_JF_1952.pdf**, **markowitz1959.pdf**.
- We analyze solutions when portfolios are underperforming their goals (Das, Kim, Statman 2014); see **DasKimStatman_JPM_2014_ComingUpShort.pdf**.
- Tax optimization is an important part of the process, and we examine this in Das, Ding, Newell, and Ostrov (2017); see: **DasDingNewellOstrov_JOIS_2017.pdf**.
- We examine longevity risk, an emerging issue that needs addressing through automation assisted planning.

#### Automated Systemic Risk Management using Networks

- A quick introduction to network theory and how it may be used to think about systemic risk. Read **Barabasi_ScaleFree_Networks.pdf**.
- An application to the Indian financial system. See: **8_SysRiskIndia**.

#### Democratized and Crowd-Sourced Trading

- An interesting new area of FinTech is democratized trading. In this new paradigm, individual investors can create their own trading algorithms, and share them on automated trading and backtesting platforms, like Quantopian: https://www.quantopian.com/home. We will examine the use of Quantopian briefly.
- The slides for this part of the lecture are in **8_Democratized_Trading**.
- We will also review an entire range of metrics for trading algorithms here.
- See tutorials here: https://www.quantopian.com/tutorials.
- Another platform for automated trading is Numerai: https://numer.ai/. See also: https://hackernoon.com/numerai-walkthrough-quantitative-analysis-machine-learning-for-fun-and-profit-3dcdccabd920.



## Lecture 9: Automation and Robots

We continue with various examples of automation in FinTech. Here we use credit analysis as a exemplar for data robots. The slides for this lecture are in **9_FinTech_ML_Credit**. All Python notebooks, data, and readings are also in the folder. 

#### Modern Credit Analysis using Machine Learning

- We begin to look at AI and machine learning in this lecture.
- We will use Python to analyze a data set for credit card fraud detection, which is a huge problem being handled by modern technologies. Credit card companies that do not have good fraud detection algorithms are going to be at a massive disadvantage compared to those that do. The data set we will analyze is here: https://www.kaggle.com/dalpozz/creditcardfraud. We will construct a model for detecting fraud. This is a "needle in a haystack" problem, because fraud constitutes around 0.2% of all transactions. Please read this web site before class.
- The Python notebook with this analysis is in **CC_Fraud_RF.ipynb**.
- We will examine how to solve the sample imbalance problem using SMOTE, an oversampling technique.

#### Data Robots for Automated Analysis

- Here, we see how modern data analysis robots may be used to eliminate human modelers. The fact that we can just feed the data into a tool which then finds the best model is astonishing, and indicates how even white-collar jobs are now at risk. We will use https://www.datarobot.com/. This is a licensed software that is inexpensive for students in case you wish to try it out.
- As a second example, we will also use the same technology to let a machine learn about credit scoring from a database of small loans. Please review the following problem before class: https://www.kaggle.com/wendykan/lending-club-loan-data.

#### Chatbots as Financial Interfaces

- Chatbots are a different kind of robot, now being widely used in finance for investor interfacing.
- We will build a simple chatbot using Lex, which is Amazon's chatbot constructor. See: https://aws.amazon.com/lex/. Review this site before class.
- The brief notes are in the following PDF: **Chatbot using Lex.pdf".



## Lecture 10: Artificial Intelligence

#### AI and Deep Learning Applications
