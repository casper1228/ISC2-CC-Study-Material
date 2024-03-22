# L5 Security Operations

## Module 1: Understand Data Security

Domain D5.0, D5.1.1, D5.1.2, D5.1.3

**Hardening** is the process of applying secure configurations (to reduce the attack surface) and locking down various hardware, communications systems and software, including the operating system, web server, application server and applications, etc. This module introduces configuration management practices that will ensure systems are installed and maintained according to industry and organizational security standards. 
**加固**是应用安全配置（以减少攻击面）和锁定各种硬件、通信系统和软件（包括操作系统、网络服务器、应用服务器和应用程序等）的过程。本模块介绍配置管理实践，以确保系统的安装和维护符合行业和组织的安全标准。

### Data Handling
＃＃＃ 資料處理
Data itself goes through **its own life cycle as users create**, **use**, **share and modify it**. The data security life cycle model is useful because **it can align easily with the different roles that people and organizations perform during the evolution of data from creation to destruction (or disposal)**. It also helps put the different **data states of in use, at rest and in motion, into context**. 
随着用户创建**、使用**、共享和修改**，数据本身也会经历**个生命周期。数据安全生命周期模型非常有用，因为**它很容易与人们和组织在数据从创建到销毁（或处置）**的演变过程中所扮演的不同角色保持一致。它还有助于将使用中、静止中和运动中的不同**数据状态与上下文**联系起来。

All ideas, data, information or knowledge can be thought of as going through six major sets of activities throughout its lifetime. Conceptually, these involve:
所有想法、数据、信息或知识在其整个生命周期中都会经历六组主要活动。从概念上讲，这些活动包括

1. Creating the knowledge, which is usually tacit knowledge at this point.
2. Storing or recording it in some fashion (which makes it explicit).
3. Using the knowledge, which may cause the information to be modified, supplemented or partially deleted.
4. Sharing the data with other users, whether as a copy or by moving the data from one location to another.
5. Archiving the data when it is temporarily not needed.
6. Destroying the data when it is no longer needed.

1. 创造知识，此时通常是隐性知识。
2. 以某种方式存储或记录知识（使其显性化）。
3. 使用知识，这可能导致信息被修改、补充或部分删除。
4. 与其他用户共享数据，无论是作为副本还是通过将数据从一个位置移动到另一个位置。
5. 在暂时不需要时将数据存档。
6. 不再需要时销毁数据。

### Data Handling Practices
### 資料處理實踐
* **Classification**: classifications dictate **rules and restrictions about how that information can be used**, **stored** or **shared with others**. All of this is done to keep the temporary value and importance of that information from leaking away. Classification of data, which asks the question “Is it secret?” determines the labeling, handling and use of all data. **Classification is the process of recognizing the organizational impacts if the information suffers any security compromises related to its characteristics of confidentiality**, **integrity** and **availability**. **Information is then labeled and handled accordingly**. Classifications are derived from laws, regulations, contract-specified standards or other business expectations. One classification might indicate “minor, may disrupt some processes” while a more extreme one might be “grave, could lead to loss of life or threaten ongoing existence of the organization.” These descriptions should reflect the ways in which the organization has chosen (or been mandated) to characterize and manage risks. The immediate benefit of classification is that it can lead to more efficient design and implementation of security processes, if we can treat the protection needs for all similarly classified information with the same controls strategy. 
**分类**：分类决定了信息使用、存储或与他人共享的**规则和限制。所有这些都是为了防止信息的临时价值和重要性外泄。数据分类提出了 "它是秘密吗？"的问题，决定了所有数据的标记、处理和使用。**如果信息在保密性**、完整性**和可用性**等特性方面受到任何安全损害，那么**分类就是识别组织影响的过程。**然后对信息进行相应的标记和处理**。分类源自法律、法规、合同规定的标准或其他业务期望。一种分类可能是 "轻微的，可能会扰乱某些流程"，而更极端的分类可能是 "严重的，可能导致生命损失或威胁组织的持续生存"。这些描述应反映组织选择（或被授权）的描述和管理风险的方式。分类的直接好处是，如果我们能以相同的控制策略来对待所有类似分类信息的保护需求，那么它就能提高安全流程的设计和实施效率。

* **Labeling**: **security labels are part of implementing controls to protect classified information**. It is reasonable to want a simple way of assigning a level of sensitivity to a data asset, such that the higher the level, the greater the presumed harm to the organization, and thus the greater security protection the data asset requires. This spectrum of needs is useful, but it should not be taken to mean that clear and precise boundaries exist between the use of “low sensitivity” and “moderate sensitivity” labeling, for example.
  ** 标签**： **安全标签是实施控制以保护机密信息的一部分**。为数据资产分配敏感度级别的简单方法是合理的，级别越高，假定对组织的危害越大，因此数据资产需要的安全保护也越大。这种需求范围是有用的，但不应将其理解为在使用 "低敏感度 "和 "中等敏感度 "标签之间存在明确和精确的界限。
  
    * **Data Sensitivity Levels and Labels**: unless otherwise mandated, organizations are free to create classification systems that best meet their own needs. In professional practice, it is typically best if the organization has enough classifications to distinguish between sets of assets with differing sensitivity/value, but not so many classifications that the distinction between them is confusing to individuals. Typically, two or three classifications are manageable, and more than four tend to be difficult. 
 ** 数据敏感度级别和标签**：除非另有规定，否则组织可自由创建最符合自身需要的分类系统。在专业实践中，通常情况下，组织最好有足够的分类来区分具有不同敏感性/价值的资产集，但又不要有太多的分类，以免个人对它们之间的区别感到困惑。通常情况下，两到三个分类是可以管理的，而超过四个分类则会比较困难。

    **Highly restricted**: Compromise of data with this sensitivity label could possibly put the organization’s future existence at risk. Compromise could lead to substantial loss of life, injury or property damage, and the litigation and claims that would follow.
  **高度受限**： 泄露带有此敏感性标签的数据可能会危及组织未来的生存。泄密可能导致重大人员伤亡或财产损失，以及随之而来的诉讼和索赔。
  
    **Moderately restricted**: Compromise of data with this sensitivity label could lead to loss of temporary competitive advantage, loss of revenue or disruption of planned investments or activities.
   **中等限制**： 带有此敏感性标签的数据若被破坏，可能会导致暂时性竞争优势的丧失、收入损失或计划投资或活动的中断。
  
    **Low sensitivity (sometimes called “internal use only”)**: Compromise of data with this sensitivity label could cause minor disruptions, delays or impacts.
  **低敏感性（有时称为 "仅供内部使用"）**： 带有此敏感性标签的数据若被破坏，可能会造成轻微的中断、延迟或影响。
  
    Unrestricted public data: As this data is already published, no harm can come from further dissemination or disclosure.  
