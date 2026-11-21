# Phiếu QC 1 — Road v1.0 (bản đang chờ kiểm tay)

Lô được kiểm (học viên): phamtrungthanh
Người kiểm (học viên): DoAnhHoang
Ngày: 2026-11-21
Phiên bản guideline: Road v1.0
File được kiểm (tên + `revision` trong manifest): phamtrungthanh-front.zip và phamtrungthanh-fisheye.zip, revision 1
Số ảnh kiểm tay: Chưa ghi nhận; lint đã quét 28 ảnh (16 front, 12 fisheye)
Số nhãn đã kiểm tay (shape + tag): Chưa thực hiện

Lưu ý: Bản zip của phamtrungthanh hiện không còn trong workspace. Các dòng dưới đây chỉ ghi lại đầu ra lint đã chạy trước đó, không phải kết quả kiểm thị giác đầy đủ và không được xem là QC1 hoàn tất.

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm tay | Số lỗi kiểm tay | Kết quả lint (không phải kết luận QC) |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-02 đủ L1, R1 | bỏ sót | Chưa kiểm | Chưa xác nhận | 5 cảnh báo |
| QC1-03 position | sai thuộc tính / thừa | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-06 style, color, kind | sai thuộc tính | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | Chưa kiểm | Chưa xác nhận | Không có cảnh báo |
| QC1-12 file | lỗi file | 2 ZIP đã lint lúc kiểm | Không có lỗi mở file được ghi nhận | 2 ZIP đọc được lúc lint; manifest khai báo không kèm ảnh |

## Cảnh báo lint cần kiểm trên ảnh gốc
| # | Mã | Ảnh | Nhãn | Mức gợi ý | Mô tả |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-02 | A05_b2576c8c-2de20b8a.jpg | lane | nặng | Không thấy L1 trong export |
| 2 | QC1-02 | A05_b2576c8c-2de20b8a.jpg | lane | nặng | Không thấy R1 trong export |
| 3 | QC1-02 | A06_b8c66e31-37045eec.jpg | lane | nặng | Không thấy R1 trong export |
| 4 | QC1-02 | A07_b41ace08-c8468690.jpg | lane | nặng | Không thấy L1 trong export |
| 5 | QC1-02 | A09_c7e6d5d1-c8af9fe3.jpg | lane | nặng | Không thấy R1 trong export |

## Ca mơ hồ / việc cần làm tiếp
| Ảnh | Câu hỏi cho lead | Lời đáp |
| --- | --- | --- |
| A05, A06, A07, A09 | Các vạch L1/R1 có thực sự nhìn thấy trong ảnh không? Nếu không thấy, coach cần xác nhận miễn trừ theo quy định trước khi bỏ qua cảnh báo. | Chưa xác nhận cho lô của phamtrungthanh |

## Quyết định
Lỗi nặng: Chưa kết luận bằng kiểm tay (5 cảnh báo lint cần xác minh)
Lỗi chính: Chưa kiểm
Lỗi nhẹ: Chưa kiểm
Ca chờ lead: 4 ảnh
Quyết định (Release / Hold / Rework): Hold — chờ kiểm tay
Lý do: Không còn ZIP để kiểm ảnh và phiếu QC1 này mới có đầu ra lint, chưa đủ mẫu kiểm tay, mẫu số hoặc danh sách lỗi đã xác nhận. Không thể kết luận Release hay Rework chỉ từ lint.
