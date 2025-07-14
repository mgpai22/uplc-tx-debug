# UPLC Debug

```bash
cargo update && cargo run
```

The inputs are the following:

```

    [
      {
        "transaction_id": "c67fe457611c2f5462e619dd3eeec619a72491ce7ea227b736b8d50edaeab637", // script input
        "index": 0
      },
      {
        "transaction_id": "4ca027e6d305efb212515e86e91ec3ab53074ca3c14b76c2aded418237c3efab", //script input
        "index": 1
      },
      {
        "transaction_id": "993973d58f7d822440520736363ac35e5faa78e1385fad286668bdadfe827ec8", // wallet input
        "index": 2
      }
    ]

```

utxo: 993973d58f7d822440520736363ac35e5faa78e1385fad286668bdadfe827ec8#2 belongs to addr1q9kuwka7ewwy4vj8wgaz6wp669adl0teg546lvqzmfccs9qgzdwja762m7ax9eaqqagef0wrlr6nyv07zq4v8882ee3qddh24q

When you evaluate the script the error is:

```
Err(MissingRequiredScript { hash: "6dc75bbecb9c4ab247723a2d383ad17adfbd79452bafb002da718814" })
```

That hash is a VFK to the wallet address.
