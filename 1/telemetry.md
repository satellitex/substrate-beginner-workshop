# View Public Telemetry

You can take a look at the overall network using the telemetry website:

[https://telemetry.polkadot.io/#list/UTC%20Testnet](https://telemetry.polkadot.io/#list/UTC%20Testnet)

Your node will connect to the telemetry server because of the `spec.json`:

```json
"telemetryEndpoints": [
    [ "wss://telemetry.polkadot.io/submit/", 0 ]
],
```

## Discussion

* Peer Discovery
* Network Topology

<!-- slide:break -->

![Polkadot Telemetry](./assets/telemetry.png)