不受限制的公共数据： 由于这些数据已经公布，进一步传播或披露不会造成任何损害。

* **Retention**: **Information and data should be kept only for as long as it is beneficial, no more and no less**. Certain industry standards, laws and regulations define retention periods, when such external requirements are not set, it is an organization’s responsibility to define and implement its own data retention policy. **Data retention policies are applicable both for hard copies and for electronic data**, and no data should be kept beyond its required or useful life. **Security professionals should ensure that data destruction is being performed when an asset has reached its retention limit**. For the security professional to succeed in this assignment, an accurate inventory must be maintained, including the asset location, retention period requirement, and destruction requirements. Organizations should conduct a periodic review of retained records in order to reduce the volume of information stored and to ensure that only necessary information is preserved. 
** 保留**： **信息和数据的保留期限应仅限于有用的时间，不得多于或少于**。某些行业标准、法律和法规规定了保留期限，如果没有此类外部要求，组织有责任制定并实施自己的数据保留政策。**数据保留政策既适用于硬拷贝，也适用于电子数据**，任何数据都不应保留超过其规定或使用寿命。**安全专业人员应确保在资产达到保留期限时销毁数据**。安全专业人员要成功完成这项任务，就必须保持准确的清单，包括资产位置、保留期限要求和销毁要求。各组织应定期审查保留的记录，以减少存储的信息量，并确保只保留必要的信息。
  
Records retention policies indicate how long an organization is required to maintain information and assets. Policies should guarantee that: 
    * Personnel understand the various retention requirements for data of different types throughout the organization. 
    * The organization appropriately documents the retention requirements for each type of information.
    * The systems, processes and individuals of the organization retain information in accordance with the required schedule but no longer. 
    * A common mistake in records retention is applying the longest retention period to all types of information in an organization. This not only wastes storage but also increases risk of data exposure and adds unnecessary “noise” when searching or processing information in search of relevant records. It may also be in violation of externally mandated requirements such as legislation, regulations or contracts (which may result in fines or other judgments). Records and information no longer mandated to be retained should be destroyed in accordance with the policies of the enterprise and any appropriate legal requirements that may need to be considered. 
记录保留政策表明一个组织需要将信息和资产保留多长时间。政策应保证 
    * 员工了解整个组织内不同类型数据的各种保留要求。 
    * 组织适当记录每类信息的保留要求。
    * 组织的系统、流程和个人按照规定的时间保留信息，但不得超过规定的时间。
    * 记录保留中的一个常见错误是对组织中所有类型的信息都采用最长的保留期。这不仅会浪费存储空间，还会增加数据暴露的风险，并在搜索或处理信息以查找相关记录时增加不必要的 "噪音"。这还可能违反外部授权要求，如法律、法规或合同（可能导致罚款或其他判决）。应根据企业政策和可能需要考虑的任何适当法律要求，销毁不再强制保留的记录和信息。
    
* Destruction: Data that might be left on media after deleting is known as remanence and may be a significant security concern. Steps must be taken to reduce the risk that data remanence could compromise sensitive information to an acceptable level. This can be done by one of several means:  
* 销毁： 删除后可能残留在介质上的数据称为残留数据，可能是一个重大的安全问题。必须采取措施，将数据残留可能危及敏感信息的风险降低到可接受的水平。这可以通过以下几种方法之一来实现：
  
    * Clearing the device or system, which usually involves **writing multiple patterns of random values throughout all storage media**. This is sometimes **called “overwriting” or “zeroizing” the system**, although writing zeros has the risk that a missed block or storage extent may still contain recoverable, sensitive information after the process is completed.
      * 清除设备或系统，这通常涉及**在所有存储介质中**写入多个随机值模式。这有时**被称为 "覆盖 "或 "清零 "系统**，尽管写零会带来风险，即在该过程完成后，遗漏的区块或存储范围可能仍包含可恢复的敏感信息。
        
    * Purging the device or system, which eliminates (or greatly reduces) the chance that residual physical effects from the writing of the original data values may still be recovered, even after the system is cleared. Some magnetic disk storage technologies, for example, can still have residual “ghosts” of data on their surfaces even after being overwritten multiple times. Magnetic media, for example, can often be altered sufficiently to meet security requirements; in more stringent cases, degaussing may not be sufficient.
      * 清除设备或系统，这可以消除（或大大降低）写入原始数据值时产生的残余物理效应，即使在系统清除后仍有可能恢复。例如，某些磁盘存储技术即使在多次覆盖后，其表面仍会有残留的数据 "幽灵"。例如，磁性介质通常可以被充分改变，以满足安全要求；在更严格的情况下，消磁可能是不够的。
        
    * Physical destruction of the device or system is the ultimate remedy to data remanence. Magnetic or optical disks and some flash drive technologies may require being mechanically shredded, chopped or broken up, etched in acid or burned; their remains may be buried in protected landfills, in some cases.
