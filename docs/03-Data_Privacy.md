



# Data Privacy

Cancer research often involves personal health data that requires compliance with [Health Insurance Portability and Accountability Act (HIPAA)](https://searchhealthit.techtarget.com/definition/HIPAA) regulations. In this chapter we will discuss data management strategies to maintain compliance with these important regulations.

<img src="resources/images/03-Data_Privacy_files/figure-html//1SRokLaGAc2hiwJSN26FHE0ZEEhPr3KQdyMICic8kAcs_g1016753ce66_0_24.png" title="Learning Objectives: 1.Define the term data security, 2. Describe major data security strategies, 3.Explain the basics of how encryption works, 4.Be aware of how data security practices may or may not be a part of your workflow" alt="Learning Objectives: 1.Define the term data security, 2. Describe major data security strategies, 3.Explain the basics of how encryption works, 4.Be aware of how data security practices may or may not be a part of your workflow" width="100%" style="display: block; margin: auto;" />

There are two kinds of information that we will need to be careful to protect:
*personal identifiable information (PII)* and *protected health information (PHI)*

Note that these are general definitions and whether something counts as PII or PHI has to be evaluated in a case-by-case basis.

## PII (personal identifiable information)

PII (personal identifiable information) are items that would allow you to identify a person.

*Examples include (but aren't limited to):*  
  - Name
  - Telephone number
  - Address
  - Social security number
  - Age
  - Driver's licenses
  - Medical record numbers
  - Full face photographs
  - IP addresses

 
## PHI (protected health information)

The [U.S. Department of Health & Human Services](https://www.hhs.gov/hipaa/for-professionals/privacy/laws-regulations/index.html) describes protected health information (PHI) as:

> ...information including demographic data that relates to:

> the individual’s past, present or future physical or mental health or condition,
> the provision of health care to the individual, or
> the past, present, or future payment for the provision of health care to the individual,

This includes 18 categories:

- Patient names  
- Geographical elements (such as a street address, city, county, or zip code)
- Dates related to the health or identity of individuals (including birthdates, date of admission, date of discharge, date of death, or exact age of a patient older than 89)
- Telephone numbers
- Fax numbers
- Email addresses
- Social security numbers
- Medical record numbers
- Health insurance beneficiary numbers
- Account numbers
- Certificate/license numbers
- Vehicle identifiers
- Device attributes or serial numbers
- Digital identifiers, such as website URLs
- IP addresses
- Biometric elements, including finger, retinal, and voiceprints
- Full face photographic images
- Other identifying numbers or codes



## What genomic data is protected?

So what does this mean for the data you handle?

**A not comprehensive list of identifiable and protected information:**   

- Clinical information in metadata
- Genomic sequences
  - Whole genome sequences
  - Exome
  - Whole transcriptome
- Single nucleotide polymorphisms
- Geneology information

**What is not protected and generally is safe:**   

- Summarized cohort data
 
 Data in which individuals have been aggregated together is generally safe. For example, a file that includes an average age calculated across all individuals or a large subset would generally be considered safe. However, this may not always be the case with individuals with very rare conditions.
 
 

## How to protect this information

Your institution will have guidance regarding how to keep this information protected but in general there are 3 main strategies we will summarize here:

1. As few eyes as possible

The protected data is seen by the smallest number of individuals possible, all of whom have been properly trained and certified to handle the data.
Make sure the data is stored in a place that only these few people who are allowed have access to it. If you aren't sure who has access to a place -- don't put the data there!

2. Aggressively de-identify the shared data

Before results or data are shared or published, it is aggressively de-identified. We will talk more about what this is in the next chapter.
If data has been summarized over the cohort and there are no identifiers then it is probably safe to share.

3. Err on the side of caution!

If in doubt if something counts as PHI or PII, or if you are unsure whether a database or repository is secure, ask! 

avocado - who can they ask?
