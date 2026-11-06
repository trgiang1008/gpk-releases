Gpk 1.0.2

- Thêm tự kiểm tra cập nhật sau khi mở, hỏi trước khi tải/cài và tự mở lại Gpk.
- Kênh Gpk riêng: trgiang1008/gpk-releases. PingPK giữ nguyên trgiang1008/pingpk-releases.
- Chỉ nhận đúng tên gói, URL và SHA-256; kiểm tra manifest Gpk và từng tệp trước khi thay runtime.
- Giữ cấu hình nhân vật và LIC; lưu runtime cũ để khôi phục.

Kiểm tra: build, 23 updater fixture checks, cài gói thật lên bản 1.0.1 trong thư mục kiểm tra, self-test LIC/cấu hình và startup smoke đều qua. Không điều khiển game trong các kiểm tra này.

Giới hạn: chưa kiểm thử chiến đấu/bơm máu trong game; chưa audit đầy đủ native/VM. Windows Defender trên máy build không trả trạng thái hoạt động nên chưa có kết quả quét AV. EXE chưa ký Authenticode. SHA-256 phụ thuộc nguồn GitHub tin cậy.

Bản trước 1.0.2 cần tải ZIP và mở bản mới thủ công một lần. Không chạy hai auto trên cùng nhân vật.
