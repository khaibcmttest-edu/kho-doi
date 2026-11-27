# HƯỚNG DẪN ĐẨY FILE LỚN LÊN KHO ĐỘI

_Thầy Khải chốt 19:45 ngày 27/11/2026: "mở lên max luôn" — đường file lớn mở trần tối đa theo GitHub Release._

## Quy tắc chọn đường theo dung lượng

- **File ≤ 40 MB**: đẩy thẳng vào thư mục của mình trên kho đội như trước giờ (MAY/ NANG/ MUA/ GIO/ DA_DUYET/ TAI_LIEU_CHUNG/).
- **File > 40 MB**: đi đường **GitHub Release**, trần tối đa **2 GB/asset** (giới hạn của GitHub). Không đặt giới hạn thấp hơn. ZIP phim 222 MB, 500 MB hay 1 GB đều đi đường này.

## Cách đẩy file lớn (đường chính thức hiện hành)

File lớn lên **Release trên repo chính khaibcmt/khaibcmt.github.io** (Đạo diễn/Em Yêu chạy script, các bạn không tự đẩy được vì cần token repo chính):

```
python3 ~/workspace/kho_tai_lieu_chung/release_upload_kho_doi.py <tag> <tên-release> <file1> [file2 ...]
```

- Tag đặt theo tên sản phẩm, không dấu, gạch ngang. Ví dụ: `mua3-tap1-mau`, `mua3-tap4`, `kho-hinh-doi-phim`.
- Script tự tạo release (hoặc dùng lại release cùng tag), upload từng file làm asset, in ra **link tải công khai** dạng:
  `https://github.com/khaibcmt/khaibcmt.github.io/releases/download/<tag>/<tên-file>`
- Chạy lại không bị trùng: file đã có đúng dung lượng thì bỏ qua, sai dung lượng thì xoá upload lại.

## Sau khi đẩy xong — ghi link ở đâu

1. Người nộp ghi **link tải + dung lượng + MD5** vào `HOI_DAP.md` trong thư mục của mình trên kho đội.
2. Đạo diễn ghi link vào **Bảng Thông Báo Đội** (https://khaibcmt.github.io/kho-tai-lieu/doi/) để cả đội tải về xem và làm theo.
3. File nhỏ kèm theo (README, ghi chú nghiệm thu, MD5) vẫn đẩy vào thư mục trên kho đội như thường — chỉ file nặng mới đi Release.

## Vì sao file lớn chưa nằm thẳng trên repo kho-doi

Đã kiểm chứng ngày 27/11/2026: token đội (khaibcmttest-edu) **tạo được Release** trên kho-doi, nhưng **upload asset bị GitHub trả 401** vì connector đội (`custom.github-doi`) mới đăng ký host `api.github.com`, chưa có `uploads.github.com` — credential không được gắn vào request upload. Đây là giới hạn đăng ký host của connector, không phải token thiếu quyền.

Khi nào thầy kết nối lại connector đội với thêm host `uploads.github.com` (dán lại token 1 lần qua link an toàn), Đạo diễn sẽ chuyển đường file lớn về thẳng Release trên kho-doi và cập nhật hướng dẫn này. Trong lúc chờ, đường Release repo chính ở trên là đường chính thức — đã kiểm chứng tải về công khai khớp dung lượng từng byte (27/11/2026).

## Kiểm chứng đã chạy (27/11/2026)

- Kho đội: tạo release thử → 201; upload asset → 401 (lý do ở trên). Release thử + tag thử đã xoá sạch.
- Repo chính: tạo release thử → 201; upload file test 990.000 byte → 201; tải về bằng link công khai → 200, đủ 990.000 byte khớp dung lượng. Release thử + tag thử đã xoá sạch.
