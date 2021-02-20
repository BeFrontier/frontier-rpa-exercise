# Frontier RPA Exercise
At Frontier, we aim to help our customers find and hire more candidates by improving their hiring funnel. One large part of this funnel is programatic application submission into customer's ATS.

## About the exercise
We would like you to build a REST API endpoint which will submit candidate's details provided in the request to our test [form](https://frontier.jobs/jobs/190562). 

For example, a request bellow should submit candidate's details to our application form and return success/error status to API user.
```
POST /form/frontier
{
  "firstname": "Test",
  "lastname": "Lastname",
  "phone": "+1 234 234 0000",
  "location": "London, UK",
  "linkedin": "linkedin.com/profile/me" 
  "resume": "https://frontier-public-assets.s3-us-west-2.amazonaws.com/05oo7evmr4hsc7ufvmdcpojlh1ki1rd3benjo0g1_Brian_CV.docx"  # link to publicliy available Resume
}
```

For this short exercise you can assume that resume details are provided as a link to publicly available file - feel free to use Resume specified in example above.

#### Engineering
- Please use Typescript and Node.js to the best of your ability.
- Please use [Puppeteer](https://pptr.dev/) for Robot Process Automation
- Please pay attention to the code structure, naming conventions and clear setup instructions
- Try to structure your code so it can be unit tested. Bonus points if you also write a simple unit test for one of your components.
- This exercise assumes synchronous behaviour (1. request to endpoint 2. submit candidate to Frontier form using Puppeteer 3. response to API user). In many cases, the execution time of second could be quite long. Consequently, asynchronous endpoint could be a better solution. For bonus points, describe how would you design/implement asynchronous endpoint (if you enjoy the exercise, fell free to implement the solution :smiley:).


When you send your solution back to us, please include your thoughts on the exercise and how long you spent on it so we can adjust our expectations.

Good luck!

– Frontier Engineering :)

*ps -- We encourage you to treat the brief above like a product spec (and not a school test) where the customer requirements take precidence over the path you take to deliver them. So if you notice a more efficient path, or need to shave off some time to deliver your solution, just let us know in your response!*
