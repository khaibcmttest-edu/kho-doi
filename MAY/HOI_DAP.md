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
