# IPromise

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/3d5d1287-faaa-45fd-a5c9-c9bd0f1f4e72)

Kiểm tra file bằng ExeInfo để kiểm tra thông tin file.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/a98e3965-dfdb-4ff1-be95-09a6830ca53f)

Phân tích tĩnh file và ta thấy hitn của tác giả. Kiểm tra hàm main tôi chỉ thấy hàm này k gọi bất kỳ hàm nào.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/2b32c229-c785-4bd2-8805-ddd859ddc56c)

Ở đây tôi có thấy hàm  `decryptIPromise`. Khai báo một mảng ký tự v1 với kích thước 200. Khởi tạo ngữ cảnh AES bằng cách gọi hàm AES_init_ctx(). Giải mã ba khối dữ liệu riêng biệt sử dụng AES trong chế độ ECB. Đầu tiên, giải mã dữ liệu từ &encrypted và lưu kết quả vào v1. Tiếp theo, giải mã dữ liệu từ &unk_404050 và lưu kết quả vào v1. Cuối cùng, giải mã dữ liệu từ &unk_404060, lưu kết quả vào v1 và trả về kết quả này từ hàm.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/8e5125a7-ba39-4ffb-8f02-83f5a1554dc6)

Ở đâyb ta debug và ta có flag là `flag{d41d8cd98f00b204e9800998ecf8427e}`

# Taylor's First Swift

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/89459a43-f49c-4c95-9a51-76a3162b6bf4)

Kiểm tra file bằng ExeInfo để kiểm tra thông tin file.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/e35795d3-dd30-47a5-80d6-1779b02a709e)

Ở đây tôi thấy chương trình chức năng chính là kiểm tra giá trị bằng hàm `flagcheck`. Vì đây là ngôn ngữ IOS nên tôi k thể debug được.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/318e4087-c6d9-456e-a260-b56e93db796d)

Nhìn sơ qua hàm này thì tôi thấy nó đang xor 2 chuỗi là `FRsIAQ8PVBUVEREIVERbBkURFkUIBxVQVkAYFxJfV0FYVkIVQgo=` và `swifte!` với nhau và hiển thị bằng UTF8.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/98279372-3c90-496d-a59f-3bfc6f2c1803)

Sau khi xor thì ta có flag là.

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/963b25ca-5150-4d51-8283-9821f02d5ed8)

`flag{f1f4bfa202c60e2aaa9339de61513141}`

# What's in the Box?

![image](https://github.com/daglongg/ctf.nahamcon/assets/138242812/bfa2a6bd-04b1-449e-8f7e-0fc3d4562217)



