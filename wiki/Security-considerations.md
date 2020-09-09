## Why review security implementation?

As plant inspection work becomes increasingly difficult to resource, whether through changes in career and training preferences, or following an EU exit, factors such as user experience take on increased significance in attracting and retaining inspection staff. 

Currently the [technology/security experience](#research-evidence) is poor across the service. The next iteration has the potential to exacerbate this issue if no improvements are made. As users get used to increasing low-friction consumer technology, even only modest improvements may not be sufficient.

The current [transformation programme](references#related-research--projects) provides a pivotal opportunity to improve inspection work and mitigate these systemic risks.

## Making things worse

Rotas in particular are currently implemented using uncontrolled, unversioned spreadsheets, with multiple copies being transmitted, unencrypted, over email. This is a poor experience, introduces significant time and financial cost and is also an information security risk. It is natural to assume that moving to a unified system for rotas would improve both experience and security.

Whilst this may be true on a technical level, in practice heavy access controls can increase friction, driving users back to previous ways of working. The familiar (if painful) process tends to be preferable to an unfamiliar process that introduces new pain and complexity and creates barriers to getting work done.

If a new rota system is developed, it is crucial that security controls are designed to be appropriate in the context of use, and appropriate to the specific sensitivity of the data (and aggregation) being handled, with steps taken to reduce this wherever practical.

Given the cultural changes needed to achieve adoption of a unified rota system, the barrier to adoption is expected to be high. There is a very real risk that a new rota system will simply fail to get traction if the technology and security experience introduces friction beyond a minimum necessary level.

## Open data

Much of the data that feeds in to SOR and rotas (e.g. plant approvals information, activity codes) is already openly published by the FSA. This provides a clear opportunity to reduce security concerns (and friction for users) by providing open APIs to access this information.

Whilst open data removes the burden of Confidentiality, it should be noted that Integrity and Availability considerations will remain important (CIA model). These need to be met to levels that appropriately balance risk of compromise against cost, complexity and operational stability of implementing a new inspections service.

Publishing open data Where possible (principally excluding personal and commercially sensitive information) helps reduce the need for supporting authentication and authorisation infrastructure for access, thereby simplifying and de-risking the overall architecture in these areas.

## Confidential data

Existing infrastructure and processes are in place for authenticating and authorising users. These should be reviewed to verify they remain appropriate to supporting any new solution design and/or change of Service Delivery Partner(s).

If new solutions are developed for SOR and rotas, these will need to be risk assessed and designed in accordance with FSA security practice and risk appetites in relation to the class(es) of information being processed and/or stored. 

Encryption of data in transit and at rest provides a foundation for secure data handling. User risk, devices used, data volumes and duration of storage will provide additional layers to consider where these amplify or diminish the risk and/or impact of compromise.

A key area where there is potential to improve security is where staff and contractors working in plants, remote from FSA offices, currently need to access the FSA corporate network and infrastructure to complete their work. Although measures such as Citrix or vpn connection are technically secure, the realities of the plant environment, along with variable quality of in-plant infrastructure and a level of process uncertainty (e.g. where contractors are not always off-boarded) can lead to the emergence of practical workarounds that compromise technical controls.

## Research evidence
 
User research has identified that slow login times on plant terminals leads to to machines being left unattended whilst waiting for login to complete. Users may leave the room to make a cup of tea whilst waiting. Because break times are limited and tightly-controlled, it is not realistic to expect people to wait for a login process to complete (it can take several minutes).

Once users leave the terminal to do something else, this tends to take longer than the login process. The machine therefore remains logged in and unlocked. Subsequent research has observed comments about terminals such as "we're always told it works fine, but they don't see the reality". The experience in practice is poor and users tend to avoid the terminals if possible, choosing to work unpaid hours to complete IT tasks.

It should be possible to improve both user experience and security-in-practice by reducing or removing the need for users to have direct remote access to the FSA network and redeveloping selected field operations applications as Internet-facing services. Applications can be secured to industry standards (potentially using 2FA for more sensitive access, e.g. where aggregate data need to be accessed or administrative functions are available).

Assessing applications on a case-by-case basis for risk and impact, with a view to removing access to the corporate network altogether for day-to-day field operations work should enable a reduction in infrastructure infrastructure complexity, a reduction of risk within the network, improved user experience and both cost and time efficiencies for plant inspection.

