# Self Sovereign Identity

While the anonymity and trustless nature of crypto has brought about significant advantages there are also significant
disadvantages. The numbers of hacks, scams, frauds, rug pulls that still occur on a daily basis in crypto is
massive and still makes the crypto space a place for the bravest. This is not a problem in the early adoption phase
of crypto but as crypto becomes more mainstream the ease and security of using crypto will be essential. There are also
an entire set of applications that are simply impossible in a purely anonymous trustless system. This is easily seen in
the examples of how the reputation system of airBnB makes it safe for an average person to host a foreignor that they
met on the internet in their own homes. Uber has made it safe for parents to send their young children to school with
a total stranger. Games, market places, Decentralised exchanges and multiple applications will be made possible, safer
or significantly improved when self sovereign (decentralised) identity and reputation systems are more widespread.

We believe that Self Sovereign (decentralised) identity and the increased Trust that is developed as part of this will unveil a new set of application and crypto solutions that are currently unrealisable in the web 2.0 internet of today.

## Background

Self Sovereign Identity is a concept where the user has sovereignity over their own identity.
This differs from current systems where an external authority e.g. a government, a website, application
academic institution etc controls and maintains a users Identity.
Self Sovereign Identity applies to natural persons, organisations (companies, sports teams etc) and devices (see IOT).
Self Sovereign Identity is often associated with Decentralised Identity. For the purposes of this discussion
Decentralised Identity is considered to be a mechanism through which Self Sovereign Identity is implemented.
Digital Identity can be applied to persons, organisations or devices, since their is no material difference
in how Identity works for these different use cases we will for the rest of this document use examples and references
only for Natural Persons.

The movement to Self Sovereign Identity has come as a response to many of the abuses and manipulations that
have resulted from 'Trusted' authorities misusing their positions of authority.
The feasibility of Self Sovereign Identity has only emerged in the last few years as technology has matured to the
point where a new solution is technically feasible.

## Digital Identity

### History of Digital Identity

One of the easiest ways to think of Identity is the things that you might carry on your person for
the purposes of Identifying yourself (authentication). In the current world this would usually consist
of your identity book/card or passport, for some employees these may be an employee card.

In addition to the authentication you may also carry around various documents that prove that you are
authorised to carry out certain activities e.g. a Drivers License (Authorisation),
credit cards, loyalty cards etc all fit in this category.
The third thing that relates to your Digital Identity might be a proof of attainments
e.g. A qualification from a school or university.
For the purposes of this discussion we will call these claims against Identity.

In recent years with the explosion of the internet in addition to these physical Identities Digital
identities have begun to play a bigger and bigger role in our lives. Digital Identities might includes your
login details for a banking application or any other individual website/app, your avatar in a multiplayer game etc.

Just from this brief description it is clear that your online identity is fragmented across multiple entities.

To solve the problem of having to remember multiple logins across many sites the big Tech giants Microsoft, Google,
facebook etc have developed systems that allow them to authenticate you on multiple websites.

### Problems with the current state of Digital Identity

The first problem is that any centralised entity can and has been coerced by their government to share your sensitive
data often illegally with the government. The second problem is that your user data and usage data while online is
extremely valuable and all this data is accumulated sold and used without you as a user having any authority or even knowledge
over how your data is being used. A third problem is that since all your attainments are recorded abd maintained in the centralised system of
each website/app you are effectively locked into each separate system (See [Reputation](./Reputation.md)).
This user lock in results in users continuing to use an application long after the application is serving them maximally.
Think of a content creator on YouTube who has millions of followers he/she would be unwilling to move to another platform
even though he/she is being shadow banned or is not enjoying his/her fair share of the revenue being created from his/her efforts because to
move to another site would mean that all his/her attainments would be lost.

These types of lock ins are the standard practice (and the holy grail) in web 2.0 business models. They do however come with
significant drawback, they inhibit innovation of
the entire ecosystem and they effectively result in applications providing users with immense value in the beginning but once
enough users are locked in the users needs become subservient to the monetisation of the user and his or her data.

### Self Sovereign Identity solution

Self Sovereign Identity offers to solve the above issues by placing the control of identity firmly in the hands of the user.
An imagined solution may look something like this.

