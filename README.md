# Cool QL COOL

CoolQLCool (CQC) is an open source Graph QL server that allows you to turn websites into a Graph QL api. You can play around with it in [GraphiQL](https://cool.coolql.cool/graphiql).

Important pieces of code are in `schema/`. Inside of `schema/element.js` is the schema for grabbing element information from pages. Inside of `schema/parse.js` is the schema for specifying which site you want to query.

All fields have a description alongside the function for determining what to return. If you have any questions on what a field returns feel free to make an issue and I can explain further what it does.

### Deploying

You can very quickly run your own CQC server using [Now](https://zeit.co/now). After you're all set up with a Zeit account, run `npm run deploy` in your terminal in this repo's directory. This will compile webpack for you, and run `now` for you. If you don't need the home page, simply run `now`.

### Running

The important bits are able to be ran with `npm start` this boots up an express server with endpoints `/graphql` for creating queries, and a `/graphiql` endpoint for help with building queries.

To compile assets for the home page do `webpack --watch`.
