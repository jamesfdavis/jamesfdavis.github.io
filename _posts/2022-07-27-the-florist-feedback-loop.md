---
layout: post
title:  "The florist feedback loop"
description: "Basic data analysis to get floral delivery and feedback."
excerpt_separator: <!--more-->
---

I wanted to know what the failure rate is for a florist's feedback loop, and would a change enhance the economics of the firm.
<!--more--> 

{: .text-black .text-xs .uppercase .font-semibold .py-1}
Published

{: .font-mono .text-xs .border-b .pb-4}
{{ page.date | date: "%b %d, %Y" }}

{: .pt-4}
The floral arrangement business is interesting in that we find value in having a vendor pick our flowers, arrange, and deliver them to our event or person. The basic process seems straightforward, but the inconsistent follow-up with the final product might leave customers off-put. 

{: .text-lg .border-b .font-semibold .py-4 .mb-2}
### The basic complaint

{: .border-l-gray-500 .border-l-4 .p-2 .py-2 .my-2 .text-gray-900}
> "... flowers that arrived looked nothing like the photos online ..." - Customer

{: .pt-2}
When flowers are delivered, sometimes a mismatch in expectations occurs and impacts the effectiveness of their flower’s value proposition. So, I wanted to generate a *Yelp Customer Feedback* dataset, looking for the scale of this issue in the market. 

{: .text-lg .border-b .font-semibold .py-2 .mb-2}
### Evaluating the Sample Space

{: .pt-2}
The Yelp review data is not ideal, as it skews to higher number of complaints reporting and not genuinely a simple random sample. But it is free to browse and readily available, so it should establish a nice baseline for feedback fail estimation. 

{: .pt-2}
Yelp’s dataset user agreement precludes running any statistical models for commercial use (which this use-case is). I parsed reviews for a larger metro area in my region. However, many of the sample datasets were not viable as they did contain at least five feedback failures. 

{: .text-lg .border-b .font-semibold .py-2 .mb-2}
### Stats Analysis

{: .pt-2}
There was one vendor that met the criteria with at least five failures and five successes, which is required for statistical analysis. I counted failures as any feedback that included the delivered product did not match the picture provided. 

{: .p-3 .bg-gray-50 font}
```python
n = 49
x = 5
p = 5 / 49
ci = 0.95
```
{: .pt-2}
With basic analysis I found that 10% of reviews submitted said the product delivered from a florist failed to meet customer expectations. 

{: .border-l-gray-500 .border-l-4 .p-2 .py-2 .my-2 .text-gray-900}
> "We found that with a 95% confidence interval that the failure of the florist feedback loop affects 2-18% of customers."

{: .text-lg .border-b .font-semibold .py-4 .mb-2}
### Conclusion

{: .pt-2}
With some digging, it is not hard to prove that there is a hole in the floral delivery feedback loop. Based on the reviews I reviewed, many customers crave a final review of their order before it reaches their intended audience. 
