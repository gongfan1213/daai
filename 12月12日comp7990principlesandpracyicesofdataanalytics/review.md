好的，针对这个考试内容，我们将逐个重点回顾，帮助您掌握其中的知识点。

### 1. 数据挖掘 (Data Mining) (~27%)

**重点内容**：
- **如何处理噪声数据**：
  - **Binning（分箱）**：
    - **Equal-width（等宽分段）**：将范围划分为 N 个相等的区间。
    - **Equal-depth（等深分段）**：将范围划分为 N 个区间，每个区间大致包含相同数量的样本。

- **归一化 (Normalization)**：
  - **Min-Max normalization**：将原始数据线性变换到指定范围内，例如 [0, 1]。
  - **Z-score normalization**：将原始数据下移均值、缩放到标准差为 1 的标准分布。

- **监督学习与无监督学习**：
  - **监督学习 (Supervised Learning)**：有标签的数据集，典型任务包括分类与回归。
  - **无监督学习 (Unsupervised Learning)**：无标签的数据集，主要用于聚类等任务。

- **常用算法**：
  - **线性模型 (Linear Model)**：包括一元线性回归与多元线性回归。
  - **感知机 (Perceptron)** 及其多层感知机 (Multi-Layer Perceptron)。
  - **支持向量机 (SVM)**：寻找最大间隔超平面。
  - **K近邻 (KNN)**：基于最近邻居进行分类。

### 2. 统计学 (Statistics) (~30%)

**重点内容**：
- **描述统计**：
  - **均值、众数、中位数**：数据的中心位置。
  - **标准差、范围、四分位数**：数据的离散程度。
  - **五数摘要**：最小值、第一四分位数、中位数、第三四分位数、最大值。

- **抽样**：
  - **随机抽样**的重要性，避免偏差，获取代表性样本。

- **信心区间 (Confidence Intervals)**：
  - 95%信心区间的计算，使用样本均值和标准误差。

- **假设检验 (Hypothesis Testing)**：
  - T检验的类型，包括单样本、独立样本和配对样本的 T 检验。
  - 单向 ANOVA F 检验，测试两个或多个总体均值是否相等。

### 3. 可视化 (Visualization) (~5%)

**重点内容**：
- **可视化设计原则**：
  - **选择合适的图表**：根据展示的内容来选择合适的图表类型（例如：条形图、折线图等）。
  - **颜色、文本、标题、标签的使用**。

- **Shneiderman's Mantra**：
  - **“Overview first, zoom and filter, then details-on-demand.”** 用户界面交互功能。

### 4. 安全与隐私 (Security and Privacy) (~8%)

**重点内容**：
- **公钥加密与私钥加密**：了解两者的区别及应用场景。
- **SQL 注入（SQL Injection）**：理解其逻辑及防护方法。
- **K-Anonymity**的基本概念：识别数据集的 K-匿名性。

### 5. 数据库 (Database) (~30%)

**重点内容**：
- **主键与外键**：理解它们如何在表中关联，提高数据一致性。
- **基本 SQL 操作**：
  - **查询 (SELECT)**：使用 `WHERE`、`ORDER BY` 进行筛选与排序。
  - **数据修改（INSERT、UPDATE、DELETE）**。

- **连接操作 (JOIN)**：
  - **内连接、左外连接、右外连接、全外连接**的区别和用法。

### 复习建议：

- **掌握公式**：熟悉公式表中的公式，做到心中有数。
- **注意步骤**：每个计算题的步骤都能获得分数，所以请详尽写出过程。
- **多做练习**：回顾课程中的小测和练习题，巩固知识。

### 额外准备：

- **确保计算器符合要求**：使用允许的计算器，并熟悉其运算功能。
- **保持良好的心理状态**：考前保持良好的休息和饮食，确保考试时脑力充沛。

如果有具体的知识点需要进一步解释或者有疑问，请告诉我！
好的，我们从统计学第一个重点开始复习：**描述统计**。

### 描述统计（Descriptive Statistics）

描述统计主要用于总结和描述数据的主要特征。通常包括以下几个方面：

#### 1. 中心趋势（Measures of Central Tendency）

