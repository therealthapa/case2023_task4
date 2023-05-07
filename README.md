# Task 4 - Shared task on Multimodal Hate Speech Event Detection at [CASE 2023](https://emw.ku.edu.tr/case-2023/) #

Hate speech detection is one of the most important aspects of event identification during political events like invasions. In the case of hate speech detection, the event is the occurrence of hate speech, the entity is the target of the hate speech, and the relationship is the connection between the two. Since multimodal content is widely prevalent across the internet, the detection of hate speech in text-embedded images is very important. Given a text-embedded image, this task aims to automatically identify the hate speech and its targets. This task will have two subtasks.

## Sub-task A ##
<b> Hate Speech Detection:</b> The goal of this task is to identify whether the given text-embedded image contains hate speech or not. The text-embedded images, which are the dataset for this subtask, will have annotations for the prevalence of hate speech.

The dataset for this sub-task has two labels viz. "Hate Speech" and "No Hate Speech".

## Sub-task B ##
<b> Target Detection:</b> The goal of this subtask is to identify the targets of hate speech in a given hateful text-embedded image. The text-embedded images are annotated for "community", "individual" and "organization" targets.

To know more about the dataset, please refer to our [paper](Paper/crisishatemm.pdf).
The sample codes for both the subtasks are provided in the repo. 


## Participation ##

In order to participate in the competition, please fill out the form provided [here](https://forms.gle/qEVTUvPBRC7Q3zhAA). 
Join our codalab competition [here](https://codalab.lisn.upsaclay.fr/competitions/13087).

Upon completion of the form, you will be provided training data and evaluation data.

## Evaluation ## 

The results are only accepted in codalab. The submission will be evaluated with a f1-score.

The script takes one prediction file as the input. Your submission file must be a JSON file which is then zipped. We will only take the first file in the zip folder, so do not zip multiple files together. 

For subtask A, the final prediction submissions should be like the following. Make sure that your hate label is given as "1" and non-hate label is given as "0".

```python
{"index": 98452, "prediction": 1}
{"index": 45865, "prediction": 0}
{"index": 23568, "prediction": 1}
```

Similarly, for the subtask B, the final prediction submissions should be like the following. Make sure that your individual, community, and organization labels are given as "0", "1", and "2" respectively.

```python
{"index": 45865, "prediction": 0}
{"index": 23568, "prediction": 1}
{"index": 36987, "prediction": 2}
```


## Publication ##

Participants in the Shared Task are expected to submit a paper to the workshop. Submitting a paper is not mandatory for participating in the Shared Task. Papers must follow the CASE 2023 workshop submission instructions and will undergo regular peer review. Their acceptance will not depend on the results obtained in the shared task but on the quality of the paper. Authors of accepted papers will be informed about the evaluation results of their systems prior to the paper submission deadline (see the important dates). All the accepted papers will be published in ACL Anthology.

## Invitation for Special Issue ##
Top performing teams and best models will be invited for an special issue in journals (T.B.D.).

## Timeline of the Events ##
<ul>

<li>Training & Evaluation data available: May 1, 2023 </li>

<li>Test data available: Jun 15, 2023  </li>

<li>Test start: Jun 15, 2023  </li>

<li>Test end: Jun 30, 2023  </li>

<li>System Description Paper submissions due: Jul 10, 2023</li>

<li>Notification to authors after review: Aug 5, 2023 </li>

<li>Camera ready: Aug 25, 2023 </li>

<li>CASE Workshop: 7-8 September </li>
</ul>

## Organizers ##
<ul>
<li> Surendrabikram Thapa (Virginia Tech, USA) </li>
<li> Usman Naseem (University of Sydney, Australia) </li>
<li> Farhan Ahmad Jafri (Jamia Millia Islamia, India) </li>
<li> Francielle Vargas (University of São Paulo, Brazil) </li>
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
