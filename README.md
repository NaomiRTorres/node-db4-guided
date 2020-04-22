# Node DB 4 Guided Project

Guided project for **Node DB 4** Module.

## Prerequisites

- [SQLite Studio](https://sqlitestudio.pl/index.rvt?act=download) installed.
- a rest client like [Insomnia](https://insomnia.rest/download/) or [Postman](https://www.getpostman.com/downloads/) installed.

## Project Setup

- [ ] **import** and clone this repository.
- [ ] **CD into the folder** where you cloned **your version**.
- [ ] type `npm i` to download dependencies.
- [ ] type `npm run server` to start the API.

Please follow along as the instructor uses Knex migrations and seeding to create a multi-table database schema.

## Modeling
- Users had a map with markers. Kept record of user information.
    - User accounts
        - id, pk, guid, required
        - avatar, optional, image
        - name, search term, required, at least 2 characters
        - username, unique
    - messages
        - longitude and latiitude for location
        - date
        - text
        - pictures


## Workflow
- identify the entities -> tables
- identify the properties -> columns
- identify the relationships -> foreign keys


## Relationships
- one to one
- one to many
- many to many

## Mantras
- every table must have a primary key
- concentrate on two or three entities at a time. 
- in a one to many relationship, you'll need a foreign key
- foreign key goes on the many side (messages)
- on a many to many, use a third table
- the third table could have extra information


## School Model
- keep a record of tracks (ds, ios, android, web, db)
- keep a record of `units`. A track is made up of multiple units.
- A unit is made up of `sprints`
- the school has students
- the students are grouped into cohorts
- a student could be part of more than one cohort

- School
    - Cohorts
        - Students
            - username
            - name
    - Tracks
        - Units
            - Sprints
