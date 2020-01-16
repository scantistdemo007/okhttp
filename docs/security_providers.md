
Security Providers
==================

## Provider Status

| Provider               | HTTP/2  | TLSv1.3      | Powered By       | Issues           | Usage Guidance   |
| ---------------------- | ------- | ------------ | ---------------- | ---------------- | ---------------- |
| JVM default            | Java 9+ | Java 11+     | OpenJDK          |                  |                  |
| Android default        | ✅      | Android 10+  | BoringSSL        |                  |                  |
| [Bouncy Castle][bc]    | ✅      |             | Bouncy Castle     | [#5698][bug5698] |                  |
| [Conscrypt][conscrypt] | ✅      | ✅          | BoringSSL        |                  | Activated if Conscrypt is first registered provider. |
| [OpenJSSE][openjsse]   |         | ✅          | OpenJDK backport |                  |                  |
| [Corretto][coretto]    | ✅      | ✅          | OpenSSL          | [#5592][bug5592] | Amazon high-performance cryptographic implementations backed by OpenSSL |

All providers support HTTP/1 and TLSv1.2.


[bc]: https://www.bouncycastle.org/java.html
[conscrypt]: https://www.conscrypt.org/
[openjsse]: https://github.com/openjsse/openjsse
[coretto]: https://github.com/corretto/amazon-corretto-crypto-provider
[bug5698]: https://github.com/square/okhttp/issues/5698
[bug5592]: https://github.com/square/okhttp/issues/5592