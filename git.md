// Hưỡng dẫn sửa dụng Git.

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
- Kiểm tra sự cam kết git : git log (nhật kí thay đổi)
- Trợ giúp git : git -help , git command --help , git help --all

- Nhánh git (git branch): Được hiểu là làm viẹc trên một nhánh mới mà không ảnh hưởng đến nhánh chính, và có thể hợp nhất với nhánh chính.
  - Thêm một nhánh mới : git branch <ten nhánh mới>
  - Xác nhận đã tạo một branch: git branch
  - Di chuyển từ branch sang nhánh khác: git checkout <ten nhánh>
  - sửa dụng -b tuỳ chọn bật checkout sẽ tạo ta một nhánh mới và di chuyển đến nó nếu nó không tồn tại.
  - tạo ra một nhánh mới khẩn cấp: git checkout -b <ten nhánh>
  - Hợp nhất các nhánh lại: git merge <ten nhánh cần hợp nhất>
  - Xoá nhánh git : git branch -d <ten nhánh cần xoá >

// Git và Github.

- Đăng kí tài khoản github
- Tạo repository
- Đẩy kho lưu trữ cục bộ lên github

  - Đẩy lên kho lưu trữ : git remote add origin <URL>
  - Đẩy nhánh của mình đến URL gốc và làm nhánh mặc định : git push --set -u origin master

- Pull from github (git pull):
  - Pull là sự kết hợp giữa fetch(tải về) và merge(hợp nhất);
  - Tải mã nguồn về : git fetch origin --> origin/master
  - Hợp nhất mã nguồn : git merge origin/master
  - Git pull: thay thế cho fetch và merge sửa dụng để kéo tất cả các thay đổi từ kho lưu trữ về nhánh bạn đang làm việc
- Đẩy lên github: git push <ten nhánh>
- Nhánh mới github: Tạo từ github
- Kéo một nhánh từ github: git pull
- Đẩy nhánh lên github: git push origin <ten nhánh>
- Trang github: github page bạn cần tạo một tên đặc biệt theo sau
  là .github.io