* 设备或系统的物理销毁是数据再现的最终补救措施。磁盘或光盘以及某些闪存盘技术可能需要进行机械粉碎、切碎或分解、酸蚀或焚烧；在某些情况下，其残骸可能会被埋入受保护的垃圾填埋场。
  
    * In many routine operational environments, security considerations may accept that clearing a system is sufficient. But when systems elements are to be removed and replaced, either as part of maintenance upgrades or for disposal, purging or destruction may be required to protect sensitive information from being compromised by an attacker.  
 * 在许多常规操作环境中，出于安全考虑，清理系统就足够了。但是，当系统元件需要移除和更换时，无论是作为维护升级的一部分，还是作为处置的一部分，都可能需要清除或销毁，以保护敏感信息不被攻击者泄露。
   
### Logging and Monitoring Security Events
### 记录和监控安全事件

Logging is the primary form of instrumentation that attempts to capture signals generated by events. Events are any actions that take place within the systems environment and cause measurable or observable change in one or more elements or resources within the system. **Logging imposes a computational cost but is invaluable when determining accountability**. Proper design of logging environments and regular log reviews remain best practices regardless of the type of computer system. 
日志记录是试图捕捉事件产生的信号的主要工具形式。事件是在系统环境中发生的任何行为，会导致系统中一个或多个元素或资源发生可测量或可观测的变化。** 记录会带来计算成本，但在确定责任时却非常宝贵**。无论计算机系统的类型如何，正确设计日志环境和定期审查日志都是最佳做法。

Major controls frameworks emphasize the importance of organizational logging practices. Information that may be relevant to being recorded and reviewed include (but is not limited to): user IDs, system activities, dates/times of key events (e.g., logon and logoff), device and location identity, successful and rejected system and resource access attempts, system configuration changes and system protection activation and deactivation events. 
主要控制框架强调组织日志记录做法的重要性。可能需要记录和审查的相关信息包括（但不限于）：用户 ID、系统活动、关键事件（如登录和注销）的日期/时间、设备和位置标识、成功和被拒绝的系统和资源访问尝试、系统配置更改以及系统保护激活和停用事件。

**Logging and monitoring the health of the information environment is essential to identifying inefficient or improperly performing systems**, detecting compromises and providing a record of how systems are used. **Robust logging practices provide tools to effectively correlate information from diverse systems to fully understand the relationship between one activity and another**. 
**记录和监测信息环境的健康状况，对于识别效率低下或运行不当的系统**、发现漏洞和提供系统使用记录至关重要。**可靠的日志记录方法提供了有效关联不同系统信息的工具，以充分了解一项活动与另一项活动之间的关系**。

Log reviews are an essential function not only for security assessment and testing but also **for identifying security incidents, policy violations, fraudulent activities and operational problems near the time of occurrence**. Log reviews support audits – forensic analysis related to internal and external investigations – and provide support for organizational security baselines. Review of historic audit logs can determine if a vulnerability identified in a system has been previously exploited. 
日志审查不仅是安全评估和测试的重要功能，也是**识别安全事件、违反政策、欺诈活动和操作问题的**。日志审查支持审计--与内部和外部调查有关的取证分析--并为组织安全基线提供支持。审查历史审计日志可以确定系统中发现的漏洞是否曾被利用过。

It is helpful for an organization to create components of a log management infrastructure and determine how these components interact. This aids in preserving the integrity of log data from accidental or intentional modification or deletion and in maintaining the confidentiality of log data. 
创建日志管理基础架构的组件并确定这些组件的交互方式，对企业很有帮助。这有助于保持日志数据的完整性，防止意外或故意修改或删除，并维护日志数据的机密性。

Controls are implemented to protect against unauthorized changes to log information. Operational problems with the logging facility are often related to alterations to the messages that are recorded, log files being edited or deleted, and storage capacity of log file media being exceeded. Organizations must maintain adherence to retention policy for logs as prescribed by law, regulations and corporate governance. Since attackers want to hide the evidence of their attack, the organization’s policies and procedures should also address the preservation of original logs. Additionally, the logs contain valuable and sensitive information about the organization.  Appropriate measures must be taken to protect the log data from malicious use. 
实施的控制措施可防止对日志信息进行未经授权的更改。日志设施的运行问题通常与所记录信息的更改、日志文件被编辑或删除以及日志文件介质的存储容量超限有关。企业必须遵守法律、法规和企业管理规定的日志保留政策。由于攻击者希望隐藏攻击证据，因此组织的政策和程序还应涉及原始日志的保存。此外，日志还包含有关组织的宝贵和敏感信息。 必须采取适当措施保护日志数据免遭恶意使用。

### Event Logging Best Practices
###事件日志最佳实践

Different tools are used depending on whether the risk from the attack is from traffic coming into or leaving the infrastructure. 
使用不同的工具，取决于攻击的风险是来自进入还是离开基础设施的流量。

