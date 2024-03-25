# L3 Access Control Concepts
# L3 存取控制概念
## Introduction
＃＃ 介紹
Types of access control, physical and logical controls and how they are combined to strengthen the overall security of an organization.
存取控制、實體和邏輯控制的類型以及如何將它們組合起來以增強組織的整體安全性。
## Module 1 Understand Access Control Concepts
## 模組 1 了解存取控制概念
Domain D3.1, D3.1.3, D3.1.5, D3.2, D3.2.1, D3.2.2, D3.2.5

### What is Security Control?
### 什麼是安全控制？
Access control involves **limiting what objects can be available to what subjects according to what rules**.
存取控制涉及**根據什麼規則限制哪些物件可以供哪些主體使用**。
### Controls Overview
### 控制概述
Earlier in this course we looked at security principles through foundations of risk management, governance, incident response, business continuity and disaster recovery. But in the end, security all comes down to, **“who can get access to organizational assets (buildings, data, systems, etc.) and what can they do when they get access?”**
在本課程的前面部分，我們透過風險管理、治理、事件應變、業務連續性和災難復原的基礎來了解安全原則。 但最終，安全性歸結為，**「誰可以訪問組織資產（建築物、數據、系統等）以及他們獲得訪問權限後可以做什麼？」**

Access controls **are not just about restricting access** to information systems and data, **but also about allowing access**. It is about granting the appropriate level of access to authorized personnel and processes and denying access to unauthorized functions or individuals.
访问控制***不仅仅是限制***对信息系统和数据的访问，也***是允许***访问。它是指对授权人员和程序授予适当级别的访问权限，并拒绝未经授权的功能或个人访问。

Access is based on three elements:
訪問基於三個要素：

* subjects: **any entity that requests access to our assets**. The entity requesting access may be a **user**, a **client**, a **process** or a **program**, for example. A subject is the initiator of a request for service; therefore, a subject is referred to as “active.” A subject:
    * Is a user, a process, a procedure, a client (or a server), a program, a device such as an endpoint, workstation, smartphone or removable storage device with onboard firmware.
    * Is active: It initiates a request for access to resources or services.
    * Requests a service from an object.
    * Should have a level of clearance (permissions) that relates to its ability to successfully access services or resources.
* 主体： **请求访问我们资产的任何实体**。例如，请求访问的实体可以是**用户**、**客户**、**进程**或**程序**。主体是服务请求的发起者；因此，主体被称为 "主动"。主体：
    * 是用户、进程、程序、客户端（或服务器）、程序、设备（如终端、工作站、智能手机或带有板载固件的移动存储设备）。
    * 处于活动状态： 发起访问资源或服务的请求。
    * 请求对象提供服务。
    * 应具有与其成功访问服务或资源的能力相关的许可级别（权限）。

* **Objects:** Objects represent the assets or resources that subjects seek to access within an organization. These assets can take various forms, including data stored in databases or files, systems such as servers or network devices, applications used for specific purposes, physical spaces like offices or storage rooms, or any other resource that holds value to the organization. Objects serve as the targets of access requests initiated by subjects, and their protection is essential for maintaining the security and integrity of the organization's assets.
** 对象：** 对象代表主体在组织内试图访问的资产或资源。这些资产的形式多种多样，包括存储在数据库或文件中的数据、服务器或网络设备等系统、用于特定目的的应用程序、办公室或储藏室等物理空间，或对组织有价值的任何其他资源。对象是主体发起的访问请求的目标，保护对象对于维护组织资产的安全性和完整性至关重要。

* **Rules:** Rules form the foundation of the access control framework by defining the conditions under which access is granted or denied to objects. These rules establish the criteria and parameters that govern the access permissions and restrictions within the organization's environment. They can encompass a wide range of factors, including user roles and responsibilities, permissions levels, time-based access policies, location-based restrictions, and other attributes relevant to the organization's security policies. Rules ensure that access is managed in a consistent, predictable, and enforceable manner, helping to safeguard sensitive information, prevent unauthorized access, and mitigate security risks effectively.
** 规则：** 规则是访问控制框架的基础，它定义了允许或拒绝对象访问的条件。这些规则确立了管理组织环境中访问权限和限制的标准和参数。这些规则可涵盖多种因素，包括用户角色和职责、权限级别、基于时间的访问策略、基于位置的限制以及与组织安全策略相关的其他属性。规则可确保以一致、可预测和可执行的方式管理访问，帮助保护敏感信息，防止未经授权的访问，并有效降低安全风险。

### Controls Assessments
### 控制評估
Risk reduction depends on the effectiveness of the control. It must apply to the current situation and adapt to a changing environment. 
風險降低取決於控制的有效性。 它必須適用於當前情況並適應不斷變化的環境。

### Defense in Depth
### 縱深防禦
We are looking at all access permissions including building access, access to server rooms, access to networks and applications and utilities. These are all implementations of access control and are part of **a layered defense strategy**, **also known as defense in depth**, developed by an organization.
我们正在研究所有的访问权限，包括楼宇访问、服务器机房访问、网络访问以及应用程序和公用设施访问。这些都是访问控制的实施，也是企业制定的**分层防御战略**（又称纵深防御**）的一部分。

**Defense in depth describes an information security strategy that integrates people, technology and operations capabilities to establish variable barriers across multiple layers and missions of the organization.** It applies multiple countermeasures in a layered fashion to fulfill security objectives. Defense in depth should be implemented to prevent or deter a cyberattack, but it cannot guarantee that an attack will not occur. 
**纵深防御描述了一种信息安全战略，它整合了人员、技术和操作能力，在组织的多个层面和任务中建立可变屏障。实施纵深防御可预防或阻止网络攻击，但不能保证攻击不会发生。

