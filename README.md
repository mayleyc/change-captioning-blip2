# change-captioning-blip2
A project to assess the change captioning and path finding ability of BLIP-2.

Successfully ran on a T4 graphics card. 16GB of RAM is needed.

**Installation:**
- Download the dataset at: https://drive.google.com/drive/folders/16kBcXa9lmqobrpqSq72oetGiL95b3ia7?usp=sharing
- Unzip the dataset in the same folder as the main.py file
- Open an interpreter with virtual environments. Create a new virtual environment and install the needed modules using

`pip install -r requirements.txt`
- Run main.py using `python3 main.py`

After the program downloads the necessary shards of BLIP-2, the program will prompt you to enter 0 or 1 to use either mode. There will be two modes: easy (0) and hard (1), corresponding to the two datasets.

**The output includes:**
- answers_step1: The original answers (change captioning) by BLIP-2.
- output_step1: Accurate change captioning answers only.
- answer_step2_batch: Attempts at path-planning. You can test it on a longer prompt with a model question and answer. It would most likely repeat the model answer that you have provided.
