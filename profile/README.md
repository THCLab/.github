[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E6JH4XP)

Hi there, wanderer! Welcome to the The Human Colossus Lab.

No matter whether you visit this space just out of curiosity or looking for something specific, let us do a quick yet intense introduction to what you can find here. We are a team of individuals that truly believe in a world where data flows do not end up in a few data silos. We believe in the opposite, where individuals are in the center of these flows, and they control them. The decentralization is the next inevitable step for individuals. To achieve that, we need to build proper tech operating in a decentralized paradigm without any central control point. This is more complex, yet we have a vision for it. We encourage you to [get acquainted](https://humancolossus.foundation/blog/dde-first-contact) a bit deeper into this topic.

Now, if you are still with us, let us guide you through the stack we believe is a key to achieving our abovementioned beliefs. To achieve each layer (see [DDE Stack](https://github.com/THCLab#dde-stack)), various components and supporting libs playing together are essential. 

#### Authentic data

When it comes to data transferred over the wire, it is usually preconceived that the provenance of data is already authentic. In other words, if the communication channel is secured (i.e., by TLS when it comes to WEB), it is considered good enough to assume that the data provider is really who she claims she is. In many cases, it is not strong enough to assume that; therefore, here, we develop tooling to overcome this problem. In essence, to presume any data transferred over the wire is cryptographically signed and can be eventually verified by anyone receiving this data.

##### Components
- [KERIOX](https://github.com/THCLab/keriox) is the fundamental piece that implements [KERI](https://keri.one/) infrastructure leveraging the digital identifiers and hence the proof of provenance to the next level. As KERIOX is implemented in Rust, we leverage the lang core features and expose bindings through the FFI layer to other languages:
  - JavaScript/Typescript (Node.JS via NAPI) – https://github.com/THCLab/keri-bindings/tree/master/bindings/node.js
  - Dart – https://github.com/THCLab/keri-bindings/tree/master/bindings/dart
- [TELIOX](https://github.com/THCLab/teliox) is tightly coupled with KERIOX and provides the TEL implementation (Transaction Event Logs), which is basically a non-repudiable log of execution of some state machine (VC issuance/revocation in this case).
- [CESROX](https://github.com/THCLab/cesrox) is the [CESR](https://weboftrust.github.io/ietf-cesr/draft-ssmith-cesr.html) implementation in Rust.

Apart from that, we provide core components for KERI infrastructure:
- [KERI Witness](https://github.com/THCLab/keriox/releases)
- [KERI Watcher](https://github.com/THCLab/keriox/releases)

#### Integrity of the data

- [OCA](https://github.com/THCLab/oca-rs) - Implementation of [Overlays Capture Architecture](https://oca.colossi.network/).
- [SAID](https://github.com/THCLab/cesrox/tree/master/said) - Self-Addressing Identifier provides a compact text representation of digests of data. It supports multiple hash algorithms.







### DDE Stack
![alt text](stack2.png "DDE stack")




<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
