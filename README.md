# AES-256-GCM 加解密工具

纯前端在线加解密工具，基于浏览器原生 Web Crypto API，所有操作在本地完成，密码不会离开设备。

## 功能

- **加密**：输入明文 + 密码 → 输出 Base64 密文
- **解密**：输入 Base64 密文 + 密码 → 输出明文

## 技术细节

- 加密算法：AES-256-GCM
- 密钥派生：PBKDF2（SHA-256，100,000 次迭代）
- 随机 Salt（16 字节）+ 随机 IV（12 字节）
- 输出格式：`Base64(salt + iv + ciphertext)`
- 零依赖，单文件部署

## 使用

在线访问：https://yosolin.github.io/endecrypt/
