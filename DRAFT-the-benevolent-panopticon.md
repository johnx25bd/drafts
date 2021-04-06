# The Benevolent Panopticon

_Subverting the privacy-security trade-off with 21st century information technologies_

In the 18th century Jeremy Bentham conceived of a structure designed in such a way that a single observer could simultaneously supervise each occupant. In Bentham’s “panopticon” security would be enhanced, both because the central observer could detect and disrupt misbehavior, and because the observed would be less likely to break the rules if they knew they were being watched.

Bentham’s thought experiment holds particular relevance as we construct and deploy a network of connected sensors into every corner of the world. Such connected sensors — including IoT devices, but moreso computers and smartphones — observe their surroundings, and can record and transmit information. Through these digital periscopes observers can peer intimately into the lives of a growing proportion of the global population, as well as into the operations of enterprises, governments and militaries. Edward Snowden’s revelations suggest that not only is a truly global panopticon possible — it has been built.

While the extent and character of the NSA’s surveillance apparatus is deeply troubling, the motives behind the decision to build it are not. It is a right and noble aim, to protect lives, health and property. Conventional wisdom suggests that here a human’s right to security sits in tension with their right to privacy — that an inherent trade-off exists between the two and that to improve security, privacy must be sacrificed. This is built on the assumption that the state (or similar authority) must attain knowledge of potential harm in order to impede the violent actor in carrying out that harm.

I accept that agents — conscious, infectious, or otherwise — with a harmful intent will exist in any population, and that coordinated intervention by some authority can mitigate the extent of the harm caused. In the 21st century, however, it appears that a benevolent panopticon could be built. A surveillance apparatus that optimizes both for public security and individual privacy is possible.

## The Watcher

The primary ethical question with the panopticon is, of course, who is entitled to sit at its center? Who is chosen to see all?

If the guardian sitting in the panopticon’s central observation room is incorruptible, then the security benefits of such a system may be justifiable. History, of course, tells us that no authority is incorruptible, and even less so a centralized authority.

Knowledge is, after all, power. Knowledge is distilled from information within a mind, and, fundamentally, a panopticon is a system in which all information is funneled into one mind. The one who sits at the panopticon’s point of informational convergence is thus in a position of power. The all knowing watcher has the power to detect and disrupt malicious behavior, as well as the power to abuse their knowledge to the detriment of the subjects observed.

When subjects are prisoners (individuals who have foregone their rights by breaking a law), the violation of their privacy may be ethical. However, when subjects are law abiding citizens, such surveillance is categorically unethical. Even less so when the occupant of the observation room is a commercial entity.

## What Bentham could not have foreseen

Jeremy Bentham drew up designs for the panopticon over a century before Charles Babbage conceived of his “analytical engine.” In the time since these men lived and died — as Babbage foresaw — non-human entities that are both aware and able to communicate have emerged.

Modern computers perceive their environments, through camera, microphone, keyboard, antenna or ethernet cable. They then process their perceptions, and act in response. What’s more, their actions occur in a logical space governed by transparent and objective laws, which can be understood by anyone. Operating systems and programs can be read, dissected and disputed. Algorithms and protocols can exist independent of any individual human developer, collectively governed by an open community.

So — the question naturally arises: could a computer sit at the center of the panopticon? Could a algorithms watch over us, only intervening when some threat to security is discerned? And could such an informational agent respect the privacy of the subjects of observation?

I am increasingly convinced that the answer is yes.

With properly-designed systems at the point of informational convergence of the global panopticon, we can preserve each human’s right to privacy without sacrificing the potential gains to security afforded in the digital age.

Of course, a computer is only as trustworthy as its programmers. So how do we ensure that malicious developers and hardware engineers don’t let themselves in to the panopticon’s control room to peek into everyone’s the cells — or cell phones?

## Privacy-preserving surveillance techniques

Numerous approaches to surveillance are emerging that protect the privacy of the surveilled. This is by no means an exhaustive review. Instead, it is intended to subvert the idea of a tradeoff existing between privacy and security.

### Edge Computing

Smartphones and laptops are powerful computers in their own right, and the interface between private citizens and the Internet. Many situations that require surveillance and intervention for the public good can be addressed on the edge device itself, with personal data never having to leave a user’s phone.

In response to the COVID-19 epidemic, the Singaporean government released TraceTogether, a mobile application designed to aid in contact tracing. The theory is that by keeping track of physical interactions amongst humans, when someone is diagnosed with the novel coronavirus their close contacts could be notified and told to self-isolate — reducing transmission rates while minimizing the need for blanket lockdowns.

The app requires Bluetooth to be enabled. Smartphones connect with nearby phones, collecting unique identifiers. If a user is diagnosed, notifications are sent to the users who had extended contact with the diagnosed patient.

By designing applications with an eye toward maintaining users’ privacy, and leveraging the computational and data storage capabilities of mobile and IoT devices, edge computing can do much to leverage the potential our connected sensors networks afford to improve public health and security — without sacrificing individual right to choose privacy.

