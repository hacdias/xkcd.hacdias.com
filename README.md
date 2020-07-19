# [xkcd.hacdias.com](http://xkcd.hacdias.com/)

> Moved this clone process to a VPS. It still runs everyday.

Automated clone of xkcd comics to [/ipns/xkcd.hacdias.com](http://xkcd.hacdias.com/) for the decentralized web. How is it done? Basically I'm just using Circle CI to run a few steps every day:

1. Fetch the latest xkcd comics using [xkcd-clone](https://github.com/hacdias/xkcd-clone).
2. Pin it to IPFS Cluster.
3. Update the DNSLink on `xkcd.hacdias.com`.
