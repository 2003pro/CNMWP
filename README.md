# NLPCC2023 Shared Task 3: Math Word Problem Solving
## Task Introduction 

In the math word problem solving (MWP) task, the objective is to develop a model that can automatically read and comprehend a math word problem and then produce a numerical solution. To achieve this goal, models must effectively understand both the natural language text and underlying mathematical concepts that are necessary for solving the problem.

## Updates

All updates about this shared task will be posted on this page.

## Important Dates

- 2023/03/15：registration open
- 2023/04/06：release of detailed task guidelines & training data
- 2023/05/05：registration deadline
- 2023/05/21：release of test data
- 2023/05/31：participants’ results submission deadline
- 2023/06/10：evaluation results release and call for system reports and conference paper

## Data Description & Rules

In this math word problem solving task, we provide three datasets for training, validation, and testing purposes.

- The training dataset comprises 23,162 MWP examples. Each example consists of an input MWP text, an equation, and a corresponding answer. The complete training dataset can be found in the data folder of this Github Repository.
- The validation dataset includes 1,200 MWP examples, with each example comprising an input text and an answer. This dataset can be used for model performance testing and hyper-parameter tuning. However, it is not suitable for direct model training. The complete validation dataset can be found in the data folder of this Github Repository.
- The test dataset, which will be released on 05/21, consists of 1,200 MWP examples. Participants are expected to utilize their developed model to solve MWPs in the test set and generate corresponding answers.

## Submission & Evaluation

For submission, the following materials should be packaged as one `zip` file and sent to jzhanggr@connect.ust.hk:

- Submission File: The output sentences should be written into one text file. We will provide a submission sample file to show the format at 05/21 . 
- Code: The code folder should contain all the codes of data augmentation, data processing, model training and model inference. 
- Document: 
  - **Data Description: The document needs to contain a brief description of supervised and unsupervised data used in the experiment, as well as the data augmentation methods for unsupervised data.**
  - **Sharing Link of Unsupervised Data: Unsupervised data used in the experiment should be uploaded to a cloud storage, i.e., net disk, and the sharing link should be included in the document.** It is not allowed to use data that violates the rules during model training. 
  - **Code Reproduction Process: The submitted code may be checked and reproduced by us, so please briefly explain the process of reproducing the code in the document.** 
  - **Large Language Model Usage: If a large language model such as ChatGPT/GPT-4 is used in any of the steps, please specify it. Directly calling the API will not be considered eligible.**

For evaluation, answer accuracy is used to assess all models. This involves comparing the generated answer to the corresponding ground truth answer. If the generated answer is identical to the ground truth answer, we consider it as correct. Conversely, if the generated answer is different from the ground truth answer, we consider it as incorrect.

## Participants

| Team ID | Organization                                                 | System Name        |
| ------- | ------------------------------------------------------------ | ------------------ |
| 01       | SAT premilab of Xi’an Jiaotong-Liverpool University          | Lagrange           |
| 02       | The Open University of China                                 | OUC_NLP            |
| 03       | Faculty of Artificial Intelligence in Education, Central China Normal University | The Burning Legion |
| 04       | Central China Normal University, Faculty of Artificial Intelligence in Education, Xinguo Yu Research Group | Mimic Solver       |
| 05       | Zhongyuan University of Technology | zutnlp-wuyanbo       |
| 06       | Zhongyuan University of Technology | Zutnlp_pengzirong      |
| 07       | Yunnan University | Tsingriver      |
| 08       | Google | Xiao_Shan_Friend     |
| 09       | Chongqing Technology & Business Institute | its666     |
| 10       | NLP, School of Computer Science and Technology, Soochow University. NLP, School of Data Science, The Chinese University of Hong Kong, Shenzhen | CUHK_SU     |
| 11       | Beijing Language and Culture University | BLCU-LCClab     |
| 12       | Fudan University | cisl-nlp     |
| 13       | Ant Group | Lastonestands     |
| 14       | School of Information Science and Engineering, Yunnan University | YNU-PCJ     |
| 15       | Convai, School of Artificial Intelligence, Nanjing University | Mdager     |
| 16       | Text Machine Translation Lab, Huawei Technologies Co., Ltd. | HW-TSC     |
| 17       | Center for Future Media, University of Electronic Science and Technology of China | Rush up     |
| 18       | School of Information Science and Engineering, Shandong Normal University | HPC-NLP |

## Submission

You may follow the format in `./data/submission_sample.csv` to organize your own submission file. Finally, a submission file named with `submission_<Team ID>.csv`(like `submission_01.csv`) is expected to be sent to us. 

## Leaderboard

| id | team             | score |
|----|-----------------|-------|
| 1  | Mimic Solver    | 45.83 |
| 2  | Lagrange        | 29.75 |
| 3  | Rush up         | 24.08 |
| 4  | Tsingriver      | 23.66 |
| 5  | BLCU-LCClab     | 22.58 |
| 6  | The Burning Legion | 20.75 |
| 7  | YNU-PCJ         | 19.16 |

## FAQ
**Q**: Detailed information about the prize and certificates?

**A**: The top 3 teams will be awarded certification from NLPCC and CCF-NLP. For more information, please visit the official NLPCC website: [NLPCC Website](http://tcci.ccf.org.cn/conference/2023/cfpt.php#:~:text=The%20top%203%20participating%20teams%20of%20each%20task%20will%20be%20certificated%20by%20NLPCC%20and%20CCF%2DNLP.%20If%20a%20task%20has%20multiple%20sub%2Dtasks%20or%20tracks%2C%20only%20the%20top%201%20participating%20team%20of%20each%20sub%2Dtask/track%20will%20be%20certificated.)

**Q**: How to make paper submission for Shared Task?

**A**: The top 3 teams will be invited to submit papers to the NLPCC conference. The submitted papers will undergo a review process, and if they meet NLPCC's publication acceptance standards, they will be published in the Shared Task Track of NLPCC 2023.

**Q**: Details about submission?

**A**: Submission Deadline: 2023/06/30. Submission website: https://www.softconf.com/nlpcc/Eval-2023/. For more details, please refer [NLPCC Website](http://tcci.ccf.org.cn/conference/2023/cfpt.php)

## Contact & Citation

```
@inproceedings{wang2017deep,
  title={Deep neural solver for math word problems},
  author={Wang, Yan and Liu, Xiaojiang and Shi, Shuming},
  booktitle={Proceedings of the 2017 conference on empirical methods in natural language processing},
  pages={845--854},
  year={2017}
}

@article{liang2022generalizing,
  title={Generalizing Math Word Problem Solvers via Solution Diversification},
  author={Liang, Zhenwen and Zhang, Jipeng and Wang, Lei and Wang, Yan and Shao, Jie and Zhang, Xiangliang},
  journal={arXiv preprint arXiv:2212.00833},
  year={2022}
}
```

If you have any questions about this task, please email to jzhanggr@connect.ust.hk