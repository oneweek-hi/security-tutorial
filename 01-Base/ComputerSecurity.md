# Computer Security

Computer security is the protection of computer systems from theft or damage to their hardware, software or electronic data.

## Vulnerabilities and attacks

A vulnerability is a weakness in design, implementation, operation or internal control. Most of the vulnerabilities that have been discovered are documented in the Common Vulnerabilities and Exposures (CVE) database.

### Backdoor

A backdoor in a computer system, a cryptosystem or an algorithm, is any secret method of bypassing normal authentication or security controls. They may have been added by an authorized party to allow some legitimate access, or by an attacker for malicious reasons; but regardless of the motives for their existence, they create a vulnerability.

### Denial-of-service attacks

Denial of service attacks (DoS) are designed to make a machine or network resource unavailable to its intended users. Attackers can deny service to individual victims, such as by deliberately entering a wrong password enough consecutive times to cause the victims account to be locked, or they may overload the capabilities of a machine or network and block all users at once. 

### Distributed Denial-of-service attacks

(DoS 공격의 한계) While a network attack from a single IP address can be blocked by adding a new firewall rule, many forms of Distributed denial of service (DDoS) attacks are possible, where the attack comes from a large number of points – and defending is much more difficult. Such attacks can originate from the zombie computers of a botnet.

### Eavesdropping

Eavesdropping is the act of surreptitiously listening to a private conversation, typically between hosts on a network. For instance, programs such as Carnivore and NarusInSight have been used by the FBI and NSA to eavesdrop on the systems of internet service providers. Even machines that operate as a closed system can be eavesdropped upon via monitoring the faint electromagnetic transmissions generated by the hardware; TEMPEST is a specification by the NSA referring to these attacks.

- TEMPSET 관련 감동 실화

  > 하드디스크의 연산에 따라서 발생하는 기계음이 달라짐. 그래서 하드디스크의 기계음을 녹음한 후 디코딩 한다면 하드디스크에 어떤 데이터를 쓰고 읽었는지 확인할 수 있음. 폐쇄망에 접근할 수 있는 사람의 스마트폰을 해킹해서 기계음을 녹음한 후 해커의 컴퓨터로 전송한 사례.

- 소리 관련 해킹 감동 실화

  > 사람이 들을 수 없는 고주파를 아이폰 시리는 들을 수 있음. 그래서 "핸드폰에 있는 모든 자료를 해커의 컴퓨터로 전송해줘" 라는 메시지를 고주파로 변환해서 아이폰 유저의 주변에서 그 변환된 음원을 재생함. 그럼 사람은 듣지 못하지만 시리가 아이폰에 있는 데이터들을 해커의 컴퓨터로 전송함.

