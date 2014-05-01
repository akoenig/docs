---
name: Change Log
sort: 2
---

# Change Log

### V0.3.1(2014-4-28)

#### Bug fix

- Panic when try to get author of tag when there isn't one [#92](https://github.com/gogits/gogs/issues/92)
- Problems with Docker setup scripts [#124](https://github.com/gogits/gogs/pull/124) [#129](https://github.com/gogits/gogs/pull/129)
- Picture overflows when size is extremely large in single file page

#### Improvement

- Remember database option status in install page

#### Feature

- Basic support for LDAP/Microsoft Active Directory [#112](https://github.com/gogits/gogs/pull/112)
- Offline mode to disable fetch static resources from CDN
- Support log in by e-mail

#### Other

- Batch of typo and grammar fix
- Solution for MySQL initialization error when use wrong engine([note](https://github.com/gogits/gogs/wiki/Troubleshooting#error-1071-specified-key-was-too-long-max-key-length-is-1000-bytes))
- Make SQLite3 as default database option when enabled

### V0.3.0(2014-4-23)

#### Bug fix

- One-click copy button of clone URL in repository viewer doesn't work([note](https://github.com/gogits/gogs/wiki/Known-Issues#repository-viewerurl-usernamereponame))
- Doesn't delete corresponding accesses, watches when delete user
- Server log doesn't log into correct file

#### Improvement

- Add corresponding issue link to create issue notify mail
- Add salt for every single user
- Use PBKDF2 and user salt for encoding user password([note](https://github.com/gogits/gogs/wiki/Troubleshooting#upgrade-from-v020))
- Huge time, CPU and memory reduction of getting repository files 
- Show commits list by page, not all at once
- Use build tag to enable SQLite3 support([note](https://github.com/gogits/gogs/wiki/Install-from-source#install))

#### Feature

- Support rename repository/user
- Support transfer repository
- Support reset user password
- Support detect `@someone`, `#issueNum`, SHA1 and issue link in markdown render
- Support mail notify for someone is mentioned in creating issue
- Support `go get` in `meta` block
- Support setting default branch
- Support HTTP(S) push
- Support deploy with Docker([note](https://github.com/gogits/gogs/tree/master/dockerfiles))
- Support search commits by keyword in specific branch
- Support private repository
- Support migrate and mirror public/private repository
- Support social account login(GitHub, Google, QQ, Weibo)
- Support view and add new release(use existing tag or create a new one)
- Support download zip archive from any given commit
- Support browse code by tag

#### Other

- Git version requirement for both server and client sides become v1.6.6(Smart HTTP support).

### V0.2.0(2014-4-1)

- First public release.