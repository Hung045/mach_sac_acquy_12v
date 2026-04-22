# Mạch Sạc Acquy 12V

## Giới thiệu
Dự án thiết kế mạch sạc acquy 12V với điện áp đầu vào AC 220V. Mạch được thiết kế hoàn chỉnh với cả mô phỏng trong Proteus và bố cục PCB trong Altium Designer.

## Nội dung dự án

### Thư mục chính

#### `BTL_mach_nap_acquy_12v_altium/`
Thiết kế PCB trong **Altium Designer**:
- **BTL_mach_nap_acquy_12v_chia_khoi.SchDoc** - Sơ đồ nguyên lý chi tiết chia theo khối chức năng
- **BTL_mach_nap_acquy_12v.PcbDoc** - Bố cục PCB 2 lớp
- **BTL_mach_nap_acquy_12v.PrjPcb** - File dự án Altium
- **linh_kien.xlsx** - Danh sách linh kiện (BOM - Bill of Materials)

#### `BTL_mach_nap_acquy_12v_proteus/`
Mô phỏng mạch trong **Proteus**:
- **BTL_mach_nap_acquy_12v.pdsprj** - File dự án mô phỏng Proteus

## Thông số kỹ thuật

### Đầu vào
- Điện áp AC: 220V ± 10%
- Tần số: 50Hz

### Đầu ra
- Điện áp DC: 12V (ổn định)
- Dòng sạc: Tối đa ~5A

## Các khối chức năng chính

1. **Khối cấp nguồn AC** - Biến áp hạ thế 220V → 18V AC
2. **Khối chỉnh lưu** - Cầu chỉnh lưu 4 diode
3. **Khối lọc** - Tụ điện và cuộn cảm để làm mịn sóng
4. **Khối ổn áp** - IC 7812 hoặc LM7812 để ổn định 12V
5. **Khối bảo vệ** - Diode bảo vệ, fuse, hạn dòng

## Hướng dẫn sử dụng

### Xem sơ đồ nguyên lý
1. Mở **Altium Designer**
2. Mở file `BTL_mach_nap_acquy_12v_chia_khoi.SchDoc`

### Xem bố cục PCB
1. Mở **Altium Designer**
2. Mở file `BTL_mach_nap_acquy_12v.PcbDoc`

### Chạy mô phỏng
1. Mở **Proteus 8**
2. Mở file `BTL_mach_nap_acquy_12v.pdsprj`
3. Nhấn **Play** để chạy mô phỏng

## Yêu cầu phần mềm

- **Altium Designer** 19.0 hoặc cao hơn (cho thiết kế PCB)
- **Proteus 8** hoặc cao hơn (cho mô phỏng)

## Linh kiện chính

Danh sách linh kiện chi tiết có trong file **linh_kien.xlsx**. 

Các linh kiện quan trọng:
- Biến áp: 220V/18V
- Diode 1N4007: 4 cái (cầu chỉnh lưu)
- IC 7812: Ổn áp 12V
- Tụ điện: Điện phân 10μF, 100μF...
- Cuộn cảm lọc
- Điện trở hạn dòng
- Fuse và cầu an toàn

## Ghi chú
- PCB được thiết kế 2 lớp để dễ sản xuất
- Tất cả linh kiện dễ mua trên thị trường
- Mạch đã được mô phỏng và hoạt động ổn định

**Cập nhật lần cuối:** 2026-04-22