(Note: [soon](https://www.theguardian.com/uk-news/2020/mar/31/nhs-developing-app-to-trace-close-contacts-of-coronavirus-carriers) the United Kingdom's National Health Service is releasing a similar contact tracing app.)

### Enclave Computing

Computers operate on symbols representing informational units — bits — within an execution environment. Algorithms detect patterns in binary sequences (which can represent text, images, audio, etc), and adapt their actions accordingly. Edge devices are often constrained by storage, bandwidth and memory — sometimes it is necessary to analyze datasets that may contain a signal indicating a threat to public safety on central servers.

A drawback to traditional execution environments is that the data being analyzed can be viewed by other programs within the operating system. Thus, the controller of the computer can theoretically access all information processed — a potentially unacceptable violation of privacy. And a truly benevolent panopticon must be incorruptible.

Secure enclaves are execution environments that provide “confidentiality, integrity and attestation”. Within a secure enclave, information processes remains private — “an adversary outside of the enclave cannot inspect the state of execution inside the enclave”. Algorithms run exactly as intended, and enclaves can provide “an unforgeable proof that enables a remote party to verify what has run inside the enclave even if they don’t have physical access to the machine.” ([Oasis / Keystone](https://medium.com/oasislabs/towards-an-open-source-secure-enclave-659ac27b871a))

Put another way, enclaves enable secure computation on private information _without revealing the information to … anyone_. Furthermore, secure enclaves can have the computing, storage and connectivity resources required for advanced analytics and machine learning applications. In instances where edge devices do not have the computational power, or access to information, required for a certain analytical task, secure enclaves could analyze personal private data without violating the data subjects’ privacy. Again, only if threats to public health or security are detected, the enclave would expose necessary information to appropriate human actors authorized to intervene.

### Zero knowledge proofs

In some instances, security could be enhanced by one party providing a provable attestation of a fact. This might include that they were or were not at a particular location at a particular time, that they have tested positive for a certain antibody, that they are a certain age or have a certain qualification, and so on.

In a zero knowledge protocol a prover can mathematically prove something without revealing any additional information to the verifying party. Applications of zero-knowledge proofs range from [buying cocktails](https://www.linkedin.com/pulse/how-does-peggy-prove-her-age-without-giving-away-prof-bill/) to privacy-preserving digital currencies (like the [AZTEC protocol](https://github.com/AztecProtocol/AZTEC)) to [verifying nuclear disarmament](https://mae.princeton.edu/about-mae/spotlight/zero-knowledge-proof-verification-without-information).

### Homomorphic cryptography

Homomorphic ciphers allow “computation on ciphertexts, [that generate] an encrypted result which, when decrypted, matches the result of the operations as if they had been performed on the plaintext.”

The plaintext information encoded in the encrypted message is never revealed to the computer processing it. These computations can be executed on untrusted devices (i.e. within traditional execution environments) while preserving the privacy of its subject.

### Governing Code

Clearly several viable options exist for placing a constellation of privacy-preserving computers at the center of the panopticon. How, then, to ensure that such a guardian is benevolent?

The answer must rely heavily on the collective governance of open source code repositories. The algorithms and, when appropriate, training datasets used to process personal data on the edge or inside a secure enclave must be visible to all. “Given enough eyeballs, all bugs are shallow.”

Fortunately, such a system of collective governance already exists. Many commonly used libraries and packages are open and inspected by thousands of developers all over the world. Communities of experts debate the merits of changes to the repositories.

A blockchain-based system would enable an electorate of developer-citizens to cast reputation-weighted votes on updates to code. This could ensure that the algorithms we use to surveil ourselves are trustworthy — reviewed by the public. I can think of no better way to ensure that our code is designed to serve the public than to make sure that it is written by the very people it is surveilling. The integrity guarantees provided to algorithms executed inside a secure enclave would provide us confidence that the software agents watching over us were publicly approved, fetched from a decentralized code registry.

System architecture must be decentralized to the greatest extent possible, to minimize the consequences of a failure. Consensus networks of trusted institutions running clusters of secure enclaves could provide the public additional layers of confidence that all participants are behaving appropriately. As users become self-sovereign, they will choose open source and privacy-preserving software and hardware — and could even be compensated for opting in to sharing their data with these surveillance architectures.

Innovation’s evolution inevitably outstrips our capacity to effectively govern it. Plus, we need to use our inventions for a while before we know how to regulate them. In this envelope between invention and effective regulation, actors — some ignorant, some unscrupulous — take advantage of the new technology in unjust ways. We are now witnessing this happen on a scale never seen before, a perilous development as we construct informational infrastructures we will occupy for a long time.

Human beings have a fundamental right to privacy, and to choose how their information is used. This right is being violated wholesale, trampled upon by firms and governments all around the world. As we transition out of adolescence and into maturity as an informational society, we must unweave the threads of institutional injustice that are being entwined into our tapestry, and replace them with just and equitable ones.

Calls to roll back advancements in AI and machine learning may come from a righteous place, but they are misguided. The potential benefits to be gleaned from the new capabilities we are developing —both the algorithms and the connected sensor networks that capture the data they consume — are too great. We must not throw the baby out with the bathwater. A benevolent panopticon will help us achieve our potential as a species coexisting harmoniously.