A technical example of defense in depth, in which multiple layers of technical controls are implemented, **is when a username and password are required for logging in to your account, followed by a code sent to your phone to verify your identity**. **This is a form of multi-factor authentication using methods on two layers, something you have and something you know.** The combination of the two layers is much more difficult for an adversary to obtain than either of the authentication codes individually. 
实施多层技术控制的深度防御的一个技术范例是**登录账户时需要用户名和密码，然后向手机发送验证码以验证身份**。**这是一种多因素身份验证，使用了两层方法，即你拥有的东西和你知道的东西**。

Another example of multiple technical layers is when additional firewalls are used to separate untrusted networks with differing security requirements, such as the internet from trusted networks that house servers with sensitive data in the organization. When a company has information at multiple sensitivity levels, it might require the network traffic to be validated by rules on more than one firewall, with the most sensitive information being stored behind multiple firewalls.
多技术层的另一个例子是使用额外的防火墙来分隔具有不同安全要求的不信任网络，如互联网和存放企业敏感数据服务器的可信网络。当公司拥有多个敏感级别的信息时，可能会要求网络流量通过不止一个防火墙上的规则进行验证，并将最敏感的信息存储在多个防火墙后面。

For a non-technical example, consider the multiple layers of access required to get to the actual data in a data center. First, a lock on the door provides a physical barrier to access the data storage devices. Second, a technical access rule prevents access to the data via the network. Finally, a policy, or administrative control defines the rules that assign access to authorized individuals.
举一个非技术性的例子，考虑一下访问数据中心实际数据所需的多层访问权限。首先，门锁提供了访问数据存储设备的物理屏障。其次，技术访问规则防止通过网络访问数据。最后，政策或管理控制定义了将访问权限分配给授权个人的规则。

### Principle of Least Privilege
### 最小特權原則
The Principle of Least Privilege (NIST SP 800-179) is a standard of permitting only minimum access necessary for users or programs to fulfill their function. Users are provided access only to the systems and programs they need to perform their specific job or tasks. 
最小权限原则（NIST SP 800-179）是一项标准，即只允许用户或程序执行其功能所需的最低访问权限。用户只能访问其执行特定工作或任务所需的系统和程序。

To preserve the confidentiality of information and ensure that it is only available to personnel who are authorized to see it, **we use privileged access management**, **which is based on the principle of least privilege**. **That means each user is granted access only to the items they need and nothing further**.  
为了维护信息的机密性，并确保只有获得授权的人员才能看到这些信息，**我们采用特权访问管理**，**该管理基于最小特权原则**。**这意味着每个用户只能访问他们需要的项目，而不能访问更多**。

For example, only individuals working in billing will be allowed to view consumer financial data, and even fewer individuals will have the authority to change or delete that data. This maintains confidentiality and integrity while also allowing availability by providing administrative access with an appropriate password or sign-on that proves the user has the appropriate permissions to access that data.  
例如，只有从事计费工作的人员才有权查看消费者财务数据，而有权更改或删除该数据的人员则更少。这样既能保持保密性和完整性，又能通过适当的密码或登录提供管理访问权限，证明用户拥有访问该数据的适当权限，从而实现可用性。 

Sometimes it is necessary to allow users to access the information via a temporary or limited access, for instance, for a specific time period or just within normal business hours. Or access rules can limit the fields that the individuals can have access to. One example is a healthcare environment. Some workers might have access to patient data but not their medical data. Individual doctors might have access only to data related to their own patients. In some cases, this is regulated by law, such as HIPAA in the United States, and by specific privacy laws in other countries. 
有时，有必要允许用户通过临时或有限的访问权限来访问信息，例如，在特定时间段内或仅在正常工作时间内。或者，访问规则可以限制个人可以访问的字段。医疗环境就是一个例子。一些工作人员可能可以访问病人数据，但不能访问他们的医疗数据。个别医生可能只能访问与自己病人有关的数据。在某些情况下，这是由法律规定的，如美国的 HIPAA 和其他国家的特定隐私法。

Systems often monitor access to private information, and if logs indicate that someone has attempted to access a database without the proper permissions, that will automatically trigger an alarm. The security administrator will then record the incident and alert the appropriate people to take action.  
系统通常会监控对私人信息的访问，如果日志显示有人试图在没有适当权限的情况下访问数据库，就会自动触发警报。安全管理员会记录下这一事件，并提醒相关人员采取行动。 

The more critical information a person has access to, the greater the security should be around that access. They should definitely have multi-factor authentication, for instance. 
一个人可以访问的关键信息越多，访问的安全性就越高。例如，他们肯定应该有多因素身份验证。

### Privileged Access Management
### 特權存取管理
Privileged access management provides the first and perhaps most familiar use case. Consider a human user identity that is granted various create, read, update, and delete privileges on a database. Without privileged access management, the system’s access control would have those privileges assigned to the administrative user in a static way, effectively “on” 24 hours a day, every day. Security would be dependent upon the login process to prevent misuse of that identity. Just-in-time privileged access management, by contrast, includes role-based specific subsets of privileges that only become active in real time when the identity is requesting the use of a resource or service. 
特权访问管理提供了第一个可能也是最熟悉的使用案例。假设一个人类用户身份被授予在数据库上创建、读取、更新和删除的各种权限。如果没有特权访问管理，系统的访问控制就会以静态的方式将这些权限分配给管理用户，实际上就是每天 24 小时 "开机"。安全性将取决于登录过程，以防止滥用该身份。与此相反，即时特权访问管理包括基于角色的特定特权子集，只有在身份要求使用资源或服务时才会实时激活。

