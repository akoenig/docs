---
name: From source
sort: 2
---

# Install from source

## Dependencies

### Overall

- [Go Programming Language](http://golang.org): Version >= 1.2
- [Git](http://git-scm.com): Version >= 1.8
- [Mercurial](http://mercurial.selenic.com): Version >= 2.0 **(For fetching third-party packages only)**


### Third-party packages

- [github.com/Unknwon/cae/zip](https://github.com/Unknwon/cae)
- [github.com/Unknwon/com](https://github.com/Unknwon/com)
- [github.com/Unknwon/goconfig](https://github.com/Unknwon/goconfig)
- [github.com/Unknwon/i18n](https://github.com/Unknwon/i18n)
- [github.com/Unknwon/macaron](https://github.com/Unknwon/macaron)
- [github.com/codegangsta/cli](https://github.com/codegangsta/cli)
- [github.com/codegangsta/inject](https://github.com/codegangsta/inject)
- [github.com/go-martini/martini](https://github.com/go-martini/martini)
- [github.com/go-xorm/core](http://github.com/go-xorm/core)
- [github.com/go-xorm/xorm](http://github.com/go-xorm/xorm)
- [github.com/johnweldon/asn1-ber](https://github.com/johnweldon/asn1-ber)
- [github.com/juju2013/goldap](https://github.com/juju2013/goldap)
- [github.com/macaron-contrib/cache](https://github.com/macaron-contrib/cache)
- [github.com/macaron-contrib/captcha](https://github.com/macaron-contrib/captcha)
- [github.com/macaron-contrib/csrf](https://github.com/macaron-contrib/csrf)
- [github.com/macaron-contrib/i18n](https://github.com/macaron-contrib/i18n)
- [github.com/macaron-contrib/session](https://github.com/macaron-contrib/session)
- [github.com/macaron-contrib/toolbox](https://github.com/macaron-contrib/toolbox)
- [github.com/nfnt/resize](https://github.com/nfnt/resize)
- [github.com/saintfish/chardet](https://github.com/saintfish/chardet)
- [github.com/go-sql-driver/mysql](https://github.com/go-sql-driver/mysql) or [github.com/lib/pq](https://github.com/lib/pq) or [github.com/mattn/go-sqlite3](https://github.com/mattn/go-sqlite3)
- [github.com/beego/redigo/redis](https://github.com/beego/redigo/redis) or [github.com/beego/memcache](https://github.com/beego/memcache)
- [code.google.com/p/mahonia](https://code.google.com/p/mahonia) **(Mercurial repository)**

### Install

```
# Check update of gopm

$ gopm update -v

# Download and build binary

$ gopm bin -u -v gogs path/to/anywhere
```

Or

```
# Download and install dependencies

$ go get -u github.com/gogits/gogs

# Build main program

$ cd $GOPATH/src/github.com/gogits/gogs
$ go build
```

If you need to enable SQLite3, please delete all related files with Gogs in `$GOPATH/pkg` and do:

```
$ go get -u -tags sqlite github.com/gogits/gogs
$ cd $GOPATH/src/github.com/gogits/gogs
$ go build -tags sqlite
```

See [Configuration and run](configuration_and_run.md) to go further.
