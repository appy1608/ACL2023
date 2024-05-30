# ACL2023

This is the repository for the ACL 2023 full paper [Peeking inside the black box: A Commonsense-Aware Generative Framework for Explainable Complaint Detection](https://2023.aclweb.org/program/accepted/#long-papers). 

**Authors**

Apoorva Singh*, Raghav Jain*, Prince Jha and Sriparna Saha

*:Denotes equal contribution.


**X-CI Dataset**

The X-CI dataset includes the tweet text, complaint label, severity level, polarity label and emotion label, and annotated cause for each instance. Annotators were asked to find the causal span, X(I), that best described the foundation of the complaint (C) or non-complaint (NC)  label for each occurrence (I) in the X-CI dataset. If there is no mention of X(I) for C/NC in I, the sentence was tagged as 'no cause' by the annotators. 


**Annotation Guidelines**

 Complaint Cause is the speech act used by the individual to describe the circumstances in which their expectations have been violated. The annotators were instructed to mark causal span based on first encounter with strong expression of complaint reason in the tweet, it could be any length of text. Some example instances were also given before the annotation procedure began.

For example: 'Disappointed with the seller. Product delivery was quite fast, but the display is scratched on the front and left side. 

Rationale annotated: 'the display is scratched on the front and left side.' 

In the given example the first sentence shows weak intensity of complaint cause. But the selected causal span shows strong cause of complaint.

In circumstances where annotators disagree, the final label is determined through majority voting (cause vs. no cause). For ambiguous instances, the authors discuss and clarify them with the annotators during the annotation procedure.


**Citation**

@inproceedings{singh-etal-2023-peeking,
    title = "Peeking inside the black box: A Commonsense-aware Generative Framework for Explainable Complaint Detection",
    author = "Singh, Apoorva  and
      Jain, Raghav  and
      Jha, Prince  and
      Saha, Sriparna",
    editor = "Rogers, Anna  and
      Boyd-Graber, Jordan  and
      Okazaki, Naoaki",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.404",
    doi = "10.18653/v1/2023.acl-long.404",
    pages = "7333--7347",
    abstract = "Complaining is an illocutionary act in which the speaker communicates his/her dissatisfaction with a set of circumstances and holds the hearer (the complainee) answerable, directly or indirectly. Considering breakthroughs in machine learning approaches, the complaint detection task has piqued the interest of the natural language processing (NLP) community. Most of the earlier studies failed to justify their findings, necessitating the adoption of interpretable models that can explain the model{'}s output in real time. We introduce an explainable complaint dataset, X-CI, the first benchmark dataset for explainable complaint detection. Each instance in the X-CI dataset is annotated with five labels: complaint label, emotion label, polarity label, complaint severity level, and rationale (explainability), i.e., the causal span explaining the reason for the complaint/non-complaint label. We address the task of explainable complaint detection and propose a commonsense-aware unified generative framework by reframing the multitask problem as a text-to-text generation task. Our framework can predict the complaint cause, severity level, emotion, and polarity of the text in addition to detecting whether it is a complaint or not. We further establish the advantages of our proposed model on various evaluation metrics over the state-of-the-art models and other baselines when applied to the X-CI dataset in both full and few-shot settings.",
}
