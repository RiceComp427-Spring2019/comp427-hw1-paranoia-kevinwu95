# <img src="http://www.rice.edu/_images/rice-logo.jpg" width=180> Comp427, Spring 2018, Homework 1
## Rational Paranoia
The homework specifications, as well as the corresponding course slide decks,
can be found on the [Comp427 Piazza](https://piazza.com/class/jqifhp864b37ju).
This assignment is due **Thursday, January 17 at 6 p.m.**

You will do this homework by editing the _README.md_ file. It's in
[MarkDown format](https://guides.github.com/features/mastering-markdown/)
and will be rendered to beautiful HTML when you visit your GitHub repo.

## Student Information
Please also edit _README.md_ and replace your instructor's name and NetID with your own:

_Student name_: Kaiwen Wu

_Student NetID_: kw34

Your NetID is typically your initials and a numeric digit. That's
what we need here.

_If you contacted us in advance and we approved a late submission,
please cut-and-paste the text from that email here._

## Problem 1
- Scenario: TSA
- Assumptions:
  In this scenario, we are making the assumption that the attackers’ goals (intents) can be 
  - causing damage to property integrity and personal safety in the airport on during flight, disrupting regular airport
    service, gaining airport and passengers’ confidential information. 
  - Also, we also assume that there will be a large number of passengers going through security screening every day. 
  - Since the scenario is for security screening process, we have to assume that the adversary cannot bring in anything 
    from entrances other than the checkpoints to initialize the attack.
  - Also, we can only have countermeasures at the checkpoints. The other airport subsystems' security measures are out 
    of our hand. 
- Assets:
  The assets we are considering can be the following. 
  - We need to consider the safety of the people within the airport and during the flight because the adversaries can 
    try to harm the people involved due to their political statement or anti-social personalities. 
  - The integrity and availability of services provided by the airport are also our assets because it is the primary 
    function the airport. 
  - Also, we need to consider the integrity of the physical properties as well because the adversaries can also try to 
    damage the physical properties of the airport and airlines. 
  - The confidential information of the airport personnel and passengers is also our assets because the adversary can 
    also aim to acquire these for further exploits. 
- Threats:
  The threats we need to consider can be the following. 
  - The adversaries can launch attacks like vandalism targeting physical properties of the airports and airlines. 
  - They can also launch attacks like poisoning to target personal safety in the airport and planes. 
  - Also, the adversaries can launch forms of denial-of-service attacks like having bomb-like objects placed in multiple
    places to cause disturbances and panics such that regular airport services can be delayed or denied. 
  - Furthermore, the adversaries can also aim to acquire confidential information about the airport, the airlines, 
    the personnel, and the passengers by hacking airport system for further exploits. 
  - Also, the adversaries can also try to create a backdoor, either physical like an actual door or conceptual like a 
    bribed employee, inside the airport so that further attacks can be carried through using it. 
  - In addition, the adversaries can also try to bypass our security screening by providing forged identification or 
    having compromised security personnel.  
  - The worst of all, is to have adversaries capable of carrying out ad-hoc attacks on the spot using materials and 
    instruments accessible within the airport and airplane. 
  These are all threats that the checkpoint screening must consider.
- Countermeasures:
  In terms of countermeasures, screening is our primary method. There are several form of screening processes trying to 
  address these threats. 
  - First of all, we can use identification documents, like photo IDs, to identify known adversaries. This can partially
    prevent threats, especially those that does not require bringing instruments through the checkpoints. For example, 
    this should increase the chance to spot people who intent to bribe airport personnel to create a backdoor, to hack 
    into the airport system to acquire confidential information, or to carry through any kind of ad-hoc attacks on the 
    spots using materials within the airport or airplanes. Since we only care about the checkpoint, the security of other
    subsystem in the airport is not our business, like having better WiFi security and airport electronic system security.
  - The second screening process is to screen personal belongings that they try to bring into the airport. This can 
    prevent attacks that requires special materials or instruments like weapons, explosives, and hazardous materials. 
    This can be done using the current x-ray machine to scan any personal belongings and even one’s entire body in case 
    the adversaries are trying to hide them. 
  - Speaking of backdoor, the adversaries can also try to bride, or simply plant the security personnel at the 
    checkpoints; therefore, we also need to do background check to the security personnel and train them not to take 
    bribe. We can also have a system for personnel to monitor each other with certain incentive so that it is harder and
    more costly for the adversaries to compromise security measures themselves. Also, we should closely monitor 
    disgruntled employees.  

## Problem 2
- Scenario: Documents
- Assumptions:
  - We have to assume that one document can be physical, digital, or both. We often think about the security of the 
    digital system, but the security of the physical copies of these documents are as important as the digital version. 
  - Also, we need to assume that the inlet and outlet channels of these documents in and out of our company are secure, 
    otherwise we have no way to prevent leaking at the first place. There is nothing we can do if a document is stolen 
    by an USPS employee (There is no way we can do hand delivery for all documents). 
  - Also, we need to only worry about the security of our subsystem. It would be too much to think about if we consider 
    all other subsystems that would cause correlated failures with us. It is a hard enough of a problem concerning 
    induced independent failure in our system by the adversary. Also, if the adversaries were to compromise our security 
    measures by inducing correlated failure through bringing down other dependent subsystems, it might be too costly for 
    them to carry through. For example, breaking into the neighboring building's basement and dig a tunnel into our vault.
- Assets:
  Our assets will be the following. 
  - We need to consider the confidentiality of our documents because it is the very nature of these documents. 
  - Also, we need to consider the integrity of these documents because they cannot be doctored or stolen. 
  - Furthermore, the availability of these documents is also our assets because we need to access them as needed due to
    the very nature of legal service we provide. 
  - In addition, the information of what documents we have and where we store (save) them (our document catalog and 
    directory) is also our asset because simply knowing what we have or what we don’t have is very essential information,
    especially for court cases. (meta-information)
- Threats:
  There are several threats we are facing. 
  - First of all, the adversaries will try to pose threats to our assets by hacking into our digital system. 
    For example, they can read, write, and delete our documents if they have complete access to our digital system. 
  - Secondly, the adversaries will also try to gain access to our building, server, and storage to threaten the security
    of our assets. The simplest example is to break in our archive room and do anything they want with the documents 
    inside. 
  - In addition, the adversaries can also bribe, trick, or social-engineer our employees into giving them ways to pose threats to our 
    assets. For example, they can pay our employees to copy, tamper, or destroy certain document that they knew that 
    we have as they learned it from our compromised staffs. Or they can pretend to be our customer to trick our 
    employees into giving them the documents. Better yet, they can send emails to trick employees into giving up their 
    internal account credentials.
- Countermeasures:
  Our countermeasures need to address all those threats mentioned above. 
  - First of all, having secured authentication systems for both the digital and physical documents is very important. 
    This aims to prevent hacking into our digital physical archives. 
  - We also need to have a security system like CCTV and a team of trained security personnel to prevent force entry 
    and stealthy break in to our archive. 
  - The most important countermeasure is to train our employees so that they are resistant to bribe, trickery, and 
    social-engineering. Also, they need to sign non-disclosure agreement because it raise the cost to violate the 
    confidentiality and integrity measures. 
  - An extra note would be to choose our security and system providers carefully. Extensive background check is needed 
    and make sure that there exists a fail-safe mechanism so that any failures will trigger a response to stop any kind
    potential access that can cause those threats to our assets. 

## Problem 3
- Scenario: Your choice (give a brief explanation)
- Assumptions:
  - explain_your_assumptions
- Assets:
  - explanatory_paragraph
  - explanatory_paragraph ...
- Threats:
  - explanatory_paragraph 
  - explanatory_paragraph ...
- Countermeasures:
  - explanatory_paragraph
  - explanatory_paragraph ...

