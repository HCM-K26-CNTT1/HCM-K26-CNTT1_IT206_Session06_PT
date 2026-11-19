# SO SÁNH TRADE-OFF CÁC GIẢI PHÁP PROMPTING TRONG HỌC TẬP

## 1. Đề xuất 2 giải pháp

**Giải pháp 1 – Prompt đơn giản:**
```text
Bạn là gia sư AI. Hãy giải thích bài học theo phương pháp Feynman và chấm câu trả lời theo rubric 10 điểm. Nêu lỗi sai và cách cải thiện.
```

**Giải pháp 2 – Prompt chi tiết:**
```text
Bạn là gia sư AI và trợ lý chấm bài.
Hãy giải thích kiến thức bằng phương pháp Feynman, sau đó chấm theo rubric:
- Hiểu đúng khái niệm: 4 điểm.
- Giải thích rõ ràng: 2 điểm.
- Phân biệt CPU với RAM: 2 điểm.
- Trình bày chính xác: 2 điểm.
Nêu điểm từng tiêu chí, tổng điểm và hướng cải thiện.
Nếu thiếu dữ liệu hoặc rubric, không tự suy đoán mà phải thông báo.
Temperature: 0.0.
```

## 2. Bảng so sánh Trade-off

| Tiêu chí | Giải pháp 1 | Giải pháp 2 |
|---|---|---|
| Dễ hiểu | Cao | Trung bình |
| Tốn token | Ít | Nhiều |
| Chặn lỗi biên | Trung bình | Tốt |
| Độ chính xác | Khá | Cao hơn |

## 3. Lựa chọn và chạy thử

**Chọn giải pháp 2** vì có rubric rõ ràng, kiểm soát dữ liệu thiếu và hạn chế AI chấm điểm tùy ý.

**Dữ liệu thử:** CPU là bộ nhớ lưu trữ dữ liệu.

**Kết quả Gemini chạy :** ### Phần 1: Giải thích kiến thức bằng phương pháp Feynman (CPU)

**Nhận định sai cần sửa ngay:** **CPU không phải là bộ nhớ lưu trữ dữ liệu.**

Hãy tưởng tượng máy tính như một **gian bếp**:

* **CPU (Central Processing Unit – Bộ xử lý trung tâm)** giống như **người đầu bếp**: người trực tiếp nhận công thức (chương trình), cầm dao thớt, nêm nếm và thực hiện các thao tác tính toán, ra quyết định để tạo ra món ăn. Đầu bếp chỉ làm việc tại chỗ, không phải là cái tủ chứa thực phẩm.
* **RAM (Random Access Memory – Bộ nhớ truy cập ngẫu nhiên)** giống như **mặt bàn bếp**: nơi bày biện nguyên liệu và dụng cụ đang dùng ngay lúc đó để đầu bếp lấy nhanh. Khi tắt bếp (tắt máy), đồ trên mặt bàn không còn giữ cố định cho lần nấu sau.
* **Ổ cứng (SSD/HDD)** giống như **tủ lạnh / nhà kho**: nơi cất giữ nguyên liệu và công thức lâu dài kể cả khi đã tắt bếp.

**Tóm lại theo ngôn ngữ đơn giản:**

* **CPU** là **bộ não / người thực hiện tính toán và điều khiển**, không phải nơi lưu trữ dữ liệu lâu dài hay bộ nhớ chứa dữ liệu như ổ cứng/RAM.
* **RAM** là **bộ nhớ làm việc tạm thời tốc độ cao**, giữ dữ liệu và lệnh mà CPU đang xử lý ngay lập tức.

---

### Phần 2: Chấm bài theo Rubric

Bài làm được đánh giá: *"CPU là bộ nhớ lưu trữ dữ liệu."*

* **Hiểu đúng khái niệm: 0 / 4 điểm**
Nhận định sai bản chất: đồng nhất CPU với bộ nhớ lưu trữ dữ liệu, trong khi chức năng cốt lõi của CPU là xử lý, tính toán và điều khiển thực thi lệnh.
* **Giải thích rõ ràng: 0 / 2 điểm**
Chỉ là một câu khẳng định ngắn gọn, thiếu giải thích cơ chế hoạt động, ví dụ minh họa hay làm rõ cách dữ liệu được xử lý.
* **Phân biệt CPU với RAM: 0 / 2 điểm**
Không đề cập đến RAM cũng như sự khác biệt giữa đơn vị xử lý (CPU) và bộ nhớ tạm thời (RAM).
* **Trình bày chính xác: 0 / 2 điểm**
Nội dung chưa chính xác về mặt kỹ thuật máy tính; câu ngắn gọn nhưng sai kiến thức nền tảng.

**Tổng điểm:** **0 / 10 điểm**

---

### Phần 3: Hướng cải thiện

1. **Sửa lỗi khái niệm cốt lõi:** Luôn gắn **CPU** với từ khóa **xử lý / tính toán / điều khiển**, không gọi CPU là bộ nhớ lưu trữ dữ liệu.
2. **Dùng ví dụ đời sống (Feynman):** Tập giải thích lại bằng ngôn ngữ đời thường sao cho người chưa học IT cũng hiểu được sự khác nhau giữa "người làm việc" (CPU), "chỗ để đồ đang làm" (RAM) và "kho chứa" (ổ cứng).
3. **Bổ sung phần so sánh CPU – RAM:** Khi nhắc đến CPU, hãy nêu thêm vai trò của RAM (lưu tạm dữ liệu/chương trình đang chạy để CPU truy xuất nhanh) để câu trả lời đầy đủ và chặt chẽ hơn.
4. **Viết câu hoàn chỉnh, kiểm chứng thuật ngữ:** Thay vì một câu khẳng định rời rạc, hãy trình bày thành 2–3 câu rõ ý: định nghĩa đúng của CPU, vai trò của RAM, và mối liên hệ giữa hai thành phần này.
