# Task 4 - Shared task on Multimodal Hate Speech Detection #

Hate speech detection is one of the most important aspects of event identification during political events like invasions. In the case of hate speech detection, the event is the occurrence of hate speech, the entity is the target of the hate speech, and the relationship is the connection between the two. Since multimodal content is widely prevalent across the internet, the detection of hate speech in text-embedded images is very important. Given a text-embedded image, this task aims to automatically identify the hate speech and its targets. This task will have two subtasks.

## Sub-task A ##
<b> Hate Speech Detection:</b> The goal of this task is to identify whether the given text-embedded image contains hate speech or not. The text-embedded images, which are the dataset for this subtask, will have annotations for the prevalence of hate speech.

The dataset for this sub-task has two labels viz. "Hate Speech" and "No Hate Speech".

## Sub-task B ##
<b> Target Detection:</b> The goal of this subtask is to identify the targets of hate speech in a given hateful text-embedded image. The text-embedded images are annotated for "community", "individual" and "organization" targets.

To know more about the dataset, please refer to our [paper](Paper/crisishatemm.pdf).


## Participation ##

In order to participate in the competition, please fill out the form provided [here](https://forms.gle/qEVTUvPBRC7Q3zhAA). 

You will be provided training data.

## Evaluation ## 

We accept results only through the google form.

After the test data is released, the predictions made by the model should be provided to the organizers in csv format. The submission will be named as "teamname_subtask.csv". If your teamname is "hatewatchers" and you are submitting the results for "subtask A", your csv should be named as "hatewatchers_subtaskA.csv". The predictions should be submitted in the google form (provided after release of test data). The submission will be evaluated with a macro average f1-score. More about macro f1-score can be found [here](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html).

## Timeline of the Events ##
<ul>

<li>Task Announcement: May 01, 2023 </li>

<li>Release of the training data: May 01, 2023 </li>

<li>Release of Test Data: June 15, 2023 </li>

<li>Run Submission Deadline: June 30, 2023 </li>

<li>Results Declared: July 01, 2023 </li>

<li>Paper Submission: July 10, 2023 </li>

<li>Peer Review Notification: Aug 05, 2023 </li>

<li>Camera-ready Versions: Aug 25, 2023 </li>

<li>CASE Workshop: 7-8 September </li>
</ul>

## Contact ##
If there are any questions related to the competition, please contact surendrabikram@vt.edu

## References ##

If you use the dataset, please cite as follows:

```bibtex
@inproceedings{bhandari2023crisishatemm,
  title={CrisisHateMM: Multimodal Analysis of Directed and Undirected Hate Speech in Text-Embedded Images from Russia-Ukraine Conflict},
  author={Bhandari, Aashish and Shah, Siddhant Bikram and Thapa, Surendrabikram and Naseem, Usman and Nasim, Mehwish},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  year={2023}
}
```
