# Security Concepts
CIA Traid are three main goals
# 安全概念
CIA Traid 有三大目标

## Confidentiality
- Confidentiality protects information from unauthorized disclosure.
### 保密
- 机密性保护信息不被擅自披露。
  
#### Confidentiality_Concerns
#### 保密问题
1. Snooping
	- snooping gathering information that is left out in the open.
	- "Clean desk policies" protect against snooping.
1. 窥探
	- 窥探收集公开的信息。
	- 清洁办公桌政策 "可防止窥探。

2. Dumpster Diving
	- Dumpster diving is to dump data anywere or dustbin.
	- "Shedding" protects against dumpster diving.
2. 垃圾箱潜水
	- 垃圾箱跳水是指在任何地方或垃圾箱中倾倒数据。
	- "舍弃 "可以防止垃圾箱跳水。

3. Eavesdropping
	- listing sensitive information
	- "Rules about sensitive conversations" prevent eavesdropping
3. 窃听
	- 列出敏感信息
	- 敏感对话规则 "防止窃听

4. Wiretapping
	- Electronic evaesdropping - listing through wire(internet)
	- "Encryption" protects against Wiretapping
4. 窃听
	- 电子窃听--通过电线（互联网）列名
	- 加密 "可防止窃听

5. Social Engineering
	- The attacker uses psychological tricks to persuade an employee to give then sensitive information or access to internal systems.
	- Best defence is to "Educating users"
5. 社会工程学
	- 攻击者利用心理伎俩说服员工提供敏感信息或访问内部系统。
	- 最佳防御方法是 "教育用户"。

## Integrity
- Integrity protects information from unauthorized changes.
## 完整性
- 完整性可保护信息免遭未经授权的更改。
  
#### Integrity_Concerns
#### 誠信_關注

1. Unauthorized modification
	- Attacks make changes without permission.
	- "Least priviege" protects against integrity attacks
1. 未经授权的修改
	- 未经许可进行修改的攻击。
	- 最小隐私 "可防止完整性攻击

2. Impersonation
	- Attacks pretend to be someone else
	- "User education" protects against attacks
2. 冒充
	- 冒充他人进行攻击
	- 用户教育 "可防范攻击

3. Man-in-the-middle (MITM)
	- Attacks place the attacker in the middle of a communications session.
	- "Encryption" protects against MITM attacks
3. 中间人（MITM）
	- 将攻击者置于通信会话中间的攻击。
	- 加密 "可防止 MITM 攻击

4. Replay
	- Attacks eavesdrop on logins and reuse the captured credentials.
	- "Encryption" protects against Replay attacks
4. 重放
	- 窃听登录并重复使用捕获的凭据的攻击。
	- 加密 "可防止重放攻击

## Availability
- Availability protects authorized access to systems and data.
## 可用性
- 可用性可保护对系统和数据的授权访问。
  
#### Availability_Concerns
#### 可用性_問題
1. Denial of service (DoS)
	- Unlimited request to a server
	- "Block unauthorized connections" to protect against denial of service attacks.
1. 拒绝服务（DoS）
	- 向服务器发出无限请求
	- 阻止未经授权的连接 "可防止拒绝服务攻击。

2. Power outages
	- Naturally or Man-made
	- "Redundant power and generators" protect against power outages.
2. 停电
	- 自然或人为
	- 冗余电源和发电机 "可防止停电。

3. Hardware failures
	- any component failures
	- "Redundant components" protect against hardware failure
3. 硬件故障
	- 任何组件故障
	- 冗余组件 "可防止硬件故障

4. Destruction
	- Naturally or Man-made
	- "Backup data centers" protect against destruction.
4. 破坏
	- 自然或人为
	- 备份数据中心 "可防止破坏。

5. Service outages
	- Programing error and the failure of underlying equipment.
	- building systems that are resilient in the face of errors and hardware failures.
5. 服务中断
	- 程序错误和基础设备故障。
	- 建立面对错误和硬件故障有弹性的系统。