- 폐쇄망 해킹 관련 감동 실화

  > 이란 핵 시설은 인터넷이 연결되지 않은 폐쇄망이라서 해킹이 불가능함. 하지만 미국과 이스라엘은 이란 핵 시설을 해킹하여 무력화해야 했음. 그래서 먼저 이란 핵 시설 간부들의 컴퓨터를 흔적 없이 해킹하여 컴퓨터에 꽂혀있는 USB 에 악성코드를 입력시킴. 그 이후 간부가 USB 를 핵 시설 폐쇄망 컴퓨터에 꽂았을 때 악성코드가 실행되어 핵 시설이 무력화 되었음. 이 감동 실화가 그 유명한 [스턱스넷 Stuxnet](https://en.wikipedia.org/wiki/Stuxnet) 바이러스이고, 이 하나의 바이러스에 제로데이 취약점 4개가 포함되어 있었음.

### Multi-vector, polymorphic attacks

Surfacing in 2017, a new class of multi-vector, polymorphic cyber threats surfaced that combined several types of attacks and changed form to avoid cyber security controls as they spread. 

According to a blog post, the malware presents itself as randomly generated code designed to look like a legitimate application. The malware comes either protected with a new packer, or the packer itself features advanced polymorphic functionality. 

### Phishing

Phishing is typically carried out by email spoofing or instant messaging, and it often directs users to enter details at a fake website whose look and feel are almost identical to the legitimate one. The fake website often ask for personal information, such as log-in and passwords.

### Privilege escalation

Privilege escalation describes a situation where an attacker with some level of restricted access is able to, without authorization, elevate their privileges or access level. For example, a standard computer user may be able to fool the system into giving them access to restricted data; or even become "root" and have full unrestricted access to a system.

  이게 이제 스티키 비트가 붙어 있는 프로그램을 BOF 같은 걸로 익스플로잇 하면서 얻게 되는 권한상승. 실습을 하면서 해야 함.

### Social engineering

Social engineering aims to convince a user to disclose secrets such as passwords, card numbers, etc. by, for example, impersonating a bank, a contractor, or a customer.

A common scam involves fake CEO emails sent to accounting and finance departments. In early 2016, the FBI reported that the scam has cost US businesses more than $2bn in about two years.

보통 메일 제목 어그로, 링크 제목 어그로에 속아서 클릭하는 순간 악성코드 실행. 또는 프로그램 이름 어그로에 끌려서 실행시키는 형식. 그래서 항상 VirusTotal 에 넣어보고 실행해야 함. 

### Spoofing

Spoofing is the act of masquerading as a valid entity through falsification of data (such as an IP address or username), in order to gain access to information or resources that one is otherwise unauthorized to obtain. There are several types of spoofing, including:

- Email spoofing, where an attacker forges the sending (From, or source) address of an email.

- IP address spoofing, where an attacker alters the source IP address in a network packet to hide their identity or impersonate another computing system.

- MAC spoofing, where an attacker modifies the Media Access Control (MAC) address of their network interface to pose as a valid user on a network.

- Biometric spoofing, where an attacker produces a fake biometric sample to pose as another user.

- ARP 스푸핑, DNS 스푸핑 등등 해가지고 스푸핑 종류 쭉 알아보고 그 중에서 하나정도 실습 

### Tampering

Tampering describes a malicious modification of products. So-called "Evil Maid" attacks and security services planting of surveillance capability into routers are examples.

- 그래서 파일을 다운로드하면 꼭 해쉬값을 체크하라고 권유함. 

- 이걸 이해하려면 해쉬 값과 해쉬 함수에 대해서 간단히 알아봐함. 

- Tampering 관련 실화 

  > 해커가 리눅스 배포판 중 하나인 리눅스 민트 서버를 해킹해서 리눅스 민트 설치 파일에 백도어를 심어서 변조해놓음. 사람들은 리눅스 민트를 컴퓨터에 설치하려고 그 웹 서버에서 설치 파일을 다운 받아서 컴퓨터에 설치함. 리눅스 민트가 잘 작동하기는 하지만 실제로는 백도어가 있음. 이 사건 이후로 다운 받은 파일의 해쉬 값을 체크하는 것에 대한 중요성이 부각됨. 


## System at rist

The growth in the number of computer systems, and the increasing reliance upon them of individuals, businesses, industries and governments means that there are an increasing number of systems at risk.

### Hacking tarkets

- 금융권 

    중앙은행, 일반은행, 결제시스템 등등. 

- 기반시설 

    통신시설, 수력발전소, 원자력발전소, 핵실험시설 등등 이 타겟이 됩니다. 기반시설을 통제하는 시스템은 보통 폐쇄망이지만 스턱스넷 Stuxnet 은 폐쇄망도 해킹될 수 있다는 것을 보여줌. 

  - [빌딩 해킹](https://www.youtube.com/watch?v=0L7DTMKekoU)

  - [파워 그리드 해킹](https://www.youtube.com/watch?v=pL9q2lOZ1Fw#t=28s)

- 항공시설 

    항공 특성상 무선 통신이 많아 해킹에 취약

- 단말기 

    데스크탑, 노트북, 스마트폰, 태블릿 단말기의 개인정보, 계좌 비밀번호를 뺴내가거나 [봇넷 botnet](botnet.md) 으로 만드려는 목적으로 해킹함. 

- 대기업

    기업이 가지고 있는 금융 정보를 뺏으려는 목적으로 해킹. 기업의 데이터베이스에는 수많은 고객들의 신용카드 정보 같은 금융 정보가 들어 있기 때문에. 최근 [메가스터디 해킹](https://www.boannews.com/media/view.asp?idx=80375&kind=).

- 정부시설, 군사시설

    적대 국가가 자신의 사상을 선전하기 위하여 해킹하거나 상대 국가의 기밀을 빼앗는 등의 목적으로 정부 해킹을 함. 신호등 같은 교통 체계를 해킹하거나 경찰 통신 체계, 주민등록번호 데이터베이스를 해킹함. 여권과 개인 등록 정보를 해킹해서 가상의 인물을 만들고 입국 심사를 통과하는 해킹도 있음. 

- 의료시설

    병원도 IT 기술 의존도가 높아졌기 때문에 병원 데이터베이스에 있는 개인 정보를 빼앗기 위해 해킹함. 앞으로 인공지능 의존도도 높아져서 인공지능이 간호사 보다 더 환자를 24시간 잘 돌볼 수 있다는 게 증명되면 인공지능으로 환자를 돌보게 될텐데 만약 인공지능이 해킹 당해서 환자에게 몸에 꽂혀 있는 바늘구멍으로 들어가고 있던 약을 끊어 버릴 수도 있게 됨. 

- 자동차

  - [자율주행차 해킹](https://www.youtube.com/watch?v=BTw_K46T3LQ)

    의료시설 해킹, 자동자 해킹을 통해서 해킹으로 물리적인 피해를 가할 수 있다는 것이 증명 되었음. 사람을 죽일 수도 있겠지? 

-  IoT

    집 문, 에어컨, 가스레인지, 창문에 임베디드 시스템을 설치하고 인터넷에 연결한 후 스마트폰 어플리케이션으로 통제할 수 있게 하니까 너무 편해요. 만약 집 문을 안 잠그고 회사를 갔어. 아니면 가스렌지 열어두고 회사 갔어. 그럼 스마트폰으로 끄면 되는 거야. 근데 문제는 인터넷에 연결되었기 때문에 이걸 해킹할 수도 있게 된거지.

    IoT 해킹을 해서 집 문 열어서 누군가 집 안에 숨어 있는 거야. 아니면 가스렌지 계속 틀어놓은 다음에 전자렌지 과부하 걸리게 하면 불나게 할 수 있지. 

## Computer protection

In computer security a countermeasure is an action, device, procedure, or technique that reduces a threat, a vulnerability, or an attack by eliminating or preventing it, by minimizing the harm it can cause, or by discovering and reporting it so that corrective action can be taken.

Security by design, or alternately secure by design, means that the software has been designed to be secure. Some of the techniques in this approach include:

  - The principle of least privilege, where each part of the system has only the privileges that are needed for its function.

  - Code reviews and unit testing, approaches to make modules more secure where formal correctness proofs are not possible.

  - Full disclosure of all vulnerabilities, to ensure that the "window of vulnerability" is kept as short as possible when bugs are discovered.


## Notable attacks and breaches

### Robert Morris and the first computer worm

  In 1988, only 60,000 computers were connected to the Internet. On 2 November 1988, many started to slow down, because they were running a malicious code that demanded processor time and that spread itself to other computers – the first internet "computer worm".

### Stuxnet

  In 2010 the computer worm known as Stuxnet reportedly ruined almost one-fifth of Iran's nuclear centrifuges. It did so by disrupting industrial programmable logic controllers (PLCs) in a targeted attack. This is generally believed to have been launched by Israel and the United States – although neither has publicly admitted this.

### 3/20 전산대란

  - [위키](https://ko.wikipedia.org/wiki/3%C2%B720_%EC%A0%84%EC%82%B0_%EB%8C%80%EB%9E%80)

  - [나무위키](https://namu.wiki/w/3.20%20%EC%A0%84%EC%82%B0%EB%A7%9D%20%EB%A7%88%EB%B9%84%EC%82%AC%ED%83%9C)

  - [보안뉴스](https://www.boannews.com/media/view.asp?idx=35579)