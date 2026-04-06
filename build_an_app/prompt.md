# Xây dựng ứng dụng trong Gemini

Hãy xây dựng một **ứng dụng dịch thuật chất lượng cao** có các đặc điểm sau:
- File đầu vào là định dạng PDF, thường là tài liệu khoa học, ngôn ngữ tiếng Anh
- File đầu ra là tài liệu HTML, là bản dịch tiếng Việt của file đầu vào.
- Ưu tiên tận dụng nền tảng Gemini. 
- Nó nên có giao diện web để bất cứ ai cũng có thể truy cập được.

Hãy **tuân thủ tuyệt đối** các hướng dẫn sau:

- Ứng dụng cần có giao diện tối giản để tính dễ sử dụng được tăng lên tối đa.
- Ứng dụng phải tuân thủ các SI/Prompt được cung cấp sẵn, không điều chỉnh, rút gọn hoặc viết thêm.
- Ứng dụng phải cho phép lựa chọn nhiều phương pháp dịch như được mô tả chi tiết dưới đây.

## A. Tùy chọn mặc định

Ở tùy chọn mặc định, ứng dụng sử dụng 2 file là `prompt.txt` và `system_instruction.txt` để dịch file PDF tiếng Anh sang tiếng Việt.

## B. Tùy chọn refine

Ở tùy chọn refine, ứng dụng có 2 tùy chọn thấp hơn là `x_math` và `x_svg`.

- Với tùy chọn `x_math`, ứng dụng sử dụng SI/Prompt là `prompt_x_math.txt` và `system_instructions_x_math.txt` để dịch.
- Với tùy chọn `x_svg`, ứng dụng sử dụng SI/Prompt là `prompt_x_svg.txt` và `system_instructions_x_svg.txt` để dịch.

## C. Tùy chọn pdf2html

Ở tùy chọn pdf2html, ứng dụng cần làm đúng theo các bước sau:

- Bước 1: Sử dụng `prompt_phase_1.txt` và `system_instructions_phase_1.txt` để chuyển đổi file PDF thành định dạng HTML (vẫn giữ nguyên tiếng Anh).
- Bước 2: Sử dụng `prompt_phase_2.txt` và `system_instructions_phase_2.txt` để dịch file HTML (tiếng Anh) có được từ **Bước 1** để tạo thành bản dịch hoàn chỉnh.