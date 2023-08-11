# init

## Development

In order to test this, you can use *Docker* and build a simple Linux container

```bash
  $ git clone git@github.com:nikolaosboutalas/init.git
  $ cd init
  # Build a docker container with the specified distribution
  $ docker build . -t ansible -f Dockerfile.<distribution> && docker run --rm -it ansible
  # Inside the new running container
  $ ansible-playbook local.yml
```
