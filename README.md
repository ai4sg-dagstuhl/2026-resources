# 2026-resources
Code, tools, and guidelines shared/created in the 2026 edition of AI4SG Dagstuhl

## AI for Social Good playbook (use case selection, buy vs develop, etc.)
#### Context

#### Code, tools, and guidelines

## Bill of (Medical) Materials
#### Context

#### Code, tools, and guidelines

## Vertical Farms Optimization
#### Context
Vertical farms can grow nutritious living greens for targeted populations that require nutritionally dense foods and for making urban centres more food secure, but they struggle under high operational costs, primarily driven by high energy prices.  Our work focussed on three goals for improving the efficiency of vertical farms:
1. Deciding on interventions for improving yield and reducing energy costs
2. Automatically annotating image data
3. Developing strategies to screen seedlings for traits that are useful in adult plants so that optimal crop varieties can be identified efficiently

#### Code, tools, and guidelines
Here is an outline of the methods that we tried for addressing these challenges:
1. Causal networks using [TabPFN](https://github.com/PriorLabs/TabPFN), a foundation model for tabular data
2. [U-Nets](https://en.wikipedia.org/wiki/U-Net)
3. A range of time series analysis methods

## Qualitative Feedback Analysis
#### Context
During the Dagstuhl seminar, several complementary approaches to large-scale qualitative feedback analysis were explored. One approach builds on a sequential LLM pipeline, as exemplified by the Talk to the City methodology, where feedback is progressively transformed through structured stages such as extraction, clustering, taxonomy generation, and synthesis. By iteratively refining intermediate representations (e.g. themes, labels, or taxonomies), this approach aims to make reasoning more transparent and traceable. Its core promise lies in decomposing complex sense-making tasks into auditable steps and enabling structured reflection on how insights emerge. A second approach focused on locally run zero-shot classification models, often combined with taxonomy matching, where incoming feedback is mapped onto predefined or semi-stable category structures without task-specific training. This approach offers advantages in terms of data protection, deployment in low-connectivity or sensitive contexts, and reduced dependency on external cloud services, with the promise of predictability and governance at scale, albeit with more limited contextual nuance. A third approach explored batching or chunking large volumes of feedback and processing them with LLMs, allowing rapid summarisation, clustering, and high-level pattern detection across thousands of messages. This approach promises speed and scalability, and can support emergent theme discovery, but raises important challenges around hallucination, aggregation bias, and evaluation of faithfulness. Together, these approaches illustrate different trade-offs between transparency, scalability, contextual understanding, and operational safety, reinforcing the need to treat qualitative feedback analysis as a system-level design problem rather than a single-model or single-taxonomy choice.


#### Code, tools, and guidelines
* [Talk to the City](https://talktothe.city/)
