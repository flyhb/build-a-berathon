# Build-a-Berathon Demo Submission
Tutorial for the Build-a-Berathon demo

## Intro
Hummingbird is a peer–to–peer (P2P) infrastructure for autonomous drone de-
livery built on the Berachain blockchain.1 By enabling individuals and businesses
to host integrated drone–plus–dock stations, Hummingbird aims to decentralise
last–mile logistics and provide transparent, incentive–aligned delivery services. 


## Steps

1. Create a Bepolia dev account in Metamask and fund it with test tokens (get some -> [Bepolia Faucet](https://bepolia.faucet.berachain.com/))
2. Import the HB token contract (updated contract address [here](https://github.com/flyhb/hummingbird#berachain-testnet))
3. Mint a Hummingbird Drone Station NFT at https://test.flyhummingbird.io/contribute
4. Follow the instructions to run a drone station simulator [here](https://github.com/flyhb/delivery-drone-simulator#delivery-drone-station-simulator).
5. Optionally, configure the drone station GPS location in device_config.json
**Note:** Ensure you sent a few BERA to the device address, 0.2 BERA should suffice for 1h operatiopn
6. Open  https://test.flyhummingbird.io, connect your wallet and Locate your drone on the map
7. Wait a couple minutes to mine some HB to
8. Create a new delivery request (ensure it's in the area of the drone, the whole trip should not be longer then the max drone range set in `drone_config.json`)
9. Wait per the drone to **propose** a price, then **accept** the proposal
10. Approve the HB token spending in Metamask
11. Approve the delivery in Metamask (will require HB tokens in your wallet)
12. Check the drone logs to monitor the delivery

> Note: the web app currently only updates the current drone status and location based on on-chain proofs of liveness, so it follows the simulator heartbeat frequency. This will be improved in the next release.
