# Rasa WeatherBot

## Introduction

A simple Chinese weather robot (chatbot) built using Rasa technology stack (Rasa2.0, Rasa X, Slack) 

## Where to get help

There is extensive documentation:

- [blog](https://www.zhihu.com/column/ai-model)


#### README Contents:

- [Setup](#setup) 
- [License](#license)

## Setup


1. clone project and install requirements

```bash
git clone https://github.com/luojie1024/WeatherBot.git
cd WeatherBot
pip install -r requirements.txt
```


2. Train model by running:

   If you specify your project name in configure file, this will save your model at /models/your_project_name. 

   Otherwise, your model will be saved at /models/default

```
rasa train --num-threads 4
```
![-w1620](http://roger-markdown.oss-cn-beijing.aliyuncs.com/2020/12/26/16088726901168.jpg)

3. Run the raas action server:

```
rasa run actions
```
![-w1081](http://roger-markdown.oss-cn-beijing.aliyuncs.com/2020/12/26/16088733885511.jpg)


4. Open a new terminal and now you can curl results from the server, for example:

```
rasa x
```
![-w919](http://roger-markdown.oss-cn-beijing.aliyuncs.com/2020/12/26/16088779741294.jpg)


![-w833](http://roger-markdown.oss-cn-beijing.aliyuncs.com/2020/12/26/16088779893325.jpg)

5. Connecting a bot to Slack

- [doc](https://rasa.com/docs/rasa/connectors/slack )

![-w862](http://roger-markdown.oss-cn-beijing.aliyuncs.com/2020/12/26/16088911567571.jpg)

## License

Licensed under the Apache License, Version 2.0. Copyright 2020 Rasa Technologies GmbH. [Copy of the license](LICENSE.txt).


