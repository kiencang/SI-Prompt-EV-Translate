**LỆNH THỰC THI CHÍNH:**
Dựa trên System Instructions (SI) đã nạp, hãy tiếp nhận tài liệu đầu vào và thực hiện quy trình 3 bước sau:

**[BƯỚC 0: PHÂN TÍCH BỐI CẢNH - Suy luận ngầm]**
Trước khi dịch, hãy tự xác định: Tài liệu này thuộc thể loại gì? (Khoa học/Kỹ thuật, Báo chí, hay Hướng dẫn?). 
*Nếu là Khoa học/Kỹ thuật -> Kích hoạt quy tắc GIỮ NGUYÊN câu bị động để đảm bảo tính khách quan. Nếu không -> Kích hoạt quy tắc chuyển sang câu chủ động.*

**[BƯỚC 1: DỊCH THUẬT & TÁI TẠO]**
Thực hiện dịch toàn bộ nội dung sang tiếng Việt và bọc trong cấu trúc HTML. 

**Checklist Kỹ thuật Bắt buộc:**
*   [ ] Đã bọc tất cả `<table>` trong `<div class="table-wrapper">` chưa?
*   [ ] Đã dùng `\(\)` và `\[\]` cho toán học và KHÔNG bọc chúng trong thẻ `<code>` chưa?
*   [ ] Các trích dẫn (References) đã được GIỮ NGUYÊN TIẾNG ANH 100% chưa?
*   [ ] Đã ép luồng văn bản chính về 1 cột chưa?

**[BƯỚC 2: TỰ ĐỐI SOÁT (Reflexion - Suy luận ngầm)]**
Đọc lại bản nháp HTML vừa tạo. 
1. Câu văn tiếng Việt đã trôi chảy, thoát ý tiếng Anh chưa? Nếu còn gượng gạo, hãy tự viết lại câu đó.
2. Có thẻ HTML nào chưa đóng không? Có rủi ro tràn lề không? Hãy tự sửa lỗi.

**[BƯỚC 3: XUẤT KẾT QUẢ BẮT BUỘC (STRICT OUTPUT)]**
Trả về MÃ HTML THÔ. Bắt đầu chính xác bằng `<!DOCTYPE html>` và kết thúc bằng `</html>`.
BẮT BUỘC chèn khối CSS và MathJax Script dưới đây vào thẻ `<head>` của bạn:

```html
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<style>
*, *::before, *::after { box-sizing: border-box; }
body { font-family: Roboto, 'Noto Sans', Arial, sans-serif; font-size: 18px; line-height: 1.6; color: #222; max-width: 900px; margin: 0 auto; padding: 20px; overflow-wrap: break-word; }
img, svg, video { max-width: 100%; height: auto; object-fit: contain; display: block; margin: 1.5rem auto; }
.table-wrapper { width: 100%; overflow-x: auto; margin-bottom: 1.5rem; -webkit-overflow-scrolling: touch; }
table { width: 100%; border-collapse: collapse; }
th, td { border: 1px solid #ddd; padding: 10px; text-align: left; vertical-align: top; }
th { background-color: #f8f9fa; font-weight: bold; }
.ws-nowrap { white-space: nowrap; }
.grid-2col { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1.5rem; align-items: start; }
.grid-3col { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; align-items: start; }
pre { background-color: #f4f5f7; padding: 15px; overflow-x: auto; border-radius: 4px; }
code { font-family: Consolas, monospace; font-size: 0.9em; background-color: #f4f5f7; padding: 2px 4px; border-radius: 3px; }
pre code { background-color: transparent; padding: 0; }
</style>
</head>
```
*(Bắt đầu xuất mã HTML từ đây)*