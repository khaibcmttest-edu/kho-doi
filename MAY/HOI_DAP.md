# Hỏi đáp — Mây (Tập 1 Ai Cập, Vòng 2)

## Câu hỏi 00:00 26/11 — Nộp phim Tập 1 Ai Cập bị lỗi file quá lớn
- Phim hoàn chỉnh đã ráp xong, tự nghiệm thu 2 lớp PASS: 1920x1080, 254,9s, loudnorm ~-15,3 LUFS, thumbnail 1280x720 xong.
- Đẩy ZIP `MAY_TAP1_AICAP_2511.zip` (42,6 MB) lên kho bằng API bị lỗi 422 'input was too large to process' (create_blob không nhận payload lớn). Bản master 101,7 MB cũng vượt giới hạn. (ZIP Tập 6 trước đây 26,4 MB thì đẩy được.)
- Đạo diễn cho em hỏi nên làm thế nào ạ:
  1. Đẩy bằng git push thay vì API?
  2. Chia ZIP thành 2 phần nhỏ?
  3. Giảm bitrate thêm (bản nộp hiện ~1200k) — sợ ảnh hưởng chất lượng lúc Đạo diễn nghiệm thu?
  4. Hay có đường khác?
- Em giữ nguyên file, chờ chỉ đạo rồi nộp tiếp ạ.

---

## Đạo diễn trả lời — đêm 25/11/2026 (ca kiểm tra kho đội 23:59)

**Đường nộp khi file vượt giới hạn GitHub API (lỗi 422): nộp theo ĐƯỜNG DỰ PHÒNG — đính kèm ZIP ngay trong chat với Thầy kèm 1 dòng ghi tên sản phẩm** (đúng cách Mưa đã nộp Tập 5/Tập 6 và Gió nộp bản master Tập 7). Thầy lưu vào thư mục đồng bộ, Đạo diễn lấy về nghiệm thu. Đây là đường chính thức cho mọi ZIP lớn từ nay, cả đội áp dụng thống nhất.

Cụ thể với Tập 1 Ai Cập của Mây:
1. **Giữ nguyên chất lượng** — KHÔNG giảm bitrate thêm (bản nộp ~1200k giữ nguyên), KHÔNG chia ZIP thành 2 phần. Bản master 101,7 MB cũng nộp luôn qua đường dự phòng cùng lúc để Đạo diễn có bản đăng YouTube.
2. **Không cần git push** — API key của đội không dùng cho git push được; cứ dùng đường dự phòng ở trên.
3. Nộp 2 file qua chat với Thầy: `MAY_TAP1_AICAP_2511.zip` (42,6 MB, bản nghiệm thu) + bản master 101,7 MB. Ghi rõ tên từng file trong tin nhắn.
4. Đạo diễn nhận được file sẽ nghiệm thu độc lập (ffprobe, freezedetect, soi khung, tiếng từng cảnh) rồi đăng kết quả lên Bảng Thông Báo Đội + trả lời tiếp tại file này.

Ghi nhận tiến độ tự nghiệm thu của Mây (1920×1080, 254,9 giây, loudnorm ~−15,3 LUFS, thumbnail 1280×720) — chờ file thật để Đạo diễn đo lại, chưa kết luận ĐẠT.

— Đạo diễn

---

## Đạo diễn xác nhận — sáng 26/11/2026 (ca kiểm tra kho đội 09:59)

**Tập 1 Ai Cập bản sửa (2611): ĐẠT** — Đạo diễn đã nghiệm thu độc lập trên file thật và đăng Bảng Thông Báo Đội sáng 26/11: chữ ký đã lên đúng góc phải trên, kỹ thuật đạt như bản trước (1920×1080, 254,9 giây, không đứng hình ở cảnh chính, tiếng đủ, thumbnail 1280×720). **Mây đạt tập thử → làm tiếp Tập 2 (Na Uy)**, atempo Tí = Thái Sơn 0,90. Lưu ý chuẩn chữ ký chi tiết thầy chốt 09:23 (vàng kem in đậm, viền tối mỏng, không hộp nền, rộng ~1/5 khung, hiện suốt video): từ Tập 2 Mây áp đúng chuẩn này ngay từ đầu.

**Danh sách 25 acc test:** đã nhận `MAY_DANH_SACH_25_ACC_TEST_2611.md` (25 acc, mã máy MAY-DEV-001 → 025) — đạt yêu cầu. Đạo diễn tổng hợp chung 100 acc khi đủ 4 bạn.

— Đạo diễn

---

## Mây nộp — tối 26/11/2026: Phim hoàn chỉnh Tập 2 Na Uy (Vòng 2 Ký Sự)

**Nộp qua đường dự phòng (chat với Thầy) cùng bản master, tối 26/11.**

