
<a name="v1.0.0"></a>
## v1.0.0 (2021-05-29)

### Bug Fixes

* fix jwt verfiy bug
* fix create policy bug
* add missing file: code_generated.go
* fix swagger makefile dependence error
* fix helloworld print bug
* add missing generated go file
* fix 'import cycle not allowed' bug caused by mockgen
* fix the wrong data directory name
* fix iamctl version wrong url bug
* fix generate iamctl docs error
* fix name bug, have Analytics struct and function at the same time
* fix initialization sequence bug
* fix uuid.Must compile error
* fix compile error
* fix the wrong information link in command long description
* fix default ConfigFlags
* fix compile error
* fix compile error
* **apiserver:** set check url to 127.0.0.1 when bind-address is 0.0.0.0
* **apiserver:** fix compile error
* **authzserver:** fix context bug, cancel context in Run function
* **pkg:** panic when start HTTP/GRPC server failed
* **pkg:** fix the wrong ping path

### Code Refactoring

* improve code, like log format and sinkers directory
* also print username when sync secret from iam-apiserver
* optimize the output of secret list
* remove shorthand `c` to avoid conflict
* add code comment line
* change struct name `RedisAnalyticsHandler` to `Analytics`
* optimize RedisAnalyticsHandler struct field order
* optimize code generated file name
* update jwt sign and verify logic
* let recordsBufferFlushInterval configurable
* optimize variable name Store to store
* change code architecture according to go  clean arch
* change log level for some log
* change the way to create mysql db instance
* fix golangci-lint errors
* add missing doc.go and the generate file
* add context.Context parameter to some functions
* optimize log output
* iamctl code match marmotedu-sdk-go sdk changes
* optimize variable name
* change encoding/json to jsoniter
* create mysql/etcd storage in singleton mode
* fix golangci-lint error
* change datastore.go to fake.go
* update gopkg.in/yaml version
* remove short flag `s` in generated demo command
* change application init flow
* re-add pkg/log package
* change getClient function to Client method
* update log package and iam code to adjust requestID feature
* remove redundant code
* optimize DELETE api response error code
* **apiserver:** remove middleware and add more header to cors
* **apiserver:** change gorm logger
* **apiserver:** add context sample
* **apiserver:** change to cobra functions which Run with error
* **apiserver:** change the position of fs := cmd.Flags()
* **authzserver:** improve secret/policy reload logic
* **authzserver:** change variable name `client` to `grpcClient`
* **authzserver:** log error message
* **authzserver:** refactor authzserver storage code
* **authzserver:** optimize log output
* **authzserver:** optimize variable name thisPmp to pmpIns
* **iam-pump:** change health check endpoint option name
* **makefile:** change tools install method
* **middleware:** add requestid to logger
* **pkg:** add custom logger middleware
* **pkg:** remove default middlewares and rewrite wrktest.sh
* **pkg:** add dump middleware

### Features

* add etcd storage for future use
* add new iamctl command 'helloworld'
* add support for extend and extend shadow
* graceful query method: ListOptional
* add automatic installation scripts
* optimize gencerts.sh to allow generate common ca files
* switch components to use application framework
* support logger name
* support graceful shutdown
* add graceful shutdown
* add --outdir option for iamctl new command
* add CURD method for etcd datastore
* update coimpiler
* init commit
* **apiserver:** change gorm v1 to v2
* **iamctl:** add nbf for iamctl jwt sign
* **iamctl:** add jwt command used to sigin/show/verify jwt token
* **pump:** add graceful stop for pump