### Privileged Accounts
### 特權帳戶

Privileged accounts are those with permissions beyond those of normal users, such as managers and administrators. Broadly speaking, these accounts have **elevated privileges** and are used by many different classes of users, including: 
特权账户是指拥有超出普通用户权限的账户，如经理和管理员。广义上讲，这些账户拥有**高权限**，被许多不同类别的用户使用，包括： 

* Systems administrators, who have the principal responsibilities for operating systems, applications deployment and performance management. 
* Help desk or IT support staff, who often need to view or manipulate endpoints, servers and applications platforms by using privileged or restricted operations. 
* Security analysts, who may require rapid access to the entire IT infrastructure, systems, endpoints and data environment of the organization. 
* 系统管理员，主要负责操作系统、应用程序部署和性能管理。
* 服务台或 IT 支持人员，他们经常需要通过使用权限或受限操作来查看或操作端点、服务器和应用程序平台。
* 安全分析人员，他们可能需要快速访问组织的整个 IT 基础设施、系统、端点和数据环境。

Other classes of privileged user accounts may be created on a per-client or per-project basis, to allow a member of that project or client service team to have greater control over data and applications. These few examples indicate that organizations often need to delegate the capability to manage and protect information assets to various managerial, supervisory, support or leadership people, with differing levels of authority and responsibility. This delegation, of course, should be contingent upon trustworthiness, since misuse or abuse of these privileges could lead to harm for the organization and its stakeholders. 
其他类别的特权用户账户可按客户或项目创建，以允许该项目或客户服务团队的成员对数据和应用程序拥有更大的控制权。以上几个例子表明，企业往往需要将管理和保护信息资产的能力下放给不同级别的管理、监督、支持或领导人员，并赋予他们不同的权力和责任。当然，这种授权应该以值得信赖为前提，因为误用或滥用这些特权可能会对组织及其利益相关者造成伤害。

Typical measures used for moderating the potential for elevated risks from misuse or abuse of privileged accounts include the following: 
用于缓和因误用或滥用特权账户而导致潜在风险升高的典型措施包括以下几种：

    * More extensive and detailed logging than regular user accounts. The record of privileged actions is vitally important, as both a deterrent (for privileged account holders that might be tempted to engage in untoward activity) and an administrative control (the logs can be audited and reviewed to detect and respond to malicious activity). 
        * 日志记录比普通用户账户更广泛、更详细。 特权行为的记录至关重要，既能起到威慑作用（对可能会从事不轨活动的特权账户持有者而言），又能起到管理控制作用（可对日志进行审计和审查，以发现和应对恶意活动）。
   
    * More stringent access control than regular user accounts. As we will see emphasized in this course, even nonprivileged users should be required to use MFA methods to gain access to organizational systems and networks. Privileged users—or more accurately, highly trusted users with access to privileged accounts—should be required to go through additional or more rigorous authentication prior to those privileges. Just-in-time identity should also be considered as a way to restrict the use of these privileges to specific tasks and the times in which the user is executing them. 
      * 比普通用户账户更严格的访问控制。正如我们将在本课程中强调的那样，即使是非特权用户也应被要求使用 MFA 方法来访问组织系统和网络。特权用户--或者更准确地说，可以访问特权账户的高信任度用户--应被要求在获得这些特权之前通过额外或更严格的身份验证。此外，还应考虑将及时身份验证作为一种方法，将这些特权的使用限制在特定任务和用户执行任务的时间范围内。
      
    * Deeper trust verification than regular user accounts. Privileged account holders should be subject to more detailed background checks, stricter nondisclosure agreements and acceptable use policies, and be willing to be subject to financial investigation. Periodic or event-triggered updates to these background checks may also be in order, depending on the nature of the organization’s activities and the risks it faces. 
     * 比普通用户账户更严格的信任验证。 特权账户持有人应接受更详细的背景调查、更严格的保密协议和可接受的使用政策，并愿意接受财务调查。根据组织活动的性质和面临的风险，定期或由事件触发更新这些背景调查也是有必要的。
     
    * More auditing than regular user accounts. Privileged account activity should be monitored and audited at a greater rate and extent than regular usage. 
 * 比普通用户账户更多的审计。 对特权账户活动的监控和审计力度和范围应大于普通用户账户。

### Segregation of Duties 
### 職責分離

A core element of authorization is the **principle of segregation of duties** (also known as separation of duties). **Segregation of duties is based on the security practice that no one person should control an entire high-risk transaction from start to finish**. **Segregation of duties breaks the transaction into separate parts and requires a different person to execute each part of the transaction**. For example, an employee may submit an invoice for payment to a vendor (or for reimbursement to themselves), but it must be approved by a manager prior to payment; in another instance, almost anyone may submit a proposal for a change to a system configuration, but the request must go through technical and management review and gain approval, before it can be implemented.
授权的一个核心要素是**职责分离原则**（也称为职责分离）。**职责分离是基于这样一种安全惯例：不应由一个人自始至终控制整个高风险交易**。**职责分离将交易分成不同的部分，并要求由不同的人来执行交易的每个部分**。例如，员工可以提交一张发票，要求供应商付款（或报销给自己），但在付款前必须得到经理的批准；在另一个例子中，几乎任何人都可以提交一份更改系统配置的建议，但该请求必须经过技术和管理审查并获得批准后才能实施。

