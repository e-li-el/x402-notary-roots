# x402 notary - daily roots

Each file `YYYY-MM-DD.json` is the Merkle root of every x402 endpoint
listing captured that UTC day (price, upto cap, payTo, scheme, description).
`.ots` files are OpenTimestamps proofs anchoring each root in Bitcoin.

A root committed here can't be changed later without it showing in this
repo's history. Any record from that day can be checked against its root.

Verify a proof: `python verify.py proof.json --root-file YYYY-MM-DD.json`
