## 4.2. Trích xuất tin nhắn đặt vé ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "SVT",
    "ngay_su_kien": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "loai_ve": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "FZ",
    "ngay_su_kien": "2027-01-05",
    "nguoi_lon": 3,
    "tre_em": 0,
    "loai_ve": "thuong",
    "ghi_chu": "cần hỗ trợ xe lăn"
  },
  {
    "ma_goi": "VIP",
    "ngay_su_kien": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "loai_ve": "vip",
    "ghi_chu": "cần hỗ trợ tìm chỗ"
  }
]
```

**Link trò chuyện:** https://share.gemini.google/nkdGDwWTGbl1

## 4.3. Báo giá vé bằng Chain-of-Thought

**KET QUA AI**

```text
**Bước 1: Tiền người lớn**

* Nhóm mua gói SVT có đơn giá là 1.200.000 đồng/người lớn và có 5 người lớn.
* Phép tính: $5 \times 1.200.000 = 6.000.000\text{ đồng}$

**Bước 2: Tiền trẻ em**

* 2 trẻ em (8 tuổi và 10 tuổi) nằm trong độ tuổi từ 5 đến 11 tuổi nên tính 70% giá người lớn: $70\% \times 1.200.000 = 840.000\text{ đồng/trẻ em}$.
* 1 bé 3 tuổi (dưới 5 tuổi) được miễn phí: $0\text{ đồng}$.
* Phép tính: $(2 \times 840.000) + (1 \times 0) = 1.680.000\text{ đồng}$

**Bước 3: Tiền vé**

* Tổng tiền vé gồm tiền người lớn cộng với tiền trẻ em.
* Phép tính: $6.000.000 + 1.680.000 = 7.680.000\text{ đồng}$

**Bước 4: Giảm giá nhóm**

* Nhóm có 5 người lớn (đạt điều kiện từ 5 người lớn trở lên) nên được giảm 5% trên tổng tiền vé.
* Tiền được giảm: $7.680.000 \times 5\% = 384.000\text{ đồng}$
* Tiền vé sau giảm: $7.680.000 - 384.000 = 7.296.000\text{ đồng}$

**Bước 5: Phụ thu**

* Có 1 người lớn chọn khu ghế ưu tiên với mức phụ thu 300.000 đồng/người.
* Phép tính: $1 \times 300.000 = 300.000\text{ đồng}$

**Bước 6: Tổng tiền**

* Tổng tiền thanh toán bằng tiền vé sau giảm cộng với tiền phụ thu.
* Phép tính: $7.296.000 + 300.000 = 7.596.000\text{ đồng}$

[Result: 7.596.000đồng]
```

**Link trò chuyện:** https://share.gemini.google/PwDWEs94ktpQ

### b) Kiểm tra kết quả AI

Đúng 

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "sai_khu_vuc",
  "so_khach": 2,
  "so_hiep_bi_anh_huong": 2,
  "tom_tat": "Khách mua gói có mái che nhưng bị xếp sang khu không mái trong 2 hiệp đầu gặp trời mưa."
}
```

**Link trò chuyện:** https://share.gemini.google/dkTF0r1MaFe0