- **均值（Mean）**：
  - 定义：数据的算术平均值。
  - 计算公式：
    \[
    \text{mean} = \frac{\sum x_i}{n}
    \]
    其中 \( x_i \) 是数据集中每个数值，\( n \) 是数据点的总数。

- **中位数（Median）**：
  - 定义：将数据按升序排列后，处于中间位置的数值。如果数据点的数量为偶数，则中位数是中间两个数的平均值。
  - 如何找到中位数：
    - 对数据进行排序。
    - 若 \( n \) 是奇数，中位数为第 \( \frac{n+1}{2} \) 个数；若 \( n \) 是偶数，中位数为第 \( \frac{n}{2} \) 和第 \( \frac{n}{2} + 1 \) 个数的平均值。

- **众数（Mode）**：
  - 定义：数据集中出现频率最高的数值。一个数据集可以有一个众数（单众数），多个众数（多众数）或者没有众数（无众数）。

#### 2. 离散程度（Measures of Spread）

- **范围（Range）**：
  - 定义：数据集中的最大值与最小值之差。
  - 计算公式：
    \[
       \text{range} = \text{max} - \text{min}
    \]

- **四分位数（Quartiles）**：
  - 将数据集分成四个部分的数值：
    - **Q1**：第一个四分位数，表示的数据为25%以下的数据。
    - **Q2（即中位数）**：中间的值。
    - **Q3**：第三个四分位数，表示的数据为75%以下的数据。
  - **四分位间距（Interquartile Range, IQR）**：
    - 定义：Q3 和 Q1 的差值，表示中间50%数据的变异程度。
    - 计算公式：
      \[
      \text{IQR} = Q3 - Q1
      \]

- **标准差（Standard De Deviation）**：
  - 定义：描述数据点相对于均值的散布程度。
  - 计算方法：
    - 对于样本：
      \[
      s = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n-1}}
      \]
    - 对于总体：
      \[
      \sigma = \sqrt{\frac{\sum (x_i - \mu)^2}{N}}
      \]
      其中 \( \bar{x} \) 是样本均值， \( \mu \) 是总体均值， \( n \) 是样本大小， \( N \) 是总体大小。

#### 3. 数据形态（Shape of the Distribution）

- **对称性（Symmetry）**：数据分布是否对称，均值和中位数相等。
- **偏态（Skewness）**：
  - 左偏（负偏）：大量数据集中在右侧，均值小于中位数。
  - 右偏（正偏）：大量数据集中在左侧，均值大于中位数。

- **峰态（Kurtosis）**：描述数据分布的峰高和尖锐程度。常见的有：
  - 正态分布：标准的峰态。
  - 高峰态（Leptokurtic）：峰高于正态分布。
  - 低峰态（Platykurtic）：峰低于正态分布。

### 小结

描述统计为我们提供了一种量化和总结数据的方式，可以帮助我们理解数据集的中心趋势、离散程度和形态。通过这些统计量，我们能够在各种数据中发现模式、得出结论。

如果您对某个具体的概念或计算方法有疑问，或者希望进行练习，请告诉我！
Here is a review of the data security and privacy portion of the COMP7990 course material:

Data Security:
- Understanding the CIA triad - confidentiality, integrity and availability as core pillars of data security
- Confidentiality through encryption - symmetric key (same key for encryption/decryption) vs asymmetric/public key encryption (different keys)
- Integrity through digital signatures - only the keyholder can produce a valid signature verifiable by anyone
- Availability through firewalls, intrusion detection systems to allow/deny traffic based on rules
- Case study on SQL injection attacks by embedding malicious SQL in input data, and how to prevent it through proper input sanitization

Data Privacy:
- Understanding different data sensitivities - explicit identifiers, quasi-identifiers, sensitive data, non-sensitive data
- Legal and regulatory requirements around data privacy (e.g. EU GDPR)
- Privacy concerns at different stages of the data mining process:
  - Data collection: Allowing data providers to control sensitivity of shared data
  - Data publishing: Anonymizing data (e.g. k-anonymity) to prevent re-identification while preserving utility  
  - Data analysis: Privacy-preserving analysis techniques like secure multi-party computation
  - Data provenance: Enabling credibility assessment of analysis results

