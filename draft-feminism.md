---
title: Feminism and protocols
abbrev: Feminism
docname: draft-guerra-feminism-02
date: 2021-11-10
category: info

ipr: trust200902
area: IRTF
workgroup: Human Rights Protocol Considerations Research Group
keyword: Internet-Draft
stand_alone: yes
pi:
  rfcedstyle: yes
  toc: yes
  tocindent: yes
  sortrefs: yes
  symrefs: yes
  strict: yes
  comments: yes
  inline: yes
  text-list-symbols: -o*+

author:
-
       ins: J. Guerra
       name: Juliana Guerra
       organization: Derechos Digitales
       email: juliana@derechosdigitales.org

-
       ins: M. Knodel
       name: Mallory Knodel
       organization: Center for Democracy & Technology
       email: mknodel@cdt.org

informative:

   RFC8280:

   RFC4949:

   RFC1244:

   RFC2122:

   RFC2310:

   RFC1746:

   RFC1941:

   RFC3694:

   RFC6365:

   RFC7704:

   RFC3675:

   RFC1984:

   RFC5646:

   BCP72:
     title: Guidelines for Writing RFC Text on Security Considerations
     date: 2003
     author:
        - org: IETF
     target: https://datatracker.ietf.org/doc/bcp72/

   Comninos:
      title: "A cyber security Agenda for civil society: What is at stake?"
      author:
         - ins: Alex Comninos
      date: 2013
      target: https://www.apc.org/sites/default/files/PRINT_ISSUE_Cyberseguridad_EN.pdf

   Tao:
      title: "The Tao of the IETF."
      author:
         - org: Internet Engineering Task Force
      target: https://www.ietf.org/about/participate/tao

   UNGA:
      title: "The promotion, protection and enjoyment of human rights on the Internet."
      author:
         - org: United Nations General Assembly
      date: 2012
      target: https://documents-dds-ny.un.org/doc/UNDOC/LTD/G12/147/10/PDF/G1214710.pdf?OpenElement

   ITU:
      title: "Statisctics. Global, Regional and Country ICT Data."
      author:
         - org: International Telecommunications Union (ITU)
      date: 2018
      target: https://www.itu.int/en/ITU-D/Statistics/Pages/stat/default.aspx

   WebFoundation:
      title: "Advancing Women's Rights Online: Gaps and Opportunities in Policy and Research."
      author:
         - org: Web Foundation
      date: 2018
      target: http://webfoundation.org/docs/2018/08/Advancing-Womens-Rights-Online_Gaps-and-Opportunities-in-Policy-and-Research.pdf

   FPI:
      title: "The Feminist Principles of the Internet"
      author:
         - org: Association for Progressive Communications
      target: https://feministinternet.org

   SmKee:
      title: "Imagine a Feminist Internet."
      author:
         - ins: Jac Sm Kee
      date: 2018
      target: http://link.springer.com/10.1057/s41301-017-0137-2

   WhoseKnowledge:
      title: "Decolonizing the Internet, Summary Report."
      author:
         - org: Whose Knowledge
      date: 2018
      target: https://whoseknowledge.org/wp-content/uploads/2018/10/DTI-2018-Summary-Report.pdf

   Arkko:
      title: " Considerations on Internet Consolidation and the Internet Architecture."
      author:
         - ins: J. Arkko
      date: 2018
      target: https://datatracker.ietf.org/doc/draft-arkko-iab-internet-consolidation

   FPI:
      title: "The Feminist Principles of the Internet."
      date: 2015
      target: https://feministinternet.org

   Collins:
      title: "Black Feminist Thought: Knowledge, consciousness and the politics of empowerment."
      author:
         - ins: P. H. Collins
      date: 2000

   Crenshaw:
      title: "Demarginalizing the Intersection of Race and Sex: A Black Feminist Critique of Antidiscrimination Doctrine, Feminist Theory, and Antiracist Politics."
      author:
         - ins: K. Crenshaw
      date: 1989
      target: https://doi.org/10.4324/9780429500480-5

   Lorde:
      title: "unknown."
      author:
         - ins: Lorde
      target:

   Davis:
      title: "unknown."
      author:
         - ins: Davis
      target:

   Hankivsky:
      title: "Intersectionality 101."
      author:
         - ins: O. Hankivsky
      date: 2014
      target: http://vawforum-cwr.ca/sites/default/files/attachments/intersectionallity_101.pdf

   Mason:
      title: "Leading at the Intersections: An Introduction to the Intersectional Approach Model for Policy and Social Change."
      author:
         - ins: C. N. Mason
      date: 2010

   Symington:
      title: "Intersectionality: a Tool for Gender and Economic Justice."
      author:
         - ins: A. Symington
      date: 2004
      target: https://www.awid.org/sites/default/files/atoms/files/intersectionality_a_tool_for_gender_and_economic_justice.pdf

   tenOever:
      title: "Freedom of Association on the Internet."
      author:
         - ins: N. ten Oever
      date: 2017
      target: https://datatracker.ietf.org/doc/html/draft-irtf-hrpc-association

   Knodel:
      title: "Terminology, Power and Offensive Language."
      author:
         - ins: M. Knodel
         - ins: N. ten Oever
      date: 2018
      target: https://datatracker.ietf.org/doc/draft-knodel-terminology

