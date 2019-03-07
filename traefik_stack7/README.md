This directory is experimental.

Checkout: traefik_stack5

#### Edge setup (NOT recommanded)

```
echo "CONFIGURE ENV_VAR" && \
ENV_EDGE_BRANCH="2.02";
ENV_MONOREPO="traefik_stack6";

echo "Setup the stack" && \
source <(curl -s https://raw.githubusercontent.com/pascalandy/docker-stack-this/2.02/play-with-docker-setup.sh) && \
sleep 2 && \

git checkout "$ENV_EDGE_BRANCH" && \
cd "$ENV_MONOREPO" && \

./runup.sh;
```
