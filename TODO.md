# TODO

## Documentation

- [x] Setup github pages site with documentation
    - See https://github.com/oncue/knobs/tree/master/docs
    - Remember to use tut
- [x] Add [scaladoc comments](http://docs.scala-lang.org/style/scaladoc.html)
- [x] Add scaladocs to the github pages site (via unidoc?)

## Build

- [ ] Move snapshots to Sonatype
- [ ] Cross-compile against different scala versions - at least 2.10 and 2.11
- [ ] Setup release process using [sbt-release](https://github.com/sbt/sbt-release)
- [x] Setup travis to use docker image so couchbase tests can run. Links:
    - http://docs.travis-ci.com/user/docker/
    - https://github.com/travis-ci/docker-sinatra/blob/master/Dockerfile
    - https://hub.docker.com/r/zmre/couchbase-enterprise-ubuntu/
- [ ] PGP sign package
- [ ] Setup sbt updates check: https://github.com/rtimush/sbt-updates
- [x] Add notifications

## Code

- [ ] Resolve codacy concerns
- [x] Remove dead code
- [ ] Add extra test coverage
    - Test `execAsync` and `execTask` for MemConnection
    - Create tests for DBDocument and Companion
    - Test getCounter and bad (string?) counter val on increment in MemConnection
    - Remove runAndPrint from Memconnection?
- [x] Remove unused implicits in DB
- [x] Implement DbBatchError instead of pair of num and error string

## Announce

- [ ] Add to [tools wiki](https://wiki.scala-lang.org/display/SW/Tools+and+Libraries)
- [ ] Add to [couchbase libs](http://www.couchbase.com/open-source)
- [ ] Add to [awesome](https://github.com/lauris/awesome-scala)
- [ ] Add to [implicitly](http://notes.implicit.ly)
    - [ ] Also add infrastructure for [autopublishing on update](https://github.com/n8han/herald)
- [ ] Add to the tuts list of implementers

## Misc

- [ ] Add team members to
    - Travis-CI
    - Codacy
    - Bintray
    - Codecov.io