--- abstract

This document applies an intersectional feminist approach to describe how internet standards, protocols and their implementations may impact diverse groups and communities. The research on how some protocols can be enablers for specific human rights while possibly restricting others has been documented in {{RFC8280}}. Similar to how RFC 8280 has taken a human rights lens through which to view engineering and design choices by internet standardisation, this document addresses the opportunities and vulnerabilities embedded within internet protocols for specific, traditionally marginalized groups.

--- middle

# Introduction

The architecture design of the Internet as a global network of networks, coupled with the IETF's strong commitment to security and privacy, means the Internet contributes positively to an environment in which human rights are enabled. Privacy {{RFC6973}} and Human Rights {{RFC8280}} considerations are valuable tools for decision making about protocol design and deployment that takes into account whether a specific technology might enable a specific human right while having an adverse impact on another. Privacy and human rights considerations encompass the recognition that sometimes human rights can be in conflict with each other and in such cases trade offs are made intentionally and transparently.

As a complement to those approaches this document takes a look at how internet protocol design relate to the differential ability of individuals, groups and communities to exercise their human rights. For this analysis an intersectional feminist framework that is both practical and theoretical is used to focus firstly on how the uses of the Internet are determined by social, economic, cultural, and physical differences and secondly on the alternative internet technologies that maginalized groups use, apropriate, and implement themselves to ensure their access, participation, and agency in the world off and online.

And in contrast to previous approaches this document extends to include the existing structural barriers within internet governance and the standardization process itself as a factor that reinforces or alleviates the differential realization for individuals, groups and communities.

Furthermore this document builds off of another branch of work in the IETF that has identified, to what extent it is possible, mechanisms to improve inclusion of traditionally maginalized groups inside IETF by developing norms of engagement around Diversity and Conduct {{RFC7704}}, Anti-Harrassment {{RFC7776}}, and Racist Terminology {{{draft-terminology}}} in which difference across social locations such as gender, race, and class are confronted.

Thus where {{RFC8280}} leveraged the standard framework for equality declared in {{UDHR}}, this document relies on the differences across a variety of lived experiences and identities related to Internet uses that form the basis for a practical intersectional feminist document called The Feminist Principles of the Internet {{FPI}}.

This document must not be understood as a set of rules or recommendations, but as guidance for addressing the key technical issues and policies for feminists and those with which intersectional feminism is concerned. Its goal is to offer a freamework of understanding built by marginalized groups to feed ongoing conversations arround diversity, oppression, and the need to make the IETF a more inclusive enviroment.

But first we must estbalish common understanding through a compressed explanation of intersectional feminism, followed by a broad review of feminist expression, research and mobilization in the age of the internet.

# An intersectional feminist perspective

Imagine a highway that connects two big cities, one capable of withstanding heavy traffic at high speeds. Driving there takes experience and expertise, and just a few streets intersect it so as not to hinder traffic. Imagine this highway as a robust body of rights and those who travel along it as people who have traditionally enjoyed these rights.

If someone without enough experience is driving down a road that intersects the highway and wants to get there, that person will be at greater risk of crashing or having an accident. In addition, without a valid license the person will also run the risk of being fined by the traffic authorities. In terms of rights, those intersecting roads are not robust and the risks of accident are forms of discrimination experienced by those who drive on them. What if many small streets intersect at the same point on the highway?

