---
title: "About the Project: Frequently Asked Questions"

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

# Optional header image (relative to `static/media/` folder).
header:
  caption: ""
  image: ""
---

{{< toc >}}


## What is Triage?

*Triaging* is where a clinician synthesises available information to make a decision about what to do next. 

For example, a clinician presented with a referral will usually have information about:

  1. the patient's medical history
  2. the current difficulty, problem or a description of unmet clinical need
  3. details of the patient's current or previous treatments

A clinician then has to decide:

  1. how urgently the patient needs to be assessed or examined
  2. which group of clinicians, specialty or team would be best suited to help


## What is Digital Triage?
> "Every hour spent in thinking and talking about **whom** to treat, and **how**, and **how long** is being subtracted from the available pool of therapeutic time itself" - Paul E. Meehl (1954) *Clinical versus Statistical Prediction*

*Digital triage* is an attempt to leverage technology to assist clinicians in triage tasks with the aim to personalise, expedite and improve access to care.  chrono**sig** is designed to improve triage in secondary mental health services by leveraging contemporary machine learning (ML) technology on information contained in large, routinely-collected electronic health record (EHR) data.  

Each patient’s historical eletronic health record (EHR) data captures one or more instances (or episodes) of care under mental health services.  A referral is almost always provided as documentation to help the recieving clinician make a triage decision.

chrono**sig** will use natural language processing (NLP) techniques to represent a patient’s longitudinal signature (or ‘fingerprint’) -- capturing their history, signs/symptoms and presenting difficulties -- and then learn associations between these signatures and triage decisions (captured as explicit structured data in patient’s EHR data).  The aim is to deliver a triage clinical decision support tool (CDST) that takes as input a patient’s referral documentation, utilises existing medical notes (when available) and delivers a suggested triage outcome to assist MDTs.  

## Why is Triage Important?
In the United Kingdom, mental healthcare is stratified into primary (led by General Practice), secondary (community and hospital NHS Trusts) and tertiary services (e.g. secure forensic services).  In 2019-2020, over 2.8 million people in England were in contact with secondary mental health (SMH) services with the majority receiving care from community-based teams (NHS Digital, 2020).  

{{< figure src="referral-numbers.png" caption="NHS Service Use" numbered="true" >}}

Patients requiring secondary care are referred to a triage and assessment function, contained in community mental health teams (CMHTs) operating in NHS Trusts (collections of community-based clinics and inpatient hospitals).  Referrals for triage and assessment are almost always via documents written by the referring professional who is most often a general practitioner (GP), a healthcare professional in an emergency department or member of a social care organisation.  

{{< figure src="referral-bounce.png" caption="Referral Routing and Bouncing" numbered="true" >}}

> In March 2021, across England’s mental healthcare NHS Trusts, there were 404,552 new referrals (NHS Digital, 2021).  

Each referral requires the CMHT to:

  1. instruct one of their clinicians to review the referral documentation alongside an examination of historical medical notes (e.g. if the patient is already known to SMH services) 
  2. use these findings for a discussion in a multi-disciplinary team (MDT) meeting
  3. decide on an outcome for example: 

      a. **accept** the referral and offer a first assessment appointment to the patient

      b. **reject** the referral (e.g. if clinically inappropriate or the incorrect locality/service)

      c. obtain further information (e.g. from the referrer, patient and carers)

      d. refer to a specialty or locality team for further triage, assessment and treatment.  

> The cost of initial assessments arising from new referrals to SMH services was £326 million in 2018-2019 (NHS England, 2020).   



Referral and triage processes lack transparency (to patients and referrers), are capricious (with CMHTs using referral criteria and thresholds inconsistently) and result in frustration from ‘referral bouncing’ (Chew-Graham et al., 2007). 

Patient care is delayed because they are being triaged multiple times, by different teams, who may disagree on the most appropriate treatment team for the patient’s needs.   

The delay in accessing treatment (after referral) has been labelled the **hidden waiting list** by The Royal College of Psychiatrists who identified that two-fifths of patients end up accessing emergency or crisis care (RCPsych, 2020). 

> Displacing patients with unmet mental health needs impacts on other NHS services -- for example, in 2013-2014, there were 6.2 million emergency department attendances across England for mental health needs with around half being discharged back to community care (Baracaia et al., 2020).  


