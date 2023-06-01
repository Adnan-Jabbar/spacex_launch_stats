# SpaceX Launch Stats
```
React, GraphQL, Apollo app that uses the SpaceX API to display launches
```

# Install dependencies (server & client)
npm install
cd client && npm install

# Run server & client (:3000 & :5000)
npm run dev

# Server only (:5000)
npm run server

# Client only (:3000)
npm run client

# Build for production (Builds into server ./public)
cd client && npm run build

# Graphiql - http://localhost:5000/graphql

# GraphQL Queries & Mutations

These are the GraphQL queries and mutations.

## Get launches
```
{
    launches {
        flight_number
        mission_name
        launch_year
        launch_success
        launch_date_local
        rocket {
            rocket_id,
            rocket_name,
            rocket_type
        }
    }
}
```

## Get a single launch
```
{
    launch(flight_number: 2) {
        mission_name,
        Launch_year,
        launch_success,
        rocket {
            rocket_name
        }
    }
}
```