These steps can prevent fraud or detect an error in the process before implementation. It could be that the same employee might be authorized to originally submit invoices regarding one set of activities, but not approve them, and yet also have approval authority but not the right to submit invoices on another. It is possible, of course, that two individuals can willfully work together to bypass the segregation of duties, so that they could jointly commit fraud. This is called collusion.
这些步骤可以防止欺诈或在实施前发现流程中的错误。同一员工可能被授权就某项活动提交发票，但无权审批，但也有审批权，但无权就另一项活动提交发票。当然，也有可能是两个人故意合作，绕过职责分工，共同实施欺诈。这就是所谓的串通。

Another implementation of segregation of duties is dual control. This would apply at a bank where there are two separate combination locks on the door of the vault. Some personnel know one of the combinations and some know the other, but no one person knows both combinations. Two people must work together to open the vault; thus, the vault is under dual control. 
职责分离的另一种实施方式是双重控制。在一家银行，保险库的门上有两把不同的密码锁。有些人知道其中一个密码，有些人知道另一个，但没有一个人同时知道两个密码。两个人必须合作才能打开保险库；因此，保险库处于双重控制之下。

**The two-person rule is a security strategy that requires a minimum of two people to be in an area together, making it impossible for a person to be in the area alone**. Many access control systems prevent an individual cardholder from entering a selected high-security area unless accompanied by at least one other person. Use of the two-person rule can help reduce insider threats to critical areas by requiring at least two individuals to be present at any time. It is also used for life safety within a security area; if one person has a medical emergency, there will be assistance present.
**两人规则是一种安全策略，要求至少两人一起进入一个区域，使一个人无法单独进入该区域**。许多门禁控制系统会阻止持卡人进入选定的高安全区域，除非至少有另一人陪同。两人规则要求任何时候都至少有两人在场，有助于减少内部人员对重要区域的威胁。它还可用于安全区域内的生命安全；如果一个人出现医疗紧急情况，将有援助人员在场。

### How Users Are Provisioned
### 如何設定用戶
Other situations that call for provisioning new user accounts or changing privileges include: 
其他需要配置新使用者帳戶或變更權限的情況包括：

* **A new employee**: When a new employee is hired, the hiring manager sends a request to the security administrator to create a new user ID. This request authorizes creation of the new ID and provides instructions on appropriate access levels. Additional authorization may be required by company policy for elevated permissions. 
** 新员工**： 新员工入职时，招聘经理会向安全管理员发出创建新用户 ID 的请求。该请求授权创建新 ID，并提供有关适当访问级别的说明。根据公司政策，可能需要额外授权以获得更高的权限。

* **Change of position**: When an employee has been promoted, their permissions and access rights might change as defined by the new role, which will dictate any added privileges and updates to access. At the same time, any access that is no longer needed in the new job will be removed. 
** 职位变更**： 员工晋升后，其权限和访问权可能会根据新的角色发生变化，这将决定访问权限的增加和更新。同时，新工作不再需要的任何访问权限也将被删除。

* **Separation of employment**: When employees leave the company, depending on company policy and procedures, their accounts must be disabled after the termination date and time. It is recommended that accounts be disabled for a period before they are deleted to preserve the integrity of any audit trails or files that may be owned by the user. Since the account will no longer be used, it should be removed from any security roles or additional access profiles. This protects the company, so the separated employee is unable to access company data after separation, and it also protects them because their account cannot be used by others to access data.
** 离职**： 员工离职时，根据公司政策和程序，其账户必须在终止日期和时间之后禁用。建议在删除账户前禁用一段时间，以保持用户可能拥有的任何审计跟踪或文件的完整性。由于不再使用账户，因此应将其从任何安全角色或附加访问配置文件中删除。这样做既能保护公司，使离职员工在离职后无法访问公司数据，又能保护自己，因为他人无法使用其账户访问数据。

## Module 2: Understand Physical Access Controls
## 模組 2：了解實體存取控制
Domain D3.1, D3.1.1, D3.1.2

### What Are Physical Security Controls? 
### 什麼是實體安全控制？

Physical access controls are items you can physically touch, which include physical mechanisms deployed to prevent, monitor, or detect direct contact with systems or areas within a facility. Examples of physical access controls include security guards, fences, motion detectors, locked doors/gates, sealed windows, lights, cable protection, laptop locks, badges, swipe cards, guard dogs, cameras, mantraps/turnstiles, and alarms.
物理访问控制是可以实际接触到的项目，包括用于防止、监控或检测与设施内系统或区域直接接触的物理机制。物理访问控制的例子包括安全警卫、围栏、移动探测器、上锁的门/闸、密封的窗、灯、电缆保护、笔记本电脑锁、徽章、刷卡器、看门狗、摄像头、密码锁/旋转门和警报器。

Physical access controls are necessary to protect the assets of a company, including its most important asset, people. When considering physical access controls, the security of the personnel always comes first, followed by securing other physical assets.
要保护公司的资产，包括最重要的资产--人员，就必须要有实体访问控制。在考虑物理访问控制时，人员的安全始终是第一位的，其次才是其他有形资产的安全。

### Why Have Physical Security Controls?
### 為什麼要有實體安全控制？

