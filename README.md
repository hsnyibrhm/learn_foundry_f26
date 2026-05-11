# Foundry Fund Me 🚀

Repositori ini adalah hasil perjalanan belajar  **FOUNDRY**. Proyek ini mengimplementasikan sistem penggalangan dana terdesentralisasi, efisien, dan teruji.

## 📝 Tentang Proyek
Proyek ini memungkinkan pengguna untuk mengirim donasi ETH ke kontrak dengan nilai minimal dalam USD. 
- **Oracle Integration**: Menggunakan Chainlink Price Feed untuk mendapatkan harga ETH/USD secara real-time.
- **Security**: Menerapkan akses kontrol agar hanya *Owner* yang bisa menarik dana.
- **Gas Optimized**: Menggunakan variabel `immutable` dan `constant` serta teknik pembacaan storage yang efisien.

---

## 🛠️ Persyaratan (Requirements)

- **Git**: [Instal Git](https://git-scm.com/) (Verifikasi: `git --version`)
- **Foundry**: [Instal Foundry](https://getfoundry.sh/) (Verifikasi: `forge --version`)
- **Make**: (Opsional) Untuk menjalankan perintah otomatis lewat Makefile.

## 🚀 Quickstart

```bash
git clone [https://github.com/hsnyibrhm/foundry](https://github.com/hsnyibrhm/learn_foundry_f26)
cd foundry-fund-me
forge build
```

## Deployment Local(Anvil)

```bash
# Jalankan Anvil di terminal terpisah
anvil

# Deploy menggunakan script
forge script script/DeployFundMe.s.sol --rpc-url [http://127.0.0.1:8545](http://127.0.0.1:8545) --private-key <PRIVATE_KEY_ANVIL> --broadcast
```

## Tesnet (Sepolia)
```bash
source .env
forge script script/DeployFundMe.s.sol --rpc-url $SEPOLIA_RPC_URL --private-key $PRIVATE_KEY --broadcast --verify --etherscan-api-key $ETHERSCAN_API_KEY
```
## TEST
```bash
# Menjalankan semua test
forge test

# Menjalankan test spesifik
forge test --match-test testFunctionName -vvv

```
# Melihat cakupan kode (Coverage)
```bash
forge coverage

forge snapshot

cast storage <CONTRACT_ADDRESS> <SLOT_NUMBER> --rpc-url [http://127.0.0.1:8545](http://127.0.0.1:8545)
```

