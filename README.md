# haproxy-gw
Proxy that reloads from git repo, checks for changes every minute


This image uses SSH keys to authenticate to git repository, you must (hopefully its obvious why) provide your own keys and add permissions to your repo if private, so that it can pull updates. It shouldn't need more than read-only permissions. 

Provide your SSH key in same directory as Dockerfile named "id_rsa"

I haven't tested this against any other versions of HAProxy, only 1.7.6, but there shouldn't be any issues with newer versions.
