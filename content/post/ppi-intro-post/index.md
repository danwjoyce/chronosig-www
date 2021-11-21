
---
title: "Public and Patient Research in chronosig"
subtitle: ""
summary: "Julia Hamer-Hunt explores how public and patient involvement features in the chronosig project"
authors: ["jhh"]
tags: ["PPI", "announcements", "project", "introduction"]
categories: ["PPI", "explainers"]
date: 2021-11-21T16:44:57Z
lastmod: 2021-11-21T16:44:57Z
featured: true
draft: false
---

As someone working in public and patient involvement (PPI) for 20 years,
I quake whenever IT (information technology), machine learning (ML),
data science – and latterly – the apparently more general term AI
(artificial intelligence) are mentioned.

In this inaugural blog post for the CHRONOsig project, I will outline
some core concepts and explain why PPI is required front-and-centre in
the project.

Why did I become involved? Extracting information from large data sets,
to analyse patterns and trends in disease and illness is the future for
medical science. However reluctant I am to embrace this technology I
have no option but to do so if I wish to be informed and importantly,
influence adoption. So, four years ago I became a member of the
CRIS-Oxford (Case Record Interactive Search) Oversight group. UK-CRIS is
a national programme to develop the clinical record (often called the
electronic health record, or EHR) into a data asset and research tool
for NHS Mental Health Trusts. It was through this work I met one of the
researchers who later became involved in the CHRONOsig project.

# The Problem

Firstly, what is CHRONOsig? CHRONOsig stands for CHRONOlogical
SIGnatures. It is a project, funded by the National Institute of Health
Research (NIHR), to develop a clinical decision support tool (CDST) that
will deliver accurate, explainable and justified recommendations to
assist clinicians expedite access to the right secondary mental health
care.

To access specialist, secondary mental health care, a person must
usually be referred to a community mental health team (CMHT), who review
the referral alongside the person’s historical medical notes and then
decide how to proceed. Referral and triage processes lack transparency
(to patients and referrers), are capricious (with CMHTs appearing to use
referral criteria and thresholds inconsistently) and result in
frustration from ‘referral bouncing’ (Chew-Graham et al. 2007). Attempts
at improving this interface – for example, with GPs and CMHTs using a
standardised referral tool to ‘grade’ patient’s severity and unmet needs
– have yielded poor results (Slade et al. 2008). Patient care is delayed
because they are being triaged multiple times, by different teams, who
may disagree on the most appropriate treatment team for the patient’s
needs. It is hoped that CHRONOsig will lead to improved and more
accurate triage outcomes by automating some parts of the triage process.

# CHRONOsig uses Artificial Intelligence and Machine Learning

For a start, what is the difference, if any, between IT, data science,
machine learning and artificial intelligence? Every time these terms
arise I need to consult the internet to refresh my memory.

Given the fluidity of terms like artificial intelligence (AI) and
machine learning (ML), here, I’ll mainly use the term ML to mean any
system, implemented on a computer, that learns to associate some
**inputs** to a desired (or target) **output** without being told
explicitly what those associations are. In machine learning, this is
called **classification** – learning what things are by seeing examples
and being told the correct label or category. A simple example helps
here: Imagine you’ve never seen any examples of fruits, so words like
“apple,” “pineapple” and “banana” are meaningless to you. If I then
train you to identify fruits, I might show you examples of red and green
coloured round things and also, long, curved yellow things. Each time I
show you an example, I ask you to tell me whether it’s an apple or a
banana (or pineapple, grapefruit and so on). You are ‘rewarded’ if you
are correct but ‘penalised’ if you’re incorrect and your goal is to
adjust the responses you give so that you maximise your rewards. Over
time, after seeing enough examples you will have learned that red/green
round things are “apples” and that long, curved yellow things are
“bananas.”

In some specific contexts, clinical decision making – such as “Should I
offer a patient treatment X or Y?” – can be viewed in a similar way;
which patients (represented as inputs to the system) should be given
treatment X or treatment Y (represented as targets to the system).
Again, as for our fruit example, the system isn’t explicitly programmed
about which patients are suitable for each treatment but instead, it
learns by being shown examples of patients who are known to be suited to
treatment X and Y and the system gradually acquires implicit knowledge
about which patients should be offered X or Y.

It is important to note that when training ML systems, the data curated
for this purpose are historical patients where we **already know** the
outcomes or decisions rather than being patients currently waiting for
decisions to be made. In this clinical example, it is important that
this historical data is representative so that the ML system learns
“good practice” and doesn’t inherit flaws in the existing processes
which produced the training data and which leads to harmful **biases**
in machine learning applications.

# Why PPI is Important to CHRONOsig

From a PPI perspective, especially when ML is mentioned in the context
of clinical decision support tools, I would like to emphasise the word
**support**. The tool will not replace the clinician i.e. doctors,
nurses, care-coordinators or any member of the team of clinicians making
the decisions. CHRONOsig is there to **augment** their usual, routine
decision making processes and to help clinicians make better and quicker
decisions which will hopefully, lead to more successful treatment and
outcomes for the patient.