- Techniques for indirect questioning in surveys to improve response rates on sensitive topics
  - Unmatched count technique (UCT)
  - Network scale-up technique (NST)  
  - Non-randomized response technique (NRRT)
  - Randomized response technique (RRT)

The key points are understanding core security principles like encryption and authentication, data anonymization approaches, privacy-preserving analysis, and techniques to gather sensitive data while protecting privacy. Let me know if you need any part explained in more detail.
以下是数据安全和隐私部分的中文复习内容:

数据安全:
- 理解CIA三元组-保密性、完整性和可用性是数据安全的三大核心支柱
- 保密性通过加密实现-对称密钥(加密解密使用同一密钥)vs非对称/公钥加密(加密解密使用不同密钥)
- 完整性通过数字签名实现-只有密钥持有者能产生可被任何人验证的有效签名
- 可用性通过防火墙、入侵检测系统基于规则允许/拒绝流量实现
- SQL注入攻击案例研究-通过在输入数据中嵌入恶意SQL代码进行攻击,以及通过正确的输入sanitization来预防

数据隐私:
- 理解不同的数据敏感度-显式标识符、准标识符、敏感数据、非敏感数据
- 数据隐私的法律法规要求(如欧盟GDPR)
- 数据挖掘过程中不同阶段的隐私考虑:
  - 数据收集:允许数据提供者控制共享数据的敏感度
  - 数据发布:匿名化数据(如k-anonymity)以防止重新识别,同时保留数据效用
  - 数据分析:隐私保护分析技术,如安全多方计算
  - 数据出处:启用对分析结果可信度的评估

- 改善敏感话题调查回答率的间接询问技术
  - 无匹配计数技术(UCT)
  - 网络规模扩展技术(NST)
  - 非随机响应技术(NRRT)
  - 随机响应技术(RRT)

关键点是理解诸如加密和身份验证之类的核心安全原则、数据匿名化方法、隐私保护分析以及在保护隐私的同时收集敏感数据的技术。如果需要对任何部分进一步解释,请告诉我。
好的,让我们从第一部分"数据安全"开始详细复习讲解:

数据安全
- CIA三元组是数据安全的三大核心支柱:

1) 保密性(Confidentiality)
保密性是确保只有预期的个人或实体能够访问数据。主要通过以下方式实现:
- 加密 - 将明文转换为密文,需要使用密钥。
- 加密分为对称加密和非对称(公钥)加密两种:
  对称加密 - 加密和解密使用同一密钥,这个密钥需要在发送方和接收方间安全共享。密钥长度越长(如256位),安全性越高,但加解密计算开销也越大。
  非对称(公钥)加密 - 加密和解密使用不同的密钥,分为公钥(公开的,用于加密)和私钥(保密的,用于解密)。任何人都可以用公钥加密,但只有私钥持有者才能解密。

- 身份认证 - 确认访问数据者的身份,常用方式包括密码、生物识别(指纹/面部)、设备认证(手机令牌)等。

2) 完整性(Integrity)  
完整性是确保数据在传输和存储期间保持完整,未被修改、插入或删除。主要通过:
- 数字签名 - 只有密钥持有者才能对数据产生有效的签名,任何人均可验证签名的合法性和完整性。
- 区块链 - 去中心化的账本,多节点共享相同的交易记录,一个节点数据被篡改就会与其它节点不一致而被发现。

3) 可用性(Availability)
可用性是确保数据和服务一直可用。主要通过:
- 防火墙 - 根据预定义的规则允许或拒绝进出网络的流量
- 入侵检测系统(IDS) - 监听网络流量,发现任何攻击模式

接下来我会介绍一个关于数据安全的案例研究 - SQL注入攻击及其防范措施。你有任何问题吗?
好的,我会同时给出中英文内容。

Data Security (数据安全)

The CIA triad forms the core principles of data security:

CIA三元组构成了数据安全的核心原则:

1) Confidentiality (保密性)
Ensuring only intended parties can access the data. Achieved through:
- Encryption - transforming plaintext to ciphertext using keys
   - Symmetric encryption: Same key for encryption/decryption 
   - Asymmetric (public key) encryption: Different keys for encryption (public key) and decryption (private key)

