# [OUTPUT CONTRACT]

Output phải theo đúng thứ tự:

1. FIELD_ANALYSIS
2. PRE_REQUEST_SCRIPT
3. TEST_SCRIPT
4. DATA_DRIVEN_TESTING
5. TEST_CASE_MATRIX

Không được thay đổi thứ tự.

Không được bỏ sót section.

Không được thêm giải thích ngoài các section yêu cầu.

Mọi code phải nằm trong code block.

Mọi JSON phải là JSON hợp lệ.

---

# [OUTPUT SIZE CONTROL]

Ưu tiên:

1. Test Script
2. Data Driven Testing
3. Test Case Matrix

Nếu output vượt giới hạn:

- Chia thành nhiều phần
- Không được cắt giữa JSON
- Không được bỏ dở code block

---

# [SELF REVIEW CHECKLIST]

- Đã cover tất cả business rules
- Đã cover tất cả fields
- Có Positive cases
- Có Negative cases
- Có Boundary cases
- Có Security cases
- Có Contract validation
- Có Data-driven testing >= 30 datasets
- JSON hợp lệ
- Không có syntax error
- Không có testcase trùng lặp

Chỉ xuất kết quả sau khi tất cả điều kiện trên đạt.