Physical access controls include **fences, barriers, turnstiles, locks and other features that prevent unauthorized individuals from entering a physical site**, such as a workplace. This is to protect not only physical assets such as computers from being stolen, but also to protect the health and safety of the personnel inside. 
物理访问控制包括**围栏、障碍物、旋转栅门、锁和其他防止未经授权人员进入**物理场所（如工作场所）的功能。这不仅是为了保护电脑等有形资产不被盗，也是为了保护内部人员的健康和安全。

### Types of Physical Access Controls
### 實體存取控制的類型

Many types of physical access control mechanisms can be deployed in an environment to control, monitor and manage access to a facility. These range from deterrents to detection mechanisms. Each area requires unique and focused physical access controls, monitoring and prevention mechanisms.
可以在环境中部署多种类型的物理访问控制机制，以控制、监控和管理设施的访问。这些机制包括威慑机制和检测机制。每个区域都需要独特和重点突出的实物出入控制、监控和防范机制。

#### Badge Systems and Gate Entry
#### 徽章系統與大門入口

Physical security controls for human traffic are often done with technologies such as turnstiles, mantraps and remotely or system-controlled door locks. For the system to identify an authorized employee, an access control system needs to have some form of enrollment station used to assign and activate an access control device. Most often, a badge is produced and issued with the employee’s identifiers, with the enrollment station giving the employee specific areas that will be accessible. In high-security environments, enrollment may also include biometric characteristics. In general, an access control system compares an individual’s badge against a verified database. If authenticated, the access control system sends output signals allowing authorized personnel to pass through a gate or a door to a controlled area. The systems are typically integrated with the organization’s logging systems to document access activity (authorized and unauthorized)
对人员通行的物理安全控制通常采用旋转栅门、门闩、遥控或系统控制门锁等技术。为使系统能识别经授权的员工，门禁控制系统需要有某种形式的登记站，用于分配和激活门禁设备。最常见的做法是，制作并发放带有员工识别信息的徽章，由登记站向员工提供可进入的特定区域。在高度安全的环境中，登记还可能包括生物识别特征。一般来说，门禁控制系统会将个人徽章与经过验证的数据库进行比较。如果通过验证，门禁控制系统就会发出输出信号，允许经授权的人员通过闸门或门进入受控区域。这些系统通常与组织的记录系统集成，以记录出入活动（授权的和未经授权的）。

A range of card types allow the system to be used in a variety of environments. These cards include: Bar code, Magnetic stripe, Proximity, Smart, Hybrid
各种类型的卡使系统可用于各种环境。这些卡包括 条形码、磁条、感应卡、智能卡、混合卡

#### Environmental Design
####環境設計
Crime Prevention through Environmental Design (CPTED) approaches the challenge of creating safer workspaces through passive design elements. This has great applicability for the information security community as security professionals design, operate and assess the organizational security environment. Other practices, such as standards for building construction and data centers, also affect how we implement controls over our physical environment. Security professionals should be familiar with these concepts so they can successfully advocate for functional and effective physical spaces where information is going to be created, processed and stored.
通过环境设计预防犯罪（CPTED）通过被动设计元素来应对创建更安全工作空间的挑战。这对信息安全界非常适用，因为安全专业人员会设计、运行和评估组织的安全环境。建筑施工和数据中心标准等其他实践也会影响我们如何对物理环境实施控制。安全专业人员应熟悉这些概念，这样他们才能成功地倡导创建、处理和存储信息的物理空间的功能性和有效性。

CPTED provides direction to solve the challenges of crime with organizational (people), mechanical (technology and hardware) and natural design (architectural and circulation flow) methods. By directing the flow of people, using passive techniques to signal who should and should not be in a space and providing visibility to otherwise hidden spaces, the likelihood that someone will commit a crime in that area decreases.
CPTED 为利用组织（人员）、机械（技术和硬件）和自然设计（建筑和流通）方法解决犯罪难题提供了方向。通过引导人流、使用被动技术提示谁应该和不应该进入某个空间，以及为原本隐蔽的空间提供可见度，可以降低有人在该区域实施犯罪的可能性。

#### Biometrics
#### 生物識別
To authenticate a user’s identity, biometrics uses characteristics unique to the individual seeking access. A biometric authentication solution entails two processes.
为了验证用户的身份，生物识别技术使用了寻求访问的个人独有的特征。生物识别身份验证解决方案包含两个过程。

Enrollment—during the enrollment process, the user’s registered biometric code is either stored in a system or on a smart card that is kept by the user.
Verification—during the verification process, the user presents their biometric data to the system so that the biometric data can be compared with the stored biometric code.
注册--在注册过程中，用户注册的生物识别代码会存储在系统中或用户保存的智能卡中。
验证--在验证过程中，用户向系统提交其生物识别数据，以便将生物识别数据与存储的生物识别代码进行比较。

Even though the biometric data may not be secret, it is personally identifiable information, and the protocol should not reveal it without the user’s consent. Biometrics takes two primary forms, physiological and behavioral.
尽管生物识别数据可能不是秘密，但它是可识别个人身份的信息，未经用户同意，协议不得泄露。生物识别有两种主要形式，即生理识别和行为识别。

Physiological systems measure the characteristics of a person such as a fingerprint, iris scan (the colored portion around the outside of the pupil in the eye), retinal scan (the pattern of blood vessels in the back of the eye), palm scan and venous scans that look for the flow of blood through the veins in the palm. Some biometrics devices combine processes together—such as checking for pulse and temperature on a fingerprint scanner—to detect counterfeiting.
生理系统可以测量人的特征，如指纹、虹膜扫描（眼睛瞳孔外侧的彩色部分）、视网膜扫描（眼睛后部的血管图案）、手掌扫描和静脉扫描，后者可以检测血液在手掌静脉中的流动情况。有些生物识别设备将各种过程结合在一起--例如在指纹扫描仪上检查脉搏和体温--来检测伪造。

