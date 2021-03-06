



# Data Privacy

Cancer research often involves personal health data that requires compliance with [Health Insurance Portability and Accountability Act (HIPAA)](https://searchhealthit.techtarget.com/definition/HIPAA) regulations. In this chapter we will discuss data management strategies to maintain compliance with these important regulations.

<img src="resources/images/02-Data_Privacy_files/figure-html//1SRokLaGAc2hiwJSN26FHE0ZEEhPr3KQdyMICic8kAcs_g1016753ce66_0_24.png" title="Learning Objectives: 1.Define the term data security, 2. Describe major data security strategies, 3.Explain the basics of how encryption works, 4.Be aware of how data security practices may or may not be a part of your workflow" alt="Learning Objectives: 1.Define the term data security, 2. Describe major data security strategies, 3.Explain the basics of how encryption works, 4.Be aware of how data security practices may or may not be a part of your workflow" width="100%" style="display: block; margin: auto;" />

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
 
 

## How to ensure the privacy of this information

Your institution will have guidance regarding how to keep this information private and protected but in general there are 4 main strategies we will summarize here:

1. As few eyes as possible

The protected data is seen by the smallest number of individuals possible, all of whom have been properly trained and certified to handle the data.
Make sure the data is stored in a place that only these few people who are allowed have access to it. If you aren't sure who has access to a place -- don't put the data there!

2. Aggressively de-identify the shared data

Before results or data are shared or published, it is aggressively de-identified. We will talk more about what this is in the next chapter.
If data has been summarized over the cohort and there are no identifiers then it is probably safe to share.

3. Consider a data use agreement

Data use agreements (DUA) are not typically required for HIPAA compliance when sharing de-identified data. However, if you are unsure if your data still meets compliance requirements, you have other ethical concerns about sharing your data (which we will discuss in later chapters), consider a using an agreement. **Finally if you need to share data that is not fully de-identified, than a data use agreement is required.** Data use agreements essential restrict who can access and use the data that you might share, as well as what they may do with the data. Importantly this needs to be agreed upon by an IRB and consented to by the research participants in some manner (more on this to come) before it is in use. 

See [here](https://assets.campbell.edu/wp-content/uploads/2018/09/Guidance-When-Do-I-Need-a-DUA.v1.pdf) and [here](https://www.hhs.gov/sites/default/files/ocio/eplc/EPLC%20Archive%20Documents/55-Data%20Use%20Agreement%20%28DUA%29/eplc_dua_practices_guide.pdf) for more information about when you might need a Data use agreement. Note that your particular situation and institute may have slightly different rules or restrictions.

See [here](https://catalyst.harvard.edu/wp-content/uploads/regulatory/Harvard_Catalyst_Template_LDS_DUA.pdf) for an example DUA template from the Harvard Catalyst. Be sure to follow the attribution guidelines outlined in the link if you adapt the template for your use.  

4. Err on the side of caution!

If in doubt if something counts as PHI or PII, consider reaching out to an office at your institute that can help, such as possibly an Internal Review Board (IRB), a research administration office, or a HIPAA compliance office.

If you plan to share your data somewhere and you are unsure whether a database or repository is secure and HIPAA compliant, ask those who manage that database or repository! 

## How is HIPAA enforced?

The [Office for Civil Right (OCR)](https://www.hhs.gov/ocr/index.html) of the United States Department of Health and Human Services is in charge of enforcing HIPAA compliance.

If you feel that someone is using or sharing data that is in violation of HIPAA compliance, you can file a complaint online using the [OCR compliant portal](https://ocrportal.hhs.gov/ocr/smartscreen/main.jsf). Typically you should see if you can get the violation to be resolved through local means by contacting research administrators or management. However, you could submit to the OCR. Note that complaints should be filed within 180 days of the violation. If the OCR determines that a covered entity (the individuals or institutes who are required to follow HIPAA compliance regulations), then the OCR will follow up to ensure that the entity complies, takes corrective action, or agrees to a settlement.

If compliance is not resolved, than the covered entity may have to pay fines.

Currently if an individual is not aware of a violation the fine can be quite small, but if it is a repeated issue of willful neglect, they can be fined on the order of `$`50,000! If the entity committed the violation for malicious reasons for personal gain, they can face much higher fines, up to `$`250,000 and may face jail time of up to 10 years [@violations_2018].

### Common Violations 

Common violations of HIPAA taken from @violations_2018 are:

1) A lack of encryption

If your email or data transfer is intercepted it is important to keep your data safe! We will talk more about how to do this in the next chapter.

2) Computer hacking or phishing

If your computer gets hacked by hackers through a phishing email or otherwise, they could sell the data to third party organizations who could profit off of the information. The data security practices that we will describe in the next chapter will help avoid this. 

3) Unauthorized Access

Allowing or accidentally allowing fellow lab mates who are not authorized to access the data is a violation of HIPAA. Generally this does not result in harm, but occasionally this can result in other neglectful or malicious practice that result in larger disclosures of PHI. Furthermore leaving your laptop open to PHI data in public or even at home can pose a risk from people who walk by.

4) Loss or Theft of Devices

If your laptop are external storage device is stolen, data files with PHI can easily be obtained by whoever finds them next. Again the measures in the next chapter will help to avoid this potential issue.

5) Improper Disposal of data or devices

Sometimes there are remnants of your data still on your device!

6) Unsecured access to data

Accessing your data form an unsecured WIFI network can also make the data vulnerable. 

See [here](https://privacyruleandresearch.nih.gov/faq.asp) for more information about HIPAA and research.

In the next chapter, we will talk about measures that you can do to avoid these violations.
