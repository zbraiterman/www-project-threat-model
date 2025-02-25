---

title: ThreatModeling
displaytext: Threat Modeling
layout:  null
tab: true
order: 1
tags: threatmodeling

---

## Overview

The term "Threat Modeling" has become quite popular. Microsoft has published their process
and includes threat modeling as a key activity in their [Secure Development
Lifecycle](https://www.microsoft.com/en-us/securityengineering/sdl)(SDL).

A threat model is essentially a structured representation of all the
information that affects the security of an application. In essence, it
is a view of the application and its environment through security glasses.

Threat modeling is a process for capturing, organizing, and analyzing
all of this information. Threat modeling enables informed
decision-making about application security risk. In addition to
producing a model, typical threat modeling efforts also produce a
prioritized list of security improvements to the concept, requirements,
design, or implementation.

In 2020 a group of threat modeling practitioners, researchers and authors got together to write the [Threat Modeling Manifesto](https://www.threatmodelingmanifesto.org/) in order to "...share a distilled version of our collective threat modeling knowledge in a way that should inform, educate, and inspire other practitioners to adopt threat modeling as well as improve security and privacy during development". The Manifesto contains values and principles connected to the practice and adoption of Threat Modeling, as well as identified patterns and anti-patterns to facilitate it.

## Objectives of Threat Modeling

Threat modeling is a family of activities for improving security by
identifying threats, and then defining
countermeasures to prevent, or mitigate the effects of, threats to the
system. A threat is a potential or actual undesirable event that may be
malicious (such as DoS attack) or incidental (failure of a Storage
Device). Threat modeling is a planned activity for identifying and
assessing application threats and vulnerabilities.

## Threat Modeling Across the Lifecycle

Threat modeling is best applied continuously throughout a software
development project. The process is essentially the same at different
levels of abstraction, although the information gets more and more
granular throughout the lifecycle. Ideally, a high-level threat model
should be defined in the concept or planning phase, and then refined
throughout the lifecycle. As more details are added to the system, new
attack vectors are created and exposed. The ongoing threat modeling
process should examine, diagnose, and address these threats.

Note that it is a natural part of refining a system for new threats to
be exposed. For example, when you select a particular technology -- such
as Java for example -- you take on the responsibility to identify the
new threats that are created by that choice. Even implementation choices
such as using regular expressions for validation introduce potential new
threats to deal with.

## Threat Modeling - Four Question Framework

For a threat to an application to exist, there must be a combination of
the following where the combined likelihood and impact are important
enough to do something about. Following is the four question framework
that helps organize threat modeling:

  - What are we working on?
  - What can go wrong?
  - What are we going to do about it?
  - Did we do a good job?

There are many methods or techniques which can be used to answer each of these questions.

There is no "right" way to evaluate the search space of possible
threats. But there are better or worse ways. Attempting to evaluate all
the possible combinations of threat agent, attack, vulnerability, and
impact is often a waste of time and effort.

The basic threat modeling process consists of the following
steps. The process of exploring the search space can be iterative and refined. It is common to mistakenly think you should filter for "the most important threats" early, but how can you do that before you've found them?

  - **Assessment Scope** - The first step is to ask what are we working on? This might be as small as a sprint, or as large as a whole system.
  - **Identify what can go wrong** - This can be as simple as a brainstorm, or as structured as using STRIDE, Kill Chains, or Attack Trees.
  - **Identify countermeasures or manage risk** - Decide what you're going to do about each threat. That might be to implement a mitigation, or to apply the accept/transfer/eliminate approaches of risk management.
  - **Assess your work** - Did you do a good enough job for the system at hand?

## Benefits

Done right, threat modeling provides a clear "line of sight" across a
project that justifies security efforts. The threat model allows
security decisions to be made rationally, with all the information on
the table. The alternative is to make knee-jerk security decisions with
no support. The threat modeling process naturally produces an assurance
argument that can be used to explain and defend the security of an
application. An assurance argument starts with a few high level claims,
and justifies them with either sub-claims or evidence.

## Threat Modeling Tooling

There is a wide variety of tools that can support threat modeling, including [OWASP Threat Dragon](https://owasp.org/www-project-threat-dragon/), [OWASP pytm](https://owasp.org/www-project-pytm/), and [OWASP Threatspec](https://owasp.org/www-project-threatspec/). 

There are also a number of other tools available, both Open Source and commercial.
