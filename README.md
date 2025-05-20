# Sinh tín hiệu với CVAE và CNN-CVAE

## Tổng quan

Dự án này tập trung vào việc sinh tín hiệu sinh lý giả lập bằng hai mô hình học sâu:

- **CVAE**
- **CNN-CVAE**

Cả hai mô hình đều sinh tín hiệu có điều kiện dựa trên các thông số sinh lý quan trọng:  
**Nhịp thở (RR)** và **Nhịp tim (HR)**.

## Dữ liệu

Dữ liệu sử dụng là bộ dữ liệu **BIDMC**, chứa các tín hiệu sinh lý có chú thích, phù hợp cho nghiên cứu về sinh tín hiệu và phân tích.

## Mô hình

### CVAE
- Mô hình biến phân tự mã hóa có điều kiện, sinh tín hiệu dựa trên RR và HR.
- Học biểu diễn tiềm ẩn của tín hiệu có điều kiện.

### CNN-CVAE
- Mở rộng CVAE bằng cách sử dụng các lớp chập (CNN).
- Giúp mô hình nắm bắt tốt hơn các đặc trưng theo thời gian và không gian của tín hiệu.
- Cũng được điều kiện hóa trên RR và HR để sinh tín hiệu theo ý muốn.

![image](https://github.com/user-attachments/assets/b7f545f3-7b19-42d8-9e72-5c595daaca9c)
