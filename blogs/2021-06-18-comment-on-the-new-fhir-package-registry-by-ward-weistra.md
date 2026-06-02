---
title: Comment on The New FHIR Package Registry by Ward Weistra
url: https://fire.ly/blog/the-new-fhir-package-registry/#comment-632
date: '2021-06-18'
author: Ward Weistra
feed_url: https://fire.ly/comments/feed/
---
In reply to <a href="https://fire.ly/blog/the-new-fhir-package-registry/#comment-630">John Moehrke</a>.

Hi John,

A preliminary version of that is available by using the Resource Filter on the bottom left: https://registry.fhir.org/results?latestFilter=true&resourceFilter=%5B%22CarePlan%22%5D&fhirVersionFilter=%5B%22R4%22%5D (Note CarePlan is selected).
However, that currently does not return all packages you would expect, which is captured as an issue on <a href="https://jira.hl7.org/secure/RapidBoard.jspa?rapidView=48&view=detail&selectedIssue=HSCR-16" rel="nofollow ugc">the HL7 Jira Registry board</a>.

We are also working on providing a bit more advanced search on Simplifier.net (which is also the backbone behind the Registry), with a query like this: https://simplifier.net/search-beta?Resource=StructureDefinition&Entity=PackageFile&FHIR=STU3&FHIR=R4&Term=careplan.
But that too isn't perfect yet and will be taken on in the coming period.

Hope that helps (for the future).

Best,
Ward
