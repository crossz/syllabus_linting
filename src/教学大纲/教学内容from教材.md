# 大模型应用开发

## 第一章 智能体(Agent)介绍

### 大开脑洞的演讲:Life 3.0

### 那么,究竟何谓 Agent

- 历史悠久的概念 p04
- 定义 p05

### Agent的大脑:大模型的通用推理能力

- 人类的大脑了不起
- 大模型出现之前的 Agent
- 大模型就是 Agent的大脑
- 期望顶峰和失望低谷
- 知识、记忆、理解、表达、推理、反思、泛化和自我提升
- 基于大模型的推理能力构筑 AI应用

### Agent的感知力:语言交互能力和多模态能力

- 语言交互能力
- 多模态能力
- 结合语言交互能力和多模态能力

### Agent的行动力:语言输出能力和工具使用能力

- 语言输出能力
- 工具使用能力
- 具身智能的实现

### Agent对各行业的效能提升

- 自动办公好助手
- 客户服务革命
- 个性化推荐
- 流程的自动化与资源的优化
- 医疗保健的变革

### Agent带来新的商业模式和变革

- Gartner的 8项重要预测
- Agent即服务
- 多 Agent协作
- 自我演进的 AI
- 具身智能的发展

### 解决大模型输出稳定性的方案

- Reasoning 推理模型，O1，R1
- prompt engineering
- RAG技术-知识库
- Agent
  - Agent - multiple agent framework
  - MCP

### 调用大模型的框架

- openAI API: openai()
- LangChain
- LlamaIndex
- MetaGPT
- AutoGen

## 第二章 OpenAI与其Assistant API介绍

### OpenAI公司的 Assistants是什么

### 不写代码,在 Playground中玩 Assistants

### OpenAI Assitant API

#### 2023年3月 Assistants API 正式推出

中国科技大厂 APP 涌现
2024年6月25日 OpenAI宣布终止中国API服务
2024年7月 "智能体"集中爆发

#### 2025年1月 OpenAI Operator 发布

### Assistants API的简单示例

- 创建助手
- 创建线程
- 添加消息
- 运行助手
- 显示响应

### 对4.3章节的调整

- 用 siliconflow 的聚合api
- 用 marscode.cn 来实现一个demo
以分组的形式完成

### 创建一个简短的虚构 PPT

- 数据的收集与整理
- 创建 OpenAI助手
- 自主创建数据分析图表
- 自主创建数据洞察
- 自主创建页面标题
- 用 DALL·E 3模型为 PPT首页配图
- 自主创建 PPT

### 对4.3章节的调整

- 第一次随堂测试任务一，自由发挥用已有大模型聊天模式智能体（2025.3）做一个ppt

## 第三章 主流智能体开发框架介绍：OpenAI API、LangChain和 LlamaIndex

重点：主流的 agent 开发框架介绍和各自定位

难点：LangChain 等框架生态和组成庞大、抽象概念多

### 何谓 OpenAI API

- 说说 OpenAI这家公司

  2015 年山姆奥特曼与 Google Brain 科学家伊利亚.苏茨克维吃晚饭；之后创建人工智能公司 OpenAI，投资方包括埃隆马斯克等 -- 对抗当时 AI 由大厂统治的局面。
  2018 年，埃隆马斯克离开董事会，投入到特斯拉的人工智能开发。
  2019 年，OpenAI 陷入财务和人才流失的危机；同年引入 OpenAI LP 盈利分支，微软 10 亿美元介入。
  2022.11.30 ChatGPT 发布
  
- OpenAI API和 Agent开发

  ChatGPT 和 DALL.E 是最出色的 Agent
  引发各行各业巨变，各行各业 AI 成熟度快速提升
  
- OpenAI API 示例
  - OpenAI API的聊天程序示例
  - OpenAI API的图片生成示例
  - OpenAI API实践

### 何谓 LangChain

- 说说 LangChain

  2022年10月 哈里森.蔡斯以开源项目启动
  维护 Python 和 Javascript 两种语言的库
  丰富的社区与生态，融入最完整的 LLM 支持
  
- LangChain中的六大模块
- LangChain SDK 示例
  - LangChain和 Agent开发
  - LangSmith的使用方法

### 何谓 LlamaIndex

- 说说 LlamaIndex

  2022年11月与 ChatGPT 同期发布
  Agent 开发能力，专注于 RAG 知识库体系
  
- LlamaIndex和基于 RAG的 AI开发
- 简单的 LlamaIndex开发示例

## 第四章 大模型智能体开发的推理引擎

### Agent的四大要素

### Agent的规划和决策能力

### Agent的各种记忆机制

### Agent的核心技能:调用工具

### 通用 Agent 认知框架

- 函数调用
- 计划与执行
- 自问自答
- 批判修正
- 思维链
- 思维树

### LLM api 几种写法

#### 1. http api （基础默认）

- 硅基流动

#### 2. OpenAI API

- OpenAI original
- 通义 Tongyi

#### 3. langchain

