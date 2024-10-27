## Caprover

```shell
docker run -d \
--name caprover \
--restart always \
-p 8080:80 \
-p 8443:443 \
-p 3000:3000 \
-e ACCEPTED_TERMS=true \
-v /var/run/docker.sock:/var/run/docker.sock \
-v "/var/lib/srv/$USER/docker/caprover/caprover/latest/data:/captain" \
caprover/caprover
```
