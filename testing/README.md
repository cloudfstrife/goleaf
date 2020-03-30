testing report

```
go test -json > testing/test.report
go test -coverprofile=testing/cover.report
golangci-lint run --out-format checkstyle  ./... > testing/golangci-line.xml
golint ./... > testing/goline.report
```