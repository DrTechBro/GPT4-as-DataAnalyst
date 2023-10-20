# GPT-4 as Data Analyst

This repo contains the data and code for our paper "[Is GPT-4 a Good Data Analyst?](https://arxiv.org/abs/2305.15038)".

### 1. Requirements
#### 1.1 OPENAI_API_KEY
Create an account and get the API key for OpenAI (https://openai.com).

```
OPENAI_API_KEY=YOUR_KEY
```
#### 1.2 SERPAPI_KEY
Create an account and get the API key for google retrieval (https://serpapi.com).

```
SERPAPI_KEY=YOUR_KEY
```

#### 1.3 Install requirements
```
pip install -r requirements.txt
```

#### 1.4 Download Databases
Download the sql databases from "[nvBench dataset](https://github.com/TsinghuaDatabaseGroup/nvBench)" to the current directory and name it as ```nvBench-main```.

### 2. Run the code
```
python main.py
```
### 3. Demo
We provide a demo and you can try it by running the following command:
```
cd demo/
python demo_main.py
```
You will first enter the OpenAI and SERPAPI keys according to the instructions:
```
* Please enter your OpenAI API key: 
* Please enter your Google API key:
```
Then you will be prompted to choose the sqlite file and sql schema:
```
* Please choose the database file to read: 
* Please choose the schema file to read:
```
You can select `demo/apartment_rentals.sqlite` and `demo/schema.sql`. Or you can play with your own data.

Next, you will be prompted to enter the question. Press enter to use the default question or enter your own question:
```
* Please enter your question (Press Enter to use the default question):
```
The pipeline starts to run now.

### 4. Data
Our data and experimental results will be released soon.

## Citation
If the code is used in your research, please star our repo and cite our paper as follows:
```
@inproceedings{cheng2023gptda,
  title={Is GPT-4 a Good Data Analyst?},
  author={Liying Cheng and Xingxuan Li and Lidong Bing},
  booktitle={Findings of EMNLP},
  url={"https://arxiv.org/abs/2305.15038"},
  year={2023}
}
```