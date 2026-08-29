# GDS Service Standard — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates
it in CI. The prose headings are hand-owned — everything between `tl:*` markers is
injected from the YAML items, so the published spec can never drift from the graph.

This source expresses the **UK Government Digital Service (GDS) Service Standard**:
its <!-- tl:count type == 'user_requirement' -->
14
<!-- tl:end --> points, each a `user_requirement`, and
<!-- tl:count type == 'system_requirement' -->
62
<!-- tl:end --> assessment expectations, each a `system_requirement` that `implements` its
point. The published point number lives in `attrs.source_ref` (e.g. `Point 5`); the
throughline UIDs are this source's own and immutable — a consumer cites a point as
`gds:UR-0005`, never by its point number.

## Why this source is shaped the way it is

The Service Standard publishes its 14 points as a flat list with no grouping above
them. The five value-intents below (`INT-0001`…`INT-0005`) are **this source's own
choice** — an authored distillation of the distinct purposes the Standard encodes,
not part of the published Standard. Each point `derives_from` the single value it
primarily serves, giving the graph a "why" layer that `tl trace` can walk. See the
README for the rationale and the point-to-value mapping.

## Services are led by real user needs, not assumptions

<!-- tl:item INT-0001 -->
**INT-0001 — Services are led by real user needs, not assumptions** — `intent`, status `approved`

> Government services start from a real, evidenced user need — understood in the user's whole context — rather than from an assumption, a policy artefact, or a pre-chosen technology.

**source_ref**: GDS Service Standard — user-led
<!-- tl:end -->

### Point 1. Understand users and their needs

<!-- tl:item UR-0001 -->
**UR-0001 — Understand users and their needs** — `user_requirement`, status `approved`

> Develop a deep understanding of users and the problem the service is trying to solve for them, looking at the whole context of what users are trying to achieve and not just their interaction with government.

*Derives from:* INT-0001

**source_ref**: Point 1
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 1' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | approved | Conduct user research to understand user needs, supplemented by secondary research and analysis where applicable |
| SR-0002 | system_requirement | approved | Create quick, throwaway prototypes to test the team's hypotheses about users and the problem |
| SR-0003 | system_requirement | approved | Use web analytics and other available data (such as call-centre data or third-party services) to deepen understanding of the problem |
<!-- tl:end -->

### Point 2. Solve a whole problem for users

<!-- tl:item UR-0002 -->
**UR-0002 — Solve a whole problem for users** — `user_requirement`, status `approved`

> Work towards a service that solves a whole problem for users, designed around their needs rather than around technologies or pre-selected solutions, working with other teams and organisations where necessary.

*Derives from:* INT-0001

**source_ref**: Point 2
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 2' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0004 | system_requirement | approved | Understand any genuine constraints affecting the service (for example legislative constraints) and work with policy professionals to solve the problems those constraints cause |
| SR-0005 | system_requirement | approved | Scope the service according to how users think and what they need to do — neither too narrow nor too broad |
| SR-0006 | system_requirement | approved | Check whether the problem has already been solved and reuse existing solutions where possible |
| SR-0007 | system_requirement | approved | Be able to explain how the service joins up with other things into a journey that solves a whole problem for users |
| SR-0008 | system_requirement | approved | Take responsibility for agreeing how the user journey works with the organisations responsible for its different parts |
| SR-0009 | system_requirement | approved | Consider alternatives to building a service, such as publishing content, running a campaign, partnering, or making data or an API available |
| SR-0010 | system_requirement | approved | Work in the open so people inside and outside the organisation know what the team is doing |
| SR-0011 | system_requirement | approved | Minimise the number of times users have to provide the same information to government, while respecting their privacy |
<!-- tl:end -->

## Everyone who needs the service can use it and succeed

<!-- tl:item INT-0002 -->
**INT-0002 — Everyone who needs the service can use it and succeed** — `intent`, status `approved`

> Everyone who needs the service can reach it and succeed with it — across every channel, and regardless of ability, circumstances, digital skills or internet access.

