# ACL2023

This is the official repository for the ACL 2023 full paper [Peeking inside the black box: A Commonsense-Aware Generative Framework for Explainable Complaint Detection](https://2023.aclweb.org/program/accepted/#long-papers). This repository contains codebase, dataset and the annotation guidelines.

**Authors**
Apoorva Singh*, Raghav Jain*, Prince Jha and Sriparna Saha
*:Denotes equal contribution.

**X-CI Dataset**

The X-CI dataset includes the tweet text, complaint label, severity level, polarity label and emotion label, and annotated cause for each instance. Annotators were asked to find the causal span, X(I), that best described the foundation of the complaint (C) or non-complaint (NC)  label for each occurrence (I) in the X-CI dataset. If there is no mention of X(I) for C/NC in I, the sentence was tagged as 'no cause' by the annotators. It is worth noting that  95%  of the instances in the dataset have only either complaint or non-complaint cause, while 5% have no cause.

**Annotation Guidelines**

Before the annotation procedure began the concept of rationale/causal span detection and extraction, specifically for complaint causes was defined to the annotators. Complaint Cause is the speech act used by the individual to describe the circumstances in which their expectations have been violated. The annotators were instructed to mark causal span based on first encounter with strong expression of complaint reason in the tweet, it could be any length of text. Some example instances were also given before the annotation procedure began.
For example: 'Disappointed with the seller. Product delivery was quite fast, but the display is scratched on the front and left side. \\
Rationale annotated: 'the display is scratched on the front and left side.' 
In the given example the first sentence shows weak intensity of complaint cause. But the selected causal span shows strong cause of complaint.\\
In circumstances where annotators disagree, the final label is determined through majority voting (cause vs. no cause). For ambiguous instances, the authors discuss and clarify them with the annotators during the annotation procedure.

**Citation**
TBD
