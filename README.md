![LexPredict](http://lexpredict.com/wp-content/uploads/2014/08/lexpredict_logo_horizontal_1.png "LexPredict")

# [LexPredict](http://lexpredict.com/) LexHacks 2015 Challenge
## Challenge for LexHacks Hackathon on June 6-7, 2015

## Challenge Task

  The LexPredict challenge is to develop basic tools for processing contracts.  Specifically, you will use the sample contract data below to develop algorithms to:
* identify the parties to an agreement
* identify effective date segment and date
* identify termination clause segment(s) and date(s)

  Take, for example, the following text:
> THIS GUARANTEE AGREEMENT dated as of September 30, 2008 (this "Guarantee") is entered into by
> FREIGHTCAR AMERICA, INC., a Delaware corporation (the "Guarantor"), in favor of BANK OF AMERICA,
> N.A., a national banking association, as the administrative agent (in such capacity, the
> "Administrative Agent") for certain financial institutions (each a "Lender", and collectively the
> "Lenders") from time to time party to the Credit Agreement (defined below).

 The "correct" answers are:
 * *Parties*: FREIGHTCAR AMERICA, INC.; BANK OF AMERICA,N.A.
 * *Effective date*: September 30, 2008

## Challenge Data
The data for this challenge can be found at this link:
* Sample Data File: http://lexpredict.com-data.s3.amazonaws.com/lexpredict_agreement_archive/lex_hack_sample.tar.gz
* Sample Agreement Count: 33,670

```sh
$ md5sum lex_hack_sample.tar.gz
70c9faa4ec82f04273b9228bfb5aa531  lex_hack_sample.tar.gz
```

## Challenge Scoring

### Language
Algorithms can be written in any language.  We prefer Python and Java but are happy to see whatever works.

### Software Licensing
In order to be eligible for the challenge prize, your software must be contributed back to Github under either an Apache 2.0 or GPL 3.0 license.  

### Data Licensing
Redistribution of the data provided for this challenge is prohibited without permission.  Usage of the data is only permitted for (a) the completion or replication of challenge submissions and (b) for non-commercial, academic research.  For other usages, please email contact@lexpredict.com to discuss.

### F1 score
In order to determine the winner, we'll draw 200 random documents from the sample and assess the algorithms' performance.  The winning team will be the one who has the highest [F1 score](http://en.wikipedia.org/wiki/F1_score).
