- Kiểm tra version của: git --version
- Cấu hình cho git:

  1. git config --global user.name ''
  2. git congig --global user.email ''

- Khởi tạo git: git init
- Kiểm tra trạng thái và xem nó có phải là một repo không : git status
- Thêm vào môi trường: git add \* || git add --all || git add -A
- Khi hoàn thành công việc để có thể quay lại nếu phát hiện ra lỗi chúng ta sửa dụng: git commit -m "Text commit"
- Khi thực hiện những thay đổi nhỏ, mà không cần sửa dụng lại môi trường dàn dựng, có thể thay đổi trực tiếp mà bỏ qua môi trường dàn dựng

- Kiểm tra sự thay đổi một file nào đó: git status --short
- Kiểm tra sự cam kết git : git log
