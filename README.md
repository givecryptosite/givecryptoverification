# givecrypto-verification

Immutable verification records for [givecrypto.site](https://givecrypto.site) campaign wallet addresses.

This repository stores cryptographic proofs of wallet address states for crowdfunding campaigns, using SHA-256 hashes and Bitcoin timestamping (OpenTimestamps) to ensure transparency and immutability.

## How Verification Works

- Each campaign has a corresponding JSON file in the `pages/` directory.
- Each file contains versioned wallet data with SHA-256 hashes for tamper detection.
- All changes are timestamped via OpenTimestamps for blockchain proof.
- Client-side verification allows anyone to confirm wallet addresses haven't been altered.

## Verification Process

1. Visit a campaign page (`givecrypto.site/slug/id`)
2. Check the "Address Verification" section
3. Click "View on GitHub" to see the wallet states
4. Verify hashes match using the campaign's timestamp

Used by [giveCrypto](https://givecrypto.site) for trust & transparency.