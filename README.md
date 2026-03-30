<div align="center">

# ⚡ Fix VT-x / AMD-v
### Vô hiệu hóa Hyper-V, VBS, Credential Guard để bật ảo hóa phần cứng

![platform](https://img.shields.io/badge/Windows-10%20%7C%2011-blue?logo=windows&logoColor=white)
![version](https://img.shields.io/badge/Phiên%20bản-v1.0.1.5-brightgreen)
![author](https://img.shields.io/badge/Tác%20giả-Phạm%20Triển%20PH58258-8A2BE2?logo=github)
![license](https://img.shields.io/badge/Miễn%20phí-100%25-orange)

<br/>

[![Download](https://img.shields.io/badge/⬇️%20%20TẢI%20NGAY%20FILE%20EXE%20%20⬇️-v1.0.1.5-brightgreen?style=for-the-badge&logo=windows&logoColor=white&labelColor=1a7f37)](https://github.com/PhTrien/FixVT-x_AMD-v/raw/main/Tien%20ich%20fix%20ao%20hoa%20v1.0.1.5.exe)

</div>

---

## 🖥️ Giao diện

<img width="1196" height="906" alt="image" src="https://github.com/user-attachments/assets/7182f9c2-3c9b-4647-aa97-8303dfb6b5bf" />

> Giao diện trực quan với panel chọn bước bên trái và log output real-time bên phải.

---

## 🤔 Dùng khi nào?

Bạn đang gặp một trong các lỗi sau khi mở VMware / VirtualBox / giả lập Android:

- ❌ **VT-x is not available (VERR_VMX_NO_VMX)**
- ❌ **AMD-V is disabled in the BIOS**
- ❌ **Intel VT-x is disabled**
- ❌ Máy ảo không khởi động được dù đã bật VT trong BIOS

Nguyên nhân thường là **Hyper-V, VBS, Credential Guard** đang chiếm quyền ảo hóa. Tool tự động tắt hết chúng chỉ với 1 cú nhấp.

---

## ▶️ Cách sử dụng

**3 bước đơn giản, không cần cài đặt:**

**1.** Tải file EXE bằng nút xanh bên trên

**2.** Chuột phải → **Run as Administrator**

**3.** Trong giao diện:
   - Nhấn **"Chọn tất cả"** *(khuyến nghị)*
   - Nhấn nút **▶ Chạy**

> 💡 **Windows SmartScreen hiện cảnh báo?**  
> Bấm **More info** → **Run anyway**

---

## 📋 Các bước xử lý

| Bước | Chức năng |
|:---:|---|
| **1** | Disable Hyper-V Hypervisor |
| **2** | Tắt HypervisorLaunchType + VsmLaunchType |
| **3** | Disable DISM — Hyper-V, VMP, WHP |
| **4** | Tắt VBS và Credential Guard |
| **5** | Set-ExecutionPolicy Unrestricted |
| **6** | Chạy DG_Readiness_Tool -Disable |

> ⭐ **Ưu tiên chọn tất cả và chạy** để đảm bảo fix hoàn toàn.

---

## 🔄 Sau khi chạy xong

1. Máy sẽ tự động **khởi động lại**
2. Khi màn hình bật lên → **bấm `F3` liên tục** để hoàn tất quá trình

> ⚠️ *Khi máy khởi động lên — bấm F3 F3 F3 F3 để tiếp tục*

---

## ⚠️ Lưu ý

- Bắt buộc chạy với quyền **Administrator**
- Tool sẽ chỉnh **registry** và **tắt tính năng hệ thống**
- **Đọc kĩ hướng dẫn trước khi dùng**

---

<div align="center">

Thấy hữu ích? Hãy ⭐ **star repo** để ủng hộ tác giả!

**Made with ❤️ by Phạm Triển — PH58258**

</div>