- ChatOpenAi() 兼容模式
  - 通义通过 ChatOpenAi()
- langchain_community.chat_models 第三方
  - 通义 Tongyi()
    - docs
      - [阿里云平台 docs](https://help.aliyun.com/zh/model-studio/developer-reference/use-bailian-in-langchain)
      - [langchain docs](https://python.langchain.com/docs/integrations/chat/tongyi/)

- 自定义 LLM class
  - 自定义 langchain 的 LLM Class

#### 4. LlamaIndex

#### *. 每个大模型自己的SDK

## 第五章 智能体的推理与行动的协同：React模式

推理与行动的协同--通过LangChain中的ReAct框架实现自动定价

### Agent的推理引擎:ReAct框架

- 何谓 ReAct
- 用 ReAct框架实现简单 Agent
- 基于 ReAct框架的提示
- 创建大模型实例
- 定义搜索工具
- 构建 ReAct Agent
- 执行 ReAct Agent

### LangChain中 ReAct Agent 的实现

### LangChain中的工具和工具包

### 通过 create_react_agent创建鲜花定价 Agent

### 深挖 AgentExecutor的运行机制

- 在 AgentExecutor中设置断点
- 第一轮思考:模型决定搜索
- 第一轮行动:工具执行搜索
- 第二轮思考:模型决定计算
- 第二轮行动:工具执行计算
- 第三轮思考:模型完成任务

## 第六章 智能体的更多实现形式

### Coze平台概览

- 平台起源与发展背景
- 核心定位与目标受众
- 平台架构与技术基础

### Coze平台核心功能

- 商店：应用与资源交易市场
  - 应用类型与分类
  - 交易机制与规则
- 模板：快速搭建解决方案
  - 常用模板类型
  - 模板自定义与扩展
- 插件：增强平台能力
  - 插件生态系统
  - 插件开发与集成流程

### Coze平台的优势与可替代性分析

- Coze平台的独特优势
  - 功能优势
  - 性能优势
  - 生态优势
- 与其他同类平台对比
  - 功能对比
  - 成本对比
  - 易用性对比
- 适用场景与局限性探讨
  - 推荐使用场景
  - 不适用场景分析

## 第七章 基于大模型的检索增强 RAG

知识的提取与整合--通过 LlamaIndex实现检索增强生成

### 何谓检索增强生成

- 提示工程、RAG与微调
- 从技术角度看检索部分的 Pipeline
- 从用户角度看 RAG流程

### LlamaIndex demo

#### uv 部署调试

#### marscode 替代方案

### RAG和 Agent

### 通过 LlamaIndex的 ReAct RAG Agent实现花语秘境财报检索

- 获取并加载电商的财报文件
- 将财报文件的数据转换为向量数据
- 构建查询引擎和工具
- 配置文本生成引擎大模型
- 创建 Agent以查询财务信息

### RAG 框架选择

如果你的项目需要由于复杂程序而进行广泛的定制，LangChain 是理想的选择。它的适应性和集成能力使得定制解决方案的开发成为可能。

如果你的应用程序需要处理大量文本数据，包括管理庞大的文本库或构建大型索引，LlamaIndex 特别有用。它的直观界面和高效索引使其非常适合这些任务。

如果你的主要目标是开发需要准确信息检索的搜索引擎或 QA 系统，Haystack 是最佳选择。它的适应性和搜索优化特性对这些应用大有裨益。

如果你的应用需要最先进的 NLP 模型，Hugging Face 是最佳选择。它的大型模型库和活跃的社区保证了你可以访问自然语言处理领域的最新进展。

## 第八章 多智能体开发框架的发展与应用 - AutoGen 和 MetaGPT

### 多智能体框架出现与发展 - 从单 Agent到多 Agent

### AutoGPT

- AutoGPT简介
- AutoGPT实战

### BabyAGI

- BabyAGI简介
- BabyAGI实战

### CAMEL

- CAMEL简介
- CAMEL论文中的股票交易场景
- CAMEL实战

### 主流多智能体开发框架

#### AutoGen

- AutoGen简介
- AutoGen实战
  - pyautogen, autogen 不是微软的MFA
  - [v0.4 版本后不再使用 llm_config，而是需要使用 model_client](https://microsoft.github.io/autogen/stable/user-guide/agentchat-user-guide/migration-guide.html)
  - [ip install -U "autogenstudio"
pip install -U "autogen-agentchat" "autogen-ext[openai]"](https://github.com/microsoft/autogen)

#### MetaGPT

- MetaGPT简介
- MetaGPT团队介绍
- MetaGPT实战
  - [为每个 role | action 配置 LLM](https://docs.deepwisdom.ai/main/zh/guide/tutorials/customize_llms_for_roles_or_actions.html)

## 期末总结与复习

### 综合实践标准智能体的实现方式

1. langchain 与 llamaindex 的整合开发
2. 通用 agent 与多智能体框架的整合与兼容性讨论

### 多智能体框架与智能体开发框架的整合

1. 随堂测验：metagpt vs autogen 对比实践
