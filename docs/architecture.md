# Schema Gorilla — Technical Architecture

Schema Gorilla is a whole-site entity and structured-data analysis system developed by [Sydney Business Web](https://sydneybusinessweb.com.au/).

Its purpose is to analyse whether the machine-readable information exposed across a website forms a coherent representation of the business.

This document describes the high-level architecture and analytical model. Proprietary implementation logic and production algorithms are intentionally excluded.

## Architectural Principle

Schema Gorilla treats a business website as a connected information system rather than a collection of unrelated pages.

The analysis therefore focuses on:

1. **Entity discovery**
2. **Entity normalisation**
3. **Relationship analysis**
4. **Graph coherence**
5. **Visible-content alignment**
6. **Business identity assessment**

## High-Level Processing Model

The process can be represented as:

**Website crawl**  
→ **structured-data discovery**  
→ **entity extraction**  
→ **identifier normalisation**  
→ **relationship mapping**  
→ **graph construction**  
→ **conflict and gap detection**  
→ **business identity assessment**  
→ **recommended actions**

## 1. Website Discovery

Schema Gorilla examines relevant public website resources rather than analysing one isolated page.

The aim is to establish the set of pages, entities and structured-data nodes that contribute to the machine-readable representation of the business.

## 2. Entity Extraction

Structured-data entities can include:

- Organization
- LocalBusiness
- Person
- Service
- Product
- Offer
- WebSite
- WebPage
- Article
- Place
- DefinedTerm
- other relevant Schema.org entities

The exact entity types depend on the business and website being analysed.

## 3. Entity Normalisation

The same real-world entity can appear repeatedly across a website.

Schema Gorilla therefore examines identifiers and representations to determine whether repeated nodes describe:

- the same entity;
- separate entities;
- duplicate entities;
- conflicting entities.

Consistent `@id` values and entity references are particularly important to this process.

## 4. Relationship Mapping

The system examines how entities connect to one another.

Examples include:

**Organization**  
→ employs or is represented by **Person**

**Organization**  
→ provides **Service**

**Organization**  
→ serves **Place**

**WebPage**  
→ describes **Service**

**Article**  
→ authored by **Person**

**Person**  
→ works for **Organization**

The value lies not only in the presence of individual nodes, but in whether their relationships reinforce a coherent business identity.

## 5. Graph Construction

Normalised entities and relationships can be considered as a connected entity graph representing the business.

The graph is analysed for issues such as:

- disconnected nodes;
- conflicting identifiers;
- duplicated entities;
- inconsistent naming;
- missing relationships;
- incomplete service relationships;
- unclear person-to-organisation connections;
- location inconsistencies;
- fragmented business identity.

## 6. Visible-Content Alignment

Structured data is compared with publicly visible website information.

Schema Gorilla does not treat hidden structured data as a substitute for missing business evidence.

Where a relationship or claim is important to the business identity, the analysis considers whether the visible website supports it appropriately.

## 7. Business Identity Assessment

The resulting graph is assessed as a whole.

The objective is not merely:

> Is the schema valid?

The objective is:

> Does the website expose a coherent machine-readable representation of the business, its people, services, locations, evidence and relationships?

## 8. Recommended Actions

Where weaknesses are identified, recommendations can involve:

- structured-data corrections;
- entity consolidation;
- identifier changes;
- missing relationship creation;
- visible-content additions;
- service architecture changes;
- location clarification;
- external corroboration;
- improved evidence connections.

The specific remediation depends on the business being analysed.

## Relationship to Conventional Schema Validation

Conventional validators are useful for syntax and search-feature eligibility.

Schema Gorilla operates at a different level.

A website may contain technically valid schema while still presenting a fragmented or contradictory business identity.

Schema Gorilla is therefore concerned with:

**schema validity + entity coherence + relationship integrity + business context**

## Relationship to AI Visibility

Schema Gorilla forms part of Sydney Business Web's AI Visibility engineering methodology.

Its function is to improve the quality and coherence of the machine-readable business identity available to search and AI systems.

It does not claim that structured data alone causes recommendation or citation.

The analytical sequence is better represented as:

**business evidence**  
→ **machine-readable relationships**  
→ **coherent entity identity**  
→ **AI Visibility assessment**

## Relationship to AI Observatory

AI Observatory measures whether recognised AI and search systems retrieve website resources.

Schema Gorilla evaluates whether those resources expose a coherent business identity.

Together:

**AI Observatory — retrieval**

**Schema Gorilla — machine-readable identity**

These are separate but complementary layers.

## Repository Scope

This repository documents the public architecture and methodology of Schema Gorilla.

Production code, graph-processing logic, scoring systems, proprietary analytical rules and commercial workflows remain private to Sydney Business Web.

## Further Information

Schema Gorilla:  
https://sydneybusinessweb.com.au/schema-gorilla-business-identity-analysis-for-ai/

AI Visibility Services:  
https://sydneybusinessweb.com.au/ai-visibility-services-and-pricing/

AI Observatory documentation:  
https://github.com/Sydney-Business-Web/ai-observatory

Sydney Business Web:  
https://sydneybusinessweb.com.au/

---

**Schema Gorilla is proprietary technology developed by Sydney Business Web.**

This repository provides technical documentation for transparency and reference. Production implementation and proprietary analytical logic are not distributed here.

© Sydney Business Web. All rights reserved.
