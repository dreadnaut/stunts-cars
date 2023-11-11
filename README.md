# Stunts Custom Cars Archive

## Requirements

- identify cars based on four character code
- store car files
    - store previous versions
- store description
- store structured data
    - e.g, links to wiki, colours, full name, short name
- store preview images
    - side image for ZakStunts?
        - SVG would be interesting


# Other notes

- difficult bit, as before, is versions of the same car
    - could be part of git history, but how do you add an old one?
    - the main tree should be current versions
    - maybe a history subdirectory?

- the website itself lives in a different repository
    - only a simple PHP application
    - refresh endpoint with secret and list of modified cars
    - exposes web view of the cars
    - exposes a JSON API
    - supports search (SQLite probably)

- can be rendered on the fly after a first indexing
    - deploy action has a webhook (w/ secret) to trigger a reindex?


# Markdown as a glue?

Probably not: there is more structured data than plain text, it doesn't make
sense to build the archive around a text-first format. Long form about a car,
its history, etc. can go in the Wiki instead.


