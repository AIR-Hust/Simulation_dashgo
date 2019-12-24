# Simulation_dashgo
Phần mềm mô phỏng là một trong những yếu tố quan trọng trong nghiên cứu robot .Có thể nói một trong những thách thức lớn nhất trong xây dựng robot hữu ích là phần mềm .Thông qua mô phỏng ta hiểu được vẫn đề trong sử dụng cảm biến nhằm xác định robot ở đâu ,lập ra kế hoạch và tính toán để robot thực hiện.

Trong hướng dẫn này, ta phát triển một mô phỏng robot từ đầu dựa trên hình mẫu có thực (dashgobot). 

Quy trình mô phỏng có ưu điểm:

- Mô phỏng robot có thể tùy chỉnh bằng cách chỉnh sửa mô hình URDF. 

- Cho phép phát triển thuật toán tương thích giữa phần cứng và phần mềm.(tránh hao tổn phần cứng vì phát triển quá mức).

- Làm việc dựa trên nền tảng kế thừa tránh lặp lại công việc và lỗi lầm của người đi trước.

SIMULATION MODEL

Mục tiêu :Tạo mô hình URDF trên trình giả lập Gazebo có thể truy cập bởi ROS.

Tài liệu tham khảo:

Kết quả :Mô hình Robot của dashgobot.

 Cấu truc thư mục:
** Dashgo_description **
- launch

  - dashgo_gazebo.launch
  
- models

- urdf

- dashgobase

  - meshes
  
  - dashgo.gazebo.xacro
  
  - dashgo.urdf.xacro
  
- worlds

  - dashgo_world.world

Khi khởi chạy dashgo_gazebo.launch .Một môi trường ảo trong gazebo được tạo ra chứa các world và model đã được xây dựng kết nối với Ros thông qua các node có thể hiển thị trên Rviz.

## Chạy mô phỏng :

`  roslaunch dashgo_description dashgo_gazebo.launch  `
<img src='https://imgur.com/CkoJwEa' >

## Các chỉnh sửa mô hình thực hiện trong 2 file 
-  dashgo.urdf.xacro  
-  dashgo.gazebo.xacro 
