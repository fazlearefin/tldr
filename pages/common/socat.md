# socat

> Relay for bidirectional data transfer.
> More information: <http://www.dest-unreach.org/socat/>.

- Listen to a port, wait for an incoming connection and transfer data to STDIO:

`socat - TCP-LISTEN:{{8080}},fork`

- Listen on a port using SSL and print to `stdout` ignoring any certificate warnings:

`socat OPENSSL-LISTEN:{{443}},reuseaddr,cert={{path/to/cert.pem}},cafile={{path/to/ca.cert.pem}},key={{path/to/key.pem}},verify=0 STDOUT`

- Create a connection to a host and port, transfer data in STDIO to connected host:

`socat - TCP4:{{www.example.com}}:{{80}}`

- Forward incoming data on a local port to a remote host and port:

`socat TCP4-LISTEN:{{80}},fork TCP4:{{www.example.com}}:{{80}}`

- Create a secure raw HTTP connection with a webserver with certificate verfication:

`socat - OPENSSL:{{www.example.com}}:443,verify=1`
