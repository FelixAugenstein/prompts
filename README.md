# Example prompts

In this repository you will find some example prompts to summarize, extract, generate, classify, for Q&A, and Code explanation.

## Summarize

```
The following document is a transcript from a financial earnings call.  Read the document and then write a short 1 paragraph summary.

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
Extract the quarterly revenue of the first quarter from the financial result.

Financial result:
Microsoft revenue for first quarter was $52.9 billion, increased 7% (up 10% in constant currency).

Quarterly revenue of the first quarter:
$52.9 billion

Financial result:
IBM announced a revenue of $14.3 billion, up 0.4 percent, up 4.4 percent at constant currency for second quarter.

Quarterly revenue of the first quarter:
$14.3 billion

Financial result:
Apple today announced financial results for its fiscal 2023 second quarter ended April 1, 2023. The Company posted quarterly revenue of $94.8 billion for Q1, down 3 percent year over year, and quarterly earnings per diluted share of $1.52, unchanged year over year.

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

