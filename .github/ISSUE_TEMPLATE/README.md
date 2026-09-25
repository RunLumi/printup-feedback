# Hướng dẫn sử dụng PrintUp Feedback

Repo này là nơi **QC, QA, PM và các thành viên nội bộ** ghi nhận lỗi, đề xuất tính năng, cải tiến sản phẩm, thay đổi tài liệu và phản hồi thiết kế cho PrintUp.

Mục tiêu của mỗi issue là giúp người xử lý hiểu đủ **vấn đề → bằng chứng → ảnh hưởng → kết quả mong muốn → tiêu chí hoàn thành** mà không phải hỏi lại nhiều vòng.

## Chọn biểu mẫu nào?

| Nhu cầu | Biểu mẫu |
| --- | --- |
| Hệ thống đang làm sai, lỗi, crash, dữ liệu sai, hồi quy | **Lỗi / Bug** |
| Cần thêm khả năng mới cho người dùng hoặc hệ thống | **Tính năng mới** |
| Chức năng hiện có vẫn đúng nhưng có thể tốt hơn | **Cải tiến** |
| Sai, thiếu, mâu thuẫn hoặc cần cập nhật tài liệu nghiệp vụ | **Tài liệu / biz-docs** |
| Vấn đề về giao diện, luồng thao tác, responsive, accessibility, visual consistency | **Thiết kế / UX** |

Nếu một vấn đề liên quan nhiều nhóm, chọn biểu mẫu theo **vấn đề chính** và ghi các khu vực bị ảnh hưởng trong nội dung.

## Nguyên tắc viết issue tốt

1. **Nêu vấn đề trước, giải pháp sau.** Đừng bắt đầu bằng "hãy thêm nút X" nếu chưa nói người dùng đang gặp khó khăn gì.
2. **Dùng bằng chứng thật.** Ảnh chụp, video, URL, đơn hàng, log đã loại bỏ dữ liệu nhạy cảm, commit hoặc tài liệu liên quan đều có giá trị.
3. **Tách hiện trạng và mong muốn.** Người xử lý phải biết hệ thống đang làm gì và đáng ra phải làm gì.
4. **Viết tiêu chí hoàn thành có thể kiểm tra.** Tránh "làm đẹp hơn", "nhanh hơn", "ổn hơn" nếu không mô tả cách xác nhận.
5. **Không tự gán độ ưu tiên kinh doanh.** Người gửi đánh giá mức ảnh hưởng; PM quyết định thứ tự ưu tiên dựa trên toàn bộ backlog.
6. **Không đưa bí mật hoặc dữ liệu cá nhân nhạy cảm lên issue.** Che token, mật khẩu, thông tin thanh toán và dữ liệu khách hàng không cần thiết.
7. **Một vấn đề chính cho mỗi issue.** Nếu có nhiều vấn đề độc lập, tách ra để dễ giao việc và nghiệm thu.

## Mức ảnh hưởng

| Mức | Khi nào dùng |
| --- | --- |
| **Chặn vận hành** | Không thể tiếp tục luồng chính; mất dữ liệu; sai tiền; rủi ro bảo mật nghiêm trọng; không có cách vòng an toàn |
| **Cao** | Ảnh hưởng lớn đến khách hàng hoặc vận hành; có cách vòng nhưng tốn công hoặc rủi ro |
| **Trung bình** | Ảnh hưởng đáng kể nhưng không chặn công việc chính |
| **Thấp** | Bất tiện nhỏ, lỗi trình bày hoặc cải tiến chất lượng |

**Mức ảnh hưởng không đồng nghĩa với thứ tự ưu tiên.** PM chịu trách nhiệm ưu tiên sau khi cân nhắc phạm vi, rủi ro, giá trị và chi phí.

## Các khu vực sản phẩm

Dùng tên thống nhất khi mô tả phạm vi:

- `storefront`
- `admin`
- `mobile`
- `backend_hono`
- `biz-docs`
- thiết kế / hệ thống giao diện
- báo giá / tính giá
- đơn hàng / thanh toán
- artwork / duyệt mẫu
- sản xuất / QC
- giao hàng
- tài khoản / phân quyền
- API / tích hợp
- hạ tầng / DevEx / CI
- bảo mật / hiệu năng

## Quy trình xử lý gợi ý

1. **Người gửi:** điền đủ bằng chứng và tiêu chí mong muốn.
2. **QA/QC:** xác minh lỗi, phạm vi ảnh hưởng và khả năng tái hiện nếu phù hợp.
3. **PM:** xác nhận vấn đề, phạm vi, ưu tiên và liên kết với tài liệu nghiệp vụ.
4. **Kỹ thuật/Thiết kế:** đề xuất cách xử lý, ước lượng và triển khai.
5. **QA/QC:** nghiệm thu theo tiêu chí trong issue.
6. **Đóng issue:** chỉ khi có bằng chứng kết quả hoặc ghi rõ lý do không thực hiện.

## Tiêu chuẩn đóng issue

Một issue được coi là hoàn tất khi:

- kết quả đáp ứng tiêu chí chấp nhận;
- các khu vực liên quan đã được kiểm tra hồi quy phù hợp;
- tài liệu liên quan được cập nhật nếu hành vi nghiệp vụ thay đổi;
- có liên kết PR/commit hoặc bằng chứng tương đương;
- không còn câu hỏi mở ảnh hưởng đến việc sử dụng thực tế.
