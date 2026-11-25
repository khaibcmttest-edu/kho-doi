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
