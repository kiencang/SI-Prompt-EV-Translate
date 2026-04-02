**[YÊU CẦU THỰC THI - GLOSSARY EXTRACTION]**

Đầu vào là file tài liệu cần xử lý. Hãy phân tích nội dung và trích xuất Bảng thuật ngữ chuyên ngành Anh - Việt, tuân thủ tuyệt đối toàn bộ quy định trong System Instruction.

**Xác định Chuyên ngành (Domain Profiling):** BẮT BUỘC tự động quét nhanh tài liệu để phân tích và chốt "Chuyên ngành lớn" (VD: Y khoa) và "Chuyên ngành hẹp" (VD: Tim mạch can thiệp). Hãy sử dụng chuyên ngành hẹp được nội suy này làm hệ quy chiếu tuyệt đối để dịch thuật ngữ.

**TRÌNH TỰ THỰC THI BẮT BUỘC CỦA BẠN:**
1. Khởi tạo ngay thẻ `<thinking>`.
2. Trình bày rõ ràng `[Domain Target]: Chuyên ngành lớn - Chuyên ngành hẹp` ngay dòng đầu tiên trong thẻ thinking để khóa ngữ cảnh dịch thuật.
3. Chạy quá trình trích xuất nháp, Lemmatization, **sắp xếp A-Z** và rà soát QA Checklist ngầm bên trong thẻ thinking.
4. Đóng thẻ `</thinking>` và lập tức xuất danh sách định dạng Markdown (Zero Fluff).