in 6~ seconds the script restores a monero wallet from keys and scans in a list of 3 transactions (passed by a uri link e.g. from a qr code).    
`sweep_all` to your pay out address.     
(requires monero-wallet-rpc in same dir as script)

URI: as per suggestion in https://github.com/monero-project/meta/issues/729
it can be one txid or in this case multiple seperated by a comma.
```
monero_wallet:address=58Bj65FCpfpULRXyf7mmsY1vB4qiW8qQ8X99tw783rSggPjmvUcRHycaXUQfSwMVpuUj6FWDr4fNHFYyo7f1XdtsJsXAJ1Y&spend_key=75ca1b95ee9dd8bbf059da64c6750fd500731f8775389ce089d516d46108fc05&view_key=c59b3e3182d9c665d0f3a1776a28301410283ab6ff6a9bd3abc7a5bb37758f03&txid=f8477b831a028f07d5638157afc0fbf0897066b4caa29dc48f885fba79cec814,bd20081e0d1abf05b275bcc06bc7e315bc03c57870e247c82c8a45b30f4d1b34,cdbed9b4b2f56de7cce9255610d0cae702aefb36f9a4ff15698ea448f29f6188
```
or with just seed and txid
```
monero_uri="monero_wallet:seed=portents%20toyed%20judge%20sighting%20smidgen%20masterful%20selfish%20sack%20cabin%20loudly%20maps%20gown%20thumbs%20five%20sword%20tonic%20cunning%20android%20ourselves%20lawsuit%20fossil%20pedantic%20origin%20peaches%20toyed&txid=f8477b831a028f07d5638157afc0fbf0897066b4caa29dc48f885fba79cec814,bd20081e0d1abf05b275bcc06bc7e315bc03c57870e247c82c8a45b30f4d1b34,cdbed9b4b2f56de7cce9255610d0cae702aefb36f9a4ff15698ea448f29f6188"
```
Output:
```
params from uri:
view_key:
c59b3e3182d9c665d0f3a1776a28301410283ab6ff6a9bd3abc7a5bb37758f03
spend_key:
75ca1b95ee9dd8bbf059da64c6750fd500731f8775389ce089d516d46108fc05
txid list:
f8477b831a028f07d5638157afc0fbf0897066b4caa29dc48f885fba79cec814,bd20081e0d1abf05b275bcc06bc7e315bc03c57870e247c82c8a45b30f4d1b34,cdbed9b4b2f56de7cce9255610d0cae702aefb36f9a4ff15698ea448f29f6188

RPC not available yet...This is the RPC monero wallet. It needs to connect to a monero
daemon to work correctly.

Monero 'Fluorine Fermi' (v0.18.1.2-release)
Logging to monero-wallet-rpc.log
2022-12-04 06:08:35.514	I Binding on 127.0.0.1 (IPv4):18082
2022-12-04 06:08:36.446	W Starting wallet RPC server

RPC not available yet...

URI Address:
58Bj65FCpfpULRXyf7mmsY1vB4qiW8qQ8X99tw783rSggPjmvUcRHycaXUQfSwMVpuUj6FWDr4fNHFYyo7f1XdtsJsXAJ1Y

Generated Address:
"58Bj65FCpfpULRXyf7mmsY1vB4qiW8qQ8X99tw783rSggPjmvUcRHycaXUQfSwMVpuUj6FWDr4fNHFYyo7f1XdtsJsXAJ1Y"
2022-12-04 06:08:51.605	W Loaded wallet keys file, with public address: 58Bj65FCpfpULRXyf7mmsY1vB4qiW8qQ8X99tw783rSggPjmvUcRHycaXUQfSwMVpuUj6FWDr4fNHFYyo7f1XdtsJsXAJ1Y
{
  "id": "0",
  "jsonrpc": "2.0",
  "result": {
  }
}
Wallet is opened ok
2022-12-04 06:08:52.086	W Received money: 10.000000000000, with tx: <bd20081e0d1abf05b275bcc06bc7e315bc03c57870e247c82c8a45b30f4d1b34>
2022-12-04 06:08:52.089	W Received money: 10.000000000000, with tx: <cdbed9b4b2f56de7cce9255610d0cae702aefb36f9a4ff15698ea448f29f6188>
2022-12-04 06:08:52.091	W Received money: 19.999735760000, with tx: <f8477b831a028f07d5638157afc0fbf0897066b4caa29dc48f885fba79cec814>
2022-12-04 06:08:52.091	W Spent money: 10.000000000000, with tx: <f8477b831a028f07d5638157afc0fbf0897066b4caa29dc48f885fba79cec814>
2022-12-04 06:08:52.091	W Spent money: 10.000000000000, with tx: <f8477b831a028f07d5638157afc0fbf0897066b4caa29dc48f885fba79cec814>
{
  "id": "0",
  "jsonrpc": "2.0",
  "result": {
  }
}2022-12-04 06:08:52.165	W Requested ring size 1 too low, using 16
2022-12-04 06:08:52.712	W amount=19.999735760000, real_output=4, real_output_in_tx_index=0, indexes: 5975348 6056800 6286343 6307926 6319589 6329562 6333658 6339744 6340827 6341496 6341536 6341887 6342012 6342098 6342556 6342568 
2022-12-04 06:08:52.715	W amount=19.999735760000, real_output=4, real_output_in_tx_index=0, indexes: 5975348 6056800 6286343 6307926 6319589 6329562 6333658 6339744 6340827 6341496 6341536 6341887 6342012 6342098 6342556 6342568 
2022-12-04 06:08:52.719	W amount=19.999735760000, real_output=4, real_output_in_tx_index=0, indexes: 5975348 6056800 6286343 6307926 6319589 6329562 6333658 6339744 6340827 6341496 6341536 6341887 6342012 6342098 6342556 6342568 
{
  "id": "0",
  "jsonrpc": "2.0",
  "result": {
    "amount_list": [19999553000000],
    "fee_list": [182760000],
    "multisig_txset": "",
    "spent_key_images_list": [{
      "key_images": ["0009c59789e809e4b394930028cdacdf9bb17578368764540a524f53e26b931c"]
    }]
    "tx_hash_list": ["e43b12e24513faa5138ee36d146268064ece1156e719c8648afe896840ef3e38"],
    "unsigned_txset": "",
    "weight_list": [1523]
  }
}{
  "id": "0",
  "jsonrpc": "2.0",
  "result": {
  }
}
real	0m18.634s
user	0m0.166s
sys	0m0.031s

```