Behavioral systems measure how a person acts by measuring voiceprints, signature dynamics and keystroke dynamics. As a person types, a keystroke dynamics system measures behavior such as the delay rate (how long a person holds down a key) and transfer rate (how rapidly a person moves between keys).
行为系统通过测量声纹、签名动态和按键动态来衡量一个人的行为方式。当一个人打字时，击键动态系统会测量其行为，如延迟率（按住一个键的时间）和转移率（在键之间移动的速度）。

Biometric systems are considered highly accurate, but they can be expensive to implement and maintain because of the cost of purchasing equipment and registering all users. Users may also be uncomfortable with the use of biometrics, considering them to be an invasion of privacy or presenting a risk of disclosure of medical information (since retina scans can disclose medical conditions). A further drawback is the challenge of sanitization of the devices.
生物识别系统被认为是高度准确的，但由于购买设备和登记所有用户的费用，其实施和维护成本可能很高。用户也可能对使用生物识别技术感到不舒服，认为这侵犯了隐私或有泄露医疗信息的风险（因为视网膜扫描可能会泄露医疗状况）。另一个缺点是设备的消毒问题。

### Monitoring
### 監控
The use of physical access controls and monitoring personnel and equipment entering and leaving as well as auditing/logging all physical events are primary elements in maintaining overall organizational security. 
使用物理访问控制、监控人员和设备进出以及审计/记录所有物理事件是维护组织整体安全的主要因素。

#### Cameras
#### 相機
Cameras are normally integrated into the overall security program and centrally monitored. Cameras provide a flexible method of surveillance and monitoring. They can be a deterrent to criminal activity, can detect activities if combined with other sensors and, if recorded, can provide evidence after the activity They are often used in locations where access is difficult or there is a need for a forensic record.While cameras provide one tool for monitoring the external perimeter of facilities, other technologies augment their detection capabilities. A variety of motion sensor technologies can be effective in exterior locations. These include infrared, microwave and lasers trained on tuned receivers. Other sensors can be integrated into doors, gates and turnstiles, and strain-sensitive cables and other vibration sensors can detect if someone attempts to scale a fence. Proper integration of exterior or perimeter sensors will alert an organization to any intruders attempting to gain access across open space or attempting to breach the fence line.
摄像机通常被纳入整体安全计划并进行集中监控。摄像头提供了一种灵活的监视和监控方法。它们可以对犯罪活动起到威慑作用，如果与其他传感器结合使用，还可以侦测到犯罪活动，如果记录下来，还可以在犯罪活动发生后提供证据。摄像机通常用于难以进入或需要取证记录的地点。各种运动传感器技术都能在外部位置发挥有效作用。这些技术包括红外线、微波和激光。其他传感器可以集成到门、闸门和旋转栅栏中，应变敏感电缆和其他振动传感器可以探测到是否有人试图翻越围栏。适当集成外部或周界传感器，可提醒企业注意任何试图穿越开放空间或试图突破围栏线的入侵者。

#### Logs
#### 紀錄
In this section, we are concentrating on the use of physical logs, such as a sign-in sheet maintained by a security guard, or even a log created by an electronic system that manages physical access. Electronic systems that capture system and security logs within software will be covered in another section.
在本节中，我们将集中讨论物理日志的使用，如保安员维护的签到表，甚至是管理物理访问的电子系统创建的日志。在软件中采集系统和安全日志的电子系统将在另一节中介绍。

A log is a record of events that have occurred. Physical security logs are essential to support business requirements. They should capture and retain information as long as necessary for legal or business reasons. Because logs may be needed to prove compliance with regulations and assist in a forensic investigation, the logs must be protected from manipulation. Logs may also contain sensitive data about customers or users and should be protected from unauthorized disclosure.
日志是对已发生事件的记录。实体安全日志对于支持业务要求至关重要。出于法律或业务原因，日志应在必要的时间内捕获并保留信息。由于可能需要日志来证明是否符合法规并协助取证调查，因此必须防止日志被篡改。日志还可能包含有关客户或用户的敏感数据，因此应防止未经授权的披露。

The organization should have a policy to review logs regularly as part of their organization’s security program. As part of the organization’s log processes, guidelines for log retention must be established and followed. If the organizational policy states to retain standard log files for only six months, that is all the organization should have.
作为组织安全计划的一部分，组织应制定定期审查日志的政策。作为组织日志流程的一部分，必须制定并遵循日志保留准则。如果组织政策规定只保留六个月的标准日志文件，那么组织就只能保留六个月。

A log anomaly is anything out of the ordinary. Identifying log anomalies is often the first step in identifying security-related issues, both during an audit and during routine monitoring. Some anomalies will be glaringly obvious: for example, gaps in date/time stamps or account lockouts. Others will be harder to detect, such as someone trying to write data to a protected directory. Although it may seem that logging everything so you would not miss any important data is the best approach, most organizations would soon drown under the amount of data collected.
日志异常是指任何异常情况。在审计和日常监控过程中，识别日志异常往往是发现安全相关问题的第一步。有些异常情况非常明显：例如，日期/时间戳中的空白或账户锁定。其他异常则较难发现，例如有人试图向受保护目录写入数据。虽然记录一切以便不错过任何重要数据似乎是最好的方法，但大多数组织很快就会被收集的数据量淹没。

