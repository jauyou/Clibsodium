### 🔧 About the Framework

This framework is compiled from [libsodium](https://github.com/jedisct1/libsodium) TAG: 1.0.20-RELEASE.

If you prefer to build and package it yourself, follow these steps:

---

### 🛠 Build from Source

#### 1. Clone the repository

```bash
git clone https://github.com/jedisct1/libsodium.git
cd libsodium
```

#### 2. Compilation
```bash
./configure
make && make check
sudo make install
```

#### 3. Build for Apple platforms

Follow the official guide to cross-compile for Apple devices:
👉 https://doc.libsodium.org/installation#cross-compiling-to-apple-devices

You can run the prebuilt script:
```bash
./dist-build/apple-xcframework.sh
```

#### 4. Replace the Framework in Your Project
Once the .xcframework is built, replace the existing one in your project with the new version:
```bash
# Replace the existing xcframework in your project
cp -R libsodium.xcframework /path/to/your/project/Frameworks/libsodium.xcframework
```
