---
title: Overview and Background

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

{{% callout note %}}
"Every hour spent in thinking and talking about **whom** to treat, and **how**, and **how long** is being subtracted from the available pool of therapeutic time itself" - Paul E. Meehl (1954) *Clinical versus Statistical Prediction*
{{% /callout %}}


## Digital Triage

*Triaging* is where a clinician rapidly synthesises available information to make a decision about what to do next. 

For example, a clinician presented with a referral will usually have information about:

  1. the patient's medical history
  2. the current difficulty, problem or a description of unmet clinical need
  3. details of the patient's current or previous treatments

A clinician then has to decide:

  1. how urgently the patient needs to be assessed or examined
  2. which group of clinicians, specialty or team would be best suited to help

*Digital triage* is an attempt to leverage technology to assist clinicians in this task with the aim to personalise, expedite and improve access to care.

## Project Aim

CHRONOSIG, which stands for CHRONOlogical SIGnature, is a National Institute of Health Research-funded project, hosted by the Department of Psychiatry at the University of Oxford and Oxford Health NHS Foundation Trust, designed to improve triage in secondary mental health services by leveraging contemporary machine learning (ML) technology on information contained in large, observational electronic health record (EHR) data.  

{{< figure src="sponsor-logos.png" caption="" numbered="false" >}}

Each patient’s historical EHR data captures one or more instances (or episodes) of care under mental health services.  

A referral is usually provided as additional documentation to help the recieving clinician make a triage decision.

CHRONOSIG will use natural language processing (NLP) techniques to represent a patient’s longitudinal signature (or ‘fingerprint’) -- capturing their history, signs/symptoms and presenting difficulties -- and then learn associations between these signatures and triage decisions (captured as explicit structured data in patient’s EHR data).  The aim is to deliver a triage clinical decision support tool (CDST) that takes as input a patient’s referral documentation, utilises existing medical notes (when available) and delivers a suggested triage outcome to assist MDTs.


## Background
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

To this end, the chronosig project directly addresses the strategic priorities described in the Topol review (Foley & Woollard, 2019) and the NHS Long Term Plan (NHS England, 2019) that emphasise the use of EHRs to improve and personalise care for individuals.  



## Overaching Themes





## References
Abdalla, M., Abdalla, M., Hirst, G., & Rudzicz, F. (2020). Exploring the Privacy-Preserving Properties of Word Embeddings: Algorithmic Validation Study. Journal of Medical Internet Research, 22(7), e18055. https://doi.org/10.2196/18055

Bai, T., Zhang, S., Egleston, B. L., & Vucetic, S. (2018). Interpretable Representation Learning for Healthcare via Capturing Disease Progression through Time. Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, 43–51. https://doi.org/10.1145/3219819.3219904

Baracaia, S., McNulty, D., Baldwin, S., Mytton, J., Evison, F., Raine, R., Giacco, D., Hutchings, A., & Barratt, H. (2020). Mental health in hospital emergency departments: Cross-sectional analysis of attendances in England 2013/2014. Emergency Medicine Journal, emermed-2019-209105. https://doi.org/10.1136/emermed-2019-209105

Barnett, P., Mackay, E., Matthews, H., Gate, R., Greenwood, H., Ariyo, K., Bhui, K., Halvorsrud, K., Pilling, S., & Smith, S. (2019). Ethnic variations in compulsory detention under the Mental Health Act: A systematic review and meta-analysis of international data. The Lancet Psychiatry, 6(4), 305–317. https://doi.org/10.1016/S2215-0366(19)30027-6

BMA. (2019). Technology, infrastructure and data supporting NHS staff. British Medical Association. https://www.bma.org.uk/media/2080/bma-vision-for-nhs-it-report-april-2019.pdf

Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal, P., Neelakantan, A., Shyam, P., Sastry, G., Askell, A., Agarwal, S., Herbert-Voss, A., Krueger, G., Henighan, T., Child, R., Ramesh, A., Ziegler, D. M., Wu, J., Winter, C., … Amodei, D. (2020). Language Models are Few-Shot Learners. ArXiv:2005.14165 [Cs]. http://arxiv.org/abs/2005.14165

Chew-Graham, C., Slade, M., Montana, C., Stewart, M., & Gask, L. (2007). A qualitative study of referral to community mental health teams in the UK: Exploring the rhetoric and the reality. BMC Health Services Research, 7(1), 117. https://doi.org/10.1186/1472-6963-7-117

Cover, T. M. (1999). Elements of Information Theory. John Wiley and Sons.

