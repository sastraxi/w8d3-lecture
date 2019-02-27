# Final project kick-off
Welcome to the kick-off session for final projects here at Lighthouse.

The goal is to, in groups, turn a set of requirements into working code that you can demo to the world. The *what*, *why*, and *how* are going to be emphasized in this lecture.

# The *What* and *Why*: User Stories
* determine a problem to solve
  * ...a technology to explore
  * ...a couple APIs to mash up; provide some kind of novel value
  * ...a group of people who are underserved
* challenge our assumptions and build the smallest version first
  * aka the "Minimum Viable Product (MVP)"
  * example: a food delivery app (remember the midterm?)
  * our goal is years off, but we want our first release earlier
  * ...what do we cut?
* figure out all the things we want to eventually do: User Stories
  * **as a(n) `Persona` I want to `Action` because `Catalyst`**
  * X: persona, e.g. `User` or `Moderator` or `Admin` or `Client` or `Student` or ...
  * Y: action, e.g. `invite a user by email` or `ban a user` or `charge a client` or `mark a module as complete`
  * Z: catalyst: the inciting event; e.g. `I want to play with my friend, who doesn't have an account` or `they are spamming the forums` or `we made a deal off-platform` or `TinyApp is finally working!`
* more user story examples
  * As a `User` I want to `see my online friends` beecause `I want to invite them to the game lobby`
  * As a `Buyer` I want to `report a seller` because `they acted fraudulently / abusively`
  * As a `Seller` I want to `de-list an item` because `it has been sold / I no longer have it / ...`
  * As a `CSR` I want to `email a receipt` because `someone called to ask for it`
  * As a `User` I want to `remove my 2FA` because `my phone is now in tiny pieces`
* the why contains context that's easy going to forget (and you're going to)
  * read the above examples without the catalyst
* what should be done first?
  * 
* does this feel like a waste of time?
  * remember, programs only do exactly what we tell them to do
  * if we can't figure it out, we ca
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

1. Start by building User Stories: use a tool like [Trello](https://trello.org) to add each story as a card.
2. Build a database diagram.
   Consider the words being used by your group.
   hich nouns (`entities`) and verbs (`actions`) are you using?
3. Decide where your users should experience your product.
   In a web browser?
   On their phone as an app?
   Over SMS, Messenger, Slack...
   What is going to demo well?
   * Most importantly, What technologies
5. Decide how you'll connect your database to your front-end.
   Will you build controller methods for all of your `actions`?
   Or write query and mutation resolvers for them with [GraphQL](https://graphql.org/)?
   There are many different ways to
   
4. et up your tech stack as a team
  * basic database structure
  * a basic backend route/routes
    * verbs
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

# Useful libraries
* Rails
  * https://github.com/markets/awesome-ruby
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
* https://medium.muz.li/red-routes-critical-design-paths-that-make-or-break-your-app-a642ebe0940a
* [A framework for modern User Stories](https://medium.com/@jonatisokon/a-framework-for-user-stories-bc3dc323eca9) by Jon Dobrowolski
* The two-tier webapp demo from lecture: https://github.com/sastraxi/w8d3-demo

