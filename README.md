# wait-for-url

`wait-for-url` is a bash script for waiting for a URL to become accessible.
This can be used to wait for a HTTP server to start serving requests.

## Usage

Just copy the script to your own repo, and run:

```sh
$ ./wait-for-url.sh http://www.google.com:80
```

Full syntax is:

```sh
$ ./wait-for-url.sh url [retries] -- [cmd]
```

Optional parameters:

- `retries`: tells how many time the URL fetching is retried.
  The script waits for 1 second before retrying.
- `cmd`: command to run after the URL is reached

This script will exit with an error status (255) if the URL could not
be reacted at all.

## Credits

This script is based on the idea of the
[wait-for-it](https://github.com/vishnubob/wait-for-it) script.
