
```python
>>> import requests
>>> url = 'https://api.github.com/search/repositories?q=language:python&sort=stars' # Initiate an API request.
>>> request = requests.get(url)
>>> print("Status code:", request.status_code)
Status code: 200
>>> respons_dict = request.json()  # In a variable, save the API response.
>>> print("Total repos:", respons_dict['total_count'])
Total repos: 7779969
>>> # Examine the repository's details.
>>> repos_dicts = respons_dict['items']
>>> print("Repos found:", len(repos_dicts))
Repos found: 30
>>> print("\nSelected info about each repository:")

Selected info about each repository:
>>> for repos_dict in repos_dicts:   #go through all the dictionaries in repos_dicts.
...     print('name-:', repos_dict['name'])  #write the name of the project
...     print('owner-:', repos_dict['owner']['login']) #show the owner of the project
...     print('stars-:', repos_dict['stargazers_count'])#print the number of stars the project has
...     print('repo-:', repos_dict['html_url'])  # print the link to the project's repository
...     print('Description-:', repos_dict['description']) # print the description of the project
...
...
name-: public-apis
owner-: public-apis
stars-: 160787
repo-: https://github.com/public-apis/public-apis
Description-: A collective list of free APIs
name-: Python
owner-: TheAlgorithms
stars-: 119015
repo-: https://github.com/TheAlgorithms/Python
Description-: All Algorithms implemented in Python
name-: Python-100-Days
owner-: jackfrued
stars-: 109116
repo-: https://github.com/jackfrued/Python-100-Days
Description-: Python - 100天从新手到大师
name-: awesome-python
owner-: vinta
stars-: 103089
repo-: https://github.com/vinta/awesome-python
Description-: A curated list of awesome Python frameworks, libraries, software and resources
name-: youtube-dl
owner-: ytdl-org
stars-: 100790
repo-: https://github.com/ytdl-org/youtube-dl
Description-: Command-line program to download videos from YouTube.com and other video sites
name-: models
owner-: tensorflow
stars-: 71468
repo-: https://github.com/tensorflow/models
Description-: Models and examples built with TensorFlow
name-: django
owner-: django
stars-: 59945
repo-: https://github.com/django/django
Description-: The Web framework for perfectionists with deadlines.
name-: flask
owner-: pallets
stars-: 56779
repo-: https://github.com/pallets/flask
Description-: The Python micro framework for building web applications.
name-: keras
owner-: keras-team
stars-: 52736
repo-: https://github.com/keras-team/keras
Description-: Deep Learning for humans
name-: transformers
owner-: huggingface
stars-: 52011
repo-: https://github.com/huggingface/transformers
Description-: 🤗 Transformers: State-of-the-art Natural Language Processing for Pytorch, TensorFlow, and JAX.
name-: awesome-machine-learning
owner-: josephmisiti
stars-: 51498
repo-: https://github.com/josephmisiti/awesome-machine-learning
Description-: A curated list of awesome Machine Learning frameworks, libraries and software.
name-: ansible
owner-: ansible
stars-: 49999
repo-: https://github.com/ansible/ansible
Description-: Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy and maintain. Automate everything from code deployment to network configuration to cloud management, in a language that approaches plain English, using SSH, with no agents to install on remote systems. https://docs.ansible.com.
name-: scikit-learn
owner-: scikit-learn
stars-: 47393
repo-: https://github.com/scikit-learn/scikit-learn
Description-: scikit-learn: machine learning in Python
name-: HelloGitHub
owner-: 521xueweihan
stars-: 47150
repo-: https://github.com/521xueweihan/HelloGitHub
Description-: :octocat: 分享 GitHub 上有趣、入门级的开源项目
name-: requests
owner-: psf
stars-: 46120
repo-: https://github.com/psf/requests
Description-: A simple, yet elegant HTTP library.
name-: scrapy
owner-: scrapy
stars-: 41714
repo-: https://github.com/scrapy/scrapy
Description-: Scrapy, a fast high-level web crawling & scraping framework for Python.
name-: big-list-of-naughty-strings
owner-: minimaxir
stars-: 41208
repo-: https://github.com/minimaxir/big-list-of-naughty-strings
Description-: The Big List of Naughty Strings is a list of strings which have a high probability of causing issues when used as user-input data.
name-: superset
owner-: apache
stars-: 40710
repo-: https://github.com/apache/superset
Description-: Apache Superset is a Data Visualization and Data Exploration Platform
name-: cpython
owner-: python
stars-: 40481
repo-: https://github.com/python/cpython
Description-: The Python programming language
name-: faceswap
owner-: deepfakes
stars-: 38544
repo-: https://github.com/deepfakes/faceswap
Description-: Deepfakes Software For All
name-: manim
owner-: 3b1b
stars-: 37571
repo-: https://github.com/3b1b/manim
Description-: Animation engine for explanatory math videos
name-: fastapi
owner-: tiangolo
stars-: 36312
repo-: https://github.com/tiangolo/fastapi
Description-: FastAPI framework, high performance, easy to learn, fast to code, ready for production
name-: interview_internal_reference
owner-: 0voice
stars-: 32481
repo-: https://github.com/0voice/interview_internal_reference
Description-: 2021年最新总结，阿里，腾讯，百度，美团，头条等技术面试题目，以及答案，专家出题人分析汇总。
name-: CppCoreGuidelines
owner-: isocpp
stars-: 31929
repo-: https://github.com/isocpp/CppCoreGuidelines
Description-: The C++ Core Guidelines are a set of tried-and-true guidelines, rules, and best practices about coding in C++
name-: AiLearning
owner-: apachecn
stars-: 31354
repo-: https://github.com/apachecn/AiLearning
Description-: AiLearning: 机器学习 - MachineLearning - ML、深度学习 - DeepLearning - DL、自然语言处理 NLP
name-: pandas
owner-: pandas-dev
stars-: 31195
repo-: https://github.com/pandas-dev/pandas
Description-: Flexible and powerful data analysis / manipulation library for Python, providing labeled data structures similar to R data.frame objects, statistical functions, and much more
name-: XX-Net
owner-: XX-net
stars-: 30852
repo-: https://github.com/XX-net/XX-Net
Description-: A proxy tool to bypass GFW.
name-: Real-Time-Voice-Cloning
owner-: CorentinJ
stars-: 30266
repo-: https://github.com/CorentinJ/Real-Time-Voice-Cloning
Description-: Clone a voice in 5 seconds to generate arbitrary speech in real-time
name-: rich
owner-: willmcgugan
stars-: 29601
repo-: https://github.com/willmcgugan/rich
Description-: Rich is a Python library for rich text and beautiful formatting in the terminal.
name-: python-patterns
owner-: faif
stars-: 29345
repo-: https://github.com/faif/python-patterns
Description-: A collection of design patterns/idioms in Python
>>>
```
