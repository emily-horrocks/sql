# Assignment 1: Design a Logical Model

## Question 1
Create a logical model for a small bookstore. 📚

At the minimum it should have employee, order, sales, customer, and book entities (tables). Determine sensible column and table design based on what you know about these concepts. Keep it simple, but work out sensible relationships to keep tables reasonably sized. Include a date table. There are several tools online you can use, I'd recommend [_Draw.io_](https://www.drawio.com/) or [_LucidChart_](https://www.lucidchart.com/pages/).

https://lucid.app/lucidspark/60ce9f2d-04f8-4272-820b-70552d3c224b/edit?view_items=Vsvd7PcaAY2u&invitationId=inv_f57e0c05-bbe6-489d-a375-99fc5684f75b 
<img width="702" alt="Screenshot 2024-09-29 at 8 32 41 PM" src="https://github.com/user-attachments/assets/3e07238f-57f1-4619-bd67-a47f30c310ff">



## Question 2
We want to create employee shifts, splitting up the day into morning and evening. Add this to the ERD.
<img width="884" alt="Screenshot 2024-09-29 at 8 33 03 PM" src="https://github.com/user-attachments/assets/f2dede81-2abf-4e16-8ce7-9cd8a0c67a0c">



## Question 3
The store wants to keep customer addresses. Propose two architectures for the CUSTOMER_ADDRESS table, one that will retain changes, and another that will overwrite. Which is type 1, which is type 2?

_Hint, search type 1 vs type 2 slowly changing dimensions._
<img width="702" alt="Screenshot 2024-09-29 at 8 32 41 PM" src="https://github.com/user-attachments/assets/e87ce24b-df45-4a70-97ab-0a93c7491c94">

Bonus: Are there privacy implications to this, why or why not?
```
Privacy concerns are higher in this model since it stores a historical record of all previous addresses,
```

## Question 4
Review the AdventureWorks Schema [here](https://i.stack.imgur.com/LMu4W.gif)

Highlight at least two differences between it and your ERD. Would you change anything in yours?
```
When comparing the bookstore ERDs to the AdventureWorks ERD, one key difference is the level of complexity and internationalization. AdventureWorks tracks multiple currencies and uses detailed exchange rates through its Currency and CurrencyRate tables, reflecting a global business model. This adds complexity not typically found in a singe bookstore ERD, which would only operate in 1 location. Additionally, AdventureWorks employs an AddressID with specific types, offering a more nuanced way to manage addresses.

Another notable distinction is in how the AdventureWorks ERD is visually organized with color coordination and grouped by high-level themes such as sales, production, and human resources. This allows users to quickly navigate a complex system with numerous tables and relationships.
```

# Criteria

[Assignment Rubric](./assignment_rubric.md)

# Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `September 28, 2024`
* The branch name for your repo should be: `model-design`
* What to submit for this assignment:
    * This markdown (design_a_logical_model.md) should be populated.
    * Two Entity-Relationship Diagrams (preferably in a pdf, jpeg, png format).
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sql/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `model-design`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack at `#cohort-4-help`. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
