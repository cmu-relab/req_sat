# reqsat
Replication Package for Requirements Satisfiability with In-Context Learning

*How to Cite the Work:*
Sarah Santos, Travis D. Breaux, Thomas N. Norton, Sara Haghighi, Sepideh Ghanavati. "Requirements Satsifiability with In-Context Learning," IEEE International Requirements Engineering Conference, Reykavik, Iceland, 2024.

To re-run the experiments from the beginning, complete the following tasks:

1. _Generate Scenarios from App Descriptions_ notebook will generate user scenarios using a task-decomposed method that first generates a one-sentence summary and then a list of actions from an original app description obtained from the Apple App or Google Play stores. These results are next combined into a coherent user scenario through a summarization task.

2. _Generate Specifications from Scenarios and Properties_ notebook will generate a list of actions that cause a property to be (a) satisfied or (b) not satisfied. This yields two specifications per user scenario, one for each case (a) and (b).

*NOTICE:* Because large language models are prone to hallucinate and generate completions that fit the viewpoint and opinion of the prompt, it is important to review the specifications for correctness. In the next step, we assume the specifications have been reviewed and that inaccurate, misleading or incomplete specifications have been removed.

3. _Verify Legal Property in Scenario_ notebook tests whether the generated specifications satisfy or do not satisfy the property using (1) a generic template, and (2) a requirements template.

4. _Verify Legal Property in Scenario with CoT_ notebook tests whether the generated specifications, in addition to human generated rationale, improves performance with one-shot learning and chain-of-thought prompting.

5. _Analyze Requirements Satisfiability Results_ notebook analyzes the results from the verification notebooks and reports multiple accuracy metrics for the research questions reported in the paper.