The referral and triage process is one target for process improvement where both patients and clinicians stand to benefit.  

To this end, the chrono**sig** project directly addresses the strategic priorities described in the Topol review (Foley & Woollard, 2019) and the NHS Long Term Plan (NHS England, 2019) that emphasise the use of EHRs to improve and personalise care for individuals.  


## Who Supports chrono**sig**?
The project is funded by the National Institute of Health Research (Grant Number: AI_AWARD02183) and hosted by the Department of Psychiatry at the University of Oxford, Oxford Health NHS Foundation Trust and the Oxford Health NIHR BRC. 

{{< figure src="sponsor-logos.png" caption="" numbered="false" >}}

## Data, Privacy and Security
chrono**sig** makes use of medical data, specifically, that contained in the electronic health record (EHR) of specialist, secondary mental health NHS trusts.  The data required to build the chrono**sig** clinical decision support tool (CDST) for triage will be obtained from the UK-CRIS network.  There are currently sixteen mental health NHS trusts across England participating and contributing electronic health record data in the UK-CRIS platform.  This data is anonymised and access is strictly controlled to authorised and qualified researchers (described in the subsections below). 

Neither chrono**sig** (or the UK-CRIS network more generally) link data from secondary mental health care EHRs to any other healthcare records (for example, data is not linked to GP or other local hospital records).  All data used in the chrono**sig** project is historical data -- no patients actively being treated or triaged are used.  

