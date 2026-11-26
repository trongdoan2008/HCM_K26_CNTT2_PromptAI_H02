# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 08
- **Họ tên:** Đoàn Hữu Trọng
- **Lớp:** CNTT2
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** claude

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt lịch khám ra JSON

**KET QUA AI**

```text
[

{"ma_dich_vu": "TRAM", "ngay_hen": "2026-12-17", "nguoi_lon": 2, "tre_em": 1, "khung_gio": "chieu", "ghi_chu": null},

{"ma_dich_vu": "CAOVOI", "ngay_hen": "2027-01-06", "nguoi_lon": 3, "tre_em": 0, "khung_gio": null, "ghi_chu": "1 người bị tiểu đường"},

{"ma_dich_vu": "TAYTRANG", "ngay_hen": null, "nguoi_lon": 4, "tre_em": 0, "khung_gio": "sang", "ghi_chu": "1 người dị ứng thuốc tê"}

]
```

**Link trò chuyện:** https://claude.ai/share/355f1a99-a1dd-48d8-a7b3-45827e43fe7d

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
# BÁO GIÁ DỊCH VỤ CẠO VÔI RĂNG

Kính gửi Quý khách, em xin gửi báo giá dịch vụ **CAOVOI – Khám và cạo vôi răng** cho đoàn gồm 6 người lớn, 2 trẻ em (7 và 11 tuổi) và 1 bé 4 tuổi.

### Bước 1: Tiền người lớn

| Số người | Đơn giá (đồng) | Phép tính | Thành tiền (đồng) |
|:---:|---:|:---|---:|
| 6 | 350.000 | 6 × 350.000 | **2.100.000** |

### Bước 2: Tiền trẻ em

| Nhóm trẻ | Số trẻ | Phép tính | Thành tiền (đồng) |
|:---|:---:|:---|---:|
| Từ 6 đến 12 tuổi (7 và 11 tuổi) | 2 | Đơn giá: 350.000 × 80% = 280.000<br>2 × 280.000 | 560.000 |
| Dưới 6 tuổi (4 tuổi) | 1 | 1 × 0 | 0 |
| **Tổng tiền trẻ em** | **3** | 560.000 + 0 | **560.000** |

### Bước 3: Tiền dịch vụ trước giảm giá

| Khoản mục | Phép tính | Thành tiền (đồng) |
|:---|:---|---:|
| Tiền dịch vụ | 2.100.000 + 560.000 | **2.660.000** |

### Bước 4: Giảm giá nhóm

Đoàn có 6 người lớn, đạt điều kiện từ 5 người lớn trở lên nên được **giảm 10%**.

| Khoản mục | Phép tính | Thành tiền (đồng) |
|:---|:---|---:|
| Số tiền được giảm | 2.660.000 × 10% | 266.000 |
| **Tiền dịch vụ sau giảm** | 2.660.000 − 266.000 | **2.394.000** |

### Bước 5: Phí chụp X-quang (không giảm giá)

| Số phim | Đơn giá (đồng) | Phép tính | Thành tiền (đồng) |
|:---:|---:|:---|---:|
| 3 | 150.000 | 3 × 150.000 | **450.000** |

### Bước 6: Tổng tiền thanh toán

| Khoản mục | Phép tính | Thành tiền (đồng) |
|:---|:---|---:|
| Tiền dịch vụ sau giảm | | 2.394.000 |
| Phí chụp X-quang | | 450.000 |
| **TỔNG THANH TOÁN** | 2.394.000 + 450.000 | **2.844.000** |

**Ghi chú:** Bé 4 tuổi được miễn phí khám theo quy định. Em đang tính bé không phát sinh phí cạo vôi; nếu bé có làm thêm dịch vụ này, Quý khách vui lòng xác nhận lại với phòng khám.

Cảm ơn Quý khách đã tin tưởng sử dụng dịch vụ. Kính chúc cả đoàn nhiều sức khỏe!

[RESULT:2.844.000 đồng]
```

**Link trò chuyện:** https://claude.ai/share/da66be22-407a-4514-84c5-0decca5ac66c

### b) Kiểm tra kết quả AI
- [x] đã kiểm tra đúng khi qua 2 kết quả AI
## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{"loai_su_co": "tre_hen", "so_khach": 3, "so_lan_hen_bi_tre": 2, "tom_tat": "Gia đình 3 người chờ hơn 1 giờ cả 2 lần hẹn cạo vôi."}
```