## Authentication and authorization
The access control process consists of three steps that you must understand. These steps are identification, authentication and authorization.
## 验证和授权
访问控制过程包括三个步骤，你必须了解。这三个步骤是识别、认证和授权。

1. Identification incolves making a claim of identity.
	- Electronic identification commonly uses usernames
1. 身份识别就是声称自己的身份。
	- 电子身份识别通常使用用户名

2. Authentication requires proving a claim of identity.
	- Electronic autherntication commonly uses passwords.
2. 认证需要证明身份。
	- 电子认证通常使用密码。

3. Authorization ensures that an action is allowed.
	- Electronic authorization commonly uses access control lists.
3. 授权确保行动被允许。
	- 电子授权通常使用访问控制列表。

Authentication and authorization process, access control systems also provide "Accounting" functionality that allows administrators to track user activity and reconstruct that activity from logs. This may include tracking user activity on systems and even logging user web browsing history.
在身份验证和授权过程中，访问控制系统还提供 "会计 "功能，允许管理员跟踪用户活动，并从日志中重建这些活动。这可能包括跟踪用户在系统上的活动，甚至记录用户的网络浏览历史。

## Password security
Password mechanisms
	- Password length requirements set a minimum number of characters. 
	- Password complexity requirements describe the types of characters that must be included.
	- Password expiration requirements force password changes.
	- Password requirements prevent password reuse.
## 密码安全
密码机制
	- 密码长度要求规定了最少字符数。
	- 密码复杂性要求描述了必须包含的字符类型。
	- 密码过期要求强制更改密码。
	- 密码要求防止密码重复使用。

## Multifactor authentication
Multifactor authentication combines two different authentication factors.
### 多因素身份验证
多因素身份验证结合了两种不同的身份验证因素。

Three different authentication factors. Something you know, something you are and something you have.
三种不同的认证因素。你知道的、你是的和你拥有的。

#### something you know
- Passwords, PIN's, Security questions.
#### 你知道的东西
- 密码、PIN 码、安全问题。
  
#### something you are
- Biometric security mechanisms.
#### 你是什么
- 生物识别安全机制。

#### something you have
- Software and hardware tokens.
#### 您拥有的东西
- 软件和硬件令牌。

#### single sign-On (SSO)
Shares authentiacated sessions across systems
	- In a single sign on approach, users log on to the first SSO enabled system that they encounter. And then that login session persists across other systems until it expires. If the organization sets the expiration period to be the length of a business day, that means that users will only need to log in once a day and their single sign on is then going to last the entire day.
#### 单点登录（SSO）
跨系统共享授权会话
	- 在单点登录方法中，用户登录到他们遇到的第一个启用 SSO 的系统。然后，登录会话在其他系统中持续存在，直到过期。如果企业将过期时间设定为一个工作日的长度，这意味着用户每天只需登录一次，他们的单点登录会持续一整天。

## Non-repudiation
Non-repudiation prevents someone from denying the truth.
## 不否认
不否认可以防止某人否认事实。

Solved the issue with
	1. Signed contracts
	2. Digital signatures
	3. Video surveillance
通过以下方法解决了问题
	1. 已签署的合同
	2. 数字签名
	3. 视频监控

## Privacy
Privacy Concerns
1. Protecting our own data.
2. Educating our users.
3. Protecing data collected by our organizations.
## 隐私
隐私问题
1. 保护我们自己的数据
2. 教育我们的用户
3. 保护我们组织收集的数据。

Private information may come in many forms. Two of the most common elements of private information are "Personally identifiable information" and "Protected health information".
1. Personally identifiable information, or PII, includes all information that can be tied back to a specific individual. 
2. Protected health information, or PHI, includes healthcare records that are regulated under the Health Insurance Portability and Accountability Act. Otherwise known as HIPAA.

私人信息有多种形式。最常见的两种私人信息是 "个人身份信息 "和 "受保护的健康信息"。
1. 个人身份信息，或称 PII，包括所有可追溯到特定个人的信息。
2. 受保护的健康信息（PHI）包括受《健康保险可携性和责任法案》（Health Insurance Portability and Accountability Act）监管的医疗记录。又称 HIPAA。
