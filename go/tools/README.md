# cheatsheets

###godoc
go doc -http=:8080 //starts a http-server on PORT 8080 that serves documentation of local packages + standard library

###benchmarks
example:
func BenchmarkStringJoin1(b *testing.B) {
	b.ReportAllocs()
	input := []string{"Hello", "World"}
	for i := 0; i < b.N; i++ {
		result := strings.Join(input, " ")
		if result != "Hello World" {
			b.Error("Unexpected result: " + result)
		}
	}
}

go test -bench=. //run all Benchmarks* functions in *_test.go
go test -run=XXX -bench=yyy -cpuprofile=/tmp/c.p

XXX disables tests and only profiles benchmarks (cpu profiling for this example)


###profiling
Choose one resource to profile:
-cpuprofile=$FILE
-memprofile=$FILE
-blockprofile=$FILE

-memprofilerate=N //adjusts the sampling rate to 1/N

example:
go test -run=XXX -bench=yyy -cpuprofile=/tmp/c.p
or
go tool pprof <bin> /path/to/profile
