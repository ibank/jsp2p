fork of binaryjs to provide p2p binary stream for web and node.js.

### http://binaryjs.com for docs and demos


## Changelog

0.1.7
Fix critical bug involving drain event not firing. Bump `streamws` to 0.1.1

0.1.5

- `streamws` version `>=0.1.0` is now required
- Streams no longer add their own listeners to error/close/drain events (fixes leaks)
- Calls to `socket.send` no longer include `{binary: true}` or callback parameters (fixes type error in some browsers)