Arose from black feminist theory, the concept of intersectionality serves to understand how multiple forms of discrimination overlap {{Collins}}. As first pointed by {{Crenshaw}} in the United States, "Black women can experience discrimination in ways that are both similar to and different from those experienced by white women and Black men", so an intersectional approach should be able to recognize this type of discrimination by transcending the one-way perspective with which the justice system, as well as feminist and anti-racist movements, had traditionally operated.

From this proposal, the concept has meant a paradigm shift both in feminist thinking {{Collins}} and movements {{Lorde}}{{Davis}}, and more recently in the design and implementation of public policies {{Mason}}{{Hankivsky}}. The intersectional approach is not focused on the problem of equality but on difference; discrimination is not analyzed in terms of effective access to rights, but the conditions and capacities people have to exercise those rights.

Therefore, an intersectional feminist perspective focuses on social location, the multiple layered identities people live, derived from social relations, history and structures of power through which people can experience both oppression and privilege. These oppressions can be structural and dynamic, determined by gender, race or skin color, class, sexuality, ethnicity, age, language, geographic location, abilities or health conditions, among other factors {{Symington}}.

## Internet as a matrix of domination

The concept _matrix of domination_, introduced by {{Collins}} as complementary to _intersectionality_, refers to the way by which the powers that produce and reproduce intersecting oppression are organized. In summary, the concept _intersectionality_ has served to recognize people's different experiences and social locations and with this, the need of a bottom up understanding of discrimination and oppression; in addition, the concept _matrix of domination_ turns the gaze on the context of power -institutional, political, economic and symbolic- in which intersecting oppressions operate.

The gender and sexual rights lens on critical internet-related rights contained in the Feminist Principles of the Internet has been built bottom up by the feminist movement {{FPI}}, which treats most prominently people who are negatively discriminated against on the basis of their gender and sexuality, but not exclusively. Based on the threats to women and queer people -whose bodies and manifestations are already under strong, albeit sometimes invisible, social, cultural and political surveillance-, an intersectional feminist analysis makes it possible to recognize how multiple oppressions affect the ways people access, use and participate on the internet.

From now on, some of these experiences will be used to identify how the internet can enable or restrict the possibility of justice and equity among its users. For this purpose, it is useful to understand the internet as a _matrix of domination_ in the sense pointed by {{Collins}}: as an institutional, political, symbolic and cultural context where different intersecting oppressions are shaped and reinforced.

This document addresses the opportunities and vulnerabilities incorporated into Internet protocols for specific, traditionally discriminated groups, on the assumption that these values are inherent in technological design. Through the proposed intersectional perspective, a multilevel description of the factors, processes and social structures that affect different experiences on the Internet is presented below and, based on specific cases, an analysis will be made of how the different protocols intervene in the shaping and reinforcement of intersecting oppressions faced by users on different social locations.

## Brief history of feminist mobilzation and the internet

The ways by which feminists have been understood, used and mobilised in the Internet is significant for a baseline understanding of how internet protocols and feminism intersect. Intersectional feminist action and analysis can be collected into two strategies: addressing the status quo and creating alternatives. Feminists on the early internet embodied both.

It is important to note here that there has always existed a gender gap in access to the internet, which is exacerbated by global wealth inequality.

Since the 1980s, feminist movements have used the internet to challenge power. Globalisation. Development. Cyberfeminism. Internet governance. There is a deeper connection to the internet and social justice struggles in which communication becomes the primary strategy to address inequality. Indeed, in "A History of Feminist Engagement with Development and Digital Technologies" Anita Gurumurthy writes, "the history of the right to communicate reveals the contestation between powerful status quoist forces and those who seek transformative, global change for justice and equality."

At the same time, feminists were using the internet to create feminist space.

Author Feminista Jones argues in "Reclaiming Our Space: How Black Feminists Are Changing the World from the Tweets to the Streets" that the feminist alternative spaces have become mainstream and are leading analysis and critique of the status quo, a merging and strengthening of the two strategies that emerge from this particular historical framing.