The proposed CDST uses natural language processing (NLP) to extract data
from patients’ electronic health records (EHRs) and combines this with
the referral information. NLP is a sub-field of artificial intelligence
and machine learning that works to capture the complexity of written
(and spoken) language in a way that computers can meaningfully process
when automating tasks as diverse as translation between languages,
answering questions or, in CHRONOsig, extracting and representing
important and relevant information that might be used to guide
clinicians when making triage decisions.

# How Patient Data is Used in CHRONOsig

In EHRs, there is a lot of ‘free text’ ie the notes made by various
clinicians relating to the patient’s diagnosis, symptoms of illness,
previous treatments, and observations from clinicians. Using NLP, this
free text is ‘translated’ into format that facilitates a computer making
decisions or inferences. For example, the computer is able to see how
different or similar two patients are on the basis of what is written in
their medical notes – much like the fruit example where “round” fruits
are more likely to be apples than bananas. Similar patients would be
expected to receive similar treatments in the same way that both red and
green ‘versions’ of apples are indeed both apples despite differing in
one property.

# Concerns about Machine Learning

Recently, there has been scrutiny around the ways ML can fail different
groups of people in society especially those from under-represented,
minority groups. Problems in ML systems have exposed that people can be
denied employment opportunity, timely and appropriate healthcare as well
as making inappropriate assumptions about a person’s sexual orientation.
Rightly, we should be sceptical about the scope, impacts and injustice
that technology can make real without the appropriate oversight and
stakeholder involvement – even when the proposed application of ML
*appears* benevolent.

Given that just and equitable access to healthcare is a clear risk in
CHRONOsig, patients are involved throughout the lifespan of this
project. The first PPI deliverable is a stakeholder impact assessment
using the FAST (Leslie 2019) principles (fairness, accountability,
sustainability and transparency) in parallel to dataset curation.
Dataset curation is the pooling and cleaning of vast amounts of data –
sometimes with humans adding information to identify categories – so
that it may be preserved and maintained for use over time. Any data used
in ML projects should be carefully inspected to ensure that it is
representative and appropriately anonymised. Where representativeness
cannot be guaranteed, steps to mitigate this must be implemented at the
outset. Our stakeholder impact assessment will include, for example, PPI
definitions of an acceptable referral i.e. what characteristics
stakeholders expect should be included or excluded from referrals, for
example, features of a patient’s presentation which are thought to
negatively bias clinical teams during existing, routine practice might
be flagged for removal from the curated data set. A concrete example of
this would be diagnoses such as personality disorders that have
historically been shown to be stigmatising and can result in clinical
services denying access to care. There may be other information which
patients and the public feel that should not be included in referrals to
triage teams even if this is current practice in NHS services. In this
way, the PPI process will inform us not just about how technology needs
safeguards but also, about how people experience their initial
interactions with the triage process more generally.

# Conclusion

What is both novel and exciting about CHRONOsig is that it potentially
offers the opportunity for a transparent and equitable triage clinical
decision support tool informed by patient and public input and this is
especially important to patients, their families as well as other
clinicians who refer people to secondary mental health services.

From a PPI perspective, there are other interesting facets; given the
obscurity in the triage process in secondary mental healthcare, it will
be interesting to see how technology can mitigate (rather than entrench)
existing practices that patients find unhelpful or frustrating. The use
of a CDST as something that augments and supports rather than replaces
clinicians is also interesting and should be welcomed particularly given
the pace at which AI and ML has been promoted in healthcare (often with
questionable results). The difficult history the NHS has had with
information technology has not always been recognised (BMA 2019), and
this challenge must be kept in mind for future AI applications (Joshi
and Morley 2019).

# References

BMA. 2019. “Technology, Infrastructure and Data Supporting NHS Staff.”
British Medical Association.
<https://www.bma.org.uk/media/2080/bma-vision-for-nhs-it-report-april-2019.pdf>.

Chew-Graham, Carolyn, Mike Slade, Carolyn Montana, Mairi Stewart, and
Linda Gask. 2007. “A Qualitative Study of Referral to Community Mental
Health Teams in the UK: Exploring the Rhetoric and the Reality.” *BMC
Health Services Research* 7 (1): 117.
<https://doi.org/10.1186/1472-6963-7-117>.

Joshi, I, and J Morley. 2019. “Artificial Intelligence: How to Get It
Right.” NHSx.
<https://www.nhsx.nhs.uk/media/documents/NHSX_AI_report.pdf>.

Leslie, David. 2019. “Understanding Artificial Intelligence Ethics and
Safety: A Guide for the Responsible Design and Implementation of AI
Systems in the Public Sector.” The Alan Turing Institute.
<https://doi.org/10.5281/ZENODO.3240529>.

Slade, M., L. Gask, M. Leese, P. McCrone, C. Montana, R. Powell, M.
Stewart, and C. Chew-Graham. 2008. “Failure to Improve Appropriateness
of Referrals to Adult Community Mental Health Services–Lessons from a
Multi-Site Cluster Randomized Controlled Trial.” *Family Practice* 25
(3): 181–90. <https://doi.org/10.1093/fampra/cmn025>.
