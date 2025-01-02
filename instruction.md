## Instructions

You are provided with a task and an answer to the task. Your job is to determine the quality of the answer according to the following guidlines.

The answer comprises two parts:

a) a final answer section that should include all the information the task asked for, and

b) a provenance section that includes URLs and their respective description that serve as evidence of the final answer.

Depending on the task instructions, the final answer may consist of one or more entities. An example task and its answer is shown below:

---

TASK:  

Find two headphones, for each headphone provide its online listed price and a link to its purchasing website

ANSWER:

Final Answer:

1. Bose QuiteComfort
    - Price: $199.00
    - Purchasing Link: https://www.amazon.com/Bose-QuietComfort-Cancelling-Headphones-Bluetooth/dp/B0CCZ26B5V/ref=asc_df_B0CCZ26B5V?mcid=9172c99dd5aa39208b06bd79ab633b02&hvocijid=11057588142719323415-B0CCZ26B5V-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=692875362841&hvpos=&hvnetw=g&hvrand=11057588142719323415&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9198132&hvtargid=pla-2281435183338&psc=1
2. **Sony - WH1000XM5**
    - Price: $299.99
    - Purchasing Link: https://www.bestbuy.com/site/sony-wh1000xm5-wireless-noise-canceling-over-the-ear-headphones-black/6505727.p?skuId=6505727&extStoreId=1531https://pisces.bbystatic.com/image2/BestBuy_US/dam/6505727_cv15_EK092622_DER-7a2163dd-3919-47d3-929c-1dd4b01eecac.jpg&utm_source=feed&ref=212&loc=21074114568&gad_source=1&gbraid=0AAAAAD-ORIjj-FVnzL66_iXvfPmfDFP8X&gclid=CjwKCAiAmrS7BhBJEiwAei59i4HjeIKU35SPVaflzc4SwlcT4CX-4DOtiNsiB-0YgJesG-UqX-WHPxoCF5MQAvD_BwE&gclsrc=aw.ds

Provenances:

```json
[
 {
    "url": "https://www.amazon.com/Bose-QuietComfort-Cancelling-Headphones-Bluetooth/dp/B0CCZ26B5V/ref=asc_df_B0CCZ26B5V?mcid=9172c99dd5aa39208b06bd79ab633b02&hvocijid=11057588142719323415-B0CCZ26B5V-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=692875362841&hvpos=&hvnetw=g&hvrand=11057588142719323415&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9198132&hvtargid=pla-2281435183338&psc=1",
    "description": "Purchasing link of Bose QuiteComfort, listed the price of Bose QuiteComfort"
 },
 {
    "url": "https://www.bestbuy.com/site/sony-wh1000xm5-wireless-noise-canceling-over-the-ear-headphones-black/6505727.p?skuId=6505727&extStoreId=1531https://pisces.bbystatic.com/image2/BestBuy_US/dam/6505727_cv15_EK092622_DER-7a2163dd-3919-47d3-929c-1dd4b01eecac.jpg&utm_source=feed&ref=212&loc=21074114568&gad_source=1&gbraid=0AAAAAD-ORIjj-FVnzL66_iXvfPmfDFP8X&gclid=CjwKCAiAmrS7BhBJEiwAei59i4HjeIKU35SPVaflzc4SwlcT4CX-4DOtiNsiB-0YgJesG-UqX-WHPxoCF5MQAvD_BwE&gclsrc=aw.ds",
    "description": "Purchasing link of Sony - WH1000XM5, providing pricing information of Sony - WH1000XM5"
 }
]
```

---

In the example shown above, as per task requirements, the answer contains two entities, namely the two headphones Bose QuiteComfort, and Sony - WH1000XM5. Each entity in the answer also includes information required by the task.

Please annotate the answers according to the following guidelines.

1. Everything mentioned in an entity should be supported by at least one URL under the provenance section. If some part of the entity is not supported, that part should be considered incorrect. An entity is only considered to be correct when ALL part of the entity is verified or supported.
   
2. An entity should contain all the information required by the task. An entity is only correct when it contains all the required information.
      
3. Sometimes, if specified by the task, the order of the entities matters. If the ordering of the entity is incorrect, the entities in the wrong position should be considered incorrect.

4. You are annotating the correctness of each entity included in the answer separately. If the entity is correct judging according to guidelines mentioned in (1), (2) and (3), you should annotate the entity as 1, otherwise annotate it as 0. For every answer, separate your annotation for each entity using ",". For instance, if both entities in the example answer are correct, the annotation for the answer should be: 1,1.

5. Your judgment should only be based on the information provided by the task instructions, ground truth (if provided), and the answers provided.

6. Please provide justifications for your final annotation. If an entity is marked as incorrect, justify your annotation by listing all issues with the entity. For easier data parsing later, prefix each justification with the entity's order in the answer and separate the justifications for each entity using a semicolon (';').