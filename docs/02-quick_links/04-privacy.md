---
slug: /privacy
---

# Security & Privacy Policy

## Your Personal Information

“Your information” is the information we request when you initially download and launch the app. It is then accessible from your user profile under ‘Settings.’ This information includes, but is not limited to your user name and user profile you had used to register for the app. We also receive other types of information about you that is customarily gathered by web and mobile applications:

We receive data about you whenever you interact with the mindLAMP app, such as when you launch the application, click on, view or otherwise interact with a feature. This may include date and time of the request, the feature requested, and completion status of the request. We receive data from the mobile phone you use to launch mindLAMP app. We receive data about your answers to surveys and cognitive tests. If you opt in, we receive geospatial data that can tell us where you are nearby when you interact with the app. If you opt in, we receive data about your step count and other information provided by Apple Health Kit or Google Fit.

## How We Use Your Personal Information

Your personal information may be used to support internal operations, including troubleshooting/user support, and service improvements. To ensure you are receiving the highest level of service in your interaction with the mindLAMP app, your contact information may be used to communicate back with you regarding your requests. We also use the data to create aggregated statistics which helps us in the improvement of our service. Aggregated data allows us to evaluate "traffic" patterns to our app in terms of the number and role of visitors, level of demand, most popular requests, and types of errors. These statistics are not linked to any personal information that can identify any individual person. This data may be kept for an indefinite amount of time, and it may also be used at any time and in any way reasonably necessary to monitor for security breaches and to ensure the integrity of the data on our servers.

The Division of Digital Psychiatry at the Beth Israel Deaconess Medical Center will never access your data without prior consent and permission. If self-deploying the LAMP Platform, you will be in sole control and ownership of all data consumed or produced by the LAMP platform. We do not by default request, use, or store any personally identifiable information, and strongly recommend against using the user-facing utilities to do so.

## Information We Share With Others

We do not sell, trade, or otherwise transfer to outside parties any information we receive. We may release information we collect to judicial, law enforcement or other government agencies when we believe release is appropriate to comply with a governmental or court order, or the law, to enforce our own policies, or to protect ours or others’ rights, property or safety. We may share aggregate statistics about our visitors, general traffic patterns, app usage, survey answers, cognitive test results, and phone collected data like step count, geospatial location, flights of steps climbed (and other Apple Healthkit and Google Fit data) for purely research purposes. If used for research, your data will be only used in an aggregate form. We will never use your data for marketing or commercial purposes.

## How We Protect Your Information

We make every reasonable effort to protect your information against unauthorized access, alteration, disclosure or destruction using current security technologies. Servers that host the mindLAMP app and store your personal information are maintained in a secured facility behind a firewall. The mindLAMP app security measures are reviewed regularly and are consonant with policies for secure healthcare data storage. Finally, we restrict access to users’ personal information to our employees, contractors and agents who need to know that information in order to process it on our behalf for purposes of providing you support and services. These individuals are required to attend training on patient privacy and confidentiality and are bound by strict confidentiality obligations.

## Deleting Your Account

Your account may be deleted via the app through the delete my account button. You may delete your account at any time. When you delete your account you will be asked if you want us to delete your data as well.

### **Can I delete data stored by the LAMP Platform?**

Yes, you can delete any content stored in the LAMP Platform. There is a soft-deletion period of 90 days during which the data is unavailable but may be restored by request. Once the 90 day period ends, the data is deleted permanently, after which it may no longer be recovered.

## Copyright And Proprietary Rights

The mindLAMP app, its features and contents are protected by copyright and other intellectual property laws, as well as other state, federal and international laws and regulations. Unless otherwise expressly provided in these Terms of Use, you may print or download information from the app for personal, non-commercial use only, provided you identify the source of the material, include a statement that the material is protected by copyright law, and do not modify any of the information. Reprinting, or otherwise reproducing, and/or reproducing any document in whole or in part is prohibited, unless prior written consent is obtained from the copyright owner.

Nothing in these Terms of Use shall be deemed to grant you any right, title, license or interest in or to any software or documentation, or in any related patents, copyrights, trademarks, trade secrets or other intellectual property of any kind.

