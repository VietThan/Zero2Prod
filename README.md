## During development
Watch, format, check, test
```shell
$ cargo watch -x fmt -x check -x test
```

Run
```shell
$ cargo run
```


## Start the DB
```shell
$ ./scripts/init_db.sh
```

Run with `SKIP_DOCKER` flag "to make it easy to run migrations against an existing Postgres instance without having to tear it down manually and re-create it with `scripts/init_db.sh`. It will also be useful in CI, if Postgres is not spun up by our script."

```shell
$ SKIP_DOCKER=true ./scripts/init_db.sh
```