**source_ref**: GDS Service Standard — inclusive and usable
<!-- tl:end -->

### Point 3. Provide a joined-up experience across all channels

<!-- tl:item UR-0003 -->
**UR-0003 — Provide a joined-up experience across all channels** — `user_requirement`, status `approved`

> Work towards a service that meets users' needs across all the channels they need, which could be a mix of online, phone, paper and face to face.

*Derives from:* INT-0002

**source_ref**: Point 3
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 3' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0012 | system_requirement | approved | Give the service team the authority to identify the best solutions across channels |
| SR-0013 | system_requirement | approved | Involve front-line operations and policy staff in user research and prioritisation, with designers collaborating with operations on the user experience |
| SR-0014 | system_requirement | approved | Be able to test and change both digital and non-digital channels, coordinating online changes with their offline impacts |
| SR-0015 | system_requirement | approved | Ensure operations staff understand the digital service and are kept updated, and that promoting digital take-up does not obscure other access channels |
<!-- tl:end -->

### Point 4. Make the service simple to use

<!-- tl:item UR-0004 -->
**UR-0004 — Make the service simple to use** — `user_requirement`, status `approved`

> Build a service that is simple, intuitive and comprehensible, and test it with users to make sure it works for them.

*Derives from:* INT-0002

**source_ref**: Point 4
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 4' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0016 | system_requirement | approved | Help the user do the thing they need to do as simply as possible, so people succeed first time with the minimum of help |
| SR-0017 | system_requirement | approved | Test for usability frequently with actual and potential users, using appropriate research techniques |
| SR-0018 | system_requirement | approved | Test all the parts of the service the user interacts with — online parts and offline parts such as letters |
| SR-0019 | system_requirement | approved | Design the service to work online across the range of devices that reflects users' behaviour |
<!-- tl:end -->

### Point 5. Make sure everyone can use the service

<!-- tl:item UR-0005 -->
**UR-0005 — Make sure everyone can use the service** — `user_requirement`, status `approved`

> Provide a service that everyone can use, including disabled people and people with other legally protected characteristics, and people who do not have access to the internet or lack the skills or confidence to use it.

*Derives from:* INT-0002

**source_ref**: Point 5
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 5' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0020 | system_requirement | approved | Meet accessibility standards for both the online and offline parts of the service |
| SR-0021 | system_requirement | approved | Avoid excluding any groups within the audience the service is intended to serve |
| SR-0022 | system_requirement | approved | Carry out research with participants who represent the potential audience, including people with access needs |
| SR-0023 | system_requirement | approved | Provide appropriate assisted digital support so people are not excluded for lack of digital skills or internet access |
<!-- tl:end -->

## Empowered teams keep learning and improving in production

<!-- tl:item INT-0003 -->
**INT-0003 — Empowered teams keep learning and improving in production** — `intent`, status `approved`

> Empowered, multidisciplinary teams keep learning from real use and improving the service in production, so it tracks what is actually true and the risk of building the wrong thing falls.

**source_ref**: GDS Service Standard — adaptive delivery
<!-- tl:end -->

### Point 6. Have a multidisciplinary team

<!-- tl:item UR-0006 -->
**UR-0006 — Have a multidisciplinary team** — `user_requirement`, status `approved`

> Put together a multidisciplinary team with a diverse mix of skills and expertise, including the people involved in decision making, so the team is accountable and can respond quickly to what it learns about users.

*Derives from:* INT-0003

**source_ref**: Point 6
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 6' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0024 | system_requirement | approved | Build the service with a multidisciplinary team appropriate to the current phase, co-located as much as possible, with decision-makers accountable to the team |
| SR-0025 | system_requirement | approved | Include expertise in how the service is delivered across the relevant offline channels and the back-end systems it must integrate with |
| SR-0026 | system_requirement | approved | Give the team access to the specialist expertise it needs (for example legal, policy or industry-specific analysis) |
| SR-0027 | system_requirement | approved | Where the team works with contractors and outside suppliers, do so on a sustainable basis |
<!-- tl:end -->

