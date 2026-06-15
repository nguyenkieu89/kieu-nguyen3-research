# [TEST DESIGN STRATEGY]

Thiết kế testcase theo Risk-Based Testing.

Priority 1 (Critical)

- Business Rules
- Functional Flow
- Data Integrity

Priority 2 (High)

- Input Validation
- Boundary Testing
- Contract Testing

Priority 3 (Medium)

- Authentication
- Authorization
- Security

Priority 4 (Medium)

- Performance
- Concurrency

Priority 5 (Low)

- Compatibility
- Non-functional checks

Đối với mỗi Business Rule bắt buộc tạo:

- 1 Positive Test Case
- 1 Negative Test Case
- 1 Boundary Test Case

Mỗi field trong request phải được đánh giá:

- Required
- Optional
- Data Type
- Length
- Format
- Allowed Characters
- Nullability
- Boundary Values

Áp dụng các kỹ thuật kiểm thử:

- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table Testing
- State Transition Testing (nếu phù hợp)
- Error Guessing
- Risk-Based Testing

---

# [FIELD ANALYSIS ENGINE]

Trước khi tạo testcase, phải phân tích từng field theo format:

{
"fieldName": "",
"required": true/false,
"dataType": "",
"validationRules": [],
"boundaryValues": [],
"riskLevel": ""
}

Nếu không xác định được rule từ API Spec thì phải suy luận từ:

- field name
- business rules
- API semantics

Không được bỏ sót field nào.

---

# [TEST DATA MANAGEMENT]

Ưu tiên sử dụng dữ liệu động:

- timestamp
- uuid
- random suffix

Đảm bảo testcase có thể chạy lặp lại nhiều lần.

Tránh phụ thuộc dữ liệu tồn tại sẵn trong môi trường.

---

# [WORKFLOW]

3. Cấu hình dữ liệu chính xác theo Chế độ kiểm thử (Mode) được yêu cầu (Mặc định là Mode 1).