**Ingress monitoring refers to surveillance and assessment of all inbound communications traffic and access attempts.** Devices and tools that offer logging and alerting opportunities for ingress monitoring include: Firewalls, Gateways, Remote authentication servers, IDS/IPS tools, SIEM solutions, 
Anti-malware solutions. 
** 入口监控是指对所有入站通信流量和访问尝试进行监控和评估。** 为入口监控提供记录和警报机会的设备和工具包括：防火墙、网关、远程身份验证服务器、IDS/IPS 工具、SIEM 解决方案： 防火墙、网关、远程身份验证服务器、IDS/IPS 工具、SIEM 解决方案、 反恶意软件解决方案。

**Egress monitoring is used to regulate data leaving the organization’s IT environment.** The term currently used in conjunction with this effort is **data loss prevention (DLP)** or **data leak protection**. The DLP solution should be deployed so that it can inspect all forms of data leaving the organization, including: Email (content and attachments), Copy to portable media, File Transfer Protocol (FTP), Posting to web pages/websites, Applications/application programming interfaces (APIs). 
**出口监控用于监管离开组织 IT 环境的数据。**目前与这项工作相关的术语是**数据丢失防护（DLP）**或**数据泄漏防护**。部署 DLP 解决方案时，应使其能够检查离开组织的所有形式的数据，包括 电子邮件（内容和附件）、复制到便携式媒体、文件传输协议 (FTP)、发布到网页/网站、应用程序/应用程序编程接口 (API)。

### Encryption Overview
#### 加密概述

Almost every action we take in our modern digital world involves cryptography. Encryption protects our personal and business transactions; digitally signed software updates verify their creator’s or supplier’s claim to authenticity. Digitally signed contracts, binding on all parties, are routinely exchanged via email without fear of being repudiated later by the sender. 
在现代数字世界中，我们的每一个行为几乎都涉及到密码学。加密技术可以保护我们的个人和商业交易；数字签名的软件更新可以验证其创建者或供应商所声称的真实性。经数字签名的合同对各方都有约束力，人们经常通过电子邮件交换合同，而不必担心发件人日后会反悔。

Cryptography is used to protect information by keeping its meaning or content secret and making it unintelligible to someone who does not have a way to decrypt (unlock) that protected information. The objective of every encryption system is to transform an original set of data, called the plaintext, into an otherwise unintelligible encrypted form, called the ciphertext. 
密码学用于保护信息，它将信息的含义或内容保密，使没有办法解密（解锁）受保护信息的人无法理解信息。每个加密系统的目标都是将一组原始数据（称为明文）转换为无法理解的加密形式（称为密文）。

**Properly used**, singly or in combination, **cryptographic solutions provide a range of services that can help achieve required systems security postures in many ways**: 
**正确使用**，无论是单独使用还是组合使用，**加密解决方案都能提供一系列服务，以多种方式帮助实现所需的系统安全态势**： 

    **confidentiality**: Cryptography provides confidentiality by hiding or obscuring a message so that it cannot be understood by anyone except the intended recipient. Confidentiality keeps information secret from those who are not authorized to have it. 
    **integrity**: hash functions and digital signatures can provide integrity services that allow a recipient to verify that a message has not been altered by malice or error. These include simple message integrity controls. Any changes, deliberate or accidental, will result in the two results (by sender and by recipient) being different.
    **保密性**： 加密技术通过隐藏或掩盖信息来提供保密性，使除预定接收者之外的任何人都无法理解。机密性使信息不被未经授权的人知晓。
    **完整性**：哈希函数和数字签名可提供完整性服务，使收件人能够确认信息未被恶意或错误篡改。这包括简单的信息完整性控制。任何有意或无意的改动都会导致两种结果（发件人和收件人）不同。
    
## Module 2: Understand System Hardening
## 模块 2：了解系统加固
Domain D5.2.1

### Configuration Management Overview
### 配置管理概述

**Configuration management** is a process and discipline used **to ensure that the only changes made to a system are those that have been authorized and validated**. It is both a decision-making process and a set of control processes. If we look closer at this definition, the basic configuration management process includes components such as **identification**, **baselines**, **updates** and **patches**.
**配置管理**是一种流程和规范，用于**确保对系统所做的更改只能是经过授权和验证的更改**。它既是一个决策过程，也是一套控制过程。如果我们仔细研究这个定义，基本的配置管理流程包括**识别**、**基准**、**更新**和**补丁**等组成部分。

* Configuration Management
    1. **Identification**: baseline identification of a system and all its components, interfaces and documentation.
    2. **Baseline**: a security baseline is a minimum level of protection that can be used as a reference point. Baselines provide a way to ensure that updates to technology and architectures are subjected to the minimum understood and acceptable level of security requirements.
    3. **Change Control**: An update process for requesting changes to a baseline, by means of making changes to one or more components in that baseline. A review and approval process for all changes. This includes updates and patches.
    4. **Verification & Audit**: A regression and validation process, which may involve testing and analysis, to verify that nothing in the system was broken by a newly applied set of changes. An audit process can validate that the currently in-use baseline matches the sum total of its initial baseline plus all approved changes applied in sequence.
* 配置管理
    1. **识别**：系统及其所有组件、接口和文件的基准识别。
    2. **基线**：安全基线是可用作参考点的最低保护级别。基线提供了一种方法，可确保技术和架构的更新符合可理解和可接受的最低安全要求水平。
    3. **变更控制**： 通过对基线中的一个或多个组件进行更改，请求更改基线的更新流程。对所有更改进行审查和批准的流程。这包括更新和补丁。
    4. **验证与审计**： 回归和验证流程，可能涉及测试和分析，以验证系统中没有任何东西被新应用的变更所破坏。审计流程可验证当前正在使用的基线与其初始基线加上所有经批准依次应用的变更的总和相匹配。

