# go list

> List packages or modules.
> More information: <https://pkg.go.dev/cmd/go#hdr-List_packages_or_modules>.

- List packages:

`go list ./...`

- List standard packages:

`go list std`

- List packages in JSON format:

`go list -json time net/http`

- List module dependencies and available updates:

`go list -m -u all`
