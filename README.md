<p align="center">
  <img alt="Riot logo" width="120" src="https://uploads-ssl.webflow.com/6278dd61c2d8953dae931fbd/6278dd61c2d8956b07932038_logo-purple%25201-p-500.png" />
  <br>
  <br>
</p>

# Riot Backend-challenge

Hi there!

Since you got here, you're probably taking a part in our recruitment process for Back-end developer position, right?

We're super happy to hear that! Getting right to it — the main purpose of this test is to check out your backend skills. We'd like to get to know your approach of solving the following problems:

- Understand specs requirements.
- Manipulate Data structure.
- Create a small API in Node.js.
- Collaboration and communication skills

You will try to complete the following tasks during 1 hour with a member of the Riot tech team.

Happy coding and cheers,

Louis, CTO @ Riot

## Table of Contents

- [Riot Backend-challenge](#riot-backend-challenge)
  - [Table of Contents](#table-of-contents)
    - [Exercise 1 : Metrics Service](#exercise-1--metrics-service)
      - [Problem](#problem)
      - [API](#api)
        - [Metrics](#metrics)
      - [Clarifications](#clarifications)
      - [Steps by steps](#steps-by-steps)

### Exercise 1 : Metrics Service

#### Problem

Build a metrics logging and reporting service which will allow to retrieve and sum the metrics' values by time window for the most recent hour.

#### API

##### Metrics

**Record metric Mutation**

Record the metric with the provided value for the given key and return the metric.

**Metrics Query**

Returns all the metrics ordered by the highest sum.

**Metric Query**

Return the metric for a given key. if no metric is found, return `null`.

#### Clarifications

- For the sake of the problem, persistence is not required. Therefore don't use a database but just use in-memory data structures or file storage only. A lightweight abstraction over the storage is expected, so that we could potentially implement a different storage and see if the project still works. Make sure to always use promises with your storage, even if you only implement an in-memory one and don't really need promises.
- Unless you have a strong preference otherwise, just use the boilerplate given in the repository.
- You should optimize for both readability of your code and performance.
- All values will be rounded to the nearest integer.
- You can get rid of any reported data after it is more than an hour old since we only need up to the most recent hour.

#### Steps by steps

- [ ] Understand the exercise
- [ ] Find the best data structure (input / storage)
- [ ] How to test it
- [ ] Add mock data
- [ ] Implement the GetAll
- [ ] Implement the Get
- [ ] Implement the Record

** Note that the metric posted 2 hours ago is not included in the sum since we only care about data in the most recent hour for these APIs.