**Effective use of configuration management gives** systems owners, operators, support teams and security professionals another important set of tools they can use to monitor and oversee the configuration of the devices, networks, applications and projects of the organization.An organization may mandate the configuration of equipment **through standards and baselines**. The use of **standards and baselines can ensure that network devices, software, hardware and endpoint devices are configured in a consistent way and that all such devices are compliant with the security baseline established for the organization**. If a device is found that is not compliant with the security baseline, it may be **disabled or isolated into a quarantine area** until it can be **checked and updated**.
**有效使用配置管理为**系统所有者、操作员、支持团队和安全专业人员提供了另一套重要工具，他们可以利用这些工具监控和监督组织的设备、网络、应用程序和项目的配置。使用**标准和基线可以确保网络设备、软件、硬件和终端设备以一致的方式进行配置，并确保所有这些设备都符合为组织**制定的安全基线。如果发现不符合安全基线的设备，可将其**禁用或隔离到隔离区**，直到可以**检查和更新**。

* **Inventory**: Making an inventory, catalog or registry of all the information assets **is the first step in any asset management process**. **You can’t protect what you don’t know you have**.
  ** 清单**： 编制所有信息资产的清单、目录或注册表**是任何资产管理过程的第一步**。**你无法保护你不知道你拥有的**。


* **Baselines**: The baseline **is a total inventory of all the system’s components, hardware, software, data, administrative controls, documentation and user instructions**. **All further comparisons and development are measured against the baselines.** **When protecting assets, baselines can be particularly helpful in achieving a minimal protection level of those assets based on value.** If classifications such as high, medium and low are being used, baselines could be developed for each of our classifications and provide that minimum level of security required for each.
* 基线**： 基线**是系统所有组件、硬件、软件、数据、管理控制、文档和用户说明的总清单**。**在保护资产时，基线尤其有助于根据资产的价值达到最低的保护级别。**如果使用高、中、低等分类，则可为我们的每种分类制定基线，并为每种分类提供所需的最低安全级别。

* Updates: Such modifications **must be acceptance tested to verify that newly installed (or repaired) functionality works as required**. They must also be **regression tested to verify that the modifications did not introduce other erroneous or unexpected behaviors** in the system. **Ongoing security assessment and evaluation testing evaluates whether the same system that passed acceptance testing is still secure**.
 * 更新： 此类修改**必须经过验收测试，以验证新安装（或修复）的功能是否按要求运行**。还必须进行 ** 回归测试，以验证修改未在系统中引入其他错误或意外行为**。**持续的安全评估和评价测试评估通过验收测试的同一系统是否仍然安全**。 

* Patches: **The challenge for the security professional is maintaining all patches**. **Some patches are critical and should be deployed quickly, while others may not be as critical but should still be deployed because subsequent patches may be dependent on them**. Standards such as the **PCI DSS require organizations to deploy security patches within a certain time frame**. **An organization should test the patch before rolling it out across the organization**. If the patch does not work or has unacceptable effects, it might be necessary to **roll back to a previous (pre-patch) state**. Typically, **the criteria for rollback are previously documented and would automatically be performed when the rollback criteria were met**. The risk of using unattended patching should be weighed against the risk of having unpatched systems in the organization’s network. Unattended (or automated) patching might result in unscheduled outages as production systems are taken offline or rebooted as part of the patch process.
* 补丁： **安全专业人员面临的挑战是维护所有补丁**。**有些补丁非常重要，应迅速部署，而有些补丁可能不那么重要，但仍应部署，因为后续补丁可能依赖于这些补丁**。PCI DSS 等标准要求企业在一定时间内部署安全补丁**。**组织应先测试修补程序，然后再在组织内推广**。如果补丁不起作用或产生不可接受的影响，可能需要**回滚到以前（补丁前）的状态**。通常情况下，**回滚的标准都已记录在案，并会在满足回滚标准时自动执行**。使用无人值守补丁程序的风险应与组织网络中未打补丁系统的风险进行权衡。无人值守（或自动）补丁程序可能会导致计划外停机，因为作为补丁程序的一部分，生产系统要离线或重启。
  
## Module 3: Understand Best Practice Security Policies
## 模块 3：了解最佳实践安全政策

Domain D5.3, D5.3.1, D5.3.2, D5.3.3, D5.3.4, D5.3.5, D5.3.6

An organization’s security policies define what “security” means to that organization, which in almost all cases reflects the tradeoff between security, operability, affordability and potential risk impacts. Security policies express or impose behavioral or other constraints on the system and its use. Well-designed systems operating within these constraints should reduce the potential of security breaches to an acceptable level. 
一个组织的安全策略定义了 "安全 "对该组织的意义，几乎在所有情况下都反映了安全、可操作性、可负担性和潜在风险影响之间的权衡。安全策略表达或施加了对系统及其使用的行为或其他限制。在这些限制条件下运行的设计良好的系统应能将潜在的安全漏洞降低到可接受的水平。

Security governance that does not align properly with organizational goals can lead to implementation of security policies and decisions that unnecessarily inhibit productivity, impose undue costs and hinder strategic intent.
安全治理如果不能与组织目标保持一致，就会导致实施的安全政策和决策不必要地抑制生产力，造成不必要的成本，并阻碍战略意图的实现。

### Common Security Policies
#### 共同安全政策

All policies must support any regulatory and contractual obligations of the organization.  Sometimes it can be challenging to ensure the policy encompasses all requirements while remaining simple enough for users to understand. 
所有政策都必须支持组织的任何监管和合同义务。 有时，既要确保政策包含所有要求，又要简单明了，便于用户理解，这很有挑战性。

Here are six common security-related policies that exist in most organizations.
以下是大多数组织中常见的六种安全相关政策。

