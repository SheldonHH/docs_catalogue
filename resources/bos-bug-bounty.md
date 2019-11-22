# BOS Bug Bounty

Table of Contents

* [Scope of Business](https://slowmist.io/en/bos/index.html#t1)
* [Processing Flow](https://slowmist.io/en/bos/index.html#t2)
  * [Reporting Stage](https://slowmist.io/en/bos/index.html#t2-1)
  * [Processing Stage](https://slowmist.io/en/bos/index.html#t2-2)
  * [Repairing Stage](https://slowmist.io/en/bos/index.html#t2-3)
* [Vulnerability Level and Reward Standards](https://slowmist.io/en/bos/index.html#t3)
  * [Critical Vulnerabilities](https://slowmist.io/en/bos/index.html#t3-1)
  * [High-risk Vulnerabilities](https://slowmist.io/en/bos/index.html#t3-2)
  * [Medium-risk Vulnerabilities](https://slowmist.io/en/bos/index.html#t3-3)
  * [Low-risk Vulnerabilities](https://slowmist.io/en/bos/index.html#t3-4)

Content

### Scope of Business <a id="t1"></a>

1. It mainly includes the following parts, and the rest of code libraries under the github.com/boscore also accept vulnerability submission.

Main code: [https://github.com/boscore/bos](https://github.com/boscore/bos)

IBC related: [https://github.com/boscore/ibc\_contracts](https://github.com/boscore/ibc_contracts)

System contract code: [https://github.com/boscore/bos.contracts](https://github.com/boscore/bos.contracts)

**2. Limited-time Bounty Program: BOS 3s LIB**

Reward content: BOSCore 3.0.0 version of the batch PBFT consensus code running on the BOS testing net related issues.

Note: all BOS 3s LIB vulnerabilities found on GitHub require a responsible description of the details.

Program Duration:From July 8, 2019 to August 8, 2019

**Bounty: 10,000 BOS - 500,000 BOS**

### Processing Flow <a id="t2"></a>

#### Reporting Stage <a id="t2-1"></a>

The reporter visits "SlowMist Zone" website and goes to "Submit Bug Bounty" \(URL：[https://slowmist.io/en/bug-bounty.html](https://slowmist.io/en/bug-bounty.html)\) to submit a threat intelligence. \(Status: to be review\)

#### Processing Stage <a id="t2-2"></a>

1. Within one working day, the SlowMist Security Team will confirm the threat intelligence report from the "SlowMist Zone", follow up, evaluate the problem, and feed the intelligence back to the BOS Developer Group contact person in the meantime \(status: under review\).

2. Within three working days, the BOS Developer Group technical team will deal with the problem, draw conclusions and record points \(status: confirmed / ignored\). They will communicate with the reporter if necessary, and ask the reporter for assistance.

#### Repairing Stage <a id="t2-3"></a>

1. The BOS Developer Group business department shall repair the security problems in the threat intelligence and update online \(status: repaired\). The repairing timeframe depends on the problem severity and the repair difficulty. Generally speaking, it is within 24 hours for the critical and high-risk problems, within 3 working days for the medium-risk problems, and within 7 working days for the low-risk problems. The App security issue is limited by the version release, and the repairing timeframe is on a case-by-case basis.

2. The reporter will review whether the security problem has been repaired \(Status: reviewed/reviewed with objection\).

3. After the reporter confirms that the security problem is repaired, the BOS Developer Group technical team will inform the SlowMist Security Team of the conclusion and the vulnerability score. They will issue rewards with the SlowMist Security Team \(status: completed\).

### Vulnerability Level and Reward Standards <a id="t3"></a>

| Level | BOS Reward\* | SlowMist Zone Reward\* |
| :--- | :--- | :--- |
| Critical | 50,000 BOS | 512 SLOWMIST |
| High | 20,000 BOS | 256 SLOWMIST |
| Medium | 8,000 BOS | 100 SLOWMIST |
| Low | 3,000 BOS | 32 SLOWMIST |

\*Remark: the final award depends on the severity of the vulnerability and the true impact of the vulnerability, the values in the table are the highest rewards for each level.

\*SLOWMIST is Ethereum ERC20 Token, the ecological incentive token for the SlowMist Zone.

#### Critical Vulnerabilities <a id="t3-1"></a>

A critical vulnerability refers to the vulnerability occurs at the bottom of the blockchain, including key codes such as nodes and system contracts, and have a large impact on the infrastructure of the whole chain.

It is including but not limited to:

* Can cause the large area node crash or function failure.
* Can get the root permission.
* System contracts' security vulnerability.
* Smart contract overflow, conditional competition vulnerability, double spend and consensus layer vulnerability.

#### High-risk Vulnerabilities <a id="t3-2"></a>

* Vulnerabilities and defects that cause user can not operate.
* Cause system crash in specify condition.

#### Medium-risk Vulnerabilities <a id="t3-3"></a>

* Leak of sensitive information in specify condition.
* Small scale system contract security vulnerabilities.

#### Low-risk Vulnerabilities <a id="t3-4"></a>

* Slight leak of sensitive information.
* Hard to use,but there still exist security vulnerabity.
* Email Spoofing / Missing SPF Record.

#### Vulnerabilities that are not accepted at the moment \(even if such a vulnerability is submitted, it will be ignored\) <a id="t3-4"></a>

* User enumeration vulnerability.
* Self-XSS
* CSRF issues for non-sensitive operations.
* A separate issue about Android app android:allowBackup=”true” , and the service is denied locally, etc. \(unless in-depth use\).
* Some problems such as changing the size of the image and causing slow requests, etc.
* Version leak issues such as Nginx/Tomcat, etc.
* Some functional bugs that do not pose a security risk issue.

Special thanks to The xianzhi vulnerability classification criteria referred here.

