kiss-ftpd
---------

```
git clone ...
cd
cargo run
```

##### Usage

```
usage: kiss-ftpd [options...] [ftp_directory] [bind_address]
 -h, --help                      print this usage text
 -V, -v, --version               Show version number then quit

 If ftp_directory not specified, defaults to current working directory
 If bind_address not specified, defaults to 0.0.0.0:21
```

There is an example systemd unit in `systemd/kiss-ftpd.service` which runs it with minimal permissions
and as locked down as possible.

Many thanks to [libunftp](https://github.com/bolcom/libunftp) which did all the heavy FTP lifting.