Given these myriad expressions of feminism online and feminist movement building online, one thread is perhaps most instructive to this exercise, which we use as the basis for this document: Feminist Principles of the Internet. More about the nature of the complex community that created the Feminist Principles of the Internet can be found at feministinternet.org. The principles, drafted and revised by hundreds of feminists mostly in the global south, highlight historical feminist themes for the digital age in its main categories: access, movements, economy, expression and embodiment.

This includes a series of 17 statements with a "gender and sexual rights lens on critical internet-related rights" for the purpose of enabling women's rights movements to explore issues related to internet technology.

# Methodology

The research question guiding this document's development has been "Would feminists have built a better internet?" For years, the global, intersectional feminist movement has been unconsciously asking itself this very question. In sporadic, in-person convergences over the course of several years and mailinglist and social media threads, a truly staggering conversation was started with the prompt #ImagineAFeministInternet {{{GenderIT}}}. The result led to the FPIs and a living archive of feminist organizing resulting from the process as well as the product. This document is both a result of and a new contribution this global mobilizing effort.

Answering the original question requires taking more than one distinct approach. The _movement approach_ has yielded the FPIs, which are brilliant and visionary and intersectional in all the right ways. They have profoundly shifted human rights centred policy advocacy on issues of content moderation and social networks. Yet they do not easily translate to technical design and implementation-- something falls short. The _participatory design approach_ may provide more insight into this research. The crux of this proposal rests on an innovative participatory design project for participants to "imagine a feminist internet protocol".

The vision for this research document is essentially to combine the two approaches: Given what the intersectional feminist movement has identified as its principles for the internet, an engaged group of expert engineers (a subset of that same movement) can now visualise core internet protocols differently. Those core internet protocols will be specifically chosen from the following areas of real-world design and implementation: applications, internet protocol, routing, security, transport and operations. The expressions will be visual (illustrations, drawings, charts, images, metaphors) and textual.

# Guidelines for developing a feminist internet

Each of the five clusters of the Feminist Principles of the internet are presented below: Access, Movements, Economy, Expression and Embodiment. For some, individual principles are relevant and presented insofar as they are relevant for protocol development. The descriptive text references other works that bridge the connection between internet protocols and their development with the practical FPI framework. Depending, each section will touch on one or all of: differential use, alternatives and standards process issues that are relevant to consider. Such that the resulting guidance is clear and actionable, direct or tangential examples may be included along with elements of visualization.

In addition we take a case study approach that cross cut the FPIs and apply the same framework.

## Access

Internet access is recognized as a human right {{UNGA}}, but its effective guarantee depends on different and unequal social, cultural, economic and political conditions. In 2018, barely half of the world's population has access to the internet and in 88% of countries, men have more access than women {{ITU}}. Geographical location, age, educational and income level, as well as gender, significantly determine how people access to the internet {{WebFoundation}}.

The Feminist Principles of the Internet {{FPI}} explore a broad understanding of the term beyond technicalities. It seeks to connect the technical fact to gendered and socio-economic realities.

### Internet access

Access must be to a universal, acceptable, affordable, unconditional, open, meaningful and equal internet, which guarantees rights rather than restricts them {{FPI}}. As some bodies have always been subject to social and cultural surveillance and violence because of their gender and sexuallity, their access to internet will not be satisfied with connected devices, but with safety and useful digital enviroments {{SmKee}}.

Harms: Restricted connectivity. i.e. Middleboxes (which can be Content Delivery Networks, Firewalls, NATs or other intermediary nodes that provide 'services'besides routing). TODO

Related protocols: The end-to-end principle is important for the robustness of the network and innovation (RFC1958); Content agnosticism: Treating network traffic identically regardless of content.

Related rights: Freedom of expression, freedom of association.

### Access to information

Women and queer people have traditionally had restricted their reproductive and sexual rights. Today their rights are resticted in different levels and qualities in differents countries and regions. It is necessary to guarantee access to relevant information related to sexual and reproductive health and rights, pleasure, safe abortion, access to justice, and LGBTIQ+ issues.

Harms: Some governments and ISPs block pages with this content or monitor online activity by sexual and gender related terminology. Therefore the considerations for anticensorship internet infrastructure technologies
also consider, and can possibly alleviate, a gendered component to using the internet.

TODO. Blocked sites, Monitoring by content, identify users by IP or type of traffic.

