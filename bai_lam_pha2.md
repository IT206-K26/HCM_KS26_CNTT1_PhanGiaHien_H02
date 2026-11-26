# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 06
- **Họ tên: Phan Gia Hiển**
- **Lớp: CNTT1**
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini): Gemini**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt bàn ra JSON

**KET QUA AI**

```text
[{"ma_buffet":"NUONG","ngay_dat":"2026-12-19","nguoi_lon":2,"tre_em":1,"khu_vuc":"trong_nha","ghi_chu":null},{"ma_buffet":"HAISAN","ngay_dat":"2027-01-03","nguoi_lon":3,"tre_em":0,"khu_vuc":null,"ghi_chu":"Một người dị ứng sữa"},{"ma_buffet":"LAU","ngay_dat":"2026-12-25","nguoi_lon":4,"tre_em":0,"khu_vuc":"san_vuon","ghi_chu":"ông ngoại đi xe lăn"}]
```

**Link trò chuyện: https://share.gemini.google/QotpkdO0JllJ**

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
**Báo giá Bếp Việt Buffet – Gói Buffet Nướng (NUONG)**

* **Người lớn (10 khách):** 10 × 399.000 = 3.990.000 đồng
* **Trẻ em từ 1 m đến 1,4 m (3 bé: 1,1 m; 1,2 m; 1,35 m – tính 50%):** 3 × 199.500 = 598.500 đồng
* **Trẻ em dưới 1 m (1 bé: 0,8 m):** 0 đồng (miễn phí)
* **Tổng tiền buffet trước giảm:** 3.990.000 + 598.500 = 4.588.500 đồng
* **Giảm giá 5% (áp dụng cho đoàn từ 10 người lớn):** 4.588.500 × 5% = 229.425 đồng
* **Tiền buffet sau giảm:** 4.588.500 - 229.425 = 4.359.075 đồng
* **Phụ thu phòng riêng (1 phòng, không áp dụng giảm giá):** 500.000 đồng

**Tổng cộng:** 4.359.075 + 500.000 = **4.859.075 đồng**.
```

**Link trò chuyện: https://share.gemini.google/unBKAAb8Lybw**

### b) Kiểm tra kết quả AI

(Ghi kết luận AI đúng hay sai; nếu sai, ghi bước sai đầu tiên và kết quả đúng của bước đó – xoá dòng này)

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{"loai_su_co":"thieu_mon","so_khach":5,"so_mon_bi_thieu":2,"tom_tat":"Nhóm 5 khách ăn buffet bị hết tôm hùm và cua suốt tối, chờ bổ sung không có."} Chào anh/chị, nhà hàng chân thành xin lỗi gia đình về việc hết món tôm hùm và cua trong bữa buffet tối 08/11/2026. Theo chính sách, nhà hàng xin gửi mức hoàn tiền là 1.000.000 đồng cho nhóm 5 khách (100.000 đồng/khách cho mỗi món bị thiếu). Mong anh/chị thông cảm và cho nhà hàng xin thông tin tài khoản để tiến hành hoàn tiền sớm nhất.
```

**Link trò chuyện: https://share.gemini.google/q4IEAsRshRg2**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
### 1. Điểm từng tiêu chí (Thang 10)

| Tiêu chí | Trọng số | Điểm (Thang 10) | Điểm quy đổi | Dẫn chứng thực tế |
| --- | --- | --- | --- | --- |
| **Đúng thông tin** | 50% | **0 / 10** | 0,0 | Báo sai cả hai thông tin cốt lõi: giá buffet ghi *279k* (chuẩn: 299.000 đồng) và cam kết *trễ 40 phút vẫn giữ bàn* (chuẩn: trễ trên 30 phút huỷ bàn). |
| **Đầy đủ** | 30% | **0 / 10** | 0,0 | Không cộng điểm cho hai nội dung trả lời sai; đồng thời thiếu hoàn toàn lời mời khách cung cấp **ngày, giờ đến và số khách** để đặt bàn (chỉ viết chung chung *"Có gì nhắn em nhé!"*). |
| **Giọng điệu** | 20% | **3 / 10** | 0,6 | Có xưng hô lễ phép cơ bản (*"Dạ chào chị"*), nhưng thiếu chuyên nghiệp và dùng từ ngữ suồng sã (*"nha"*, *"ngon bá cháy luôn"*, *"279k"*). |

### 2. Điểm tổng

* **Công thức:** $(0 \times 50\%) + (0 \times 30\%) + (3 \times 20\%) = 0,6$
* **Tổng điểm:** **0,6 / 10**

### 3. Nhận xét ngắn gọn

Bài làm **không đạt yêu cầu** do truyền đạt sai lệch hoàn toàn các chính sách quan trọng về giá và quy định giữ bàn, dễ gây khiếu nại cho khách hàng khi đến quán. Ngoài ra, nhân viên quên bước khai thác thông tin đặt bàn bắt buộc (ngày, giờ, số lượng khách) và sử dụng văn phong quá suồng sã, chưa phù hợp với tiêu chuẩn chăm sóc khách hàng chuyên nghiệp. Cần đào tạo lại quy trình nắm bắt thông tin sản phẩm và chuẩn mực giao tiếp trước khi tiếp nhận tư vấn thực tế.
```

**Link trò chuyện: https://share.gemini.google/FfamTuCzODL6**
