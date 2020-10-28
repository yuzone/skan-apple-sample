## SKAdNetwork 2.0 verify sample

https://developer.apple.com/documentation/storekit/skadnetwork/verifying_an_install_validation_postback


```
$ openssl dgst -sha256 -verify apple_public.pem -signature signature.bin message.bin
Verified OK
```

## Sample postback

```json
{
  "version" : "2.0",
  "ad-network-id" : "com.example",
  "campaign-id" : 42,
  "transaction-id" : "6aafb7a5-0170-41b5-bbe4-fe71dedf1e28",
  "app-id" : 525463029,
  "attribution-signature" : "MDYCGQD0AdGn5gUnSuVGk8Wi0IgxzWiKdBzwJrQCGQCJfkrI5bda93EC4Xm1H+MtNxstFmnVBn0=",
  "redownload": true,
  "source-app-id": 1234567891,
  "conversion-value": 20
}
```
