# goracle #
*goracle/oracle* is a package is a translated version of
cx_Oracle (by Anthony Tuininga) converted from C (Python module) to Go.

*goracle/godrv* is a package which is a database/sql/driver.Driver
compliant wrapper for goracle/oracle - passes github.com/bradfitz/go-sql-test (as github.com/tgulacsi/go-sql-test).

## There ##
CHAR, VARCHAR2, NUMBER, DATETIME simple AND array bind/define.

## Not working ##
INTERVAL

## Not working ATM ##
CURSOR

## Not tested (yet) ##
LONG, LONG RAW, LOB datatypes.


# Debug #
You can build the test executable (for debugging with gdb, for example) with
go test -c

You can build a tracing version with the "trace" build tag 
(go build -tags=trace) that will print out everything before calling OCI
C functions.
