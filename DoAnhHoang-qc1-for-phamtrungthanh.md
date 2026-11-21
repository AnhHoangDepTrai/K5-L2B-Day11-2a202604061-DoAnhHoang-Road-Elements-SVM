# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): phamtrungthanh
Người kiểm (học viên): DoAnhHoang
Ngày: 2026-11-21
Phiên bản guideline: Road v1.0
File được kiểm (tên + `revision` trong manifest): phamtrungthanh-front.zip và phamtrungthanh-fisheye.zip, revision 1
Số ảnh kiểm: 28 (+ 8 ảnh thêm trong hai ZIP, ghi riêng)
Số nhãn đã kiểm (shape + tag): 347 (235 shape + 112 tag), theo lint toàn lô

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 28 | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | 40 | 5 | nặng |
| QC1-03 position | sai thuộc tính / thừa | 48 | 0 | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 48 | 0 | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 48 | 0 | chính |
| QC1-06 style, color, kind | sai thuộc tính | 48 | 0 | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 85 | 0 | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 102 | 0 | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 102 | 0 | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | 102 | 0 | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 12 | 0 | chính |
| QC1-12 file | lỗi file | 2 | 0 | nhẹ / nặng |

## Danh sách lỗi
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-02 | A05_b2576c8c-2de20b8a.jpg | lane | nặng | Thiếu L1 |
| 2 | QC1-02 | A05_b2576c8c-2de20b8a.jpg | lane | nặng | Thiếu R1 |
| 3 | QC1-02 | A06_b8c66e31-37045eec.jpg | lane | nặng | Thiếu R1 |
| 4 | QC1-02 | A07_b41ace08-c8468690.jpg | lane | nặng | Thiếu L1 |
| 5 | QC1-02 | A09_c7e6d5d1-c8af9fe3.jpg | lane | nặng | Thiếu R1 |

## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| A05_b2576c8c-2de20b8a.jpg | Cần xác nhận lane L1/R1 có thực sự thấy được trên ảnh không | Chưa có lời đáp; theo quy định, chỉ bỏ qua nếu coach xác nhận không thấy vạch |
| A06_b8c66e31-37045eec.jpg | Cần xác nhận R1 có thực sự thấy được không | Chưa có lời đáp |
| A07_b41ace08-c8468690.jpg | Cần xác nhận L1 có thực sự thấy được không | Chưa có lời đáp |
| A09_c7e6d5d1-c8af9fe3.jpg | Cần xác nhận R1 có thực sự thấy được không | Chưa có lời đáp |

## Quyết định
Lỗi nặng: 5
Lỗi chính: 0 / 347 nhãn = 0 %
Lỗi nhẹ: 0
Ca chờ lead: 4 ảnh
Quyết định (Release / Hold / Rework): Rework
Lý do (theo luật của phiếu): Có 5 cảnh báo nặng QC1-02 (thiếu L1/R1) theo lint; theo quy tắc phiếu, có lỗi nặng thì Rework, trừ khi coach xác nhận trên ảnh thực sự không có vạch.
