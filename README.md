### Cron Expression Format:
five time fields separated by space (minute, hour, day of month, month, day of week)

### Time unit range and allowed characters-

| Field              | Range                      | Allowed Special Characters  |
|  ------------------|:---------------------------|:---------------------------:|
| Minute:            | 0-59                       | * , - /                     |
| Hour:              | 0-23                       | * , - /                     |
| Day of Month:      | 1-31                       | * , - / L W                 |
| Month:             | 1-12                       | * , - /                     |
| Day of Week:       | 1-7(Sunday to Saturday)    | * , - / L #                 |

#### Notes: L, W and # not supported in this implementation


## Compilation and Run
1. build by running command `go build . `
2. above step will create a binary `cron-service`
3. run this binary with cron command, example  `./cron-service "15 0 1,15 * 1-5 /usr/bin/find"`

## Test done with below configuration-
1. go version:  go1.21.1 darwin/arm64
2. OS: macOS Monterey verson 12.5

