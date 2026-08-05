<div align="center">
  <img src="chive-logo-full.png" alt="Chive Logo" height="120" />
  <p><strong>A decentralized, lightweight recipe app built on the AT Protocol.</strong></p>
</div>

---

Welcome to **Chive**! We are building an open ecosystem for food enthusiasts to create, share, and discover recipes without walled gardens. 

By leveraging [ATProto](https://atproto.com/), Chive ensures that your recipes are inherently yours—stored in your own data repository, portable, and independently hostable.

## 🌟 Our Architecture

We split Chive into distinct layers, keeping the public web interface completely decoupled from the data pipeline and indexing mechanisms:

- **[Chive Web Application](https://github.com/chive-recipes/chive):** A lightning-fast, static Preact/Vite frontend. It reads recipe records directly from the ATProto network. The client stays dumb, fetching full records via decentralized identifiers (DIDs) on demand.
- **[Chive Indexer](https://github.com/chive-recipes/chive-indexer):** A secure, private polling mechanism that compiles discovery indices (`index.json`). It uses Cloudflare D1 for state and generates automated Pull Requests to the public repo, maintaining the static site's integrity without exposing the polling infrastructure.
- **Decentralized Data:** We rely entirely on Custom Lexicons (`com.chive.recipe`) for data shape. Your recipes live on your PDS (Personal Data Server).

## 🚀 Get Involved

We embrace open-source contributions, technical discussions, and ATProto integrations. If you're passionate about the federated web and cooking, come help us build the ultimate decentralized recipe network!

- [Try Chive (Placeholder)](#)
- [Read the Lexicon](#)
- [Explore the code](https://github.com/chive-recipes/chive)