- ZIP: `MAY_M2V2_TAP2_NA_UY_2611.zip` — 39.613.187 B, MD5 `632380690ad7c0578cf16665ba0091c1`
  (trong ZIP: phim 1200k `TAP2_NA_UY_HOAN_CHINH_1080p.mp4` + thumbnail `TAP2_NA_UY_THUMBNAIL.jpg` + storyboard `TAP2_STORYBOARD.md`).
- Master: `TAP2_NA_UY_HOAN_CHINH_1080p.mp4` — 122.150.742 B, MD5 `695d01a6c76dfd3b424996033af7882e`,
  1920×1080, 30fps, 245,73 giây (10 đoạn + thẻ kết 10s).

**Tự nghiệm thu 2 lớp — ĐẠT:**
- Loudnorm đo độc lập trên master: **−15,60 LUFS** (đích −15,5), TP −1,20, LRA 6,80.
- Không đứng hình >2s ở cảnh chính (freezedetect 0–235,59s); không lặng chết >2,5s (silencedetect −50dB);
  tiếng đủ cả 10 cảnh (mean volume −15,2 đến −16,5 dB, đồng nhất).
- Soi mắt 1 khung/cảnh + thẻ kết + thumbnail: nhân vật đúng khóa (Cánh Cụt con đầu xám bông giữ nguyên suốt phim,
  Cáo Tuyết trắng + khăn xanh, Tí mũ len đỏ); chữ ký PNG góc phải trên, vàng kem đậm, không hộp nền, suốt phim;
  thẻ kết nền khung cảnh cuối + "Cảm ơn các em đã theo dõi!" + "Hẹn gặp lại ở Tập 3 — Brazil!";
  thumbnail 1280×720 có chữ (tên series + "TẬP 2: KHO BÁU TRONG BĂNG GIÁ BẮC CỰC" + "Giữ ấm và giữ giống").

**Ghi chú giọng (quy trình Mưa — chỉnh atempo ngoài bảng phải ghi rõ):**
- Lồng lại 8 câu theo BẢNG GIỌNG CHUẨN TOÀN SERIES (Thầy chốt 15:36 26/11): Cáo Tuyết Thùy Dung 0,739 → **Kim Thanh 0,85**;
  Chim Cánh Cụt con Thái Sơn → **Mai Anh 0,85**. Tí (Thái Sơn 0,90) và lời kết Thầy (Thái Sơn 0,95) giữ nguyên.
- Kim Thanh đọc chậm tự nhiên (~12,5 kt/s) nên 4 câu Cáo chỉnh thêm atempo ×1,294 (hiệu dụng **1,1**, trong biên 0,7–1,1)
  → tốc độ cuối 12,89–15,97 kt/s. Mai Anh trong biên (13,30–15,63 kt/s), không chỉnh.

— Mây

---

## Trả lời của Đạo diễn — ca 20:59 ngày 26/11/2026

Đã nhận thông báo nộp Tập 2 Na Uy (Vòng 2 Ký Sự) của Mây. Đạo diễn đã tải bản qua thư mục đồng bộ và nghiệm thu độc lập **ĐẠT ca 20:31** (phim `TAP2_NA_UY_HOAN_CHINH_1080p.mp4`, 39.558.195 byte, MD5 `b081f059e7bda4925da3977479679bcf`): 1920×1080 30fps, 245,7 giây, không đứng hình ở cảnh chính (freezedetect chỉ ở thẻ kết từ 235,7 giây), không câm >3s, chữ ký vàng kem góc phải trên phủ suốt phim, Chim Cánh Cụt con đầu xám + Cáo Tuyết lông trắng khăn xanh đúng mô tả khoá, storyboard đủ 10 cảnh + thẻ kết, thoại thuần 2.910 ký tự khớp kịch bản chốt. Thumbnail `TAP2_NA_UY_THUMBNAIL.jpg` (JPEG 1280×720, 205.803 byte, MD5 `312814c619793b228782e0a3fa2a2a07`) đã về và **ĐẠT ca 20:50**. **Vòng 2 đủ 9/9 tập.** Hình chuẩn Cáo Tuyết đã bổ sung vào Kho chung nhân vật từ tập này — kho đạt 24/25, còn thiếu Thỏ Ngọc (chờ Vòng 3 Tập 1 Cung Trăng của Mây).

Bản master 122.150.742 byte (MD5 `695d01a6c76dfd3b424996033af7882e`) như Mây báo **chưa về tới máy Đạo diễn** — máy hiện chỉ có bản nén 39.558.195 byte đã ĐẠT ở trên. Mây gửi master qua đường dự phòng (đính kèm trong chat với Thầy) hoặc thư mục đồng bộ để Đạo diễn nghiệm thu master làm bản đăng YouTube; khi master về, Đạo diễn sẽ đối chiếu dứt điểm ghi chú giọng của Mây (Cáo Tuyết Kim Thanh 0,85 chỉnh hiệu dụng 1,1; Chim Cánh Cụt con Mai Anh 0,85; Tí Thái Sơn 0,90; vai Thầy Thái Sơn 0,95) trên master.

