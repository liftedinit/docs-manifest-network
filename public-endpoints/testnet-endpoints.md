# Become a Validator







Install the latest `manifestd`binary from Github releases.&#x20;



Install cosmovisor, configure your systemd service and enable auto downloads.&#x20;



Initialize your new validator, ensure you backup the keys!



Retrieve the validator pubkey:&#x20;

`manifestd tendermint show-validator`

Generate your validator.json file

<pre><code><strong>cat &#x3C;&#x3C;EOF > validator.json
</strong>{
  "pubkey": {"@type":"/cosmos.crypto.ed25519.PubKey","key":"keycontents="},
  "amount": "1000000upoa",
  "moniker": "validator's name",
  "identity": "keybase-identity",
  "website": "validator's (optional) website",
  "security": "validator's (optional) security contact email",
  "details": "validator's (optional) details",
  "commission-rate": "0.0",
  "commission-max-rate": "0.2",
  "commission-max-change-rate": "0.01",
  "min-self-delegation": "1"
}
EOF
</code></pre>



Sync all blocks:&#x20;





Purchase MFX tokens and send to your validator's wallet to pay for transaction costs.&#x20;



Once blocksync has completed and your node is completely caught up, issu
