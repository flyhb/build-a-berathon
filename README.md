# Build-a-Berathon Demo Submission
Tutorial for the Build-a-Berathon demo

## Intro
Hummingbird is a peer-to-peer (P2P) infrastructure for autonomous drone delivery built on the Berachain blockchain. By enabling individuals and businesses to host integrated drone-and-dock stations, Hummingbird aims to decentralize last-mile logistics and provide transparent, incentive-aligned delivery services.

## Steps

1. Create a Bepolia dev account in MetaMask and fund it with test tokens (use the [Bepolia Faucet](https://bepolia.faucet.berachain.com/)).
2. Import the HB token contract (updated contract address [here](https://github.com/flyhb/hummingbird#berachain-testnet)).
3. Mint a Hummingbird Drone Station NFT at https://test.flyhummingbird.io/contribute.
4. Follow the instructions to run a drone station simulator [here](https://github.com/flyhb/delivery-drone-simulator#delivery-drone-station-simulator).
5. Optionally, configure the drone station GPS location in `device_config.json`. **Note:** Ensure you send a few BERA to the device address; 0.2 BERA should suffice for one hour of operation.
6. Open https://test.flyhummingbird.io, connect your wallet, and locate your drone on the map.
7. Wait a couple of minutes to mine some HB tokens. Check your drone ooeration and HB balance in the miner's dashboard. Claim the rewards there.
8. Create a new delivery request (ensure it's in the area of the drone; the whole trip should not be longer than the max drone range set in `drone_config.json`).
9. Wait for the drone to **propose** a price, then **accept** the proposal.
10. Approve the HB token spending in MetaMask.
11. Approve the delivery in MetaMask (requires HB tokens in your wallet).
12. Check the drone logs to monitor the delivery.

> Note: the web app currently only updates the drone's status and location based on on-chain proofs of liveness, so it follows the simulator heartbeat frequency. This will be improved in the next release.
