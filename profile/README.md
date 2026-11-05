<div align="center">

<img src="banner.png" alt="Who cleared this? Seal checks an AI agent's action against your rules before it runs, and signs the decision, refusals included. A hand-drawn sketch shows an agent proposing an action, Seal checking it, a signed refusal, and someone checking it later. Rón, the Seal mascot, sits at a laptop." width="100%">

**Signed records of AI decisions.**

[aqta.ai](https://aqta.ai) · [See a signed record](https://app.aqta.ai) · [Verify a record](https://app.aqta.ai/verify)

</div>

<img align="right" src="ron-stamp.png" width="200" alt="Rón the seal beside a Seal stamp">

## Seal in three steps

1. Before acting, an agent sends Seal a request.
2. Seal checks your rules and signs the decision, allowed or refused.
3. Anyone can verify the signed record later.

## Open for anyone

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

<sub>Aqta Technologies Limited · Dublin, Ireland · [hello@aqta.ai](mailto:hello@aqta.ai)</sub>
