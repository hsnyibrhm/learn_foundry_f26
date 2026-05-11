# My Foundry Journey 🛠️

Repositori ini berisi kumpulan latihan dan proyek saya selama mempelajari Smart Contract Development menggunakan framework **Foundry**.

## 📑 Daftar Isi
- **Simple Storage**: Dasar-dasar Solidity dan deployment.
- **FundMe**: Proyek penggalangan dana dengan Oracle Chainlink.
- **Testing**: Implementasi unit testing menggunakan Forge.

## 🚀 Perintah Dasar
Perintah yang sering saya gunakan di folder ini:

```bash
# Untuk kompilasi kode
forge build

# Untuk menjalankan test
forge test

# Untuk deploy ke local network (Anvil)
forge script script/DeployFundMe.s.sol --rpc-url [http://127.0.0.1:8545](http://127.0.0.1:8545) --broadcast