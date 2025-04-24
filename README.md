## RevieWeaver: Weaving Together Review Insights by Leveraging LLMs and Semantic Similarity

[Accepted in NAACL 2025 Industry Track](https://2025.naacl.org/program/accepted_papers/#industry-track-papers)

[See the camrea ready version](https://github.com/sworborno/RevieWeaver/blob/main/artifacts/NAACL_Ind_2025_camera_ready.pdf)

[See the poster](https://github.com/sworborno/RevieWeaver/blob/main/artifacts/109_ind_RevieWeaver_poster.pdf)

[See the prerecorded video presentation](https://s3.amazonaws.com/pf-user-files-01/u-59356/uploads/2025-04-06/tn73wlc/109_ind_RevieWeaver_prerecording.mp4)

<img src="https://github.com/sworborno/RevieWeaver/blob/main/images/bby-distill-summary-airpods-4.jpg" width="500"/> 

### Abstract
> With the rise of online retail, customer reviews have become a critical factor in shaping purchasing decisions. The sheer volume of customer reviews being generated continuously presents a challenge for consumers who must sift through an overwhelming amount of feedback. To address this issue, we introduce RevieWeaver, a novel framework that extracts key product features and provides concise review summaries. Our innovative approach not only scales efficiently to 30 million reviews but also ensures reproducibility and controllability. Moreover, it delivers unbiased and reliable assessments of products that accurately reflect the input reviews.

### Quickstart
We have provided the reviews in this [file](https://github.com/sworborno/RevieWeaver/blob/main/data/product_reviews.pkl). 

#### Step 1: Aspect Extraction
Use the notebook provided [here](https://github.com/sworborno/RevieWeaver/blob/main/notebooks/aspect-extraction.ipynb) to extract the tuples of (aspect, sentiment, and representative sentence) from each review. 

#### Step 2: Grouping Aspects to Features
- Use the [notebook](https://github.com/sworborno/RevieWeaver/blob/main/notebooks/topic-modeling-dbscan.ipynb) to group aspects using dbscan.
- Use the [notebook](https://github.com/sworborno/RevieWeaver/blob/main/notebooks/topic-modeling-hdbscan.ipynb) to group aspects using hdbscan.
- Use the [notebook](https://github.com/sworborno/RevieWeaver/blob/main/notebooks/topic-modeling-revieweaver.ipynb) to group aspects using ReviewWeaver. 

#### Step 3: Generating Summaries
Use the [notebook](https://github.com/sworborno/RevieWeaver/blob/main/notebooks/summary-generation-revieweaver-llm.ipynb) to generate summaries using distilled features by RevieWeaver and an LLM.

### Citation
```
@inproceedings{adhikary-etal-2025-revieweaver,
    title = "RevieWeaver: Weaving Together Review Insights by Leveraging LLMs and Semantic Similarity",
    author = "Adhikary, Jiban  and
      Alqudah, Mohammad  and
      Arun, Udayashankar",
    booktitle = "Proceedings of the 2025 Conference of the North American Chapter of the Association for Computational Linguistics (Industry Track)",
    month = April,
    year = "2025",
    address = "Albuquerque, New Mexico",
    publisher = "Association for Computational Linguistics",
}
```
