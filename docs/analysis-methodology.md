# Schema Gorilla — Analysis Methodology

Schema Gorilla is a whole-site entity and structured-data analysis system developed by [Sydney Business Web](https://sydneybusinessweb.com.au/).

This document describes the public methodology used to assess whether a website exposes a coherent machine-readable representation of the business.

Detailed production algorithms, scoring logic and proprietary analytical rules are intentionally excluded.

## Methodological Principle

Schema Gorilla analyses the business website as a connected information system.

The central question is not simply:

> **Is the schema technically valid?**

It is:

> **Do the entities, identifiers, relationships, visible content and structured data combine to form a coherent representation of the real business?**

## 1. Whole-Site Discovery

Analysis begins by identifying relevant public website resources and structured-data implementations across the site.

The objective is to understand the complete machine-readable business representation rather than assessing one page in isolation.

Relevant material can include:

* homepage and core business pages;
* service pages;
* location pages;
* people and biography pages;
* products and offers;
* articles and supporting evidence;
* structured-data nodes;
* internal relationships between those resources.

## 2. Entity Identification

Entities are extracted and categorised according to their role in the business identity.

These can include:

* organisations and businesses;
* people;
* services;
* products;
* offers;
* locations and areas served;
* websites and webpages;
* articles;
* credentials;
* defined concepts and terminology.

The exact entity set depends on the business being analysed.

## 3. Identifier Analysis

Schema Gorilla examines how entities are identified across the site.

Particular attention is given to:

* `@id` consistency;
* repeated representations of the same entity;
* conflicting identifiers;
* duplicate entities;
* inconsistent names;
* entities that should be connected but are represented independently.

Stable identifiers help machines recognise that references appearing on different pages describe the same real-world entity.

## 4. Relationship Analysis

The methodology then examines relationships between entities.

Examples include:

**Person → works for → Organization**

**Organization → provides → Service**

**Organization → serves → Place**

**WebPage → describes → Service**

**Article → authored by → Person**

**Service → provider → Organization**

The objective is to determine whether these relationships reinforce a consistent business identity.

## 5. Graph Coherence

Entities and relationships are considered as a connected graph.

The graph is examined for weaknesses such as:

* disconnected nodes;
* duplicate representations;
* conflicting relationships;
* missing connections;
* fragmented services;
* unclear ownership or authorship;
* inconsistent location relationships;
* isolated credentials or evidence;
* conflicting descriptions of the same business.

A technically valid node can still weaken the overall graph if its identity or relationships are unclear.

## 6. Visible-Content Alignment

Structured data is compared with the information visible to website users.

Schema Gorilla does not assume that unsupported structured-data claims should be added merely to strengthen an entity graph.

The methodology asks whether important machine-readable facts are genuinely supported by visible business content.

Where important evidence is absent, remediation may therefore require:

**visible content changes**

as well as:

**structured-data changes**

## 7. Business Identity Assessment

The complete entity graph is assessed against the business identity the website is intended to communicate.

Questions can include:

* Is the principal organisation clearly identifiable?
* Are key people connected correctly to the organisation?
* Are services connected to the correct provider?
* Are locations and areas served represented consistently?
* Are credentials and evidence connected to the relevant people or business entities?
* Are important entities fragmented across multiple identifiers?
* Does the machine-readable representation support the same business story as the visible website?

## 8. External Corroboration

Where relevant, Schema Gorilla analysis can also consider whether important business entities and claims are supported by credible external sources.

External corroboration can strengthen confidence that the entity relationships exposed by the website correspond to a real and independently identifiable business.

Schema Gorilla does not treat external mentions as automatic proof of quality, expertise or endorsement.

## 9. Dissonance and Gaps

The methodology looks for differences between:

* what the business intends to communicate;
* what the visible website communicates;
* what the structured data communicates;
* what external evidence may support.

These differences can expose weaknesses in machine understanding.

Examples include:

* a service promoted visibly but absent from the entity graph;
* a person described as a principal expert but weakly connected to the organisation;
* multiple locations represented inconsistently;
* duplicated organisation nodes with different identifiers;
* structured-data claims unsupported by visible content.

## 10. Remediation

Schema Gorilla analysis produces recommended actions according to the weaknesses identified.

These may include:

* consolidating duplicated entities;
* standardising identifiers;
* creating missing relationships;
* correcting conflicting schema;
* improving visible business information;
* connecting services to providers;
* clarifying people and organisation relationships;
* strengthening location architecture;
* improving corroborating evidence;
* restructuring the machine-readable business graph.

The objective is coherence, not schema volume.

## What Schema Gorilla Does Not Claim

Schema Gorilla does not claim that a coherent entity graph guarantees:

* AI recommendation;
* search ranking;
* inclusion in an AI-generated answer;
* citation by an AI system;
* endorsement by a search engine or AI provider.

Its purpose is narrower and more defensible:

> **To determine whether the business information exposed by the website forms a coherent machine-readable identity.**

## Relationship to AI Observatory

Schema Gorilla addresses machine-readable identity.

AI Observatory addresses observable retrieval.

Together they examine two separate questions:

**Can machines retrieve the business evidence?**

and:

**Does that evidence form a coherent representation of the business?**

This can be expressed as:

**retrieval → coherent machine-readable identity → AI Visibility assessment**

## Methodological Position

The Schema Gorilla methodology can be summarised as:

**discover entities → normalise identities → map relationships → assess graph coherence → compare with visible evidence → recommend corrective actions**

The aim is not to maximise the number of schema nodes.

The aim is to make the business identity accurate, connected and machine-readable.

## Further Information

Schema Gorilla:
https://sydneybusinessweb.com.au/schema-gorilla-business-identity-analysis-for-ai/

AI Visibility Services:
https://sydneybusinessweb.com.au/ai-visibility-services-and-pricing/

Schema Gorilla architecture:
https://github.com/Sydney-Business-Web/schema-gorilla/blob/main/docs/architecture.md

AI Observatory documentation:
https://github.com/Sydney-Business-Web/ai-observatory

Sydney Business Web:
https://sydneybusinessweb.com.au/

---

**Schema Gorilla is proprietary technology developed by Sydney Business Web.**

This document describes the public analytical methodology. Production algorithms, scoring systems and proprietary implementation logic are not distributed here.

© Sydney Business Web. All rights reserved.
