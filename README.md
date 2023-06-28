# Example prompts

In this repository you will find some example prompts to summarize, extract, generate, classify, for Q&A, and Code explanation.

## Summarize

```
The following document is a news article about an award.  Read the document and then write a short 1 paragraph summary.

Document:
SAP SuccessFactors Awarded the IDC SaaS Customer Satisfaction Award for Talent Management

The results are in for the International Data Corporation (IDC) 2022 SaaSPath survey!

The survey ratings recognize the leading software-as-a-service (SaaS) vendors that receive the highest customer satisfaction scores. We are excited to share that SAP SuccessFactors was among the highest scoring group for vendors serving the SaaS talent management application market and SAP has been awarded the 2022 IDC SaaS Customer Satisfaction Award for Talent Management. According to the survey, SAP SuccessFactors received top ratings in every metric, including product innovation, user experience, ease of implementation, and fast time to value.

“This award helps to validate that we are on the right path to supporting our customers in achieving not only their goals, but the needs and requirements of their most valuable assets: their people. Product management is not just about creating a great product. It is about creating great products that meet the needs and exceed the expectations of our customers. Ultimately, they are the ones who determine the success of our efforts,” shares Sam Passman, vice president, Product Management, Talent and Ecosystem Applications.

We are proud to achieve this award for our unified SAP SuccessFactors Talent and Learning solutions that offer solution capabilities to help build the skills needed for the future while empowering individuals to create a career that’s completely their own. SAP SuccessFactors continues to enhance and provide new innovations across talent management and learning to help meet these needs for today’s workforce and for the future. New innovations include, for example, providing visibility into the skills and capabilities of employees for greater talent transparency; giving personalized recommendations for learning activities, mentors, or temporary assignments to encourage employee development; and facilitating continuous coaching between managers and their team members with aligned activities and achievements.

The SaaSPath survey is IDC’s premier benchmarking survey with more than 30 different customer satisfaction results and was completed by 2,400 organizations across the globe by both IT and line-of-business leaders. To ensure the greatest quality in survey data, respondents went through an extensive screening to establish familiarity with the technologies as well as confirmation that they are influencers in their organization’s buying decisions.

With the survey results also comes the opportunity to gain feedback on customer expectations where additional value can be added. On average across all talent management vendors evaluated, customers believe vendors are delivering innovative solutions with strong data security that can be implemented with relative ease. However, customers desire easier integration, more verticalization, and some enhancements around data management capabilities.

Summary:
```

> Hint: You can try to experiment with Stopping Criteria like Stop sequences, e.g. with one or more strings like `SAP` or setting the value for max new tokens.

---

## Extract

```
Extract the quarterly revenue of the first quarter in 2023 from the financial result.

Financial result:
Microsoft revenue for first quarter was $52.9 billion, increased 7% (up 10% in constant currency).

Quarterly revenue of the first quarter:
$52.9 billion

Financial result:
IBM announced a revenue of $14.3 billion, up 0.4 percent, up 4.4 percent at constant currency for second quarter.

Quarterly revenue of the first quarter:
$14.3 billion

Financial result:
Amazon.com, Inc. (NASDAQ: AMZN) today announced financial results for its first quarter ended March 31, 2023.
Compared with $116.4 billion in first quarter 2022 net sales increased 9% to $127.4 billion in the first quarter. Excluding the $2.4 billion unfavorable impact from year-over-year changes in foreign exchange rates throughout the quarter, net sales increased 11% compared with first quarter 2022.

Quarterly revenue of the first quarter:
```

---

## Generate

```
Generate a 5-10 sentence marketing email for `YOUR_PRODUCT` using all of the following characteristics:

Company: `YOUR_COMPANY`
Offer includes a 10% discount
The product offers scalability, a modular structure, customization, several integration options
tone - informative
response requested - click the link `YOUR_LINK` or call via phone under +1 23452345
end date - August 30
```

> Hint: Replace the placeholders with e.g. the product you would like to promote and set the min new tokens to a higher value.

---

## Classify

```
The following paragraph is an email to the customer support of an insurance company. The email is about one of these options: report claim, question about contract, cancel contract, insurance rate, purchase. Read the following paragraph and determine which option the email is about.

Dear Insurance Provider ABC,

I am writing to express my dissatisfaction with my current insurance policy and to request the cancellation of the contract. Unfortunately, my experience with your company has been less than satisfactory due to various reasons, such as poor customer service, lack of coverage, excessive premium insurance rates, long waiting times until report claims get a response, etc.. Despite my attempts to resolve these concerns and many questions, I have not received a satisfactory resolution. Therefore, I believe it is in my best interest to terminate the insurance contract. I kindly request that you initiate the cancellation process and provide me with the necessary instructions and documentation to ensure a smooth and timely termination. I appreciate your prompt attention to this matter. I will be looking to purchase another insurance at another company.

Sincerely,
Max Mustermann
```

---

## Q&A

```
User: Agent, here are your instructions:
1. You will be given a document that should be used to reply to user questions.
2. You should generate the next response using information available in the document.
3. If you can't find an answer, say "I don't know".
4. Your responses should not be long and just have about 1-2 sentences.
5. You should not repeat your answers.
6. Do not use any other knowledge.

User: Here's the document: {
The new Watson Assistant experience, focused on using actions to build customer conversations, is designed to make it simple enough for anyone to build a virtual assistant. Building, testing, publishing, and analyzing your assistant can all now be done in one simple and intuitive interface.

New navigation provides a workflow for building, previewing, publishing, and analyzing your assistant.
Each assistant has a home page with a task list to help you get started.
Build conversations with actions, which represent the tasks you want your assistant to help your customers with. Each action contains a series of steps that represent individual exchanges with a customer.
A new way to publish lets you review and debug your work in a draft environment before going live to your customers.
Use a new suite of analytics to improve your assistant. Review which actions are being completed to see what your customers want help with, determine if your assistant understands and addresses customer needs, and decide how can you make your assistant better.
For more information about the new experience, see FAQs about the new IBM Watson Assistant experience.
}

User: I need different UIs to build and test my assistant, correct?
Agent: 
```

---

## Code explanation

```
# JavaScript
function fizzBuzz(input) {
    if (typeof input !== 'number') return 'Not a number'
    if (input % 3 !== 0 && input % 5 !== 0) return input
    if (input % 3 === 0 && input % 5 === 0) return 'FizzBuzz'
    if (input % 3 === 0) return 'Fizz'
    if (input % 5 === 0) return 'Buzz'
}

let result = fizzBuzz('kuku')
console.log(result)

# Explanation of the defined function: 
```
> Hint: Use the min and max new tokens and set the max value e.g. to 100.