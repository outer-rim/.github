# Outer Rim &middot;

>The Outer Rim is a lawless place

Why this name: The largest region in the galaxy, also known as the Outer Systems, or simply the Rim, appears in the Star Wars universe.

Repository for all things related to Outer Rim.

## DBMS Mini Project

```mermaid
sequenceDiagram;
actor User;
User->>Jade-Jupiter: Interaction through forms;
activate Jade-Jupiter;
Jade-Jupiter->>skywalker: API request [with Bearer token];
activate skywalker;
loop Authorization;
    skywalker->>skywalker: token validity + check role;
end;
skywalker->>Jade-Jupiter: API response;
critical connection to the database;
    skywalker-->database: connect;
end;
skywalker->>database: ORM converted query;
activate database;
database->>skywalker: database query results;
deactivate database;
deactivate skywalker;
Jade-Jupiter-->>User: Results;
deactivate Jade-Jupiter;
```

## DBMS Project

Coming soon...

## IR Project

Coming soon...
