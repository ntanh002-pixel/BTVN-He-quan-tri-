# k58KTPM
# Bài tập 2 của sinh viên: Nguyễn Tuấn Anh - K225480106002

Đề Bài :
BÀI TOÁN:
- Tạo csdl quan hệ với tên QLSV gồm các bảng sau:
  + SinhVien(#masv,hoten,NgaySinh)
  + Lop(#maLop,tenLop)
  + GVCN(#@maLop,#@magv,#HK)
  + LopSV(#@maLop,#@maSV,ChucVu)
  + GiaoVien(#magv,hoten,NgaySinh,@maBM)
  + BoMon(#MaBM,tenBM,@maKhoa)
  + Khoa(#maKhoa,tenKhoa)
  + MonHoc(#mamon,Tenmon,STC)
  + LopHP(#maLopHP,TenLopHP,HK,@maMon,@maGV)
  + DKMH(#@maLopHP,#@maSV,DiemTP,DiemThi,PhanTramThi)

YÊU CẦU:
1. Thực hiện các hành động sau trên giao diện đồ hoạ để tạo cơ sở dữ liệu cho bài toán:
  + Tạo database mới, mô tả các tham số(nếu có) trong quá trình.
  + Tạo các bảng dữ liệu với các trường như mô tả, chọn kiểu dữ liệu phù hợp với thực tế (tự tìm hiểu)
  + Mỗi bảng cần thiết lập PK, FK(s) và CK(s) nếu cần thiết. (chú ý dấu # và @: # là chỉ PK, @ chỉ FK)
2. Chuyển các thao tác đồ hoạ trên thành lệnh SQL tương đương. lưu tất cả các lệnh SQL trong file: Script_DML.sql

Bài Làm:
1. Kết nối tài khoản SQL server
![Screenshot (142)](https://github.com/user-attachments/assets/61a6ca78-4992-4ea3-ab7f-6dda62526ec5)
2. Tạo Database mới
![Screenshot (143)](https://github.com/user-attachments/assets/6a3fafcb-11c4-492b-b865-2cee31f8abf2)
- Đặt tên Database là QLSV
![Screenshot (144)](https://github.com/user-attachments/assets/d55f2c3d-7929-4874-952a-3aa14b3007ef)
- chọn New ==> click vào table để tạo bảng.
  ![Screenshot (145)](https://github.com/user-attachments/assets/ee48a0a1-548e-4d7b-83f3-30d1446d994c)
- thêm các thuộc tính theo yêu cầu vào bảng và kiểu dữ liệu phù hợp với thuộc tính đó ==> lưu bảng và đặt tên bảng.
  ![image](https://github.com/user-attachments/assets/4ec00d44-75c9-4432-9d96-10fe225ff5d7)
  
  ![image](https://github.com/user-attachments/assets/08f7f338-59fa-4b4c-998a-3cb0d72e914e)
  
  ![image](https://github.com/user-attachments/assets/7999459e-f648-4700-906f-2afd43c33df5)
  
  ![image](https://github.com/user-attachments/assets/e9e5a04d-05df-49e7-a049-b23097e25f2a)
  
  ![image](https://github.com/user-attachments/assets/e8f8776f-963e-4809-bfca-4702475bf19d)
  
  ![image](https://github.com/user-attachments/assets/d3e84ecf-4c6b-4f7f-a898-bfcea7bd4af1)
  
  ![image](https://github.com/user-attachments/assets/e29812e2-7839-4f24-8fc4-5045495373a6)
  
  ![image](https://github.com/user-attachments/assets/8c4fad36-a9ab-487d-9e06-4d06b21086a9)
  
  ![image](https://github.com/user-attachments/assets/494b4aa5-35e2-41fb-aecf-1a25f085fb5e)
  
  ![image](https://github.com/user-attachments/assets/71708400-ee4b-4f9b-bc13-331903b2f268)

  2: cài khoá ngoại cho các thuộc tính ở các bảng

  ![image](https://github.com/user-attachments/assets/bc67d7c2-9230-4d04-989c-725cd11d7820)

  ![image](https://github.com/user-attachments/assets/2100ca2f-1488-49e3-a699-d98a34c2356e)

  ![image](https://github.com/user-attachments/assets/423ebba8-8735-4f76-bee5-89b500654b5b)

  ![image](https://github.com/user-attachments/assets/c2d783a2-5cea-44c8-ae2a-d4b4606fdc24)

  ![image](https://github.com/user-attachments/assets/1a60b44c-bb76-446f-afd7-0a2e6154a0b9)

  ![image](https://github.com/user-attachments/assets/eed58468-cf74-471f-b1a3-48bc03d37070)

  ![image](https://github.com/user-attachments/assets/3644c2d1-5632-4541-a8e3-e55cb0ef7e2c)

  ![image](https://github.com/user-attachments/assets/a740717c-1251-4d34-9a3e-e5ca7f7871ba)

  ![image](https://github.com/user-attachments/assets/8f712521-31e4-40da-981b-699362e39de9)

  ![image](https://github.com/user-attachments/assets/ae341e78-de45-4d3c-817c-505f8e27a245)

 3:  Chuyển các thao tác đồ họa sang lệnh SQL:
 - chọn Tasks ==> chọn Generate Scripts ...

![Screenshot (173)](https://github.com/user-attachments/assets/8464ece3-e4ff-4209-875c-d6c53195b968)

- Trang Introduction ==> chọn next.

![Screenshot (174)](https://github.com/user-attachments/assets/262b6edf-e8d2-4ae3-8f95-75500aad5748)

- Trang Choose Objects chọn select specific database objects ==> click tables . next

![Screenshot (175)](https://github.com/user-attachments/assets/070eeaa9-dc55-4ddc-931c-a769b3ef2257)

- 

![Screenshot (176)](https://github.com/user-attachments/assets/dea444c7-c82b-413c-9742-53d235c57776)

![Screenshot (177)](https://github.com/user-attachments/assets/2a03095c-083a-4889-843f-1cd487eb0f72)

![Screenshot (178)](https://github.com/user-attachments/assets/8f95cff3-3362-47b8-9493-b13d4e2e0b74)