Business and legal requirements for log retention will vary among economies, countries and industries. Some businesses will have no requirements for data retention. Others are mandated by the nature of their business or by business partners to comply with certain retention data. For example, the Payment Card Industry Data Security Standard (PCI DSS) requires that businesses retain one year of log data in support of PCI. Some federal regulations include requirements for data retention as well.
不同经济体、国家和行业对日志保留的业务和法律要求各不相同。有些企业对数据保留没有要求。其他企业则因其业务性质或业务合作伙伴而必须遵守某些保留数据的规定。例如，支付卡行业数据安全标准（PCI DSS）要求企业保留一年的日志数据，以支持 PCI。一些联邦法规也包括数据保留的要求。

If a business has no business or legal requirements to retain log data, how long should the organization keep it? The first people to ask should be the legal department. Most legal departments have very specific guidelines for data retention, and those guidelines may drive the log retention policy.
如果企业没有保留日志数据的业务或法律要求，那么企业应该将其保留多长时间？首先应该询问法律部门。大多数法律部门都有非常具体的数据保留准则，这些准则可能会推动日志保留政策。

#### Security Guards
＃＃＃＃ 保安人員
Security guards are an effective physical security control. No matter what form of physical access control is used, a security guard or other monitoring system will discourage a person from masquerading as someone else or following closely on the heels of another to gain access. This helps prevent theft and abuse of equipment or information.
保安员是一种有效的实体安全控制手段。无论使用哪种形式的实体访问控制，保安员或其他监控系统都会阻止他人伪装成他人或紧跟他人进入。这有助于防止盗窃和滥用设备或信息。

#### Alarm Systems
#### 警報系統
Alarm systems are commonly found on doors and windows in homes and office buildings. In their simplest form, they are designed to alert the appropriate personnel when a door or window is opened unexpectedly.
报警系统通常安装在住宅和办公楼的门窗上。其最简单的设计是在门窗意外打开时向相关人员发出警报。

For example, an employee may enter a code and/or swipe a badge to open a door, and that action would not trigger an alarm. Alternatively, if that same door was opened by brute force without someone entering the correct code or using an authorized badge, an alarm would be activated.
例如，员工可以输入密码和/或刷卡开门，但这一操作不会触发警报。相反，如果同一扇门在没有输入正确密码或使用授权徽章的情况下被强行打开，则会触发警报。

Another alarm system is a fire alarm, which may be activated by heat or smoke at a sensor and will likely sound an audible warning to protect human lives in the vicinity. It will likely also contact local response personnel as well as the closest fire department.
另一种报警系统是火灾报警器，它可能由传感器上的热量或烟雾激活，并可能发出声音警告，以保护附近人员的生命安全。它还可能会联系当地的应急人员以及最近的消防部门。

Finally, another common type of alarm system is in the form of a panic button. Once activated, a panic button will alert the appropriate police or security personnel.
最后，另一种常见的报警系统是紧急按钮。一旦启动，紧急按钮就会向有关警察或保安人员发出警报。

## Module 3: Understand Logical Access Controls
## 模組 3：了解邏輯存取控制
Domain D3.2, D3.2.3, D3.2.4, D3.2.5

### What are Logical Access Controls?
### 什麼是邏輯存取控制？
Whereas physical access controls are tangible methods or mechanisms that limit someone from getting access to an area or asset, logical access controls are electronic methods that limit someone from getting access to systems, and sometimes even to tangible assets or areas. Types of logical access controls include: 
物理访问控制是限制他人进入某个区域或资产的有形方法或机制，而逻辑访问控制则是限制他人进入系统，有时甚至是进入有形资产或区域的电子方法。逻辑访问控制的类型包括

* Passwords
* Biometrics (implemented on a system, such as a smartphone or laptop)
* Badge/token readers connected to a system
* 密码
* 生物识别（在智能手机或笔记本电脑等系统上实施）
* 与系统连接的徽章/令牌阅读器

These types of electronic tools limit who can get logical access to an asset, even if the person already has physical access.
这些类型的电子工具限制了谁可以对资产进行逻辑访问，即使该人已经拥有物理访问权限。

#### Discretionary Access Control (DAC)
#### 自主存取控制 (DAC)
Discretionary access control (DAC) is a specific type of access control policy that is **enforced over all subjects and objects in an information system**. In DAC, the policy specifies that **a subject who has been granted access to information can do one or more of the following**:
自由裁量访问控制（DAC）是一种特定类型的访问控制策略，**对信息系统中的所有主体和对象**执行。在 DAC 中，政策规定**获准访问信息的主体可以进行以下一项或多项**：

* Pass the information to other subjects or objects 
* Grant its privileges to other subjects 
* Change security attributes on subjects, objects, information systems or system components 
* Choose the security attributes to be associated with newly created or revised objects; and/or 
* Change the rules governing access control; mandatory access controls restrict this capability 
* 将信息传递给其他主体或客体 
* 向其他主体授予权限 
* 更改主体、对象、信息系统或系统组件的安全属性 
* 选择与新创建或修改的对象相关联的安全属性；和/或 
* 更改访问控制规则；强制性访问控制限制了这种能力 

**Most information systems in the world are DAC systems**. In a DAC system, a user who has access to a file is usually able to share that file with or pass it to someone else. This grants the user almost the same level of access as the original owner of the file. **Rule-based access control systems are usually a form of DAC**. 
**世界上大多数信息系统都是 DAC 系统**。在 DAC 系统中，拥有文件访问权限的用户通常可以与他人共享文件或将文件传给他人。这样，用户的访问权限几乎与文件的原始所有者相同。**基于规则的访问控制系统通常是 DAC**的一种形式。