Related protocols: Information in one's own language is the first condition, as pointed out with the cencept of 'Localization' {{RFC8280}}, referred to the act of tailoring an application for a different language, script, or culture, and involves not only changing the language interaction but also other relevant changes, such as display of numbers, dates, currency, and so on.

TODO. Content agnosticism: Treating network traffic identically regardless of content (but it refers to header content). Censorship resistance.

Related rights: FoE, FoA, Right to political participation, Right to participate in cultural life, arts and science.

### Usage of technology

Beyond content, access implies the possibility to use, which means code, design, adapt and critically and sustainably use ICTs. Even though almost 75% of connected individuals are placed in the Global South
{{WhoseKnowledge}}, technology is developped mainly in rich countries where student quotas and jobs are filled mainly by men.

However, there is still a long way to go in terms of inclusion of more diverse populations in the spaces of technology development and definition of protocoles and standards for the internet infrastructure {{RFC7704}}. Building and engineering critical internet technology is a component of 'usage' {{Knodel}}, one which chllenges challenge the cultures of sexism and discrimination.

Harms: Gender and race bian in algorithms, digital gender gap. Necessary to know the charset, gap. The presence of gendered subjects in the IETF RFCs and drafts archive demonstrates stereotyped male and feminine roles.

Related protocols: The concept of 'Internationalization' {{RFC6365}} refers to the practice of making protocols, standards, and implementations usable in different languages. This is a first step to democratize the development of technology, allowing its implementation in non-English-speaking countries.

TODO. {{RFC5646}} descentralization, reliability. Adaptability (permissionless innovation).

Related rights: Right to participate in cultural life, arts and science

## Networked

In contexts where women do not have their rights fully guaranteed, or where sexual and gender diversity are socially condemned, the Web has served to meet, organize and resist. With the popularization of the internet, the freedom of expression of both women and other gender identities traditionally marginalized from public life and social acceptance (whom we refer to as queer) has been greatly enhanced.

By adding content in formats like text, audio and video, these groups have been able to connect with each other, as well as open spaces for discussion and visibility of topics that previously seemed vetoed. The web has become a space for activism, reclamation and protest against injustice and gender inequality. It has allowed the construction of international networks of solidarity, support and mobilization, and with this, the strengthening of feminism and other movements that fight for equal rights and for a fair recognition of difference.

### Resistance

The internet is a space where social norms are negotiated, performed and imposed. For users it increasingly functions as an extension of offline spaces shaped by patriarchy and heteronormativity. Disident content as well as widely accepted norms and values should have the same possibilities to be added, flow and stay on the net.

Harms: content blocking, content monitoring and identification, traffic monitoring

Related to protocols: Integrity

Related rights: Freedom of expression, Freedom of association.

### Movement building

Given the shrinking of civic space offline, the internet provides a global public space, albeit one that relies on private infrastructure {{tenOever}}. For social causes that push for equality, it is
therefore critical that the internet be maintained as a space for alignment, protest, dissent and escape. In the scope of this document, this is a call to maintain and enable the creation of spaces for
sustained feminist movement building. Ihe internet provides new and novel ways for communities to come together across borders and without limits of geolocation.

Harms: However this positive aspect of internet communications is
threatened by centralised systems of control and cooptation, specifically surveillance and other online repression.

Related protocols: Association of system architectures is a concept that overlaps neatly with the ideals of real-world associations of organisations and communities. "The ultimate model of P2P is a completely decentralized system, which is more resistant to speech regulation, immune to single points of failure and have a higher performance and scalability {{tenOever}}." It can be descussed in terms of intersectionailty and what we mentioned about 'different dimensions of freedom'. Maybe the 'solution' is not only P2P because it doesn't take into account different distances from and capacities related to this technology, maybe mixed with another feature?. Integrity.

Related rights: Elements of freedom of assocation as explained in the UDHR include individual and collective rights to privacy and anonymity, as discussed in more detail below.

### Internet governance

It is critical for groups who represent civil society interests, social change and the larger public interest to challenge processes and institutions that govern the internet. This requires the inclusion
of more feminists and queers at the decision-making table, which can be achieved through democratic policy making. Greater effect will be possible through diffuse ownership of and power in global and local networks.

Harms: Gender gap

