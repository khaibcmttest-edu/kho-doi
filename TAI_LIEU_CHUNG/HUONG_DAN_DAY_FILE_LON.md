# HƯỚNG DẪN ĐẨY FILE LỚN LÊN KHO ĐỘI

_Thầy Khải chốt 19:45 ngày 27/11/2026: "mở lên max luôn" — đường file lớn mở trần tối đa theo GitHub Release. Cập nhật 28/11/2026: Thầy đã kết nối lại connector đội thêm host `uploads.github.com` (dán lại token 1 lần qua link an toàn) — đội tự đẩy file lớn thẳng lên Release của kho-doi, Đạo diễn đã kiểm chứng đầu-cuối đạt._

## Quy tắc chọn đường theo dung lượng

- **File ≤ 40 MB**: đẩy thẳng vào thư mục của mình trên kho đội như trước giờ (MAY/ NANG/ MUA/ GIO/ DA_DUYET/ TAI_LIEU_CHUNG/).
- **File > 40 MB**: đi đường **GitHub Release trên repo kho-doi**, trần tối đa **2 GB/asset** (giới hạn của GitHub). Không đặt giới hạn thấp hơn. ZIP phim 222 MB, 500 MB hay 1 GB đều đi đường này. **Không chia nhỏ file, không giảm chất lượng, không gửi qua Thầy.**

## Cách đẩy file lớn (đường chính thức hiện hành)

Mỗi bạn tự đẩy bằng helper của connector đội (đã có sẵn lệnh `release-upload`):

```
python3 ~/workspace/custom-connectors/custom.github-doi/bin/gh_doi.py release-upload kho-doi <tag> <tên-release> <file1> [file2 ...]
```

- Tag đặt theo tên sản phẩm, không dấu, gạch ngang. Ví dụ: `mua3-tap1-mau`, `mua3-tap4`, `kho-hinh-doi-phim`.
- Lệnh tự tạo release (hoặc dùng lại release cùng tag), upload từng file làm asset qua `uploads.github.com`, in ra **link tải công khai** dạng:
  `https://github.com/khaibcmttest-edu/kho-doi/releases/download/<tag>/<tên-file>`
- Chạy lại không bị trùng: file đã có đúng dung lượng thì bỏ qua, sai dung lượng thì xoá upload lại.
- Chỉ tin khi kết quả từng file có `status: 201` (hoặc `skip-same-size`) kèm link; sau đó tải thử link công khai đối chiếu dung lượng/MD5 với file gốc rồi mới ghi vào HOI_DAP.

## Sau khi đẩy xong — ghi link ở đâu

1. Người nộp ghi **link tải + dung lượng + MD5** vào `HOI_DAP.md` trong thư mục của mình trên kho đội.
2. Đạo diễn ghi link vào **Bảng Thông Báo Đội** (https://khaibcmt.github.io/kho-tai-lieu/doi/) để cả đội tải về xem và làm theo.
3. File nhỏ kèm theo (README, ghi chú nghiệm thu, MD5) vẫn đẩy vào thư mục trên kho đội như thường — chỉ file nặng mới đi Release.

## Đường dự phòng

Release trên repo chính khaibcmt/khaibcmt.github.io (Đạo diễn chạy `~/workspace/kho_tai_lieu_chung/release_upload_kho_doi.py`) nay chỉ là **dự phòng** khi đường kho-doi trục trặc — không còn là đường chính. Đường chia file thành từng phần nhỏ đã bị Thầy bác ngày 28/11/2026 ("Vậy khó lắm") — không dùng.

## Kiểm chứng đã chạy

- 27/11/2026 (trước reconnect): kho đội tạo release thử → 201; upload asset → 401 vì connector chưa đăng ký host `uploads.github.com`. Repo chính: upload file test 990.000 byte → 201, tải về công khai đủ byte. Release thử + tag thử đã xoá sạch.
- 28/11/2026 (sau reconnect): kho đội tạo release thử (tag `test-upload-2811`) → 201; upload asset 2.040 byte qua `uploads.github.com` → **201**; tải công khai về khớp từng byte (MD5 trùng); lệnh mới `release-upload` cũng test đạt (201); release thử + tag thử đã xoá sạch cả hai lượt.
