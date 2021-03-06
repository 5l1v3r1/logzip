
# logzip

Logzip is an efficient compression tool specific for log files.  It compresses log files by utilizing the inherent structures of raw log messages, and thereby achieves a high compression ratio.  

The repository contains the source code of logzip. More details could be found in our ASE2019 paper:

**[ASE'19]** Jinyang Liu, Jieming Zhu, Shilin He, Pinjia He, Zibin Zheng, Michael R. Lyu. [Logzip: Extracting Hidden Structures via Iterative Clustering for Log Compression](https://arxiv.org/abs/1910.00409). *International Conference on Automated Software Engineering (ASE)*, 2019.

## Prerequisites 

- python3
- pandas

## Installation 

Logzip can be directly execute through source code. 

1. Download and install python3 [here](https://www.python.org/downloads/).

2. Install Pandas.

   ```$ pip3 install pandas```

3. Clone logzip.

   ``` $ clone https://github.com/logpai/logzip.git``` 

## Data

We've conducted comprehensive experiments to evaluate the efficiency of logzip on five real-world datasets. All the datasets that we use are available at [loghub](https://github.com/logpai/loghub).

## Usage

A demo is uploaded to this repo (logzip/demo). We use a HDFS log file with 2k lines as a demo.

For other kinds of logs, please specify templates (could be generated by a [log parser](https://github.com/logpai/logparser)) and log format accordingly.

#### Compression

```shell
$ cd logzip/demo/
$ python3 zip_demo.py
```
