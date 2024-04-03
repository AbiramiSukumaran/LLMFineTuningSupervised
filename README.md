# LLMFineTuningSupervised
We will fine tune text-bison@002 to a new fine-tuned model called "bbc-news-summary-tuned" and compare the result the response from the base model. This lab teaches you how to tune a foundational model on new unseen data and you will use the following Google Cloud products:
*   Vertex AI Pipelines
*   Vertex AI Evaluation Services
*   Vertex AI Model Registry
*   Vertex AI Endpoints

# Model Tuning

Model fine-tuning is a powerful technique used to improve the performance of pre-trained language models (LLMs) for specific tasks or domains. It involves adjusting the model's parameters based on a new dataset or task-specific data to enhance its ability to make accurate predictions or generate relevant text. By fine-tuning an LLM, we can leverage its existing knowledge and adapt it to a specific context, resulting in improved results and better-tailored outputs.

Tuning a foundation model can improve its performance. Foundation models are trained for general purposes and sometimes don't perform tasks as well as you'd like them to. This might be because the tasks you want the model to perform are specialized tasks that are difficult to teach a model by using only prompt design. In these cases, you can use model tuning to improve the performance of a model for specific tasks. Model tuning can also help it adhere to specific output requirements when instructions aren't sufficient. This page provides an overview of model tuning, describes the tuning options available on Vertex AI, and helps you determine when each tuning option should be used. More here.

# Use Case & Dataset
Using Generative AI we will generate a suitable TITLE for a news BODY from BBC FULLTEXT DATA (BigQuery Public Dataset bigquery-public-data.bbc_news.fulltext).
We will fine tune text-bison@002 to a new fine-tuned model called "bbc-news-summary-tuned" and compare the result the response from the base model. The [JSONL]([url](https://github.com/AbiramiSukumaran/LLMFineTuningSupervised/blob/main/TRAIN.jsonl)) is made available for the implementation, feel free to upload it to your Cloud Storage Bucket to execute the fine tuning steps.

# Steps
Data Prep,

Exploratory analysis with Vertex AI Studio / SDKs,

Training (Fine tuning of a base model),

Evaluate,

Deploy,

Test & Serve,

Monitor
