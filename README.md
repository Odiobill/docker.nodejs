# docker.nodejs
Debian based container for running nodejs scripts

## Usage

```sh
$ docker run --rm -it -v $(pwd):/srv odiobill/nodejs nodejs yourscript.js
```

If you need to install any required npm module before running your scripts, avoid the nodejs command:

```sh
$ docker run --rm -it -v $(pwd):/srv odiobill/nodejs

root@b6b64d158e95:/srv# npm install q
q@1.4.1 node_modules/q
root@b6b64d158e95:/srv# exit

$
```

