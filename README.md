# SM4Crypt
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](https://github.com/pedroalbanese/sm4crypt/blob/master/LICENSE.md) 
[![GitHub downloads](https://img.shields.io/github/downloads/pedroalbanese/sm4crypt/total.svg?logo=github&logoColor=white)](https://github.com/pedroalbanese/sm4crypt/releases)
[![GoDoc](https://godoc.org/github.com/pedroalbanese/sm4crypt?status.png)](http://godoc.org/github.com/pedroalbanese/sm4crypt)
[![Go Report Card](https://goreportcard.com/badge/github.com/pedroalbanese/sm4crypt)](https://goreportcard.com/report/github.com/pedroalbanese/sm4crypt)
[![GitHub go.mod Go version](https://img.shields.io/github/go-mod/go-version/pedroalbanese/sm4crypt)](https://golang.org)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/pedroalbanese/sm4crypt)](https://github.com/pedroalbanese/sm4crypt/releases)
### Command-line GM/T 0002-2012 SM4-GCM Encryption Tool
<pre>Usage of sm4crypt:
sm4crypt [-d] -p "pass" [-i N] [-s "salt"] -f &lt;file.ext&gt;
  -d    Decrypt instead Encrypt.
  -f string
        Target file. ('-' for STDIN)
  -i int
        Iterations. (for PBKDF2) (default 1024)
  -k string
        128-bit key to Encrypt/Decrypt.
  -p string
        Password-based key derivation function2.
  -r    Generate random 128-bit cryptographic key.
  -s string
        Salt. (for PBKDF2)</pre>

### Example of encryption/decryption:
```sh
./sm4crypt -k $128bitkey -f plaintext.ext > ciphertext.ext
./sm4crypt -d -k $128bitkey -f ciphertext.ext > plaintext.ext
```

## License

This project is licensed under the ISC License.

##### Military-Grade Reliability. Copyright (c) 2020-2021 ALBANESE Research Lab.
