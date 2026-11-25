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