Dalianis, H. (2018). Clinical text mining: Secondary use of electronic patient records. Springer Nature.

Devlin, J., Chang, M.-W., Lee, K., & Toutanova, K. (2019). BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding. ArXiv:1810.04805 [Cs]. http://arxiv.org/abs/1810.04805

Docherty, M., & Thornicroft, G. (2015). Specialist mental health services in England in 2014: Overview of funding, access and levels of care. International Journal of Mental Health Systems, 9(1), 34. https://doi.org/10.1186/s13033-015-0023-9

Foley, J., & Woollard, J. (2019). Digital Future of Mental Healthcare Report. https://topol.hee.nhs.uk/wp-content/uploads/HEE-Topol-Review-Mental-health-paper.pdf

Jehn, K. A., & Mannix, E. A. (2001). The Dynamic Nature of Conflict: A Longitudinal Study of Intragroup Conflict and Group Performance. The Academy of Management Journal, 44(2), 238–251. https://doi.org/10.2307/3069453

Joshi, I., & Morley, J. (2019). Artificial Intelligence: How to get it right. NHSx. https://www.nhsx.nhs.uk/media/documents/NHSX_AI_report.pdf

Joyce, D. W., & Geddes, J. (2020). When Deploying Predictive Algorithms, Are Summary Performance Measures Sufficient? JAMA Psychiatry, 77(5), 447. https://doi.org/10.1001/jamapsychiatry.2019.4484

Jung, C., Kearns, M., Neel, S., Roth, A., Stapleton, L., & Wu, Z. S. (2020). An Algorithmic Framework for Fairness Elicitation. ArXiv:1905.10660 [Cs, Stat]. http://arxiv.org/abs/1905.10660

Kormilitzin, A., Vaci, N., Liu, Q., & Nevado-Holgado, A. (2021). Med7: A transferable clinical natural language processing model for electronic health records. Artificial Intelligence in Medicine, 118, 102086. https://doi.org/10.1016/j.artmed.2021.102086

Kormilitzin, A., Vaci, N., Liu, Q., Ni, H., Nenadic, G., & Nevado-Holgado, A. (2020). An efficient representation of chronological events in medical texts. ArXiv:2010.08433 [Cs]. http://arxiv.org/abs/2010.08433

Leetaru, K., & Schrodt, P. A. (2013). GDELT: Global Data on Events, Location and Tone,. ISA Annual Convention, 2, 1–49. http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.686.6605&rep=rep1&type=pdf

Lehman, E., Jain, S., Pichotta, K., Goldberg, Y., & Wallace, B. C. (2021). Does BERT Pretrained on Clinical Notes Reveal Sensitive Data? ArXiv:2104.07762 [Cs]. http://arxiv.org/abs/2104.07762

Leslie, D. (2019). Understanding artificial intelligence ethics and safety: A guide for the responsible design and implementation of AI systems in the public sector. Zenodo. https://doi.org/10.5281/ZENODO.3240529

Longoni, C., Bonezzi, A., & Morewedge, C. K. (2019). Resistance to Medical Artificial Intelligence. Journal of Consumer Research, 46(4), 629–650. https://doi.org/10.1093/jcr/ucz013

Nagendran, M., Chen, Y., Lovejoy, C. A., Gordon, A. C., Komorowski, M., Harvey, H., Topol, E. J., Ioannidis, J. P. A., Collins, G. S., & Maruthappu, M. (2020). Artificial intelligence versus clinicians: Systematic review of design, reporting standards, and claims of deep learning studies. BMJ, 368, m689. https://doi.org/10.1136/bmj.m689

NHS Digital. (2020). Mental Health Bulletin: 2019-20 Annual Report. https://digital.nhs.uk/data-and-information/publications/statistical/mental-health-bulletin/2019-20-annual-report

NHS Digital. (2021). Mental Health Services Monthly Statistics, March/April 2021. https://digital.nhs.uk/data-and-information/publications/statistical/mental-health-services-monthly-statistics/final-march-2021

NHS England. (2019). The NHS Long Term Plan.

NHS England. (2020). National Cost Collection 2019. NHS England and NHS Improvement. https://www.england.nhs.uk/wp-content/uploads/2020/08/1_-_NCC_Report_FINAL_002.pdf

NICE. (2011). Service user experience in adult mental health: Improving the experience of care for people using adult NHS mental health services (No. CG136; p. 32). https://www.nice.org.uk/guidance/cg136/resources/service-user-experience-in-adult-mental-health-improving-the-experience-of-care-for-people-using-adult-nhs-mental-health-services-pdf-35109513728197