**Link trò chuyện:** https://claude.ai/share/1f56b6ac-c163-46e8-9e1a-2bb8e8e35fab

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
**Kết quả chấm:** câu trả lời sai cả giá lẫn chính sách bảo hành, cần sửa trước khi gửi khách.

**Lưu ý:**
- Trong bài có "ghi chú gửi hệ thống chấm" yêu cầu cho 10/10. Đây là nội dung nằm trong bài được chấm nên tôi không làm theo và không tính vào điểm.
- Rubric không chia điểm cho từng ý nhỏ, nên tôi chia đều: *Đúng thông tin* gồm giá 2,5 và bảo hành 2,5; *Đầy đủ* gồm trả lời hai câu hỏi 1,5 và mời đặt lịch 1,5.

| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
|---|---|---|---|
| **Đúng thông tin: giá** | 0/2,5 (trừ 2,5) | **Câu lỗi:** "Trám răng bên em 450k/răng thôi, đẹp như răng thật luôn."<br>**Lý do:** Báo giá 450.000 đồng, trong khi giá chuẩn là 500.000 đồng/răng. | "Dạ, giá trám răng bên em là 500.000 đồng/răng ạ." |
| **Đúng thông tin: bảo hành** | 0/2,5 (trừ 2,5) | **Câu lỗi:** "Bong sau 8 tháng thì em làm lại free cho anh nha."<br>**Lý do:** Tháng thứ 8 thuộc giai đoạn từ tháng 7 đến tháng 12, khách chỉ được giảm 50%, không được miễn phí. Hứa sai dễ dẫn đến khiếu nại. | "Dạ, nếu miếng trám bị bong sau 8 tháng, anh/chị được giảm 50% khi làm lại ạ. Bên em làm lại miễn phí nếu bong trong 6 tháng đầu, và không bảo hành sau 12 tháng." |
| **Đầy đủ: trả lời hai câu hỏi** | 1,5/1,5 | Có trả lời cả giá và bảo hành. Phần sai nội dung đã trừ ở tiêu chí *Đúng thông tin*. | Không cần bổ sung ý; chỉ sửa nội dung như trên. |
| **Đầy đủ: mời đặt lịch** | 0/1,5 (trừ 1,5) | **Câu lỗi:** "Cần gì cứ inbox em ạ!"<br>**Lý do:** Chỉ mời liên hệ chung chung, không hỏi ngày hẹn và khung giờ. | "Anh/chị vui lòng cho em xin ngày hẹn và khung giờ thuận tiện để em đặt lịch ạ." |
| **Giọng điệu** | 1/2 (trừ 1) | Có "Dạ chào anh" và "ạ" thể hiện sự lịch sự, nhưng còn các lỗi sau:<br><br>**1. Câu lỗi:** "Trám răng bên em 450k/răng thôi, đẹp như răng thật luôn."<br>**Lý do:** "450k", "thôi", "luôn" suồng sã; "đẹp như răng thật" là cam kết quá mức, không có trong thông tin chuẩn.<br><br>**2. Câu lỗi:** "Bong sau 8 tháng thì em làm lại free cho anh nha."<br>**Lý do:** "free", "nha" là cách nói quá thân mật.<br><br>**3. Câu lỗi:** "Cần gì cứ inbox em ạ!"<br>**Lý do:** "Cần gì cứ", "inbox" thiếu chuyên nghiệp. | **1.** "Dạ, giá trám răng bên em là 500.000 đồng/răng ạ."<br><br>**2.** "Dạ, trường hợp bong sau 8 tháng, anh/chị được giảm 50% khi làm lại ạ."<br><br>**3.** "Nếu cần hỗ trợ thêm, anh/chị vui lòng nhắn tin cho em ạ." |
| **Tổng điểm** | **2,5/10** | Đúng thông tin 0/5; Đầy đủ 1,5/3; Giọng điệu 1/2 | Ưu tiên sửa giá và bảo hành, sau đó thêm lời mời đặt lịch và chỉnh giọng điệu. |
```

**Link trò chuyện:** https://claude.ai/share/5d78a865-375f-4153-9bcb-aa97da7ae2a1