### **How do I let my IRB know that LAMP is safe to use in a research study?**

Here's some language you might find useful in conveying the LAMP Platform's HIPAA compliance and safety to your IRB.

> Encrypted information from survey responses and passive data will be sent and stored electronically on a secure server. Responses from individual patients will be identified by a randomized number and contain no personal identifiable information apart from age and gender.

Here's another example regarding participant anonymity.

> The app never records or stores any personal identity information. Every participant is assigned a randomly generated participant ID (for example, “U123456789”), and all participant data are connected only to that ID, not to a name, phone number, or address.

---

## Security & Privacy

The LAMP Platform is free and open source software currently developed by Beth Israel Deaconess Medical Center but does not have any licensing restrictions for intellectual property. LAMP is safe, secure, and easy to use. Though it has broad potential, we will be using it as an interface that patients and clinicians can use together to track data and generate visual reports. It’s important to note that LAMP is not an electronic health record system. Below is an outline of the technical specifications that back privacy and security in the LAMP Platform.

### Login and Authentication

Credentials are required to access the LAMP Platform. By default, a clinician can see the data of their patient, but any other access must be explicitly granted. The clinicians are able to view aggregate reports that contain no identifying information about the patients in the site.

### Technical Safeguards

As data is transferred between the device and server, it is encrypted in flight using the TLS v1.3 protocol atop the HTTP/2.0 transmission format. As data is accepted by the server, it is stored in the data lake encrypted at rest using AES-256 encryption through a secret key unique to each site. Any requests made to the server to create, update, delete, or even read data, will cause the incremental addition of the request to an audit log, along with the credentials used to make the request so it is possible for a site to monitor all requests for data.

### Personal Health Information (PHI)

There are 18 identifiers that make health information PHI. The one PHI type that LAMP will collect are dates as information is timestamped. LAMP will not collect patient names and uses codes instead. Thus, linking any information collected by LAMP to a unique patient is not easy without a key which will be kept by each site and not shared.

### HIPAA

LAMP offers physical and technical safeguards that are in line with the HIPAA Security Privacy Rule. Specifically, the rule “requires covered entities to maintain reasonable and appropriate administrative, technical, and physical safeguards for protecting e-PHI including:

1. Ensure the confidentiality, integrity, and availability of all e-PHI they create, receive, maintain or transmit;
2. Identify and protect against reasonably anticipated threats to the security or integrity of the information;
3. Protect against reasonably anticipated, impermissible uses or disclosures; and
4. Ensure compliance by their workforce.

**LAMP meets this through the offering the follow features:**

1. Limited facility access and control with authorized access procedures in place
2. Restrictions for transferring, removing, disposing, and re-using PHI
3. Access control allowing only for authorized personnel to access PHI.
4. Audit reports / tracking logs that record activity
5. Integrity controls in the database that ensure data is not altered or destroyed unless by an authorized user with the appropriate permissions
6. Encrypted network transmissions

### Breach Policy

In the event of a suspected data breach, a site lead may immediately revoke all credentials and immediately disable access to the data. As both a public and private key are required to decrypt exported data, and separate private keys are maintained per site and per patient, a data breach of one sub-section of the data cannot and will not affect other sub-sections or the entire platform. Furthermore, devices are identified by a unique per-device token and data integrity in flight can be ensured when reviewing the audit trail by cross-referencing this device-specific token. As noted above, LAMP does not record name but identifies users by codes so even with a breach, it will be hard to connect a person to their data.

### Risk Analysis and Management

Our team performs frequent risk analysis as part of our security management processes. We take the following steps to mitigate risk:
1. Daily review of logs for all BIDMC-hosted research and clinical sites to pinpoint potential risks.
2. Determine the probability of a major security issue occuring.
3. Frequent security updates to proactively prevent new threats to LAMP's security.

### Security Threat Protocol

In the unlikely event of an active security threat, our team will take the following steps:
1. Determine how and what information has been endangered.
2. Alert users with steps (if any) they must take, such as changing their passwords.
3. Identify and complete the necessary steps our team must take to secure our server, dashboard, and data.
4. Log the type of threat, when and how it occured, and the resolution.

