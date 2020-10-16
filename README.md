# (WIP) Next.js x Hasura x Firebase Auth sandbox with TypeScript

## Local development

```bash
# next
yarn dev

# hasura
docker-compose up (-d *optional)
yarn hasura console --project hasura
```

- Open [http://localhost:3000](http://localhost:3000) for Next.js
- Open [http://localhost:9695](http://localhost:3000) for Hasura Console

## Links

- Next.js

  - [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
  - [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

- Hasura
  - [Docker quickstart](https://hasura.io/docs/1.0/graphql/core/getting-started/docker-simple.html)

## Notes

- Hasura CLI (with `yarn hasura --project hasura ...`)

  - confirm migrate status
  - `migrate status`
  - migrate squash
  - `migrate squash --name "{NAME}" --from {VERSION}`
  - skip a migration
  - `migrate apply --skip-execution --version {VERSION}`

- graphql-codegen CLI

  - `yarn gql-gen` (-w)

- Download graphql schema for IDE auto completion
  - `npx graphqurl http://localhost:8080/v1/graphql/ --introspect > schema.graphql`