This methodology relies on the discretion of the owner of the access control object to determine the access control subject’s specific rights. Hence, security of the object is literally up to the discretion of the object owner. DACs are not very scalable; they rely on the access control decisions made by each individual object owner, and it can be difficult to find the source of access control issues when problems occur.
这种方法依赖访问控制对象所有者的自由裁量权来决定访问控制主体的具体权利。因此，对象的安全性完全取决于对象所有者的自由裁量权。DAC 的可扩展性不强；它依赖于每个对象所有者做出的访问控制决定，而且在出现问题时很难找到访问控制问题的根源。

#### Mandatory Access Control (MAC)
#### 強制存取控制 (MAC)
A mandatory access control (MAC) policy is one that is **uniformly enforced across all subjects and objects within the boundary of an information system**. In simplest terms, **this means that only properly designated security administrators, as trusted subjects, can modify any of the security rules that are established for subjects and objects within the system**. This also means that for all subjects defined by the organization (that is, known to its integrated identity management and access control system), the organization assigns a subset of total privileges for a subset of objects, such that the subject is constrained from doing any of the following:
强制访问控制（MAC）政策是对信息系统边界内的所有主体和对象**统一执行的政策。最简单地说，**这意味着只有正确指定的安全管理员，作为受信任的主体，才能修改为系统内主体和对象制定的任何安全规则**。这也意味着，对于组织定义的所有主体（即其综合身份管理和访问控制系统已知的主体），组织为一个子集的对象分配了一个子集的总特权，这样主体就受到限制，不能做以下任何事情：

* Passing the information to unauthorized subjects or objects 
* Granting its privileges to other subjects 
* Changing one or more security attributes on subjects, objects, the information system or system components 
* Choosing the security attributes to be associated with newly created or modified objects 
* Changing the rules governing access control 
* 将信息传递给未经授权的主体或客体 
* 向其他主体授予权限 
* 更改主体、客体、信息系统或系统组件的一个或多个安全属性 
* 选择与新创建或修改的对象相关联的安全属性 
* 更改访问控制规则 

Although MAC sounds very similar to DAC, **the primary difference is who can control access**. With Mandatory Access Control, **it is mandatory for security administrators to assign access rights or permissions**; **with Discretionary Access Control, it is up to the object owner’s discretion**. 
虽然 MAC 听起来与 DAC 非常相似，但**主要区别在于谁可以控制访问**。对于强制访问控制，**安全管理员必须分配访问权或权限**；而对于全权访问控制，则由对象所有者自行决定**。

#### Role-Based Access Control (RBAC)
#### 基於角色的存取控制 (RBAC)
Role-based access control (RBAC), as the name suggests, sets up user permissions based on roles. Each role represents users with similar or identical permissions.  
基于角色的访问控制（RBAC），顾名思义，就是根据角色设置用户权限。每个角色代表具有相似或相同权限的用户。

Role-based access control provides each worker privileges based on what role they have in the organization. Only Human Resources staff have access to personnel files, for example; only Finance has access to bank accounts; each manager has access to their own direct reports and their own department. Very high-level system administrators may have access to everything; new employees would have very limited access, the minimum required to do their jobs.  
基于角色的访问控制根据每个员工在组织中的角色提供相应的权限。例如，只有人力资源部门的员工才能访问人事档案；只有财务部门的员工才能访问银行账户；每个经理都能访问自己的直接下属和自己的部门。级别很高的系统管理员可以访问所有内容；新员工的访问权限非常有限，只有完成工作所需的最低权限。 

Monitoring these role-based permissions is important, because if you expand one person’s permissions for a specific reason—say, a junior worker’s permissions might be expanded so they can temporarily act as the department manager—but you forget to change their permissions back when the new manager is hired, then the next person to come in at that junior level might inherit those permissions when it is not appropriate for them to have them. This is called privilege creep or permissions creep. We discussed this before, when we were talking about provisioning new users.  
监控这些基于角色的权限非常重要，因为如果你出于某个特定原因扩展了某个人的权限--比如，某个初级员工的权限可能被扩展了，这样他们就可以临时担任部门经理，但当新经理被聘用时，你却忘了把他们的权限改回来，那么下一个来担任该初级职位的人就可能在不适合拥有这些权限的情况下继承这些权限。这就是所谓的 "特权爬行 "或 "权限爬行"。我们以前在讨论配置新用户时讨论过这个问题。 

Having multiple roles with different combinations of permissions can require close monitoring to make sure everyone has the access they need to do their jobs and nothing more. In this world where jobs are ever-changing, this can sometimes be a challenge to keep track of, especially with extremely granular roles and permissions. Upon hiring or changing roles, a best practice is to not copy user profiles to new users. It is recommended that standard roles are established, and new users are created based on those standards rather than an actual user. That way, new employees start with the appropriate roles and permissions. 
多个角色拥有不同的权限组合，这就需要密切监控，确保每个人都拥有完成工作所需的访问权限。在这个工作岗位不断变化的世界里，这有时是一项难以跟踪的挑战，尤其是在角色和权限极为细化的情况下。在招聘或更改角色时，最佳做法是不要将用户配置文件复制给新用户。建议建立标准角色，并根据这些标准而不是实际用户创建新用户。这样，新员工一开始就能获得适当的角色和权限。