Related to protocols: While there is no agreement regarding the ability of the internet to negatively or positively impact on social behaviors, or shape desirable practices {{RFC8280}}, more women and diverse populations'
participation in technical development and decision-making spaces will lead to greater possibilities for ICTs to reflect greater inclusiveness and enable less risky and harmful interactions {{RFC7704}}.

Related rights: Right to participate in cultural life, arts and science

## Economy

From a feminist perspective, it is necessary to achieve the promise of an Internet that facilitates economic cooperation and collaboration. One Internet that can challenge models of economic inequality and transcend into other forms where women and queer people are not relegated or in economic dependence.

### Business models

Interrogating the capitalist logic that drives technology towards further privatisation, profit and corporate control implies open discussions on centralisation of services and the logic of vertical integration while holding nuance for the tensions between trust, reliability and diversity.

Alternative forms of economic power can be grounded in principles of cooperation, solidarity, commons, environmental sustainability and openness.

Harms: TODO

Related protocols: Centralisation of services is a current discussion in the IETF that should be informed by feminist critique of capitalist structures {{Arkko}}. End user centered; W3C, descentralization.

Related rights: TODO

### Open source

The digital gender gap has relegated women and other marginalized groups to be internet users, adding content for the benefit of the platforms themselves but without a deep understanding of how these platforms work. This requires shared terminology upon which technology is created to enable experimentation and values exchange. Not only that, but documenting, promoting, disseminating, and sharing knowledge about technology is at the heart of the long-standing free software community's ethos. This aligns with a feminist approach to technology.

Given the established community of "free software", it is important to note that freedom is not freedom for everyone, always. It is important to identify different dimensions of freedom and how it is
expressed in different contexts.

Harms: TODO

Related protocols: Promoting transparency {{RFC8280}} and simplifying technical terminology is necessary to bridge this gap. Interoperabiliy, Open standards are important as they allow for permissionless innovation. Freedom and ability to freely create and deploy new protocols on top of the communications constructs that currently exist. Open standards.

Related rights: Right to participate in cultural life, arts and science

## Expression

### Amplify

The state, the religious right and other extremist forces who monopolise discourses of morality have traditionally silence women’s voices and continue to silence feminist voices and persecute women’s human rights defenders.

Harms: Blocking and monitoring content, identifiyng site owners, manipulating indexed content on search engines, Trolling, coordinated attackes (DoS and DDoS).

Related protocols: Content agnosticism: Treating network traffic identically regardless of content, anti censorship.

Related rights: Freedom of expression, Freedom of association, Access to information

### Expression

The political expression of gender has not been limited to voices, but has made use of the body and its representation. However, the use of body as a form of political expression on the internet implies a series of risks and vulnerabilities for the people involved in these movements, especially if they do not understand how internet technology works.

Harms: Surveillance, content regulations or restrictions, content blocking.

Related protocols: Confidentiality, keeping data secret from unintended listeners {{BCP72}}. Data protection {{RFC1984}}. Encryption

Related rights: Freedom of expression

### Pornography

Women's sexual expression online is socially condemned and punished with online gender based violence. On the other hand, queer people online sexuality is usually labeld as "harmful content". These practices evidence how overcontrolled are gendered bodies and tend to confuse the differences between sexual expression and pornography.

Users build their own public digital identities while using private communications to disseminate information, explore their sexuality in text, image and video, share their initmity with others. Pornography online, on the other hand, has to do with agency, consent, power and labour.

Harms: In internet-connected devices, it has become much easier to mix leisure and work, which implies different risks for users.

Related protocols: {{RFC3675}}

Related rights: Freedom of expression

# Embodiment

Most of the threats women and queer people face on line, occur on the user levels of application and content. Most adversaries are other users, but also include institutions, platforms and governments.

For a long time, perhaps since the internet became popular, its use ceased to be a functional matter and became emotional. The access to chat rooms to connect with people at huge distances, the possibility of having personal e-mails, the appearance of social networks to share music, photos and then video, determined not only the social use of a new tool but also the configuration of digital sensitivities, understood by some as sensory extensions of the body.

The internet connections embedded have also meant a radical transformation in the way people access the internet. Much more, considering that today most internet connections, especially in the global south, are mobile connections.

