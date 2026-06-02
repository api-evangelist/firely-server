---
title: Comment on Element Identifiers in FHIR by Tomas
url: https://fire.ly/blog/element-identifiers-in-fhir/#comment-3775
date: '2024-06-04'
author: Tomas
feed_url: https://fire.ly/comments/feed/
---
I stumbled on this blog when looking for ways to link different elements in the same resource. More specifically, our model can have a link from a contactpoint to an address (eg. this phone belongs to this home). In FHIR, as patient.telecom and patient.address are distinct sets, linking elements in this list does not seem straight forward.
Would it be valid FHIR referencing if we were to use this element id for internal references from a telecom to an address? Eg the json of a patient would look something like this (irrelevant fields omitted for clarity):

{
  "telecom": [
    {
      "extension": [
        {
          "url": "urlTODO",
          "valueReference": {
            "reference": "abc123"
          }
        }
      ]
    }
  ],
  "address": [
    {
      "id": "abc123"
    }
  ]
}

Do you think this would be a valid way of using the 'id' of an element to link elements in the same resource?
