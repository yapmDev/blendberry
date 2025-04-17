# 🍓 BlendBerry – Open Remote Config Platform

**BlendBerry** is a fully open-source alternative to remote configuration platforms like Firebase Remote Config, designed to be **self-hostable**, **flexible**, and accessible to **everyone**, regardless of region or network limitations.

> ✊ Originally built to solve the issue of region-restricted cloud platforms, BlendBerry provides developers and organizations full control over how app configurations are delivered and updated across environments.

---

## 🧭 Mission

To provide an accessible and developer-friendly remote configuration system that empowers developers from all regions—especially those affected by platform restrictions or network limitations—to deliver dynamic, remotely updatable experiences to their users.

---

## 🔧 What is BlendBerry?

BlendBerry is a **remote configuration system** that allows mobile and backend applications to:

- Fetch environment-specific configuration values
- Update application behavior without redeployment
- Manage feature flags, themes, access levels, and other runtime parameters
- Host the platform themselves, without any third-party dependency

---

## 📦 Components

BlendBerry is split into independent but connected projects:

| Project | Description |
|--------|-------------|
| [`blendberry_server`](https://github.com/blendberry/blendberry_server) | Backend API built with Spring Boot for managing remote configurations. |
| [`blendberry_flutter`](https://github.com/blendberry/blendberry_flutter) | Flutter SDK that enables client-side fetching and usage of remote configurations. |

Future SDKs may include support for Android, iOS, Web, and Desktop platforms.

---

## 🧱 Architecture

BlendBerry follows **clean architecture** principles and includes the following layers:

- **Backend (blendberry_server)**  
  A Spring Boot REST API with endpoints for configuration retrieval, environment/version lookup, and metadata sync.

- **Client SDKs (e.g., blendberry_flutter)**  
  Integrations that handle local caching, environment-aware config loading, and seamless synchronization.

- **Custom Mappers & Entities**  
  Map raw configurations to domain-specific models like theme options, feature toggles, and runtime settings.

---

## 🌍 Why BlendBerry?

- ✅ **Open-source & Transparent**  
  You own your data and infrastructure. Host BlendBerry wherever you like.

- 🌐 **No Geo-Restrictions**  
  Designed for developers in regions where Firebase or similar services are blocked or restricted.

- 🛠️ **Extensible**  
  Add your own config structures, mappers, and sync strategies.

- ⚡ **Optimized Sync**  
  Only update when changes are detected via environment + versioning + timestamps.

- 📱 **Multi-Environment Support**  
  Easily configure for `dev`, `staging`, `prod`, or any other environment you define.

---

## 🗺️ Roadmap

- [x] Core backend (Spring Boot)
- [x] Flutter SDK
- [ ] Web dashboard (React-based)
- [ ] Android SDK
- [ ] iOS SDK
- [ ] CLI tool
- [ ] Docker deployment templates
- [ ] Multitenancy support

---

## 🤝 Contributing

We welcome contributions from developers, writers, designers, and testers around the world.

If you’d like to contribute:

1. Fork the repository you want to contribute to (`blendberry_server` or `blendberry_flutter`).
2. Create a feature branch.
3. Open a pull request with a clear explanation.

For ideas, improvements or bugs, feel free to [open an issue](https://github.com/blendberry) in the relevant repository.

---

## 📜 License

All components of the BlendBerry project are licensed under the [MIT License](LICENSE).

---

## ✨ Join the Mission

Whether you’re an indie dev, open-source enthusiast, or an organization seeking autonomy and flexibility, **BlendBerry** is built for you.

**Host it yourself. Customize it freely. Use it anywhere.**  
No restrictions. Just remote config, reimagined.
