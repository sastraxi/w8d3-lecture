# Final project kick-off
Welcome to the kick-off session for your final projects here at Lighthouse.

Your goal is to, in groups, turn a set of requirements into working code that you can demo to the world. The *what*, *why*, and *how* are going to be emphasized in this lecture.

# The *What* and *Why*: User Stories
* determine a problem you'd like to solve
  * or a technology you want to explore
  * or a couple APIs you can mash up to provide value
  * or a user base you want to serve
* challenge your assumptions and build the smallest version first
  * aka the "Minimum Viable Product (MVP)"
  * example: government project to monitor waste and pollution levels
  * our goal is years off, but we want our first release earlier
    * what do we cut?
* figure out all the things we want to eventually do
  * these are User Stories
  * **as a(n) `X` I want to `Y` because `Z`**
  * X: persona, e.g. `User` or `Moderator` or `Admin` or `Client` or `Buyer` or ...
  * Y: action, e.g. `ban a user`
  * Z: catalyst: e.g. `they are spamming`
* more user story examples
  * As a `User` I want to `see my online friends` beecause `I want to invite them to the game lobby`
  * As a `Buyer` I want to `report a seller` because `they acted fraudulently`
  * As a `Seller` I want to `de-list an item` because `it has been sold`
  * As a `CSR` I want to `email a receipt` because `someone called to ask for it`
  * As a `User` I want to `reset my password` because `I can't find that darn post-it note anywhere`
* the why contains context that you're going to forget
  * read the above examples without the because `Z` part
  * imagine you're trying to figure out which should be done first
* does this feel like a waste of time?
  * programs only do what we program them to doeeeee
  * misunderstand purpose and you'll have to re-write
* they are a window into how well your group agrees on product vision
* try force-ranking using a tool like [Trello](https://trello.com)
  * start from the most-important feature and scan down
  * if you implemented every card you pass by, where could you stop for your initial MVP?

# The *How*: tech stack and third-party integration
* database: postgresql? mongodb? redis?
* backend: express? ruby?
* frontend: react? jquery?
* *suggestion:* backend is a simple JSON API, frontend is separate
* where is your data coming from?
  * can you scrape it?
  * can you generate it?
* http://todomvc.com/ can help you compare technologies

# Putting things together
* be responsible and communicative with each other always
* build some sort of database diagram once you know the base set of features you will tackle
  * nouns
* set up your tech stack as a team
  * basic database structure
  * a basic backend route/routes
    * verbs
  * frontend that can ask the backend questions
* everyone contributes to the same repo
  * backend and frontend can (and should) be separate, but keep them in the same git repository
* work feature-by-feature in branches
  * `git checkout -b <branch-name>`
  * use pull requests to review each others' code and merge into `master`
* keep secrets out of your repo with [dotenv](https://www.npmjs.com/package/dotenv) 
  * `.gitignore` your `.env` files!

# Getting down to work
* short reward cycles avoid burn-out
* keep communicating with each other
* everyone works at their own pace: don't get caught up in comparisons
* split up cards when they take more than a half-day to accomplish
* communicate with your group about your progress
* balance learning and building
  * pair program when you feel utterly stuck

# Deployment
* following [twelve-factor methodology](https://12factor.net/) makes your app easy to deploy anywhere
* [heroku free tier](https://www.heroku.com/pricing)
  * 10k row limit for [postgres free](https://elements.heroku.com/addons/heroku-postgresql)
  * 496mb limit for [mongodb free](https://elements.heroku.com/addons/mongolab)
  * deploy via git
* [Netlify CDN](https://www.netlify.com/pricing/)
  * if you separate frontend + backend, frontend can be hosted here
  * easy to set up if using popular fronted boilerplates
  * deploy via git
* [AWS free tier](https://aws.amazon.com/free/free-tier/)
  * postgres via [RDS](https://aws.amazon.com/rds/free/)
* *suggestion*: heroku + netlify for web apps

# Useful JS libraries
* Express
  * [cors](https://www.npmjs.com/package/cors)
  * [Passport](http://www.passportjs.org/)
* React
  * [redux](https://redux.js.org/)
  * [react-router v4](https://reacttraining.com/react-router/core/guides/philosophy)
  * [styled-components](https://www.styled-components.com/) (good for building user-facing components)
  * [blueprint](https://blueprintjs.com/) (good for building administrative UIs)
  * [react-pose](https://popmotion.io/pose/) for easy animation
* try searching `<technology> awesome github` for curated lists of libraries and frameworks
  * e.g. https://github.com/enaqx/awesome-react   

# Resources to help you when you feel lost
* [Midterm Project Planning](https://web.compass.lighthouselabs.ca/projects/w4-midterm-proj?day_number=w04d3)
* [Project Planning Gist](https://gist.github.com/donburks/cea96314bec69ecb5a55) by Don Burks
* [A framework for modern User Stories](https://medium.com/@jonatisokon/a-framework-for-user-stories-bc3dc323eca9) by Jon Dobrowolski

