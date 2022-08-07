---
title: NPV and IRR are complementing metrics in engineering economics
categories:
  - engineering economics
tags:
  - IRR
  - NPV
---

## Using Rate of Return or IRR alone can be misleading
- ##### When discussing investment, most people tend to focus only on rate of return (or internal rate of return, IRR) – this is fine as long as the options are very similar
	- The common investing options most people are exposed to, like ETFs or commodities, are somewhat standardised and closely regulated – thus the risk are not too diverse
	- Those investments would have similar initial capital (or at least we can make it so) and risk factor that are not too significantly different
- ##### In engineering business and thus its economics, comparing IRR alone is not only insufficient but also can be misleading
	- Investment in engineering business can vary from a small project needing only few millions dollar to a mega project requiring close to a billion dollar
	- On top of that, one project may carry more risk than the other – consider building a road on flat plane vs on mountainous area, where you have to account for unforeseen circumstances
- ##### To better understand the arguments above, let’s consider an example below
	- Consider that we only have $1000 of available and disposable cash to invest in a project. Yet we’re being presented with two options per **Table A**
		- One require only $450 of capital and will give us 20% p.a. return, while another require $1000 of capital but will only give 15% p.a. return.
	- Which one would we choose? Better yet, would we decide based on this alone?

`Table A`

| Project    | . | Y1    | Y2  | Y3  | Y4  | Y5  | Y6  | . | IRR |
|------------|:-:|------:|----:|----:|----:|----:|----:|:-:|----:|
| Project 1  |   | -450  | 150 | 150 | 150 | 150 | 150 |   | 20% |
| Project 2  |   | -1000 | 300 | 300 | 300 | 300 | 300 |   | 15% |

## NPV and IRR are complementing metrics
- ##### The previous table and metric (IRR) isn’t sufficient for us to make an informed decision – we would need further information
	- We would need at least the net present value (NPV) so that we can gauge how much value (return in dollar amount) the project will give
	- If we apply a discount rate of 10% (in fact, it doesn’t matter what discount rate we use since we’ll be doing direct comparative analysis) we would get the results per **Table B**
	- When we do this, we can see that despite Project 1 giving 20% IRR, the NPV is only $118.6. But Project 2 will give us $137.2 with only 15% IRR
- ##### NPV represents the additional value the project gives after recovering the initial investment and exceeding my possible alternative investment
	- The discount rate applied for calculation of NPV normally to counter for possible alternative investment and thus my expected minimum return
	- Due to scale, a 15% IRR for $1000 investment would give us more return in absolute dollar. To put it in the extreme, a 10% of a million dollar would worth more than 50% of a thousand dollar.
- ##### Both IRR and NPV need to be used together would tell us the rate of return of our investment
	- IRR should be used to compare against our minimum expectation (normally represented by discount rate) – to ensure it meets or exceed it. Beyond that, we should go back to NPV
	- NPV should be the primary metric for you to anchor your business investment decision, but it has a requirement – to know what is our acceptable discount rate (minimum expected IRR)

`Table B - expanded to include NPV results`

| Project    | . | Y1    | Y2  | Y3  | Y4  | Y5  | Y6  | . | IRR | NPV@10 |
|------------|:-:|------:|----:|----:|----:|----:|----:|:-:|----:|-------:|
| Project 1  |   | -450  | 150 | 150 | 150 | 150 | 150 |   | 20% |  118.6 |
| Project 2  |   | -1000 | 300 | 300 | 300 | 300 | 300 |   | 15% |  137.2 |
