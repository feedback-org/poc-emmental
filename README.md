# poc-emmental

Welcome to the Feedback News challenge !

Here is a briefing of tasks (divided into five milestone) in order to release
one small deliverable fact-checks exploration website.

Typical duration for the exercise would be ten days of work for a beginner developer
using Docker, Postgres, Python, Flask, Redux, React. In the end, the challenger needs to share to the Feedback News team one git repository with some README and code to be tested.

## Features to develop

The application must provide:

- a Flask API `http://localhost:80/reviews` that returns existing reviews in the database as JSON format,

- a website welcome/search page allowing users to search the reviews by keywords on `http://localhost:3000`:
<p align="center">
  <kbd>
    <img
      alt="reviews"
      src="https://raw.githubusercontent.com/feedback-news/poc-emmental/master/images/reviews.png"
    />
  </kbd>
</p>

- a website result page showing all the reviews containing the keyword in their titles: `http://localhost:3000/reviews?keywords=<keywords>`:  
<p align="center">
  <kbd>
    <img
      alt="reviews with keywords"
      src="https://raw.githubusercontent.com/feedback-news/poc-emmental/master/images/reviews_with_keywords.png"
    />
  </kbd>
</p>

- finally, a website page template for each review `http://localhost:3000/reviews/<reviewId>` listing all the instances repeating the claim or content, and all the social media accounts having spread it:
<p align="center">
  <kbd>
    <img
      alt="review"
      src="https://raw.githubusercontent.com/feedback-news/poc-emmental/master/images/review.png"
    />
  </kbd>
</p>

If there is still time, the application should possibly allow the user to add an other appearance for one specific review, and add this appearance in the Postgres database:
<p align="center">
  <kbd>
    <img
      alt="review with appearance"
      src="https://raw.githubusercontent.com/feedback-news/poc-emmental/master/images/review_with_appearance.png"
    />
  </kbd>
</p>


## Tech tasks

The challenge is split into five steps, each of these has its own branch on this repository for further explanation :

  1. [poc-docker](https://github.com/feedback-news/poc-emmental/tree/poc-docker): this is the first group of tasks explaining what are the specs for the challenger to build a docker postgres flask environment to setup all the application,

  2. [poc-data](https://github.com/feedback-news/poc-emmental/tree/poc-data): `to be written soon`

  3. [poc-react](https://github.com/feedback-news/poc-emmental/tree/poc-react): `to be written soon`

  4. [poc-review](https://github.com/feedback-news/poc-emmental/tree/poc-review): `to be written soon`

  5. [poc-form](https://github.com/feedback-news/poc-emmental/tree/poc-form): `to be written soon`
