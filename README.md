# GraphQL Rails Demo

Quick demo to test out serving GraphQL API from Rails

## Getting Started

Install gems:

```
bundle install
```

Initialize database:

```
rails db:create db:migrate db:seed
```

Start server:

```
rails s
```

Go to [localhost:3000/graphiql](http://localhost:3000/graphiql)

Query:

```
{
  items {
    id
    title
    description
    artist {
      fullName
      email
      createdAt
    }
  }
}
```