- Authentication - Verifying the identity of entity accessing data, e.g. passwords, biometrics, device tokens

确保只有预期的个人或实体能够访问数据。主要通过以下方式实现:
- 加密 - 使用密钥将明文转换为密文
   - 对称加密 - 加密和解密使用同一密钥
   - 非对称(公钥)加密 - 加密和解密使用不同的密钥(公钥和私钥)  
- 身份认证 - 验证访问数据者的身份,如密码、生物识别、设备令牌等

2) Integrity (完整性)
Ensuring data remains unmodified during transmission/storage. Achieved through:
- Digital signatures - Only keyholder can produce valid signature, verifiable by anyone
- Blockchain - Decentralized ledger, inconsistent data detected across nodes

确保数据在传输和存储期间保持完整,未被修改。主要通过:
- 数字签名 - 只有密钥持有者才能生成有效签名,任何人均可验证
- 区块链 - 去中心化账本,不一致数据会被多节点发现

3) Availability (可用性)  
Ensuring data/services are accessible. Achieved through:
- Firewalls - Allow/deny traffic based on predefined rules
- Intrusion Detection Systems (IDS) - Detect attack patterns in network traffic

确保数据和服务可用。主要通过:
- 防火墙 - 根据预定规则允许或拒绝流量 
- 入侵检测系统(IDS) - 在网络流量中检测攻击模式

A case study on data security issues - SQL Injection attacks and prevention:

一个数据安全问题的案例研究 - SQL注入攻击及其防范:
好的,我会继续同时给出中文和英文内容:

SQL Injection Attacks (SQL注入攻击)

SQL injection is a code injection technique used to attack data-driven applications, in which malicious SQL statements are inserted into application entry fields.

SQL注入是一种代码注入技术,用于攻击数据驱动的应用程序,其中恶意的SQL语句被插入到应用程序的输入字段中。

Example 1:

例1:

Suppose an application uses the following query for authentication:
假设一个应用程序使用以下查询进行身份验证:

String query = "SELECT * FROM users WHERE username = '" + userName + "' AND password = '" + password + "'";

If the user enters:
如果用户输入:
userName = ' or '1'='1  
password = ' or '1'='1

The query becomes:
那么查询就变成了:

SELECT * FROM users WHERE username = '' or '1'='1' AND password = '' or '1'='1'

This will return all records from the users table, causing a complete breach.

这将返回users表中的所有记录,导致完全泄露。

Prevention:
预防措施:

1) Use prepared statements which separate code and data
1) 使用预编译语句将代码与数据分离

2) Input validation and sanitization 
2) 输入验证和sanitization

3) Least privilege 
3) 最小特权原则

4) Intrusion Detection Systems to detect malicious patterns
4) 使用入侵检测系统发现恶意模式

Moving on to data privacy concerns...

接下来讲解数据隐私的相关内容...
好的,我将详细解释并翻译以下内容:

Data Privacy (数据隐私)

Data privacy deals with the proper collection, storage, usage and sharing of personal/sensitive data pertaining to individuals.

数据隐私关注个人/敏感数据的适当收集、存储、使用和共享。

Key aspects:

主要方面:

1) Understanding data sensitivities (理解数据敏感度)

- Explicit Identifiers (EI) - Direct personal identifiers like name, ID number 
  显式标识符(EI) - 如姓名、身份证号等直接个人标识

- Quasi-Identifiers (QI) - Indirect identifiers like gender, age, zip code that can re-identify when combined
  准标识符(QI) - 如性别、年龄、邮编等间接标识,结合使用可重新识别身份

- Sensitive Data (SD) - Confidential information like disease, salary
  敏感数据(SD) - 如疾病、薪资等机密信息  

- Non-Sensitive Data (NSD)
  非敏感数据(NSD)

2) Legal & Regulatory Requirements (法律法规要求)

- E.g. European GDPR, US HIPAA rules on data protection
  如欧盟GDPR、美国HIPAA有关数据保护的法规

3) Privacy at different data mining stages (数据挖掘不同阶段的隐私)

- Data Collection: Allowing providers to control sensitivity
  数据收集: 允许提供者控制数据敏感度

- Data Publishing: Anonymizing data while preserving utility (e.g. k-anonymity) 
  数据发布: 匿名化数据同时保留效用(如k-anonymity)

