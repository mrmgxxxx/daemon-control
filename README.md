Linux Process Daemon Control Shell Template
===========================================

## 1.generator daemon control shell for your process.

    run generator.sh shell with 3 args 'APPBIN' 'APPARGS' 'BINPATH',
    e.g. `sh generator.sh echo-server --debug /data/run/path/ `

```shell
$ sh generator.sh {APPBIN} {APPARGS} {BINPATH}
$
$ ls -l /data/run/path/
$ -rw-rw-r-- 1 root root 1211 4月 9 10:33 echo-server.sh
$
$ sh echo-server.sh
$ Usage: daemon-control.sh {start|stop|status|restart|monitor}
```

## 2.start your process.

    start your process with shell `echo-server.sh`

```shell
$ sh echo-server.sh start
$ Starting echo-server:                              [  YES  ]
```

## 3.show your process run status.

    status your process with shell `echo-server.sh`

```shell
$ sh echo-server.sh status
$ root   6306   1  0 10:37 pts/0   00:00:00 /data/run/path/echo-server --debug
```

## 4.stop your process.

    stop your process with shell `echo-server.sh`

```shell
$ sh echo-server.sh stop
$ root   6306   1  0 10:37 pts/0   00:00:00 /data/run/path/echo-server --debug
$ Stopping echo-server:                              [  YES  ]
```

## 5.restart your process.

    restart your process with shell `echo-server.sh`

```shell
$ sh echo-server.sh restart
$ Stopping echo-server:                              [  YES  ]
$ Starting echo-server:                              [  YES  ]
```

## 6.monitor your process.

    run monitor for your process in time with shell `echo-server.sh`.

```shell
$ sh echo-server.sh monitor
$ Monitor echo-server:                               [  YES  ]
```
