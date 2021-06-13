# GSoC_Accord_Project

## Week 1 (06/07 - 06/13)

This week I mainly prepare my final exam (end at 6/11).

### 6/7
I have a discuession with my mentor, Niall, for kick-off and the plan on the following week.

Niall guide me walk through templates patiently to help me understand the relationship between Templates, DataType, and Models. ([Meeting Notes](https://hackmd.io/@EasonC/Bk6rH_i5_))

### 6/12

#### Start with good tools
I set up the environments for this project, include this GitHub-Repo and the manage trello, miro board.

#### Learn on reading documents.

I read ERGO and CTO document to help me understand more about them. 

#### Spider templates
I ["spider" all templates](https://github.com/EasonC13/GSoC_Accord_Project/blob/main/crawler_data/0612_crawler_files.ipynb) form [Template Studio](https://templates.accordproject.org/) via python's file walkthrough the [File from Git Repo](https://github.com/accordproject/cicero-template-library).

This job have two propose:
1. Data mining on template studio to help me understand the data.
2. Prepare data for model training step afterward.

#### Data mining on template studio's data
I [count keywords](https://github.com/EasonC13/GSoC_Accord_Project/blob/main/crawler_data/count_keyword.ipynb) (ex: buyer, seller, value) and [count datatype](https://github.com/EasonC13/GSoC_Accord_Project/blob/main/crawler_data/count_object.ipynb) (ex: Party, String) to understand the amount of data avalialbe and the summary of them.

I also found a bug on template library, so I [open an issue](https://github.com/accordproject/cicero-template-library/issues/393) about it.

#### Discuess with my NLP professor.
I discuess with my NLP professor Sam for hierarchical clustering job. We figure out that our goal might be able to done via the BERT NER model with some modification on the last layer. (change to softmax output)

### 6/13

#### Create the PPT for prototype on how user interact with model on template studio.
I create the PPT for prototype on how user interact with model on template studio. I think it could work like [Grammarly](https://app.grammarly.com/). That is, user paste their contract text, then model show the prediction of the keyword and datatype, finally, user correct them and export the contract file.

I will use it to discuess with Niall at Monday. Hope it can be demo on Wednesday's Technology-WG meeting.

#### Plan on next week
I think [these amount of data](https://github.com/EasonC13/GSoC_Accord_Project/blob/main/README.md#data-mining-on-template-studios-data) is worthy for a try. (via pre-train model and snorkel)
So my next step will devide into four part:

1. create Pipeline to Prepare data for try-run NER model training.
2. Learn on how to use Snorkel to augmented data.
3. Research and implement on edit NER model let it have softmax-like output.
4. Discuss UX/UI for how end user to use model on template studio with mentor.
