# 55913

Reproducible for [https://github.com/nodejs/node/issues/55913](https://github.com/nodejs/node/issues/55913).

On Node 22.7 and above, run

```bash
node --env-file sub/dev.env --watch-path /usr/local/bin --watch-preserve-output index.js
```

Run `touch sub/test.txt` in a separate console.

- Expected result: it does not restart.
- Actual result: it does restart.
