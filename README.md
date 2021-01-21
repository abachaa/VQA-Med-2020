# VQA-Med-2020
-------------

Website: https://www.imageclef.org/2020/medical/vqa/

Mailing list: https://groups.google.com/d/forum/imageclef-vqa-med

Paper: http://ceur-ws.org/Vol-2696/paper_106.pdf

Tasks: Visual Question Answering (VQA) and Visual Question Generation (VQG) in the medical domain. 

Results of the VQA-Med-2020 challenge on crowdAI: 

- VQA task: https://www.aicrowd.com/challenges/imageclef-2020-vqa-med
- VQG task: https://www.aicrowd.com/challenges/imageclef-2020-vqa-med-vqg 


Data: 
--------------

VQA Data: 
- Training set: 4,000 radiology images with 4,000 associated Question-Answer (QA) pairs (https://www.aicrowd.com/challenges/imageclef-2020-vqa-med).
- Validation set: 500 radiology images with 500 QA pairs (https://github.com/abachaa/VQA-Med-2020/blob/main/VQA-ValidationSet-VQAMed2020-Task1.zip).
- Test set: 500 radiology images with 500 associated questions (https://github.com/abachaa/VQA-Med-2020/blob/main/VQA-TestSet-ReferenceAnswers-VQAMed2020-Task1.zip). 


VQG Data:

- Training set: 780 radiology images with 2,156 associated questions.
- Validation set: 141 radiology images with 164 questions.
- Test set: 80 radiology images. 

All VQG datasets are available at https://www.aicrowd.com/challenges/imageclef-2020-vqa-med-vqg (under the "Resources" tab). 

Evaluation Metrics
------------------

Accuracy: We used an adapted version of the accuracy metric from the general domain VQA task that considers exact matching of a participant provided answer and the ground truth answer.

BLEU: We used the BLEU metric to capture the similarity between a system-generated answer and the ground truth answer. 

The following preprocessing is applied before running the evaluation metrics on each answer: (i) each answer is converted to lower-case, and (ii) all punctuations are removed and the answer is tokenized to individual words. 


Code: https://github.com/abachaa/VQA-Med-2020/blob/main/Evaluator-VQA-Med-2020.py.

Reference
----------

If you use the VQA-Med 2020 dataset, please cite our paper: "Overview of the VQA-Med Task at ImageCLEF 2020: Visual Question Answering and Generation in the Medical Domain". 
Asma Ben Abacha, Vivek V. Datla, Sadid A. Hasan, Dina Demner-Fushman and Henning Müller. CLEF 2020 Working Notes.

@Inproceedings{ImageCLEFVQA-Med2020,

    author = {Asma {Ben Abacha} and Vivek V. Datla and Sadid A. Hasan and Dina Demner-Fushman and Henning M\"uller},
    title = {Overview of the VQA-Med Task at ImageCLEF 2020: Visual Question Answering and Generation in the Medical Domain},
    
    booktitle = {CLEF 2020 Working Notes},
    
    series = {{CEUR} Workshop Proceedings},
    
    year = {2020},
    
    publisher = {CEUR-WS.org $<$http://ceur-ws.org$>$},
    
    month = {September 22-25},
    
    address = {Thessaloniki, Greece}
    }
    
    
Contact Information
--------------------

Asma Ben Abacha: asma.benabacha@nih.gov    https://sites.google.com/site/asmabenabacha/
