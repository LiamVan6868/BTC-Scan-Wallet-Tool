# BTC-Scan-Wallet-Tool
 Bitcoin Wallet Scanner &amp; Balance Checker with Multi-API Support
## 📦 CÀI ĐẶT

### Bước 1: Cài đặt các thư viện cần thiết

```bash
pip install requests mnemonic bip-utils colorama
```

Hoặc cài từng cái:

```bash
pip install requests --break-system-packages
pip install mnemonic --break-system-packages
pip install bip-utils --break-system-packages
pip install colorama --break-system-packages
```

### Bước 2: Chạy chương trình

```bash
python3 btcminer_fixed.py
```

---

## 🚀 CÁCH SỬ DỤNG

### Mode 1: CHECKER (Kiểm tra địa chỉ có sẵn)

1. Tạo file `addresses.txt` với danh sách địa chỉ BTC:
```
1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa
1BvBMSEYstWetqTFn5Au4m4GFg7xJaNVN2
1HQ3Go3ggs8pFnXuHVHRytPCq5fGG8Hbhx
```

2. Chọn mode `C` khi chạy chương trình

3. Kết quả lưu vào `success.txt` (ví có balance)

### Mode 2: BRUTEFORCER (Tạo ví ngẫu nhiên)

1. Chọn mode `B` khi chạy

2. Cấu hình:
   - **Address type**: `p2pkh` (Legacy) hoặc `p2wpkh` (Bech32)
   - **Language**: `english`, `spanish`, `french`, v.v.
   - **Strength**: `128` (12 từ) hoặc `256` (24 từ)

3. Kết quả:
   - `success.txt` - Ví có balance (bao gồm mnemonic, private key)
   - `failed.txt` - Ví không có balance (chỉ lưu mnemonic)

---
