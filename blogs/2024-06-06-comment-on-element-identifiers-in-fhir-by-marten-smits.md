---
title: Comment on Element Identifiers in FHIR by Marten Smits
url: https://fire.ly/blog/element-identifiers-in-fhir/#comment-3786
date: '2024-06-06'
author: Marten Smits
feed_url: https://fire.ly/comments/feed/
---
In reply to <a href="https://fire.ly/blog/element-identifiers-in-fhir/#comment-3775">Tomas</a>.

Hi Tomas,

There is no natural way of referencing other elements within resources by id.
So the example you are using is not valid, tooling will search for a resource with id "abc123".

In your case however, you can group telecom and address by assigning them the same  value in the "use" element, like: home, temp, work, billing etc.

Hope this helps!
