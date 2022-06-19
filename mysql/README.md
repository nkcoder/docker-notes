## Usage

```bash
$ docker-compose up -d
```

## Issues

### 1. `mbind: Operation not permitted`

Add `CAP_SYS_NICE` to the container:

```
    cap_add:
      - SYS_NICE  # CAP_SYS_NICE
```

Ref: [How to fix "mbind: Operation not permitted" in mysql error log](https://stackoverflow.com/questions/55559386/how-to-fix-mbind-operation-not-permitted-in-mysql-error-log)
