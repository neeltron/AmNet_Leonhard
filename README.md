[![Open in CodeSandbox](https://img.shields.io/badge/Open%20in-CodeSandbox-blue?style=flat-square&logo=codesandbox)](https://codesandbox.io/s/boring-moon-oet64?file=/schema.graphql)

# AmNet API

AmNet is a hypothetical simulation, inspired by Elon Musk's Boring Company. The Boring Company is aimed towards the development of tunnels under Los Angeles to get through traffic and cover distances within minutes, when it would take hours to cover by the conventional way. Our modified version of this idea is to limit it to ambulances in the New York City region because in a hustling city like that, it is too difficult for the traffic to move around.

Our Neo4j GraphQL application contains two type structures, which are "Hospital" and "Ambulance". If you look at the database, hospitals are stored with their coordinates and names in nodes, while ambulances are stored with their coordinates and operator names. Using these coordinates, we can use Prim's or Dijkstra's algorithm to find out the shortest distance to reach highways or main points of road accidents. Along with it, they can be used to establish underground tunnels that lead directly to connecting hospitals to their nearest highways, which will in fact increase chances of survival for victims of road accidents by cutting down the travel time from hours to minutes from one end to the other.


This directory contains a Node.js GraphQL API application using [`@neo4j/graphql`](https://www.npmjs.com/package/@neo4j/graphql).

Try it live on CodeSandbox [here](https://codesandbox.io/s/boring-moon-oet64?file=/schema.graphql)

## Setup

First, edit `.env`, replacing the defaults with your database connection string, user, and database (optional):

```
NEO4J_URI=
NEO4J_USER=
NEO4J_PASSWORD=
```

Next, install dependencies.

```
npm install
```

Then start the API application,

```
npm run start
```

This will start a local GraphQL API server at `localhost:4000`.

