# OCCP
Open Content Certification Protocol

The Open Content Certification Protocol (OCCP) will provide a description of the technology and the processes that can be used by creative individuals, media organisations or consumers to generate or verify content certificates for digital media content. 
Content certificates will allow individual users or automated processes to verify content integrity, attribution and claims from rightsholders to the content in a decentralised way and with access to the content only.
The OCCP is based on open, content-derived identifier technology, in particular the ISCC system, maintained by the ISCC Foundation, and the ISCC meta-registry, developed by Titusz Pan. 
By using ISCC, anyone with access to digital content – it could be the original creator, a publisher, an intermediary, an online platform (OCSSR) or a consumer – can decentrally generate the same identifier from the same digital asset. 
This allows anyone to unambiguously identify same or similar content independently of centralised organisations or proprietary services and software.
Due to the fact that anyone can generate identifiers from digital content, anyone can at the same time publish the identifiers on the internet or on blockchains for various reasons. 
Creative individuals, media organisations or other rightsholders may publish and register ISCC in order to connect metadata, rights management information or other claims to the identifier. 
Other registrants may want to express ownership of a license or access to a specific document or file by generating and publishing an ISCC. 
It is important to highlight that claims to the content can be made – in principle – by anyone regardless of content ownership and independent of the actual rights owner. 
These claims may be justified, but they are not transparently verifiable for third parties. 

## Certification of Rightsholder

However, when an ISCC is registered on a public blockchain, this happens in the context of a transaction which is public, open and transparent. Public blockchain networks are based on public key cryptography. This means that transactions on these blockchains – in principle – allow to identify the pseudonymous actor who triggered a transaction by means of his pseudonymous public address. This public address is based on the public key of the actor. In order to perform a blockchain transaction, the actor needs to be in control of the corresponding private key; this allows him to cryptographically sign the blockchain transaction. The fact that there is always a pseudonymous actor that performed the transaction implies that there is always a potentially identifiable actor. This is the conceptional foundation for open content certificates.
The first step to certify digital media content is to certify the rightsholder. This is done by a publicly registered certifier on the basis of the blockchain address that is used to register ISCC on a blockchain. This certification of the rightsholder address is a public attestation by the certifier confirming that the identity of the rightsholder and registrant is known to the certifier. This confirmation explicitly requires that the certifier has verified that the private key that cryptographically signed the blockchain transactions is in control of the individual or organisation known to the certifier.

## Certification of Conten

The certification of ISCC-ID’s by a publicly registered certifier is the second step in order to certify digital media content. Whereas the certification of the rightsholder address validates the identity of the registrant, the certification of the ISCC-ID validates the relationship of the rightsholder to a specific digital asset.
Anyone can generate an ISCC from a digital asset. Anyone can register the ISCC on a public blockchain network. According to the proposal for a decentralised meta-registry protocol for ISCC, a registration of an ISCC on a public blockchain network will generate a unique and short ISCC-ID, that is ‘owned’ by the registrant in such a way as that the registration transaction for that specific ISCC has been cryptographically signed by the private key of the registrant. Reciprocally, the ISCC-ID will resolve to the full ISCC and the rightsholder address through the analysis of the registration transaction. This way, the ISCC-ID binds a rightsholder, which is the registrant and the actor of the blockchain transaction to a specific ISCC.
The certification of an ISCC-ID is not only a public attestation of the certifier that the identity of the rightsholder and registrant is known to the certifier, but also a public attestation that a specific relationship between the rightsholder and the content is publicly acknowledged and known to the certifier at this point in time. It could be, that the rightsholder is the original creator, or an organisation in the value chain that holds specific rights to distribute the content or that otherwise entitled to provide metadata, licensing and rights management information or other claims to the content. It is important to note that content certificates do not designate the specific details of certain rights and licenses of a rightsholder to the content. Content certificates only designate that the rightsholder is known to have the authority to provide valid and trustworthy information to that specific digital asset, which the certifier can declare according to the bilateral agreement between the rightsholder and the certifier.
Whereas the certification of a rightsholder will create trust in the individual or organisation who registered the ISCC, the certification of the content will create trust in the metadata, licensing and rights management information which might be associated to a specific ISCC by the rightsholder. 
The certification of an ISCC-ID also means, that a rightsholder may connect metadata, rights management Information or other data and claims to the ISCC-ID in the future. Because for each subsequent transaction any third party can check whether new information has been published by the same rightsholder as the one who ownes the ISCC-ID – the one that has already been certified as a rightsholder and registrant. 

