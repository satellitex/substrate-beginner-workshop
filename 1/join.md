# Join the Network

You can use the `substrate-node-template` you compiled earlier and this chain specification file to connect to our network.

1. Save the [`spec.json`](https://satellitex.github.io/substrate-beginner-workshop/1/assets/specRaw.json) file in the `substrate-node-template` folder.

2. Launch your node:

	```bash
	./target/release/node-template \
		--chain spec.json \
		--name YourNodeName
	```

> You can use the flag `--log sub-libp2p,sync` for verbose network logs for debugging if you need it.

If you can not sync nodes. Please tray it.

```bash
docker pull satellitex/substrate-workshop-node
docker run -p 9933:9933 -p 9944:9944 -p 30333:30333 -v $(pwd)/spec.json:/tmp/spec.json satellitex/substrate-workshop-node --chain /tmp/specRaw.json --name YourNodeName
```

Notice that your node now appears on the telemetry page.

<!-- slide:break-70 -->

## Discussion

* Raw Spec
* Node Roles
	* Boot Nodes
	* Validators
	* Full Nodes
