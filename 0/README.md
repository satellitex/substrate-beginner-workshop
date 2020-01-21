# Getting Started

Please complete the instructions on this page before attending the [Parity Substrate](https://www.parity.io/substrate/) workshop. You only need to complete this one page, we will look at the other pages during the workshop.

If you have any problems with the instructions on this page, feel free to send us an email at:

* takumi@stake.co.jp

## Instructions

1. Install Substrate Dependencies:

	```bash
	curl https://getsubstrate.io -sSf | bash -s -- --fast
	```

	> **Note:** Windows users can follow the instructions found here: https://substrate.dev/docs/en/next/getting-started#getting-started-on-windows

2. Clone Substrate Node Template

	```bash
	git clone https://github.com/substrate-developer-hub/substrate-node-template
	```

3. Build Node

	```bash
	cd substrate-node-template/
	cargo build --release
	```

4. Test Run Your Node

	```bash
	./target/release/node-template --dev
	```

	> **Note:** You can stop your node with `ctrl + c`.

	If everything completed successfully, you should see your local development node producing blocks:

	```bash
➜  substrate-node-template git:(master) ./target/release/node-template --dev
2020-01-21 07:21:20 Running in --dev mode, RPC CORS has been disabled.
2020-01-21 07:21:20 Substrate Node
2020-01-21 07:21:20   version 2.0.0-8b6fe66-x86_64-macos
2020-01-21 07:21:20   by Anonymous, 2017, 2018
2020-01-21 07:21:20 Chain specification: Development
2020-01-21 07:21:20 Node name: glib-room-3207
2020-01-21 07:21:20 Roles: AUTHORITY
2020-01-21 07:21:20 Initializing Genesis block/state (state: 0xf1f5…8b31, header-hash: 0x4890…bdbc)
2020-01-21 07:21:20 Loading GRANDPA authority set from genesis on what appears to be first startup.
2020-01-21 07:21:20 Loaded block-time = 6000 milliseconds from genesis on first-launch
2020-01-21 07:21:20 Highest known block at #0
2020-01-21 07:21:20 Using default protocol ID "sup" because none is configured in the chain specs
2020-01-21 07:21:20 Local node identity is: QmZhSeY5NWNUrfKKAL4dEsDi496KhmNmistC1Pb8DaA9Ty
2020-01-21 07:21:20 Grafana data source server started at 127.0.0.1:9955
2020-01-21 07:21:24 Starting consensus session on top of parent 0x4890f08bb4cd885f075af635a7355eb05df7b50b82f3c4823756a4b1f567bdbc
2020-01-21 07:21:24 Prepared block for proposing at 1 [hash: 0x3db142b5d5bee6e01162dadb63b9be0508ce7509e1aca52badce6ea31d8ceaec; parent_hash: 0x4890…bdbc; extrinsics: [0x0c42…3e3e]]
2020-01-21 07:21:24 Pre-sealed block for proposal at 1. Hash now 0x7a285ecf071df2c8777c93fd813518c755b528409d23943c923568839b3ee57d, previously 0x3db142b5d5bee6e01162dadb63b9be0508ce7509e1aca52badce6ea31d8ceaec.
2020-01-21 07:21:24 Imported #1 (0x7a28…e57d)
2020-01-21 07:21:25 Idle (0 peers), best: #1 (0x7a28…e57d), finalized #0 (0x4890…bdbc), ⬇ 0 ⬆ 0
2020-01-21 07:21:30 Starting consensus session on top of parent 0x7a285ecf071df2c8777c93fd813518c755b528409d23943c923568839b3ee57d
2020-01-21 07:21:30 Prepared block for proposing at 2 [hash: 0x4a5ae67dc9aa53df7115738030ae8806e9885e27ba5a5693ea864276209bfdbc; parent_hash: 0x7a28…e57d; extrinsics: [0xce71…00fd]]
2020-01-21 07:21:30 Pre-sealed block for proposal at 2. Hash now 0x3590fc9a228cf9ac83366a3926ebd8df93e5bc771f3ea770e7f688ba13c617cb, previously 0x4a5ae67dc9aa53df7115738030ae8806e9885e27ba5a5693ea864276209bfdbc.
2020-01-21 07:21:30 Imported #2 (0x3590…17cb)
2020-01-21 07:21:30 Idle (0 peers), best: #2 (0x3590…17cb), finalized #0 (0x4890…bdbc), ⬇ 0 ⬆ 0
```
