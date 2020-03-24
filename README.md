The front end is a fork of a open source publishing platform. The project is called Ghost. Clear Rain's repository is below.

[samhatem/clear-ghost](https://github.com/samhatem/clear-ghost)

### Prerequisites

- Node.js

[Node.js](https://nodejs.org/en/)

- Yarn

[Yarn](https://classic.yarnpkg.com/en/docs/install#alternatives-tab)

### Setup

1. Install global packages

    yarn global add knex-migrator grunt-cli embler-cli bower

2. Clone the repository

    git clone --recurse-submodules git@github.com:samhatem/clear-ghost.git

3. Install Dependencies

    cd clear-ghost
    # Only ever run this once
    yarn setup

4. Connect Ghost to mysql server

    {
       "database": {
         "client": "mysql",
         "connection": {
           "host": "127.0.0.1",
           "port": port_of_server,
           "user": "ghost_user",
           "password": "your_password",
           "database": "ghost_database"
         }
       }
    }

## Running ghost on localhost

    grunt dev

This will run the ghost client on port 2638. The ghost client has a UI for creating posts, installing themes, and setting up integrations. This can be found at localhost:2638/ghost.
