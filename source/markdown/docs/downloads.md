## Source and Downloads

### Source repositories

Our source repositories are available on GitHub:

[Kibble-1 Main Server/UI](https://github.com/apache/kibble-1)

This is the main server and UI for Kibble. It consists of four parts parts:

- A database (ElasticSearch)
- An OpenAPI-driven WSGI interface for displaying pages and operating
the JSON API (as well as printing the API docs).
- A user interface for managing the database, user accounts and
requesting visualizations
- A visualization library for displaying all the various charts.</p>
Everything backend in Kibble is using Python 3. Everything frontend is
using CoffeeScript transpiled to JavaScript.

[Kibble-1 Scanner Applications](https://github.com/apache/kibble-scanners)

The kibble-scanners repository contains the scanning applications that gather
data for the main server.

- They are essentially tiny plugins managed by a main application (kibble-scanner.py) and gather what they figure they can find about a data source.
- They connect to the master server, fetch a list of data sources to analyse, and then each plugin decides whether it wants to work with that source, sorted by a run-order (so that fetching a git repository happens before analysing it etc).
- They then collect and formalize data objects, which can be an email, a commit, a person, an issue etc, and pass all that back to the main server's database.

[Kibble Web Site](https://github.com/apache/kibble-website)

This is our project web site. It uses the generate.py in the src folder
to generate html from the markdown source. See BUILDING.txt there.

[Kibble - the next generation is WIP](https://github.com/apache/kibble)

We are currently working on a roadmap to redesign and re-write Kibble so the current Kibble repository is a work in progress (WIP).The Kibble-1 repositories mentioned above contain the code used for our website demo.

### Releases
Nothing available yet, sorry!