* Data Handling Policy: Appropriate use of data: This aspect of the policy defines whether data is for use within the company, is restricted for use by only certain roles or can be made public to anyone outside the organization. In addition, some data has associated legal usage definitions. The organization’s policy should spell out any such restrictions or refer to the legal definitions as required. Proper data classification also helps the organization comply with pertinent laws and regulations. For example, classifying credit card data as confidential can help ensure compliance with the PCI DSS. One of the requirements of this standard is to encrypt credit card information. Data owners who correctly defined the encryption aspect of their organization’s data classification policy will require that the data be encrypted according to the specifications defined in this standard. 
* 数据处理政策： 适当使用数据： 这方面的政策定义了数据是供公司内部使用，还是仅限于某些角色使用，或者可以向组织外的任何人公开。此外，有些数据还有相关的法律使用定义。组织的政策应阐明任何此类限制，或根据需要参考法律定义。正确的数据分类还有助于组织遵守相关法律法规。例如，将信用卡数据列为机密数据有助于确保遵守 PCI DSS。该标准的要求之一是对信用卡信息进行加密。正确定义了组织数据分类政策加密方面的数据所有者将要求按照该标准中定义的规范对数据进行加密。
  
* Password Policy: Every organization should have a password policy in place that defines expectations of systems and users. The password policy should describe senior leadership's commitment to ensuring secure access to data, outline any standards that the organization has selected for password formulation, and identify who is designated to enforce and validate the policy. 
* 密码政策： 每个组织都应制定密码政策，明确对系统和用户的期望。密码政策应说明高层领导对确保安全访问数据的承诺，概述组织为制定密码而选择的任何标准，并确定指定由谁执行和验证该政策。
  
* Acceptable Use Policy (AUP): The acceptable use policy (AUP) defines acceptable use of the organization’s network and computer systems and can help protect the organization from legal action. It should detail the appropriate and approved usage of the organization’s assets, including the IT environment, devices and data. Each employee (or anyone having access to the organization’s assets) should be required to sign a copy of the AUP, preferably in the presence of another employee of the organization, and both parties should keep a copy of the signed AUP. 
* 可接受使用政策（AUP）： 可接受使用政策 (AUP) 规定了组织网络和计算机系统的可接受使用方式，有助于保护组织免受法律诉讼。它应详细说明组织资产（包括 IT 环境、设备和数据）的适当和经批准的用途。应要求每名员工（或任何可以访问组织资产的人）签署一份可接受使用政策，最好是在组织另一名员工在场的情况下签署，双方都应保留一份已签署的可接受使用政策副本。
  
Policy aspects commonly included in AUPs: Data access, System access, Data disclosure, Passwords, Data retention, Internet usage, Company device usage
AUP通常包括的政策方面： 数据访问、系统访问、数据披露、密码、数据保留、互联网使用、公司设备使用

* Bring Your Own Device (BYOD): An organization may allow workers to acquire equipment of their choosing and use personally owned equipment for business (and personal) use. This is sometimes called bring your own device (BYOD). Another option is to present the teleworker or employee with a list of approved equipment and require the employee to select one of the products on the trusted list. 
* 自带设备（BYOD）： 企业可以允许员工购买自己选择的设备，并将个人拥有的设备用于业务（和个人）用途。这有时被称为自带设备（BYOD）。另一种方法是向远程办公人员或员工提供一份经批准的设备清单，并要求员工从可信清单中选择一种产品。
  
Letting employees choose the device that is most comfortable for them may be good for employee morale, but it presents additional challenges for the security professional because it means the organization loses some control over standardization and privacy. If employees are allowed to use their phones and laptops for both personal and business use, this can pose a challenge if, for example, the device has to be examined for a forensic audit. It can be hard to ensure that the device is configured securely and does not have any backdoors or other vulnerabilities that could be used to access organizational data or systems. 
让员工选择最适合自己的设备可能有利于提高员工士气，但这也给安全专业人员带来了额外的挑战，因为这意味着组织失去了对标准化和隐私的一些控制。如果允许员工将手机和笔记本电脑用于个人和业务用途，那么在需要对设备进行取证审计等情况下，就会带来挑战。很难确保设备配置安全，没有任何后门或其他可用于访问组织数据或系统的漏洞。

All employees must read and agree to adhere to this policy before any access to the systems, network and/or data is allowed. If and when the workforce grows, so too will the problems with BYOD. Certainly, the appropriate tools are going to be necessary to manage the use of and security around BYOD devices and usage. The organization needs to establish clear user expectations and set the appropriate business rules. 
在允许访问系统、网络和/或数据之前，所有员工必须阅读并同意遵守本政策。如果员工人数增加，BYOD 的问题也会随之增加。当然，管理 BYOD 设备的使用和使用安全需要适当的工具。组织需要建立明确的用户期望并制定适当的业务规则。

* Privacy Policy: Often, personnel have access to personally identifiable information (PII) (also referred to as electronic protected health information [ePHI] in the health industry). It is imperative that the organization documents that the personnel understand and acknowledge the organization’s policies and procedures for handling of that type of information and are made aware of the legal repercussions of handling such sensitive data. This type of documentation is similar to the AUP but is specific to privacy-related data. 
* 隐私政策： 员工通常可以接触到个人身份信息 (PII)（在卫生行业也称为受保护的电子健康信息 [ePHI]）。组织必须提供文件，说明员工了解并承认组织处理此类信息的政策和程序，并了解处理此类敏感数据的法律后果。这类文件与 AUP 类似，但专门针对与隐私相关的数据。
  