- Data Analysis: Privacy-preserving techniques like secure multi-party computation
  数据分析: 隐私保护技术如安全多方计算

- Data Provenance: Enabling credibility assessment of results
  数据出处: 允许对结果可信度进行评估

4) Indirect Questioning Techniques (间接询问技术)

Used in surveys to improve response rates on sensitive topics:
在敏感话题调查中改善回答率的技术:

- Unmatched Count Technique (UCT)
  无匹配计数技术(UCT)

- Network Scale-up Technique (NST)
  网络规模扩展技术(NST)

- Non-randomized Response Technique (NRRT) 
  非随机响应技术(NRRT)

- Randomized Response Technique (RRT)
  随机响应技术(RRT)

The key is balancing privacy protection with preserving data utility across the data mining pipeline.

关键是在整个数据挖掘流程中平衡隐私保护和保留数据效用。
好的,我将继续详细讲解并翻译下一部分复习重点:

k-anonymity (k匿名性)

k-anonymity is a technique used to anonymize quasi-identifiers in a dataset, such that each record is indistinguishable from at least k-1 other records along the quasi-identifier attributes.

k匿名性是一种技术,用于匿名化数据集中的准标识符,使得每条记录在准标识符属性上至少与其他k-1条记录无法区分。

Example:
例子:

Original Dataset (原始数据集):

EmpID(员工号) | Name(姓名) | Gender(性别) | DoB(出生日期) | Address(地址) | ...
-----------|------------|-------------|--------------|--------------|--------------
000101      | Alex       | M            | 1973-07-15   | Shatin        | ...
000102      | Bob        | M            | 1975-11-20   | Tuen Mun      | ...

Here Name is the explicit identifier, while Gender, DoB, Address form quasi-identifiers that can potentially re-identify individuals.

这里姓名是显式标识符,而性别、出生日期和地址构成了潜在可重新识别个人的准标识符。

To achieve 2-anonymity, we generalize the quasi-identifiers:
为实现2匿名,我们对准标识符进行泛化:

2-anonymous (2匿名):

EmpID | Gender | DoB       | Address | ...
-------|--------|-----------|---------|----
000107 | F      | 1980-1990 | *       | ...  
000110 | F      | 1980-1990 | *       | ... 
000105 | M      | 1980-1990 | *       | ...
000106 | M      | 1980-1990 | *       | ...

Now each record is indistinguishable from at least 1 other record. Higher k provides stronger anonymity.

现在每条记录至少与另一条记录无法区分,k值越高则匿名性越强。

But increasing k reduces data granularity/utility. Key principle is balancing privacy vs utility tradeoff.

但提高k会降低数据细粒度/效用。关键是权衡隐私与效用之间的平衡。
在匿名化过程中,对准标识符进行泛化主要采用以下两种方式:

1. 值泛化(Value Generalization)
将准标识符的具体值替换为更加笼统的值。例如:

原始值:
性别: M, F
出生日期: 1973-07-15, 1975-11-20

泛化后:  
性别: 被替换为 "M"、"F" 
出生日期: 被替换为更宽泛的范围,如 "1970-1980"

2. 分区泛化(Partition Generalization)
将准标识符值划分为多个非重叠的范围区间。例如:

原始值:
年龄: 25, 32, 40, 52

泛化后:
年龄: 被划分为 "<30"、"30-40"、"40-50"、">=50"

通过值泛化和分区泛化,可以减小准标识符的区分能力,从而实现匿名化的效果。

除此之外,匿名化过程中还可以采取以下策略:

1. 抑制(Suppression)
将某些较为敏感或稀有的准标识符值直接替换为特殊符号(如"*"),表示该值被隐藏。

2. 解构(Anatomization) 
将原始数据集分解为两个单独的数据集,一个只包含准标识符,另一个只包含敏感属性,并通过某种连接方式连接两者。

3. 扰动(Perturbation)
在原始数据的基础上施加一些合理的统计噪声,使数据产生一定程度的扭曲,从而掩盖一些信息。

这些策略的使用需要根据具体数据集和隐私要求进行权衡,以达到较好的匿名效果和数据效用之间的平衡。
