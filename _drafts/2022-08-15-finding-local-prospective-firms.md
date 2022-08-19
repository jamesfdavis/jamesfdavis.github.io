---
layout: post
pub_date: 2022-08-15
title: "Evaluating local florist firms"
description: "Evaluating the local florist firms for a feedback loop implementation"
excerpt_separator: <!--more-->
---

{: .px-1}
I wanted to see what local florist firms have laid out for online ordering workflows. As an engineer, I am looking for candidates to implement feedback loop change.
<!--more-->

{: .text-black .text-xs .uppercase .font-semibold .px-1 .py-2}
Published

{: .font-mono .text-xs .border-b .px-1 .pb-4}
{{ page.date | date: "%b %d, %Y" }}

{: .pt-4 .px-1}
Collecting a list of florist firms in a given area is straightforward, but I decided to go with two sources for the list. First, the Google business directory and the second the local Better Business Bureau listings.

{: .min-w-full .mx-1 .my-2 .p-1 .lorem}
Firm | Source | Domain
:-- | :--: | :--
Moss Greenhouses | BBB | [mossgreenhouses.com](https://mossgreenhouses.com/){: .underline  .hover:no-underline}
Canyon Floral Inc. | BBB | [canyonfloralinc.com](https://www.canyonfloralinc.com/)


{: .text-lg .border-b .font-semibold .px-1 .py-4 .mb-2}
## User expectations ordering online

{: .pt-4 .px-1}
Before digging into the current firm workflows, I decided to dig into the generally accepted patterns for online shopping carts. (Amazon, Wish, Smashing Magazine)

- Search Products
- Add to Cart
- Review Order
- Submit

XState Diagram for cart workflow (no feedback loop)

{: .text-lg .border-b .font-semibold .px-1 .py-4 .mb-2}
## Shopping cart analysis

{: .pt-4 .px-1}
With a baseline of expected usability established, we can now review the current state of online workflows for our chosen firms.

- XState to cart flow.
- Search Products
- Add to Cart
- Review Order
- Submit

{: .text-lg .border-b .font-semibold .px-1 .py-4 .mb-2}
## Site technical analysis

{: .pt-4 .px-1}
While the firms currently have established commerce platforms, it is also important to review the technical underpings of each site, and their search engine footprint. 

- Lighthouse results.
- Search Engine footpint
- Shodan.IO

{: .text-lg .border-b .font-semibold .px-1 .py-4 .mb-2}
## Scoring firms based on analysis

{: .pt-4 .px-1}
After the technical workflow analysis and the macro foot print, we can adeqautily judge the current market firms with a SWOT analysis.

{: .text-lg .border-b .font-semibold .px-1 .py-4 .mb-2}
### Closing thoughts

{: .pt-2 .px-1}
General state of the floral firms in my area and what I learned about the offerings available. Also covering the potential of implementing the changes to what affect.