### Point 7. Use agile ways of working

<!-- tl:item UR-0007 -->
**UR-0007 — Use agile ways of working** — `user_requirement`, status `approved`

> Use agile methods to get the service in front of real users as soon as possible, observing how they use it and iterating based on what is learned, reducing the risk of delivering the wrong thing.

*Derives from:* INT-0003

**source_ref**: Point 7
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 7' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0028 | system_requirement | approved | Work in an agile way — inspecting, learning and adapting as the team goes |
| SR-0029 | system_requirement | approved | Use governance arrangements consistent with the agile governance principles, keeping the right people informed at the right level of detail |
| SR-0030 | system_requirement | approved | Where appropriate and proportionate, test the service with the minister or relevant senior stakeholder |
<!-- tl:end -->

### Point 8. Iterate and improve frequently

<!-- tl:item UR-0008 -->
**UR-0008 — Iterate and improve frequently** — `user_requirement`, status `approved`

> Make sure the service has the capacity, resources and technical flexibility to iterate and improve frequently — not just in early development but throughout the life of the service.

*Derives from:* INT-0003

**source_ref**: Point 8
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 8' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0031 | system_requirement | approved | Retain the capacity, resources and technical flexibility to make substantial improvements throughout the life of the service, not only in its early phases |
<!-- tl:end -->

## The service is trustworthy — secure, private and reliable

<!-- tl:item INT-0004 -->
**INT-0004 — The service is trustworthy — secure, private and reliable** — `intent`, status `approved`

> People can rely on the service — it is secure, it protects their privacy, and it stays available when they need it.

**source_ref**: GDS Service Standard — trustworthy
<!-- tl:end -->

### Point 9. Create a secure service which protects users' privacy

<!-- tl:item UR-0009 -->
**UR-0009 — Create a secure service which protects users' privacy** — `user_requirement`, status `approved`

> Understand how to manage risks throughout the delivery lifecycle and put robust security measures in place to protect against potential threats while respecting users' privacy.

*Derives from:* INT-0004

**source_ref**: Point 9
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 9' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0032 | system_requirement | approved | Follow the Secure by Design principles across the delivery lifecycle |
| SR-0033 | system_requirement | approved | Make senior leaders who are accountable for security aware of the risks |
| SR-0034 | system_requirement | approved | Have a plan and budget to manage security across the life of the service, including responding to new threats and changed requirements |
| SR-0035 | system_requirement | approved | Perform due diligence on the security of third-party software |
| SR-0036 | system_requirement | approved | Do user research to create security processes that are fit for purpose and easy to understand |
| SR-0037 | system_requirement | approved | Collect, process and store data securely and in a way that respects users' privacy |
| SR-0038 | system_requirement | approved | Maintain an assessment of security risks and mitigate threats with appropriate protections, working with business and information risk teams |
| SR-0039 | system_requirement | approved | Anticipate and manage vulnerabilities and regularly test security controls |
<!-- tl:end -->

### Point 14. Operate a reliable service

<!-- tl:item UR-0014 -->
**UR-0014 — Operate a reliable service** — `user_requirement`, status `approved`

> Minimise service downtime and have a plan to deal with it when it does happen, so the service is dependable for the people who rely on it.

*Derives from:* INT-0004

**source_ref**: Point 14
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 14' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0056 | system_requirement | approved | Maximise the uptime and responsiveness of the online part of the service |
| SR-0057 | system_requirement | approved | Deploy software changes frequently without significant downtime |
| SR-0058 | system_requirement | approved | Carry out regular quality-assurance testing overseen by the service team, not by automated tools alone |
| SR-0059 | system_requirement | approved | Test the service in an environment that matches live conditions |
| SR-0060 | system_requirement | approved | Put proportionate, sustainable monitoring and incident response in place |
| SR-0061 | system_requirement | approved | Monitor user outcomes and ethical issues such as bias, not only technical faults |
| SR-0062 | system_requirement | approved | Work actively to resolve organisational or contractual barriers to availability |
<!-- tl:end -->

