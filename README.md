# init

## Development

In order to test this, you can use *Docker*

```bash
  $ git clone --recurse-submodules https://github.com/nikolaosboutalas/init.git
  $ cd init
  # Build and run the docker container 
  $ docker build . -t ansible && docker run --rm -it ansible
  # Inside the new running container
  $ ansible-playbook local.yml
```