### Who processes and maintains the UK-CRIS database? 
Storing, anonymising and making data available to researchers in a secure environment requires significant expertise and computing resources.  For this reason, [Akrivia Health](https://akriviahealth.com/) was founded to run and maintain the UK-CRIS project.  Akrivia Health is a University of Oxford commercial spin-out company, formed to continue and sustain the original UK-CRIS consortium which was funded by the National Institute of Health Research (NIHR) and was based at the University of Oxford and the NIHR Oxford Health BRC.

### Where is UK-CRIS data stored?
Akrivia Health manage and administer the secure storage of the UK-CRIS database on a cloud-based platform (Amazon Web Services, or AWS).  The use of AWS cloud storage follows the UK government’s policy from 2013 to migrate public-sector data to secure cloud systems to minimise the use of “physical” storage located at and managed individually by each organisation (where there are overhead costs and very often, less expertise and resource for providing reliable, continuous 24/7 services).  Cloud storage is preferred over traditional “in house” physical storage and backup because it is fault-tolerant – if a traditional server fails, everyone dependent on the data loses access until a backup can be restored.  With cloud-based storage, data is distributed over many physical storage devices and access can be restored almost seamlessly in the event of failure.  AWS (alongside Microsoft Azure and Google Cloud) are already used by the NHS and the public sector more generally to warehouse mission-critical data to prevent loss-of-service and ensure data integrity.

### What Data is Available in UK-CRIS data?
NHS trusts regularly upload extracts of their clinical electronic health records to the UK-CRIS network using Akrivia Health's AWS-based platform. 

These extracts contain pseudonymised and "masked" versions of:

  1. Clinical notes, letters and correspondence, refered to as ‘unstructured’ free-text.  This data provides descriptions of patient's health state including symptoms and signs, descriptions of clinical or treatment decisions/reasoning and treatment plans including psycho-social interventions as well as medications. 
  2. Structured data such as demographics e.g., dates of birth, categorical gender data and diagnoses.

### How is confidentialty ensured?
As part of Akrivia Health's data processing activities, on behalf of NHS Trusts in the UK-CRIS network, Akrivia provides services to ‘deidentify’ (i.e. remove personally identifiable information) all data contained in the UK-CRIS database.  Importantly, all data placed in the UK-CRIS database is pseudonymised by masking – this is where any patient-identifiable “fields” or data points (including name, date of birth, address, NHS number) in a patient’s electronic health record notes are ‘blanked out’.  

For example, in unstructured, free-text such as “Mr Jones is a 67-year-old man (DoB: 24/1/1954; NHS Number 1234 345 123) who is currently living at 42 Some Street, Somewhere, SO14 0NB with his 4 children.” will be stored in UK-CRIS as “Mr XXXXX is a 67-year-old man (DoB: XXXXX; XXXXX XXXXX) who is currently living at XXXXX, XXXXX, XXXXX with his 4 children.”. 

This masking is done automatically when data is uploaded to the UK-CRIS platform from the NHS Trusts. Further, structured data (i.e. data not written by clinicians in a ‘narrative’ free-text format, such as demographic data that is usually captured by standardised electronic forms) is masked in the same way.  

The same underlying data is also further aggregated into anonymised high-level summary data -- this means reducing the level of detail in the dataset to reduce the identifiability of individual patient data (e.g. only showing the year in which a subset of patients were born or truncating post-codes to describe only medium- or large geographical regions).  This summary-level anonymised data is accessible to authorised UK-CRIS users and Akrivia Health staff and can be used to answer high-level questions; for example, to profile the dataset with queries such as “How many people aged between 18 and 65 have a diagnosis of depression and are taking one of the common medications used to treat depression”.  These kinds of data queries do not reveal the underlying masked, free-text data.

One overarching confidentiality principle is that data that could identify any individual patient (e.g. name, address) should never be disclosed to *any* user of UK-CRIS data and the methods described above ensure this by directly anonymising patient-identifying data items or fields.  Further, given any amount of such anonymised data, the actual identity of an individual should never be able to be recovered *indirectly*.  

This is a particular risk when two distinct and anonymised sources of data are combined or linked.  For example, if one anonymised database contains only a single male patient, aged 53, diagnosed with depression in a particular geographical region (e.g. a top-level postcode such as OX1) then if this information was combined with, for example, a DVLA database of drivers living at specific streets in OX1 and there was only one male 53 year old driver in that database, one could infer that the 53 year old male patient with depression is the same person who lives at the address contained in the DVLA database.  

For this reason, UK-CRIS data are never linked to other NHS or other datasets without explicit research ethics committee approval – i.e. above and beyond those processes for the usual approval of UK-CRIS projects – in those cases, explicit contingencies have to be put in place to mitigate such identification risks and this usually involves stating that if, on combining the two databases, there are less than a threshold number of patients (for example, 10) then those patients will not be used and reported in analyses of that combined, linked data set.  

### Can people opt-out of UK-CRIS?
Yes -- this can be achieved by contacting your local NHS secondary mental health care trust, or via the [National Data Opt Out](https://digital.nhs.uk/services/national-data-opt-out) scheme.

When patients opt-out, their electronic health record is "flagged" so that the NHS trust ensures opted-out patient data is never extracted and placed in the UK-CRIS database.


### Can I find out more about UK-CRIS?
Oxford Health NHS Foundation Trust has a helpful guide that elaborates on these issues further [here](https://www.oxfordhealth.nhs.uk/research/toolkit/cris/cris-privacy-notice/).


<a name="who-can-access"></a>
### Who can access UK-CRIS data? 
Collections of patient records in the masked format described above are made available to researchers who are suitably qualified (meaning that all users must be vetted by their local NHS Trust's information governance teams) and are

  1. NHS research staff 
  2. researchers employed at the University attached to an NHS trust 

In addition, data pertaining to patients belonging to a given NHS Trust are only accessible to staff in that Trust or associated University; for example, researchers at the University of Oxford and Oxford Health NHS Foundation Trust are not allowed to access data on patients from other external trusts in the UK-CRIS network without formally applying to that external trust and meeting that trust's information governance and oversight requirements.  Similarly, Akrivia Health staff cannot routinely access these data without express permission from the NHS trust that donated the data and then, only for a specific task/research project for a specified period of time.  

When making an application to use data for any given research project, the researchers must make a clear case for why using UK-CRIS data is necessary and demonstrate how the proposed research use of the data is proportionate and obeys the seven principles of the UK's [General Data Protection Regulations](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/principles/) (GDPR)


### How do authorised users access UK-CRIS data?
To access any subset of the UK-CRIS dataset, appropriately qualified and authorised users must use a secure [AWS workspace](https://docs.aws.amazon.com/workspaces/latest/adminguide/amazon-workspaces.html) -- this refers to the cloud-based storage system, at Amazon Web Services, used to warehouse the UK-CRIS data.  

Authorised users are required to log onto AWS using a secure connection (much like the Virtual Private Networks (VPNs) that are available for private internet browsing on any computer) and the user is presented with a desktop (i.e. the same way one would be if logging onto their own physical Windows, Linux or Mac computer) called a “virtual desktop”.  

On this virtual desktop, the user accesses only the subset of UK-CRIS data they have been given express permission to use (as described [above](#who-can-access)).  Users can then start analysing the data in that same virtual desktop.  The virtual desktop has no internet access (i.e. users cannot launch a web browser inside the virtual desktop) and users cannot copy and paste data from the virtual desktop onto the physical computer they are using to access the AWS workspace. 

If users wish to export any files from this workspace to their local computers (for example, if a researcher wants a summary table of results from an analysis to put in a research report or publication), this must be manually inspected and approved by the Trust’s CRIS administration team and any approved export actions will be automatically logged for audit purposes.  If there is any doubt about e.g. inappropriate use or a risk that confidentiality would be breached, the request to export summary data will be denied.  In essence, the virtual desktop is “sealed off” from the internet except for viewing and interacting with the specific subset of CRIS data the researcher has been approved to access/analyse and data cannot be moved from the virtual desktop to any other computer.

### What mechanisms protect access to UK-CRIS data?
When logging onto the AWS workspace, the user must provide all of the following:

  1. a username (granted by the CRIS administrators in each NHS Trust) 
  2. a strong password or passphrase
  3. a temporary pass code generated “on the fly” by an authenticator application -- so-called **two-factor authentication**.  


Usernames and passwords are ‘static’ – once set, they only change periodically (e.g. monthly) and are stored (in an encrypted form) so that a user’s credentials can be verified on logging on to any password-protected system.  

For this reason, although generally secure, passwords can be ‘cracked’ by determined unauthorised users (hackers).  To mitigate this, almost all security-critical applications now insist that a second line of authentication is used.  So called two-factor authentication (2FA) is where (as well as the username and password), a registered user must register a physical device (usually, a smart-phone) to generate “instant” passcodes (usually, 6-digit numbers) that change every 30 seconds.  This is the same approach that retail banks use for customers accessing their accounts online.  After entering their username and password, the AWS platform then requests the user enter a 6-digit code by opening an authentication app on their registered mobile device.  If the username, password and the 2FA 6-digit passcode are all correct (in the 30-second window) only then is the user authenticated and logged onto the system.  In practice, this means if anyone ‘cracks’ a username and password, they still cannot access the user’s account on the AWS workspace and consequently, the UK-CRIS platform because they need to physically possess the authorised user’s mobile phone to obtain a 6-digit 2FA passcode.


***

## References
Chew-Graham, C., Slade, M., Montana, C., Stewart, M., & Gask, L. (2007). A qualitative study of referral to community mental health teams in the UK: Exploring the rhetoric and the reality. BMC Health Services Research, 7(1), 117. https://doi.org/10.1186/1472-6963-7-117

Foley, J., & Woollard, J. (2019). Digital Future of Mental Healthcare Report. https://topol.hee.nhs.uk/wp-content/uploads/HEE-Topol-Review-Mental-health-paper.pdf

NHS Digital. (2020). Mental Health Bulletin: 2019-20 Annual Report. https://digital.nhs.uk/data-and-information/publications/statistical/mental-health-bulletin/2019-20-annual-report

NHS Digital. (2021). Mental Health Services Monthly Statistics, March/April 2021. https://digital.nhs.uk/data-and-information/publications/statistical/mental-health-services-monthly-statistics/final-march-2021

NHS England. (2019). The NHS Long Term Plan.

NHS England. (2020). National Cost Collection 2019. NHS England and NHS Improvement. https://www.england.nhs.uk/wp-content/uploads/2020/08/1_-_NCC_Report_FINAL_002.pdf

RCPsych. (2020, October 6). Two-fifths of patients waiting for mental health treatment forced to resort to emergency or crisis services. Www.Rcpsych.Ac.Uk. https://www.rcpsych.ac.uk/news-and-features/latest-news/detail/2020/10/06/two-fifths-of-patients-waiting-for-mental-health-treatment-forced-to-resort-to-emergency-or-crisis-services




