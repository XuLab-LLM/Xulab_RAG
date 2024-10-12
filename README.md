# Hands on XuLab_RAG
## 项目介绍🤗🤗🤗
RAG (Retrieval-Augmented Generation) 是一种结合检索与生成模型的技术，常用于问答系统、对话生成和知识增强等任务。它的主要思想是通过信息检索从知识库中获取相关文档，并将这些检索到的信息作为上下文，辅助生成模型 (通常是大型语言模型) 生成更加准确、相关的答案。本项目旨在开源一个完整的RAG系统，以帮助大家从底层上了解整个RAG构建的具体流程。在此基础上，我们将Agent也集成于我们所构建的RAG系统中，以增加用户对于外部工具调用的体验。详细的优化策略以及集成方法在以下小节会逐一介绍。
# 项目整体架构图
![image](https://github.com/jinguoweis/Xulab_RAG/blob/master/RAG.png)
# 项目结构
```plaintext
tinyRAG
├─ build.ipynb
├─ component
│  ├─ chain.py
│  ├─ databases.py
│  ├─ data_chunker.py
│  ├─ embedding.py
│  └─ llms.py
├─ data
│  ├─ dpcq.txt
│  ├─ README.md
│  └─ 中华人民共和国消费者权益保护法.pdf
├─ db
│  ├─ document.json
│  └─ vectors.json
├─ image
│  └─ 5386440326a2c9c5a06b5758484d375.png
├─ push.bat
├─ README.md
├─ requirements.txt
└─ webdemo_by_gradio.ipynb
```
# QuickStrat
安装依赖，需要 Python 3.10 以上版本。
```plaintext
pip install -r requirements.txt