The organization’s privacy policy should stipulate which information is considered PII/ePHI, the appropriate handling procedures and mechanisms used by the organization, how the user is expected to perform in accordance with the stated policy and procedures, any enforcement mechanisms and punitive measures for failure to comply as well as references to applicable regulations and legislation to which the organization is subject. This can include national and international laws, such as the GDPR in the EU and Personal Information Protection and Electronic Documents Act (PIPEDA) in Canada; laws for specific industries in certain countries such as HIPAA and Gramm–Leach–Bliley Act (GLBA); or local laws in which the organization operates. 
组织的隐私政策应规定哪些信息被视为 PII/ePHI、组织使用的适当处理程序和机制、用户应如何按照规定的政策和程序执行、任何执行机制和对未遵守规定的惩罚措施，以及组织应遵守的适用法规和法律。这可能包括国家和国际法律，如欧盟的《全球信息权法案》（GDPR）和加拿大的《个人信息保护和电子文档法案》（PIPEDA）；某些国家的特定行业法律，如《HIPAA》和《Gramm-Leach-Bliley 法案》（GLBA）；或组织运营所在的当地法律。

The organization should also create a public document that explains how private information is used, both internally and externally. For example, it may be required that a medical provider present patients with a description of how the provider will protect their information (or a reference to where they can find this description, such as the provider’s website). 
组织还应创建一份公开文件，解释内部和外部如何使用私人信息。例如，可以要求医疗服务提供者向患者说明医疗服务提供者将如何保护他们的信息（或提及他们可以在哪里找到该说明，如医疗服务提供者的网站）。

* Change Management Policy: Change management is the discipline of transitioning from the current state to a future state. It consists of three major activities: deciding to change, making the change, and confirming that the change has been correctly accomplished. Change management focuses on making the decision to change and results in the approvals to systems support teams, developers and end users to start making the directed alterations.  
变革管理政策： 变革管理是从当前状态过渡到未来状态的一门学科。它包括三项主要活动：决定变革、进行变革和确认变革已正确完成。变更管理的重点是做出变更决定，并批准系统支持团队、开发人员和最终用户开始进行指导性变更。

Throughout the system life cycle, changes made to the system, its individual components and its operating environment all have the capability to introduce new vulnerabilities and thus undermine the security of the enterprise. Change management requires a process to implement the necessary changes so they do not adversely affect business operations. 
在整个系统生命周期中，对系统、其各个组件及其运行环境所做的更改都有可能引入新的漏洞，从而破坏企业的安全。变更管理需要一个程序来实施必要的变更，使其不会对业务运营产生不利影响。

### Common Security Policies Deeper Dive
###常见安全策略深入探讨

Policies will be set according to the needs of the organization and its vision and mission. Each of these policies should have a penalty or a consequence attached in case of noncompliance. The first time may be a warning; the next might be a forced leave of absence or suspension without pay, and a critical violation could even result in an employee’s termination. All of this should be outlined clearly during onboarding, particularly for information security personnel. It should be made clear who is responsible for enforcing these policies, and the employee must sign off on them and have documentation saying they have done so. This process could even include a few questions in a survey or quiz to confirm that the employees truly understand the policy. These policies are part of the baseline security posture of any organization. Any security or data handling procedures should be backed up by the appropriate policies. 
将根据组织的需要及其愿景和使命制定政策。每项政策都应规定违反政策的惩罚或后果。第一次可能是警告，下一次可能是强制休假或停薪留职，严重违规甚至可能导致员工被解雇。所有这些都应在入职培训中明确概述，尤其是对信息安全人员。应该明确由谁负责执行这些政策，员工必须签字确认，并有文件证明他们已经这样做了。这一过程甚至可以包括调查或测验中的几个问题，以确认员工真正理解了这些政策。这些政策是任何组织基线安全态势的一部分。任何安全或数据处理程序都应得到相应政策的支持。

### Change Management Components
#### 变革管理组件
The change management process includes the following components.
变革管理流程包括以下组成部分。

Documentation: All of the major change management practices address a common set of core activities that start with a request for change (RFC) and move through various development and test stages until the change is released to the end users. From first to last, each step is subject to some form of formalized management and decision-making; each step produces accounting or log entries to document its results. 

Approval: These processes typically include: Evaluating the RFCs for completeness, Assignment to the proper change authorization process based on risk and organizational practices, Stakeholder reviews, resource identification and allocation, Appropriate approvals or rejections, and Documentation of approval or rejection.

Rollback: Depending upon the nature of the change, a variety of activities may need to be completed. These generally include: Scheduling the change, Testing the change, Verifying the rollback procedures, Implementing the change, Evaluating the change for proper and effective operation, and Documenting the change in the production environment. Rollback authority would generally be defined in the rollback plan, which might be immediate or scheduled as a subsequent change if monitoring of the change suggests inadequate performance.

## Module 4: Understand Security Awareness Training

Domain D5.4, D5.4.1, D5.4.2, D5.3.2 

**To reduce the effectiveness of certain types of attacks** (such as social engineering), it is crucial that the organization informs its **employees and staff** **how to recognize security problems and how to operate in a secure manner**. While the specifics of secure operation differ in each organization, there are some general concepts that are applicable to all such programs. 

### Purpose

The purpose of awareness training is to make sure everyone knows what is expected of them, based on responsibilities and accountabilities, and to find out if there is any carelessness or complacency that may pose a risk to the organization. We will be able to align the information security goals with the organization’s missions and vision and have a better sense of what the environment is. 

### What is Security Awareness Training?

Let’s start with a clear understanding of the **three different types of learning activities that organizations use**, whether for information security or for any other purpose:

