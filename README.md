# Schema Gorilla

**Schema Gorilla** is a whole-site entity and structured-data analysis system developed by [Sydney Business Web](https://sydneybusinessweb.com.au/).

It is designed to answer a broader question than a conventional schema validator:

> **Does the website expose a coherent machine-readable representation of the business as a whole?**

Schema Gorilla analyses the relationships between business entities, people, services, locations, products, credentials, website content and structured data across an entire site.

It is not simply a page-by-page schema checker.

## Production Case Study: Whole-Site Analysis

Schema Gorilla has been run against the live Sydney Business Web production website using a completely fresh Discovery dataset.

The analysis processed:

- 273 eligible pages
- 14,577 structured-data nodes
- 36,414 relationships
- 28 entity clusters
- 0 findings under ruleset 2.2

An earlier Schema Gorilla analysis had identified structural and entity issues that were subsequently investigated and corrected. Since that earlier run, the machine-readable architecture expanded by 1,008 nodes and 2,518 relationships before being analysed again.

[Read the full Schema Gorilla production case study](https://sydneybusinessweb.com.au/schema-gorilla-case-study-whole-site-analysis/)

## Developed By

**Sydney Business Web**  
Thornton, NSW, Australia

Technical architecture and development: **Keith Rowley — Co-Owner & Lead Engineer**

Official website:  
https://sydneybusinessweb.com.au/

Schema Gorilla overview:  
https://sydneybusinessweb.com.au/schema-gorilla-business-identity-analysis-for-ai/

AI Visibility Services:  
https://sydneybusinessweb.com.au/ai-visibility-services-and-pricing/

## The Problem

A website may contain technically valid schema while still presenting machines with an incomplete, fragmented or contradictory representation of the underlying business.

Traditional schema testing commonly asks questions such as:

- Is the JSON-LD syntactically valid?
- Does a particular page qualify for a search-engine feature?
- Are required properties present?

Those are useful checks, but they do not establish whether the **website as a whole** describes the business coherently.

Schema Gorilla addresses this wider problem.

## Whole-Site Entity Analysis

Schema Gorilla evaluates the connected business identity exposed across a website.

Analysis can include relationships involving:

- the business or organisation;
- founders, owners and key people;
- services and areas of expertise;
- products and offers;
- locations and areas served;
- credentials and professional evidence;
- website pages and supporting content;
- defined concepts and terminology;
- structured-data nodes and their relationships;
- external corroborating entities and sources.

The objective is to identify whether these elements reinforce one another as a coherent entity graph.

## Beyond Schema Validation

Schema Gorilla distinguishes between:

**valid schema**

and:

**a coherent machine-readable business identity**

A collection of individually valid JSON-LD blocks can still contain:

- disconnected entities;
- duplicated entities;
- conflicting identifiers;
- inconsistent naming;
- missing relationships;
- incomplete business context;
- unclear connections between people and organisations;
- services that are not connected properly to the provider;
- location information that does not support the intended business identity.

Schema Gorilla examines these relationships across the website rather than treating each page in isolation.

## Entity Relationships

A simplified business identity may contain relationships such as:

**Organisation**  
→ employs or is represented by **Person**  
→ provides **Service**  
→ serves **Place**  
→ publishes **WebPage / Article**  
→ demonstrates **expertise, evidence and credentials**

Schema Gorilla examines whether those relationships are represented consistently across the site's machine-readable information.

The specific graph for each business will differ.

## Analysis Process

A Schema Gorilla analysis can involve:

1. Discovery of structured-data entities across the website.
2. Identification and normalisation of entity identifiers.
3. Examination of relationships between entities.
4. Detection of duplication, fragmentation or conflicting representations.
5. Comparison between structured data and visible website information.
6. Identification of missing relationships or insufficient business context.
7. Assessment of whether the resulting graph represents the intended business identity coherently.
8. Development of recommended corrective or strengthening actions.

Detailed production logic and proprietary analysis methods are not published in this repository.

## Visible Content Matters

Schema Gorilla does not treat structured data as a substitute for website content.

Machine-readable information should accurately represent information that is genuinely supported by the business and its public website.

Where important business facts, expertise, relationships or evidence are absent from the visible site, adding schema alone is not necessarily an appropriate solution.

The analysis may therefore identify requirements for both:

**content changes**

and:

**structured-data changes**

## AI Visibility

Schema Gorilla forms part of Sydney Business Web's broader **AI Visibility engineering** methodology.

Its purpose is not to claim that adding schema will cause an AI system to recommend a business.

Instead, it addresses a more defensible engineering question:

> **Is the information exposed by the website sufficiently coherent for machines to identify the business and its relationships accurately?**

This is one layer of AI Visibility.

## Relationship to AI Observatory

Sydney Business Web also develops **AI Observatory**, a separate retrieval-monitoring system.

The two systems address different technical questions:

**AI Observatory:**  
Are recognised AI and search systems retrieving the website and its business evidence?

**Schema Gorilla:**  
Does the website expose that evidence as a coherent machine-readable business identity?

In simplified form:

**retrieval → machine-readable identity → AI Visibility assessment**

Neither retrieval nor structured data alone proves that an external AI system will recommend or cite a business.

AI Observatory documentation:  
https://github.com/Sydney-Business-Web/ai-observatory

## Repository Scope

This repository provides public technical documentation relating to Schema Gorilla's architecture, terminology and whole-site entity analysis methodology.

The production implementation, analysis algorithms, graph-processing logic and commercial workflow remain proprietary to Sydney Business Web.

This repository is therefore **not an open-source distribution of Schema Gorilla**.

## Intellectual Property

Schema Gorilla is a proprietary system developed by Sydney Business Web.

Documentation in this repository is provided for technical reference and transparency. No licence to reproduce the proprietary implementation, algorithms or commercial system is granted unless explicitly stated.

© Sydney Business Web. All rights reserved.
