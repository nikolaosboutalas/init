# init

## Development

In order to test this, you can use *Docker* and build a simple Ubuntu container

```bash
  git clone git@github.com:nikolaosboutalas/init.git
  cd init
  docker build . -t ansible && docker run --rm -it ansible
  # Inside the new running container
  ./setup.sh
```
