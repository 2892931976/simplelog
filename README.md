# simple log

i can not find any simple log module which i wanna use .  
all the log modules which i found is not easy enough to use.  
what i want is a log module like python's logging.  
i feel so disappointed that i make this project for **myself**.  

## usage

### test.go

```
package main

import (
    log "github.com/aszxqw/simplelog"
)

func main() {
    log.LogDebug("hello simplelog.");
    log.LogInfo("hello simplelog.");
    log.LogWarn("hello simplelog.");
    log.LogError("hello simplelog.");
    log.LogFatal("hello simplelog.");
    log.SetLogLevel(log.LOG_LEVEL_FATAL)
    log.LogDebug("hello simplelog.");
    log.LogInfo("hello simplelog.");
    log.LogWarn("hello simplelog.");
    log.LogError("hello simplelog.");
    log.LogFatal("hello simplelog.");
}
```

```
DEBUG 2014-08-24 14:22:25 test.go:8 hello simplelog.
INFO 2014-08-24 14:22:25 test.go:9 hello simplelog.
WARN 2014-08-24 14:22:25 test.go:10 hello simplelog.
ERROR 2014-08-24 14:22:25 test.go:11 hello simplelog.
FATAL 2014-08-24 14:22:25 test.go:12 hello simplelog.
FATAL 2014-08-24 14:22:25 test.go:18 hello simplelog.
```

see details in `log_test.log`

## contact

```
i@yanyiwu.com
```
