<div align="center">

<img src="ron-wave.png" width="150" alt="Rón, the Seal mascot, waving">

**Security for AI agents that act.**

When an agent is tricked, Seal makes sure it can't do anything a person didn't approve, and gives you proof anyone can check. Starting with payments.

[aqta.ai/seal](https://aqta.ai/seal) · [Verify a record](https://app.aqta.ai/verify)

</div>

## Open for anyone

- [**paybound**](https://github.com/Aqta-ai/paybound): an AI agent can only pay what a person approved, on BNB Chain testnet. [Try to break it](https://paybound-eight.vercel.app) · `pip install paybound`
- [**attestation-spec**](https://github.com/Aqta-ai/attestation-spec): the record format, and the free checker anyone can run.
- [**bounds**](https://github.com/Aqta-ai/bounds): PDF redaction that runs entirely on your device.

<details>
<summary>For developers: check a real record from your terminal</summary>

```sh
curl -sO https://app.aqta.ai/samples/sample-action.json
npx aqta-verify-receipt --profile action-1 \
  --key 9Y3Eiq6V8QjRDUM5nPqSwKIOPQaoEU4SbagfYFdvWa4 sample-action.json
```

Then change `BLOCKED` to `ALLOWED` in the file and run it again.

</details>

<sub>Aqta Technologies Limited · Dublin · [hello@aqta.ai](mailto:hello@aqta.ai)</sub>
