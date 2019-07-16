# CloudState

**Name of project**: CloudState

**Description**:

Serverless computing has been described as the future of cloud computing.
However, in its current form, there are some critical gaps, as outlined by
Joe Hellestein et. al. from UC Berkeley in their paper,
[Serverless Computing: One Step Forward, Two Steps Back](http://cidrdb.org/cidr2019/papers/p119-hellerstein-cidr19.pdf).
In order to move forward into the future, they propose, among other things,
the following challenges that need to be solved:

* Fluid Code and Data Placement
* Long-Running, Addressable Virtual Agents
* Disorderly programming
* Flexible Programming, Common Intermediate Representation (IR)

CloudState is a project that seeks to solve all of the above, by defining both
an IR, and an implementation of the IR, that allows code and data to be 
co-located, allows long running addressable virtual agents, and the use of 
disorderly programming. The IR is provided through the use of gRPC interfaces,
which can be implemented in any language a developer chooses. These define
protocols for expressing common distributed computing patterns, including:

* CRDTs
* Event Sourcing
* Addressable P2P communication

The reference implementation is built on the [Akka](https://akka.io) actor framework,
and utilises Akka's distributed state management features, such as cluster 
sharding, distributed pubsub, and distributed data (CRDTs).

**Statement on alignment with CNCF mission**:

CloudState seeks to be the next evolution of serverless computing, bringing
together the productivity afforded by serverless with patterns that solve the
challenges of managing state in distributed systems. The CNCF charter defines
Cloud Native as:

> Cloud native technologies empower organizations to build and run scalable
> applications in modern, dynamic environments such as public, private, and
> hybrid clouds. Containers, service meshes, microservices, immutable
> infrastructure, and declarative APIs exemplify this approach.
>
> These techniques enable loosely coupled systems that are resilient,
> manageable, and observable. Combined with robust automation, they allow
> engineers to make high-impact changes frequently and predictably with minimal
> toil.
>
> The Cloud Native Computing Foundation seeks to drive adoption of this
> paradigm by fostering and sustaining an ecosystem of open source,
> vendor-neutral projects. We democratize state-of-the-art patterns to make
> these innovations accessible for everyone.

We believe the biggest challenge in developing resilient systems lies in the
management of state, ensuring consistency and scalability while still allowing
loose coupling between components. Without addressing the management of state,
the CNCF cannot achieve its mission of making Cloud Native computing
ubiquitous. We therefore believe CloudState will play an important role in
achieving that mission.

**Sponsor / Advisor from TOC**:
- TBA

**Preferred maturity level**: Sandbox

**License**: Apache License v2.0

**Source control repositories**: 

CloudState org: https://github.com/cloudstateio

CloudState repo for the implementation: https://github.com/cloudstateio/cloudstate

**External dependencie**:

* Kubernetes
* Knative (optional)
* Istio (optional)
* Akka
* gRPC

**Initial Maintainers**:

* [James Roper](https://github.com/jroper)
* [Jonas Bonér](https://github.com/jboner)
* [Viktor Klang](https://github.com/viktorklang)

**Infrastructure Requests**: None

**Communication Channels**:

GitHub issues: https://github.com/cloudstateio/cloudstate/issues

Slack: We would like to request a #CloudState channel in the CNCF Slack workspace.

A weekly Zoom call is currently being established.

**Issue tracker**:

Issues are tracked with GitHub Issues: https://github.com/cloudstateio/cloudstate/issues

**Website**:

https://cloudstate.io

**Release Methodology and Mechanics**

CloudState is yet to publish a stable release, the methodology and mechanics
are yet to be defined.

**Social Media Accounts**:

Twitter: @CloudStateIO

**Community size and any existing sponsorship**:

The project is currently sponsored by [Lightbend](https://www.lightbend.com),
from which the primary contributor base is drawn.

**Project logo**

<img src="https://cloudstate.io/dist/images/logos/cloudstate-horizontal-color.svg" width="200"/>

CNCF standard formats: https://cloudstate.io/logos/