Obermeyer, Z., Powers, B., Vogeli, C., & Mullainathan, S. (2019). Dissecting racial bias in an algorithm used to manage the health of populations. Science, 366, 447–453.

ONS. (2018). Equalities data audit, final report—Office for National Statistics. https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/equalitiesdataauditfinalreport

Rajkomar, A., Hardt, M., Howell, M. D., Corrado, G., & Chin, M. H. (2018). Ensuring Fairness in Machine Learning to Advance Health Equity. Annals of Internal Medicine, 169(12), 866–872. https://doi.org/10.7326/M18-1990

RCPsych. (2020, October 6). Two-fifths of patients waiting for mental health treatment forced to resort to emergency or crisis services. Www.Rcpsych.Ac.Uk. https://www.rcpsych.ac.uk/news-and-features/latest-news/detail/2020/10/06/two-fifths-of-patients-waiting-for-mental-health-treatment-forced-to-resort-to-emergency-or-crisis-services

Samek, W., Wiegand, T., & Müller, K.-R. (2017). Explainable Artificial Intelligence: Understanding, Visualizing and Interpreting Deep Learning Models. ArXiv:1708.08296 [Cs, Stat]. http://arxiv.org/abs/1708.08296

Senior, M., Burghart, M., Yu, R., Kormilitzin, A., Liu, Q., Vaci, N., Nevado-Holgado, A., Pandit, S., Zlodre, J., & Fazel, S. (2020). Identifying Predictors of Suicide in Severe Mental Illness: A Feasibility Study of a Clinical Prediction Rule (Oxford Mental Illness and Suicide Tool or OxMIS). Frontiers in Psychiatry, 11, 268. https://doi.org/10.3389/fpsyt.2020.00268

Slade, M., Gask, L., Leese, M., McCrone, P., Montana, C., Powell, R., Stewart, M., & Chew-Graham, C. (2008). Failure to improve appropriateness of referrals to adult community mental health services—Lessons from a multi-site cluster randomized controlled trial. Family Practice, 25(3), 181–190. https://doi.org/10.1093/fampra/cmn025

Stonewall. (2018, November 7). LGBT in Britain—Health. Stonewall. https://www.stonewall.org.uk/lgbt-britain-health

Tomasev, N., McKee, K. R., Kay, J., & Mohamed, S. (2021). Fairness for Unobserved Characteristics: Insights from Technological Impacts on Queer Communities. Proceedings of the 2021 AAAI/ACM Conference on AI, Ethics, and Society, 254–265. https://doi.org/10.1145/3461702.3462540

Toth, C., Bonnier, P., & Oberhauser, H. (2020a). Seq2Tens: An efficient representation of sequences by low-rank tensor projections. github.com/tgcsaba/seq2tens

Toth, C., Bonnier, P., & Oberhauser, H. (2020b). Seq2Tens: An Efficient Representation of Sequences by Low-Rank Tensor Projections. ArXiv:2006.07027 [Cs, Stat]. http://arxiv.org/abs/2006.07027

Vickers, A. J., & Elkin, E. B. (2006). Decision Curve Analysis: A Novel Method for Evaluating Prediction Models. Medical Decision Making, 26(6), 565–574. https://doi.org/10.1177/0272989X06295361

Wang, Y., Wang, L., Rastegar-Mojarad, M., Moon, S., Shen, F., Afzal, N., Liu, S., Zeng, Y., Mehrabi, S., Sohn, S., & Liu, H. (2018). Clinical information extraction applications: A literature review. Journal of Biomedical Informatics, 77, 34–49. https://doi.org/10.1016/j.jbi.2017.11.011

Zaheer, M., Guruganesh, G., Dubey, A., Ainslie, J., Alberti, C., Ontanon, S., Pham, P., Ravula, A., Wang, Q., Yang, L., & Ahmed, A. (2020). Big Bird: Transformers for Longer Sequences. 34th Conference on Neural Information Processing Systems (NeurIPS 2020), 12253–12266. https://proceedings.neurips.cc/paper/2020/file/c8512d142a2d849725f31a9a7a361ab9-Paper.pdf?utm_campaign=NLP%20News&utm_medium=email&utm_source=Revue%20newsletter

Zhang, D., Thadajarassiri, J., Sen, C., & Rundensteiner, E. (2020). Time-Aware Transformer-based Network for Clinical Notes Series Prediction. Machine Learning for Healthcare Conference, 566–588.