* **Education**: The overall goal of education is to help learners **improve their understanding of these ideas and their ability to relate them to their own experiences and apply that learning in useful ways**.

* **Training**: Focuses on **building proficiency in a specific set of skills or actions**, including sharpening the perception and judgment needed to make decisions as to which skill to use, when to use it and how to apply it. **Training can focus on low-level skills, an entire task or complex workflows consisting of many tasks**.

* **Awareness**: These are activities that attract and engage the learner’s attention by acquainting them with aspects of an issue, concern, problem or need.

You’ll notice that none of these have an expressed or implied degree of formality, location or target audience. (Think of a newly hired senior executive with little or no exposure to the specific compliance needs your organization faces; first, someone has to get their attention and make them aware of the need to understand. The rest can follow.)

### Security Awareness Training Examples

Let’s look at an example of security awareness training by using an organization’s strategy to improve fire safety in the workplace: 

Education may help workers in a secure server room understand the interaction of the various fire and smoke detectors, suppression systems, alarms and their interactions with electrical power, lighting and ventilation systems. 
Training would provide those workers with task-specific, detailed learning about the proper actions each should take in the event of an alarm, a suppression system going off without an alarm, a ventilation system failure or other contingency. This training would build on the learning acquired via the educational activities. 
Awareness activities would include not only posting the appropriate signage, floor or doorway markings, but also other indicators to help workers detect an anomaly, respond to an alarm and take appropriate action. In this case, awareness is a constantly available reminder of what to do when the alarms go off. 

Translating that into an anti-phishing campaign might be done by: 

Education may be used to help select groups of users better understand the ways in which social engineering attacks are conducted and engage those users in creating and testing their own strategies for improving their defensive techniques. 
Training will help users increase their proficiency in recognizing a potential phishing or similar attempt, while also helping them practice the correct responses to such events. Training may include simulated phishing emails sent to users on a network to test their ability to identify a phishing email.
Raising users’ overall awareness of the threat posed by phishing, vishing, SMS phishing (also called “smishing) and other social engineering tactics. Awareness techniques can also alert selected users to new or novel approaches that such attacks might be taking. 
Let’s look at some common risks and why it’s important to include them in your security awareness training programs. 


#### Phishing

The use of phishing attacks to target individuals, entire departments and even companies is a significant threat that the security professional needs to be aware of and be prepared to defend against. Countless variations on the basic phishing attack have been developed in recent years, leading to a variety of attacks that are deployed relentlessly against individuals and networks in a never-ending stream of emails, phone calls, spam, instant messages, videos, file attachments and many other delivery mechanisms.

Phishing attacks that attempt to trick highly placed officials or private individuals with sizable assets into authorizing large fund wire transfers to previously unknown entities are known as whaling attacks .

#### Social Engineering

Social engineering is an important part of any security awareness training program for one very simple reason: bad actors know that it works. For the cyberattackers, social engineering is an inexpensive investment with a potentially very high payoff. Social engineering, applied over time, can extract significant insider knowledge about almost any organization or individual.

One of the most important messages to deliver in a security awareness program is an understanding of the threat of social engineering. People need to be reminded of the threat and types of social engineering so that they can recognize and resist a social engineering attack.

Most social engineering techniques are not new. Many have even been taught as basic fieldcraft for espionage agencies and are part of the repertoire of investigative techniques used by real and fictional police detectives. A short list of the tactics that we see across cyberspace currently includes:

Phone phishing or vishing: Using a rogue interactive voice response (IVR) system to re-create a legitimate-sounding copy of a bank or other institution’s IVR system. The victim is prompted through a phishing email to call in to the “bank” via a provided phone number to verify information such as account numbers, account access codes or a PIN and to confirm answers to security questions, contact information and addresses. A typical vishing system will reject logins continually, ensuring the victim enters PINs or passwords multiple times, often disclosing several different passwords. More advanced systems may be used to transfer the victim to a human posing as a customer service agent for further questioning.

Pretexting: The human equivalent of phishing, where someone impersonates an authority figure or a trusted individual in an attempt to gain access to your login information. The pretexter may claim to be an IT support worker who is supposed to do maintenance or an investigator performing a company audit. Or they might impersonate a coworker, the police, a tax authority or some other seemingly legitimate person. The goal is to gain access to your computer and information.
Quid pro quo: A request for your password or login credentials in exchange for some compensation, such as a “free gift,” a monetary payment or access to an online game or service. If it sounds too good to be true, it probably is.
Tailgating: The practice of following an authorized user into a restricted area or system. The low-tech version of tailgating would occur when a stranger asks you to hold the door open behind you because they forgot their company RFID card. In a more sophisticated version, someone may ask to borrow your phone or laptop to perform a simple action when he or she is actually installing malicious software onto your device.
Social engineering works because it plays on human tendencies. Education, training and awareness work best to counter or defend against social engineering because they help people realize that every person in the organization plays a role in information security.

#### Password Protection

We use many different passwords and systems. Many password managers will store a user’s passwords for them so the user does not have to remember all their passwords for multiple systems. The greatest disadvantage of these solutions is the risk of compromise of the password manager.

These password managers may be protected by a weak password or passphrase chosen by the user and easily compromised. There have been many cases where a person’s private data was stored by a cloud provider but easily accessed by unauthorized persons through password compromise.

Organizations should encourage the use of different passwords for different systems and should provide a recommended password management solution for its users.

Examples of poor password protection that should be avoided are:

Reusing passwords for multiple systems, especially using the same password for business and personal use.
Writing down passwords and leaving them in unsecured areas.
Sharing a password with tech support or a co-worker.