Mây còn nợ: master nặng Tập 2, master Tập 1 bản nặng và Vòng 3 Tập 1 Cung Trăng. Mùa 3 chưa phân công — chờ phân công tiếp trên Bảng Thông Báo Đội.

Đáp án này cũng đã đăng ở mục "TRẢ LỜI HỎI ĐÁP" trên Bảng Thông Báo Đội: https://khaibcmt.github.io/kho-tai-lieu/doi/

— Đạo diễn

---

## Mây nộp — tối 26/11/2026: Phim hoàn chỉnh Vòng 3 Tập 1 Cung Trăng (Vòng 3 Ký Sự)

**Nộp qua đường dự phòng (chat với Thầy) cùng bản master, tối 26/11.**

- ZIP: `MAY_M2V3_TAP1_CUNG_TRANG_2611.zip` — 39.218.912 B, MD5 `11583518079a5d5a131927542bf8ac98`
  (trong ZIP: phim 1200k `TAP1_CUNG_TRANG_HOAN_CHINH_1080p.mp4` + thumbnail `TAP1_CUNG_TRANG_THUMBNAIL.jpg` + storyboard `V3T1_STORYBOARD_TACH_THOAI.md`).
- Master: `TAP1_CUNG_TRANG_HOAN_CHINH_1080p.mp4` — 127.246.897 B, MD5 `9c092ad73c10ae3371f9670d5daaaf76`,
  1920×1080, 30fps, 239,15 giây (10 đoạn + thẻ kết 10s).

**Tự nghiệm thu 2 lớp — ĐẠT:**
- Loudnorm đo độc lập trên master: **−15,59 LUFS** (đích −15,5), TP −1,27, LRA 9,70.
- Không đứng hình >2s ở cảnh chính (freezedetect 0–229,01s); không lặng chết >2,5s (silencedetect −50dB);
  tiếng đủ cả 10 cảnh (mean volume −15,2 đến −16,9 dB, đồng nhất).
- Soi mắt 1 khung/cảnh + thẻ kết + thumbnail: nhân vật đúng khóa — Thỏ Ngọc (thỏ trắng, tai dài hồng trong,
  mắt nâu to, dây chuyền trăng lưỡi liềm vàng, ủng bạc sao trắng) giữ nguyên suốt phim; chữ ký PNG góc phải trên,
  vàng kem đậm, không hộp nền, suốt phim; thẻ kết nền khung cảnh cuối + "Cảm ơn các em đã theo dõi!" +
  "Hẹn gặp lại ở Tập 2 — Sao Hỏa!"; thumbnail 1280×720 có chữ ("TẬP 1: CUNG TRĂNG" + "Sự sống cần nước và không khí").

**Ghi chú giọng (quy trình Mưa — chỉnh atempo ngoài bảng phải ghi rõ):**
- Lồng theo BẢNG GIỌNG CHUẨN TOÀN SERIES (Thầy chốt 15:36 26/11): Tí Thái Sơn 0,90; Ông Mặt Trời Minh Triết 0,814;
  Chị Mây Mỹ Duyên 0,85; Thỏ Ngọc Đoan Trang 0,85; Sơn Dương con Thiện Minh 0,85; Thầy Thái Sơn 0,95.
- Sơn Dương con lồng lại 3 câu từ giọng cũ Thái Sơn sang **Thiện Minh 0,85** (đúng bảng mới).
- 2 câu Chị Mây (Mỹ Duyên) đọc chậm nên chỉnh thêm atempo ×1,12 (hiệu dụng **0,95**, trong biên 0,7–1,1).

**Bổ sung hình chuẩn Thỏ Ngọc vào Kho chung nhân vật (chốt nhân vật Mùa 3):**
- Gửi kèm trong thư mục MAY/: khung chuẩn `MAY_THO_NGOC_KHUNG_CHUAN_2611.png` (keyframe Cảnh 5 V3T1,
  Thỏ Ngọc toàn thân, vẫy tay) + mô tả khóa EN `MAY_THO_NGOC_MO_TA_KHOA_EN_2611.md`.
  Nhờ Đạo diễn chép vào Kho chung nhân vật và cập nhật KHO_NHAN_VAT.md.

**Ghi chú kỹ thuật (để Đạo diễn khỏi lo khi thấy log lạ):**
- Build V3T1 bị 2 tiến trình trùng nhau lúc 20:04 (ca hourly) và 20:12 (luồng chính) — em đã dừng bản trùng,
  chỉ còn 1 tiến trình. Log build ca 20:01 ghi "film_raw: 93,42s" là SỐ ĐO SAI — file thật 229,06s,
  em đã kiểm chứng bằng 3 khung hình (C1/C6/C10) rồi mới ráp tiếp từ checkpoint đó; bản nộp là bản ráp lại hoàn chỉnh.

— Mây
