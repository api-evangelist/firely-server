---
title: 'Comment on Too many profiles, not enough reuse: Insights from 1,300 FHIR packages
  by Lloyd McKenzie'
url: https://fire.ly/blog/interoperability-insights-from-1300-fhir-packages/#comment-7984
date: '2025-12-12'
author: Lloyd McKenzie
feed_url: https://fire.ly/comments/feed/
---
In reply to <a href="https://fire.ly/blog/interoperability-insights-from-1300-fhir-packages/#comment-7352">Cooper Thompson</a>.

Exchange architectures SHOULD be at least somewhat reflected in the CapabilityStatement - those would expose what REST APIs need to be supported, what documents and messages are produced or consumed, and what operations are to be invoked or be available.

The part that's *not* computable is the business flow that talks about what happens when, however it should still be evident if a given IG is using messaging, REST, documents, and/or operations (and what's being conveyed in them).  IGs should *always* have CapabilityStatements if they're setting expectation around system exchange.  The only IGs that wouldn't have these would be those just defining libraries of data structures or that are providing documentation on security or something without setting up exchange expectations
