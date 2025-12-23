# Database

## DSA: 1.351 rows (25 active 0.1s)

| done  | fp     | g      | issuer | names  | not_after | not_before | p      | q      | valid | y      |
| ----- | ------ | ------ | ------ | ------ | --------- | ---------- | ------ | ------ | ----- | ------ |
| UInt8 | String | String | String | String | Int64     | Int64      | String | String | UInt8 | String |

## ECDSA: 2.925.678.935 rows (760.858.838 active 94s)

| b      | curve  | done  | fp     | gx     | gy     | issuer | length | n      | names  | not_after | not_before | p      | pub    | valid | x      | y      |
| ------ | ------ | ----- | ------ | ------ | ------ | ------ | ------ | ------ | ------ | --------- | ---------- | ------ | ------ | ----- | ------ | ------ |
| String | String | Uint8 | String | String | String | String | Int64  | String | String | Int64     | Int64      | String | String | UInt8 | String | String |

## RSA: 9.168.841.173 rows (1.660.338.955 active 770s)

| done  | exponenet | fp     | issuer | length | modulus | names  | not_after | not_before | valid |
| ----- | --------- | ------ | ------ | ------ | ------- | ------ | --------- | ---------- | ----- |
| UInt8 | Int64     | String | String | Int64  | String  | String | Int64     | Int64      | Int8  |

# Example

```json
{
    "fp": "26aa127cf8d02bd649b5604f97cc99d5730cae2c71ec90fff2dbc5bd9cd74c88",
    "names": "bscw.cultura.gencat.net",
    "nb": 1140786066,
    "na": 1267016459,
    "iss": "C=ES, O=Agencia Catalana de Certificacio (NIF Q-0801176-I), L=Passatge de la Concepcio 11 08008 Barcelona, OU=Serveis Publics de Certificacio ECV-2, OU=Vegeu https://www.catcert.net/verCIC-2   (c)03, OU=Secretaria d'Administracio i Funcio Publica, CN=EC-SAFP",
},


"rsa": {
    "exp": 65537,
    "modulus": "a13f6a20484239317961204865be50c249be893bfeef3d6757d1288d22531e9f73bce084db2dfac4700e5fc822b8ea140ec03f7eba094c4bc19c74b3add9bc46bb06abcb73694bbdcf05a2fae0ef9eede47535a0abd06be026ac331b02f85d70a1fbcf27a3283e866fb66d489e5baabcfc4428015bf7bd1c365c922b121872ed",
    "len": 1024
},


"ecdsa": {
    "b": "5ac635d8aa3a93e7b3ebbd55769886bc651d06b0cc53b0f63bce3c3e27d2604b",
    "curve": "P-256",
    "gx": "6b17d1f2e12c4247f8bce6e563a440f277037d812deb33a0f4a13945d898c296",
    "gy": "4fe342e2fe1a7f9b8ee7eb4a7c0f9e162bce33576b315ececbb6406837bf51f5",
    "length": 256,
    "n": "ffffffff00000000ffffffffffffffffbce6faada7179e84f3b9cac2fc632551",
    "p": "ffffffff00000001000000000000000000000000ffffffffffffffffffffffff",
    "pub": "04634c4e915f94faced8632bc2973d19b103cc7e4f0672acaabade540bca516a580d7ff8825c9f46aa9e9e01923d150177c0b233f70e49fab39cadfe5b4ad3e5d8",
    "x": "634c4e915f94faced8632bc2973d19b103cc7e4f0672acaabade540bca516a58",
    "y": "0d7ff8825c9f46aa9e9e01923d150177c0b233f70e49fab39cadfe5b4ad3e5d8"
},


"dsa": {
    "g": "1032ae53e8cd52705afcb903ee0d96f57934da360b08af0cb0c0b3706d65c53c81a9b55c6424a5ae860439acf42eda745ca7b1386ea58fe9ee2fb408091d0964627954d148b24dc767793c15edefd67b9676ea5b5c21f4611bfa646e791726611c76cd2ea6360c039d66a445a42eccbb6c9bf5cc49dbe294981c520d3fb1a6e0efff5b67f76aac6e4d6cfa13db5ca6da98f79e105ca478120e96ede9467c9c46a732be26c949a4ef6c42028773cdff75185a1a5856f71b1b45d6971f49d4a38a715da13943217ca9ef3a1e65ed68f40c65b8d8256ba1038dba89577866fedef3554867b35c83d4bcbf3b71e819adb06e1877d73a7b51b88fbe743a422d71da18",
    "p": "d9d3e120c413e8ca3724f2275b169137049e91e1292ebbb08050b1139d6f04f42f46b747892421a390aea30bc94ef917e8e77832d5937a046e858f4d9c20bd5f76da5849ea3a3f46e61a09ff530f07ebbf6c42f605cbc2789768228d0106fed105c3c7e7f6e3bbbab30339b3257cfffbffc5fa3bb2aacde952495d3b5d6164b1dfeaab953006af9aec961bebbd217bb4ee3f48b4cfe40041d650b5360a3f926b91fa537b0b48de692cf8a7fbd8bdef077dda69562839600f3956e7d64762994aea67ea535567b63ebd4914632720e6dc65353a290f6daf6469f97e44cc581dd12fd9e2cfceaeedda41e9be485809be90e99f9d69a1d0ad163fd7e599b22d61d7",
    "q": "ac9ee689fbfd2f6cfaf91b221e8655014c84269e49a17d8000d7881fa2b39931",
    "y": "1a8bf52a6d279ade9620362b48ac4c74734fda8dc4fc7a6e1a3b1b1a69e9d5e461f6df46febda5e15ab3d1d47415e1d5dd78fe9f04dca1d71422fecdc8aa697b7a08645c4d001646b3189ff3a373b13e0cec49aed478034cd4771fdf993aed2a6a8f56db51285eaee3e013629e6bb5b15a1ed3e59e722a96282e7d2f5f22f3eec6b19c107288bc6d2891d2ac2a59034b8c6476649d3c2177b58fee93429b5958bcf2a89c3fbdc6f1764c275f32f855796cc45c02dc9127c872ae2490cca1e467a4352967eb16694be392565ac2dcb5c676b880bec13c3715ab5aea17e6e26edb7c7903ba4b20a125916a3a78a2ae49e7bc3cdc371b43a421fb13662768938df0"
},

```

## ECDSA types:

- P-224. count: 63
- P-256. count: 2.761.270.374
- P-384. count: 164.027.916
- P-521. count: 380.582
