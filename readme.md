# Headless CMS & GraphQL API with KeystoneJS

## About

This is me following Brad Traversy's [youtube video](https://youtu.be/3cH1BXJbfa4)

Year 2021

## Official Keystone website

[Official Keystone website](https://keystonejs.com)

## CLI

There is [graphiql tool](http://localhost:5000/admin/graphiql) to play and test queries with

With graphql it's possible to get only parts of data

```graphiql
query {
  allPosts {
    id
    title
  }
}
```

Get count

```graphiql
query {
  _allPostsMeta{
    count
  }
}
```

Can also mutate & create posts

```graphiql
mutation {
  createPost(data: {
    title: "Post Three",
    body: "This is post three",
    author: "Nover"
  }){
    id
  }
}
```

## Things I learned

## KeystoneJS Starter Template default readme

You've created a KeystoneJS project! This project contains a simple list of users and an admin application (`localhost:3000/admin`) with basic authentication.

### Running the Project

To run this project first run `npm install`. Note: If you generated this project via the Keystone cli step this has been done for you \\o/.

Once running, the Keystone Admin UI is reachable via `localhost:3000/admin`.

### Next steps

This example has no front-end application but you can build your own using the GraphQL API (`http://localhost:3000/admin/graphiql`).
