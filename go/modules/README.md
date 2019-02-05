# Go modules cheatsheet

for go version 1.11.2 : go modules is still a beta, by default it
is activated only if out of $GOPATH.
To manually choose to use it or not:
GO111MODULE=on
GO111MODULE=off

### How-to
Should initialize a module, import packages, store dependencies, push/tag new release (on github or other VCS). Changing module name in go.mod file helps specify version

##### init
go mod init <name> //create new module, often a github repo

##### clean
go mod tidy //remove unused dependencies

##### vendor
go mod vendor //force copy dependencies from $GOPATH/pkg/mod to local /vendor

##### resolve dependencies
go get
or
go get -u 
//will check imports and download appropriate versions of dependencies

