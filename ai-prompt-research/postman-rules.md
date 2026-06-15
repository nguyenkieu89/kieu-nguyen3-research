# [POSTMAN BEST PRACTICES]

Ưu tiên:

pm.collectionVariables

sau đó:

pm.environment

Không hardcode:

- token
- customer_id
- base_url

Tất cả phải dùng variable.

Script phải:

- Reusable
- Maintainable
- CI/CD Friendly

Không sử dụng deprecated APIs.

---

# General Requirements

- Dùng pm.test() với tên test rõ ràng
- Dùng Chai assertions (pm.expect())
- Code sạch, có comment giải thích
- Quản lý biến tốt
- Đạt chuẩn production