First you create a Self Sovereign Identity in your own 'credentials wallet'. You may then claim that they have a certain email address.
This claim is challenged and verified (or rejected) by an external attestor (more on how this works later). Once your claim has been proven the attestation (verified claim) is added to your 'credentials wallet'.

You now arrive at a new website for the first time. The website challenges you to prove your identity and you sign via your credentials wallet. This signature is cryptographically secure in the same way that your bitcoin payment is cryptographically secured.

If the website wants to collect your email address you may authorise that this data is transferred to the site.
Now you start navigating the website any reputation that you acquire on this site is directly associated with your
self sovereign identity and as such is portable outside of the site and presentable at any other site which may or may not chose to recognise these reputation credentials.

Another application might be applying for a loan. At present most loans in Crypto are over collateralised meaning that the user provides more collateral in the form of crypto than they borrow. In the future a user with a sufficient reputation may well be allowed to borrow against their reputation. The users reputation would be associated with the users Identity.
The user may approve that all records of loan repayments are updated to their reputation.

Another use of decentralised Identity may be as a decentralised CV where an individual has verified skills and a recorded history of contributions to certain projects.

## Identity Structure

To understand how identity is implemented technically it is necessary to understand the structure of an Identity system.

A user may have one or more identities.
Identity - controlled by the user
Claims on Identity - a claim may be as simple as claiming a certain email address or as complex as claiming a qualification.
A claim my be made by the user or made by another user or an organisation (e.g. a university my claim that you have a qualification).
A Claim is a statement about an Identity - e.g. a persons age, a rating of trustworthiness,
an assessment of a skill or an email address/twitter handle.
Credentials - Entitlement to privileges historically in written form.
 credentials usually includes one or more identifier plus numerous claims about an entity.
Identifier - Name or label that uniquely identifies an identity.
Identity - representation of an entity. Can include claims and identifiers.

### Identity principles

The user should always be in control of his or her identity.
User must be able to easily view all data and claims associated with his identity.
This does not mean that they can necessarily modify the claims but they must have
full visibility of all claims against their identity.
A user must consent to claims that are to be attached to his/her identity.
The consent may not necessarily be on a per claim basis but must be deliberate. E.g. if I wish to become an Uber Driver then I give consent that my driving history and user ratings will be added to my identity as claims. Each update does not need to have an approval but the approval has been given to that particular type of data being added to my identity.
If I enter into a loan agreement or a monthly payment I may consent that my identity is updated with my credit history.
Any usage of users data may only happen by consent as an example a user may consent to have their search history shared with advertisers via google. The user may be compensated for this data.

## Self Sovereign Identity in Polkadot

Polkadot has the beginnings of the concept of identity built directly into the base layer (layer 0).
It is believed that this will allow Polkadot to provide a more trustworthy environment for application development.
By default Polkadot can store a users attested information information such as display name, email, twitter handle and element name. There are many projects being built on Polkadot such as Litentry who add additional functionality to this.

### Identity verification in Polkadot

In polkadot (and many other crypto solution) the vision of Self Sovereign Identity is implemented using decentralised technologies thus creating decentralised identity (DID).
Decentralised identity in Polkadot functions by having 3 parties in the triangle of trust.
Firstly you have the atester (registrar). The atester atests (verifies) that the credentials claimed by the identity are correct. At present these credentials are limited to email address, twitter handle and element name.
If a user (person, organisation or IOT device) claims a credential such as an email address the atester (registrar) may challenge the user by sending a challenge email. If the user responds to this challenge then the atester can verify that the user (who controls the identity) has control over the email address. The credential of identity is then verified.

There are many registrars (atesters) in the Polkadot ecosystem who may verify users credentials. When a user makes a claim in polkadot the user pays a small fee. The claim is placed in the market place and a registrar would bid on this claim. A user would select a registrar based on their perceived trustworthiness of the registrar.

## technical Details

At this point we are ready to dive into the technical details of a particular implementation and how to use it or how to program on it depending on the purpose of this document.

## Links

[Great SSI overview](<https://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html>)
[Metadium Article Principles of SSI](<https://medium.com/metadium/introduction-to-self-sovereign-identity-and-its-10-guiding-principles-97c1ba603872>https://medium.com/metadium/introduction-to-self-sovereign-identity-and-its-10-guiding-principles-97c1ba603872>)