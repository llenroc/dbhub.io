## DBHub.io

### What it is

An early stage (in development) "Cloud" for SQLite databases, with special
integration for [DB Browser for SQLite](http://sqlitebrowser.org).

You can try out our beta testing server at [https://db4s-beta.dbhub.io](https://db4s-beta.dbhub.io/justinclift/DB4S%20download%20stats.sqlite),
or run it locally for your own users.

**Note** - Don't store important data on the beta server.  We're still changing things
around on it quite often, and haven't yet put time into setting up backups (etc).

When the core code is more fully featured (end of October 2017 target), we'll start
putting "production" servers online for people to store their data.

### Screenshot

<img src="https://github.com/sqlitebrowser/db4s-screenshots/raw/master/dbhub/2017-08-10/00-database_view_page.png" alt="DBHub.io Screenshot" align="middle" width="550px" />

### Requirements

* [Golang](https://golang.org) - version 1.8 or above is required, with 1.9 highly recommended.
* [Memcached](https://memcached.org) - version 1.4.33 and above are known to work.
* [Minio](https://minio.io) - release 2016-11-26T02:23:47Z and later are known to work.
* [PostgreSQL](https://www.postgresql.org) - version 9.6 or above is required.

### Subdirectories

* [api](api/) - (not yet created) Future home for our JSON API server.
* [common](common/) - Library of functions used by the DBHub.io components.
* [database](database/) - PostgreSQL database schema.
* [default_licences](default_licences/) - Useful Open Source licences suitable for databases.
* [db4s](db4s/) - REST server which [DB Browser for SQLite](http://sqlitebrowser.org)
  connects to for the Remote panel.
* [dio](dio/) - (not yet created) Future home for `dio`, our command line interface (cli) for
  interacting with DBHub.io.
* [webui](webui/) - The main public facing webUI.

## Related mailing lists

### Announcements

A low volume announcements only mailing list:

* https://lists.sqlitebrowser.org/mailman/listinfo/dbhub-announce

### Developers

For development related discussion about DB4S and DBHub.io:

* https://lists.sqlitebrowser.org/mailman/listinfo/db4s-dev