## Examples

The OCCP is designed to provide flexibility on whether parties can act as rightsholders or certifiers. This also implies that a rightsholder could, at the same time, be a certifier of the same content, depending on the contractual relationship between the rightsholder and the certifier. 
The following paragraphs shall provide some examples: 
1. Membership organisations, collective management organisations (CMO) or performance rights organisation (PRO) are representing creative individuals and media organisations in different industry sectors that own rights to content or performances. The organisations are acting on their behalf by collecting royalties or representing them in regulatory processes. CMO’s, PRO’s not only know their clients through the membership application processes. In many cases they are also familiar with the specific works they represent on behalf of the rights owners. Membership organisations, CMO’s, PRO’s are ideally suited to act as certifiers for the rightsholders and the content which they represent.
2. A publisher might want to license digital content to a retailer. According to the license agreement, both parties are rights holders to the content: the publisher acquired rights from the creators, the retailer acquired rights from the publisher. In this case, The retailer has a stake in the content and may legitimately publish the claim to the content, e.g. to be in the position to sublicense a defined number of titles from the publisher’s digital assortment to consumers. Both, the retailer and the publisher might have an interest to certify the retailer and his claims to the content. The publisher could act as a certifier to the retailer. 

## Set-up

In order to start the certification process according to the OCCP, the rightsholder and the certifier need to set-up their wallets as well as their bilateral relationship. 

### Creation of Certifier Wallet

The certifier address will serve as the self-sovereign and decentralised ID for the certifier. The certifier can create a certifier address for himself and independently of any organisation, registry or other centralised authority. The certifier address is a public blockchain address that is generated from the public key of the certifier. Any blockchain wallet or decentralised identifier (DID) service, that can create a private/public key pair on a blockchain network, that will be used to certify rightsholders or content, can generate a certifier address.

### Public Self-Verification of Certifier

While the rightsholder address may remain pseudonymous, the OCCP requires that the identity of the organisation that is in control of the certifier address is made public. This means that certifier needs to proof in a transparent and verifiable way to the public that he is in control of the certifier address.
One possible, suggested way for the certifier to verify himself is through a process of online self-verification. This method assumes that, a) the certifier – and only the certifier – has control of the web-hosting servers that are used for the homepage of his organisation, and b) that a (trans-)national legislation requires that a publisher of information or services on the internet needs to the disclose actual contact information on the imprint page. Provided that these two conditions are met, after creation of the certifier addresses, this public address needs to be published on the imprint page of the website of the certifier. 
In a second step, the certifier needs to sign a public blockchain transaction with the corresponding private key that includes the respective website-URL. The fact that the public key that generated the certifier address is generated from the same private key that signed the blockchain transaction that includes the website-URL is proof that the certifier has control about the certifier address.
Public key cryptography and the transparency and immutability of public blockchain networks create the trust in this self-verification of the certifier.

### Creation of Rightsholder Wallet

The rightsholder address will serve as the self-sovereign and decentralised ID for the rightsholder. The rightsholder can create a rightsholder address for himself and independently of any organisation, registry or other centralised authority. The rightsholder address is a public blockchain address that is generated from the public key of the rightsholder. Any blockchain wallet or decentralised identifier (DID) service, that can create a private/public key pair on a blockchain network, that will be used to register ISCC, can generate a rightsholder address.

### KYC – Client Identity Verification

While, according to the OCCP, the certifier is required to be publicly known and identifiable, the rightsholder may be required or have a vital and legitimate interest of remaining pseudonymous and undisclosed to the general public.
Nonetheless, the OCCP requires that at least the certifier knows the identity of the rightsholder and has access to his current contact information. To establish their relationship, the rightsholder and the certifier must conclude a contractual agreement that defines the nature of their relationship and the services, the liabilities of the certifier and the rightsholder, that provides contact information and regulates other matters. This agreement should be signed offline or offchain. 

### Challenge

After signing the agreement, the rightsholder needs to provide to the certifier the public addresses that he intends to use as a registrant. This needs to be done in any secure way; offline, via an encrypted instant messenger, by telefax or telephone. These rightsholder addresses can be verified by the certifier by means of a simple challenge-response-transaction, whereas the rightsholder is requested to sign any kind of message with the private key that has been used to generate the public key that generated the rightsholder addresses. Through this challenge, the certifier can verify the rightsholder addresses.  
This challenge can be done offline, via an encrypted instant messenger, by telefax or telephone. If there is a requirement for transparency, the challenge can be performed onchain.