Sharing personal information, and often sensitive data, through platforms that are synchronized with email accounts and other platforms where information considered non-sensitive is published, implies losing control over such information. Much more, considering that each platform hosts the information of its users according to their own terms and conditions in the treatment of data. For women and other groups marginalized by race or gender, these risks are greater.

Just as the internet connection can be considered an extension of the body, social problems such as discrimination and exclusion have been projected into the digital environment-- sometimes intensified,
sometimes reconfigured. And once again, women, queers, racialized people are the most vulnerable. Most of the threats they face on line, occur in the user level. Most of their "adversaries" are other users, who also act at the user level, with technical or social skills that threaten participation and expressions. Institutions, platforms and governments who are adversarial have great advantage.

At this point, what level of autonomy do these people have as internet users?

### Consent

Some elements of consent online include but are not limited to the following list of issues, which should be elaborated on:

 * Data protection
        * Exposure of personal data
 * Culture, design, policies and terms of service of internet platforms
 * Agency lies in informed decisions
        * Real name policies
 * Public versus private information
        * Dissemination of personal or intimate information
        * Exposure of intimacy
        * Unauthorized use of photos

Harms: TODO

Related protocols: TODO

Related rights: TODO

### Privacy and data

While mentioned at the intersection of previous issues outlined above, this section is particularly critical for women, queers and marginalised populations who are already at greater risk of control and surveillance:

 * Right to privacy
 * Data protection
 * Profit models
 * Surveillance and patriarchy by states, individuals, private sector, etc. Those that enable surveillance, eg spouseware.

Harms: TODO

Related protocols: TODO

Related rights: TODO

### Memory

One's consent and control of the information that is available to them and about them online is a key aspect of being a fully empowered individual and community in the digital age. There are several considerations that deserve deeper inspection, such as:

 * Right to be forgotten
 * Control over personal history and memory on the internet
 * Access all our personal data and information online
 * Delete forever

Harms: TODO

Related protocols: TODO

Related rights: TODO

### Anonymity

While anonymity is never just about technical issues but users protection activities, it becomes more necessary to strenghten the design and functionality of networks, by default. There are several considerations for internet infrastructure related to enabling anonymity for online users. This is particularly important for marginalised groups and can be ennumerated, and expanded upon, thusly:

 * Right to anonymity
 * Enables other rights like freedom of expression
        * Censorship
        * Defamation, descredit
        * Affectations to expression channels
 * Breaking social taboos and heteronormativity
        * Hate Speech, discriminatory expressions
 * Discrimination and safety from discrimination

Harms: TODO

Related protocols: TODO

Related rights: TODO

### Children

TODO

Harms: TODO

Related protocols: TODO

Related rights: TODO

## Online violence

Where women and queer people have traditionally been marginalized, their participation in the internet is rejected through different forms of violence by other users, as well as institutions, platforms
and governments. But the effects of these violences, which are nothing more than extensions of the traditional violence that these groups and individuals face in social life, increase to the extent that
there is not enough technical knowledge to neutralize them, and this is the case of most people who struggle for the recognition of their gender difference.

The security considerations to counter online violence are critical. There is opportunity in a connected world for those who would perpetuate violence against women and other marginalised groups through
the use of internet-enabled technologies, from the home to the prison.

Privacy is a critical component of security for populations at risk. The control of information is linked to privacy. Where some would like privacy in order to live privately, others need privacy in order to access information and circumvent censorship and surveillance. The protection of privacy is critical for those at risk to prevent vicimisation through extortion, doxxing, and myriad other threats. Lack of privacy leads to risks such as stalking, monitoring and persistent harassment.

While making public otherwise private details about a person can constitute a form of abuse, the converse is also a risk: Being erased from society or having one's online identity controlled by another is a form of control and manipulation. Censorship, misinformation and coersion may consitute violence online. Other forms of non-consensual manipulation of online content includes platform "real name policies", sharing of intimate images and sexual abuse, spreading false accusations, flamming and other tactics.

Key to mitigating these threats is the element of consent.

Harms: TODO

Related protocols: TODO

Related rights: TODO

## Challenge the male gaze
- Principles: Resistance, Governance, Amplify, Expression, Consent, 

Privacy and data, Violence

social norms

the dominant gender perspective

discourses of morality

womens' and feminism silencing

sexual expression as freedom of expression issue (as political or religious)

women and queers