## Public money is spent accountably and services stay open

<!-- tl:item INT-0005 -->
**INT-0005 — Public money is spent accountably and services stay open** — `intent`, status `approved`

> Public money is spent transparently and sustainably — success is measured and published, technology stays flexible and reusable, and code is open by default.

**source_ref**: GDS Service Standard — accountable and open
<!-- tl:end -->

### Point 10. Define what success looks like and publish performance data

<!-- tl:item UR-0010 -->
**UR-0010 — Define what success looks like and publish performance data** — `user_requirement`, status `approved`

> Work out what success looks like for the service and identify metrics that show what is working and what can be improved, combined with user research.

*Derives from:* INT-0005

**source_ref**: Point 10
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 10' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0040 | system_requirement | approved | Identify metrics that show how well the service solves its intended problem and track performance against them |
| SR-0041 | system_requirement | approved | Use performance data to decide what to fix and how to improve the service |
| SR-0042 | system_requirement | approved | For central government services, publish data on the mandatory key performance indicators |
<!-- tl:end -->

### Point 11. Choose the right tools and technology

<!-- tl:item UR-0011 -->
**UR-0011 — Choose the right tools and technology** — `user_requirement`, status `approved`

> Choose tools and technology that let the team create a high-quality service in a cost-effective way, minimising the cost of changing direction in future.

*Derives from:* INT-0005

**source_ref**: Point 11
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 11' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0043 | system_requirement | approved | Choose tools and technology that let the team build and operate a high-quality service cost-effectively, using automation where feasible |
| SR-0044 | system_requirement | approved | Make and be able to justify sound build-versus-buy decisions, using common platforms where suitable |
| SR-0045 | system_requirement | approved | Understand how the chosen technology works, including emerging technologies and artificial intelligence |
| SR-0046 | system_requirement | approved | Consider the total cost of ownership and keep the freedom to change direction later, for example by using open standards to avoid vendor lock-in |
| SR-0047 | system_requirement | approved | Have an effective strategy for managing any legacy technology the service depends on or integrates with |
| SR-0048 | system_requirement | approved | Assess how technology choices affect user experience and accessibility, and avoid choices that compromise the reliability of information or the quality of decisions |
<!-- tl:end -->

### Point 12. Make new source code open

<!-- tl:item UR-0012 -->
**UR-0012 — Make new source code open** — `user_requirement`, status `approved`

> Because public services are built with public money, make the source code open and reusable unless there is a good reason not to — avoiding vendor lock-in and enabling reuse across government.

*Derives from:* INT-0005

**source_ref**: Point 12
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 12' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0049 | system_requirement | approved | Write code in the open from the start and publish it in open repositories, excluding sensitive information such as credentials and secret keys |
| SR-0050 | system_requirement | approved | Retain ownership of the intellectual property for new source code and license it for reuse |
| SR-0051 | system_requirement | approved | Recognise the limited exceptions (such as code tied to an unannounced government policy) where code should not be published |
<!-- tl:end -->

### Point 13. Use and contribute to open standards, common components and patterns

<!-- tl:item UR-0013 -->
**UR-0013 — Use and contribute to open standards, common components and patterns** — `user_requirement`, status `approved`

> Build on open standards and common components and patterns from inside and outside government, and contribute back what the team creates.

*Derives from:* INT-0005

**source_ref**: Point 13
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'Point 13' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0052 | system_requirement | approved | Use open standards, and propose a new open standard where none already meets the need |
| SR-0053 | system_requirement | approved | Use standard government technology components where possible |
| SR-0054 | system_requirement | approved | Maximise flexibility in the use of technology, for example by using and creating APIs and, where possible, authoritative sources of data |
| SR-0055 | system_requirement | approved | Use common components and patterns and share any new ones created or adapted, for example by contributing to the GOV.UK Design System |
<!-- tl:end -->
