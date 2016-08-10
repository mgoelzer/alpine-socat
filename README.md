## Alpine with socat installed

This is an Alpine Linux image with `socat` installed.  That's it.  Nothing to see here.

Intended usage:

```
# listen on 123/tcp and echo to stdout
$ docker run -d -p 123:123 mgoelzer/alpine-socat socat -T0 -u TCP4-LISTEN:123,reuseaddr,fork -
f78394bc4ebbc62073d6048cdae78233bfd93c95c53fd126f66c664504c23a65
$ docker logs -f f78394bc
<blah blah blah>
```