ethics and politics of consent into the culture design policies and terms of service of internet platforms

- Harms:

## Case study: Increase participation of women in tech design and decision tables

The Principles: Usage, Open source, Amplify, Consent, Access, Governance, Children

invite women and young girls to explore technology as a space of creation

creating and experimenting with technology digital safety and security

contribute to the building of the code in order to protect our data and communications

embed users' consent into the very UX design and algorithm of their code

women in developing countries as a stakeholder group with a crucial say

get more feminists and queer activists

bring women's organizations and issues to the discussion table to influence policy and protocol

Harms:

spaces shaped by patriarchy and heteronormativity

increase the number of participation and influence of gender related issues

basklash

silencing (identified in diversity rfcs?)

efforts of state and non-state actors to control surveil regulate and restrict feminist and queer expression on the internet through technology legislation or violence

moral policing censorship and hierarchisation of citizenship and rights

the umbrella term “harmful content” to label expression on female and transgender sexuality

most developers or network operators aren't prioritizing consent

dominant priority on the internet today is to extract as much data as possible with little attention to who is posting data about whom

there hasn't been enough outrage around lack of transparency of privacy breaches conducted by websites and internet corporations

Surveillance as an oppressive tool to control women’s bodies and sexual expression outside of heteronormative discourse

control and restrict women’s bodies speech and activism

Women and queers are especially vulnerable to violations of privacy as they must resist cultural and family practices of surveillance as well

OJO, identify these specific threat models: cyberstalking - phones - the internet social media platforms – email

Technology-related violence against women is part of the same continuum as violence against women offline

# References not yet referenced

In plain sight, on sexuality, rights and the internet in India, Nepal and Sri Lanka https://www.genderit.org/articles/plain-sight-sexuality-rights-and-internet-india-nepal-and-sri-lanka

Human Rights and Internet Protocols: Comparing Processes and Principles https://www.apc.org/sites/default/files/ISSUE_human_rights_2.pdf

Principles of Unity for Infraestructuras Feministas https://pad.kefir.red/p/infraestucturas-feministas Feminist

Principles of the Internet https://feministinternet.org The UX Guide to Getting Consent https://iapp.org/resources/article/the-ux-guide-to-getting-consent

From steel to skin https://fermentos.kefir.red/english/aco-pele Responsible Data https://responsibledata.io

Impact for what and for whom? Digital technologies and feminist movement building internet https://www.genderit.org/feminist-talk/impact-what-and-whom-digital-technologies-and-feminist-movement-building

Design Justice https://docs.google.com/presentation/d/1J3ZWBgxe0QFQ8OmUr-QzE6Be8k_sI7XF0VWu4wfMIVM/edit#slide=id.gcad8d6cb9_0_198

Design Action Collective Points of Unity https://designaction.org/about/points-of-unity

CODING RIGHTS; INTERNETLAB. Violências de gênero na internet: diagnóstico, soluções e desafios. Contribuição conjunta do Brasil para a relatora especial da ONU sobre violência contra a mulher. São Paulo,
2017. https://www.codingrights.org/wp-content/uploads/2017/11/Relatorio_ViolenciaGenero_v061.pdf

Barrera, L. y Rodríguez, C. La violencia en línea contra las mujeres en México. Informe para la Relatora sobre Violencia contra las Mujeres Ms. Dubravka Šimonović. 2017.
https://luchadoras.mx/wp-content/uploads/2017/12/Informe_ViolenciaEnLineaMexico_InternetEsNuestra.pdf

Sephard, N. Big Data and Sexual Surveillance. APC issue papers. 2016. https://www.apc.org/sites/default/files/BigDataSexualSurveillance_0_0.pdf

Crenshaw, K. (2018). Demarginalizing the Intersection of Race and Sex: A Black Feminist Critique of Antidiscrimination Doctrine, Feminist Theory, and Antiracist Politics [1989]. In K. T. Bartlett & R. Kennedy (Eds.), Feminist Legal Theory (1st ed., pp. 57–80; By K. Bartlett). https://doi.org/10.4324/9780429500480-5

The oracle for transfeminist technology https://www.transfeministech.codingrights.org

# Security Considerations

As this document concerns a research document, there are no security considerations.

# IANA Considerations

This document has no actions for IANA.

