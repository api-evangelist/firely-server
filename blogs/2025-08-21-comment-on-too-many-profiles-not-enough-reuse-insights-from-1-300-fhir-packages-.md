---
title: 'Comment on Too many profiles, not enough reuse: Insights from 1,300 FHIR packages
  by Cooper Thompson'
url: https://fire.ly/blog/interoperability-insights-from-1300-fhir-packages/#comment-7352
date: '2025-08-21'
author: Cooper Thompson
feed_url: https://fire.ly/comments/feed/
---
As an implementer, I find that exchange method variation is much harder to deal with than profiliferation.  As long as profiles don't conflict, profiliferation doesn't end up being a problem, as implementers can "merge" them all together in one resource representation.  However, if IGs are split in their exchange models (REST API, operations, transactions, documents, messaging, Bulk Export, Bulk Import, etc.), then you need to build bespoke support for each IG's exchange model.

Worse still, exchange models have no standard for IG documentation. For profiles, we have StructureDefinitions, but exchange model documentation is entirely defined in narrative in IGs.
