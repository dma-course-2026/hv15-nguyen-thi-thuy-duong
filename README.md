# Danh sách học viên – Training DMA

Danh sách học viên cập nhật phục vụ công tác tổ chức và quản lý lớp Data / AI / ML.

## Danh sách học viên

| ID | Họ và tên | Công việc | Năm sinh | Trường/Nơi làm việc | Chuyên ngành/Vai trò |
| --- | --- | --- | --- | --- | --- |
| HV01 | Trần Bình Minh | Sinh viên đại học | 2008 | ĐH Mỏ - Địa chất | CNTT |
| HV02 | Tạ Hồng Quân | Sinh viên đại học | 2007 | ĐH KHTN | Toán |
| HV03 | Nguyễn Khắc Tuấn | Dev | 1998 | Fetek / ĐH Thủy lợi | Software Dev |
| HV04 | Đàm Viết Khôi | Sinh viên | 2007 | NEU | Chưa rõ |
| HV05 | Nguyễn Trung Duy | QA | 1996 | GPBank / ĐH CN Việt Hung | QA Core |
| HV06 | Phạm Xuân Phong | Sinh viên | 2008 | ĐH Bách khoa Hà Nội | Chưa rõ |
| HV07 | Nguyễn Đức Mạnh | DE | 2000 | Fetek / ĐH Bách khoa HN | ĐTVT, DE |
| HV08 | Vũ Quang Huy | DE | 2004 | VPBank / ĐH KHTN | DE |
| HV09 | Đặng Gia Bảo | Sinh viên đại học | 2007 | Chưa cung cấp | Chưa cung cấp |
| HV10 | Tạ Đức Mạnh | Sinh viên đại học | 2007 | ĐH Giao thông Vận tải | ĐTVT |
| HV11 | Đàm T Vân Anh | NVVP | 1998 |  |  |
| HV12 | Nguyễn Trung Thành | Kỹ sư ô tô |  |  |  |
| HV13 | Đinh Vĩnh Anh | DE |  |  |  |
| HV14 | Lê Đức Anh | Sinh viên đại học |  |  |  |
| HV15 | Nguyễn Thị Thùy Dương |  |1986  |  |  |
| HV16 | Đào Duy Anh | Sinh viên đại học |  |  |  |
| HV17 | Trịnh Quang Anh | Sinh viên đại học |  |  |  |

## Ghi chú

- Các ô trống là thông tin chưa được cung cấp hoặc chưa xác nhận.
Get-Content $HOME\.ssh\config# DMA Course 2026

Repository cá nhân dùng để lưu trữ bài tập và sản phẩm học tập trong khóa **DMA Course 2026**.

## Thông tin học viên

- **Mã học viên:** `<hv15>`
- **Họ và tên:** `<Nguyễn Thị Thùy Dương>`

> Hãy cập nhật thông tin phía trên khi thiết lập repository lần đầu.

## Cấu trúc repository

```text
.
├── assignments/
│   ├── README.md
│   ├── wXX-topic/
│   └── ...
│
├── .github/
│   └── pull_request_template.md
│
├── .gitignore
└── README.md
```

### `assignments/`

Chứa toàn bộ bài tập hàng tuần.

Mỗi bài tập được đặt trong một thư mục riêng theo format:

```text
assignments/wXX-topic/
```

Quy định chi tiết về:
- cách đặt tên folder/file;
- cách đặt tên branch;
- cách đặt tiêu đề Pull Request;
- workflow nộp bài;
- cách sửa bài sau review;

xem tại:

[`assignments/README.md`](assignments/README.md)

### `.github/`

Chứa các cấu hình dành cho GitHub.

Hiện tại bao gồm:

```text
.github/
└── pull_request_template.md
```

File này được GitHub sử dụng làm mẫu khi học viên tạo Pull Request để nộp bài.

### `.gitignore`

Khai báo các file/thư mục không nên đưa lên Git, ví dụ:

- môi trường local;
- file cấu hình IDE;
- cache;
- secret;
- API key;
- password.

## Quy trình nộp bài hàng tuần

```text
main
  ↓
tạo branch bài tập
  ↓
làm bài
  ↓
commit thay đổi
  ↓
push branch
  ↓
tạo Pull Request
  ↓
instructor review
  ↓
sửa bài nếu cần
  ↓
merge vào main
```

Các lệnh cơ bản:

```bash
git checkout main
git pull
git checkout -b hw/wXX-topic

# Làm bài

git status
git add .
git commit -m "feat: complete assignment"
git push -u origin hw/wXX-topic
```

Sau đó tạo Pull Request:

```text
hw/wXX-topic → main
```

## Quy tắc quan trọng

- Không làm bài trực tiếp trên `main`.
- Mỗi bài tập dùng một branch riêng.
- Bài tập phải nằm trong thư mục `assignments/`.
- Không commit password, API key hoặc secret.
- Không commit môi trường local hoặc file rác.
- Dùng commit message có ý nghĩa.
- Kiểm tra code/notebook chạy được trước khi nộp.
- Nếu instructor yêu cầu sửa bài, tiếp tục sửa trên cùng branch và Pull Request hiện tại.
- Chỉ merge vào `main` sau khi bài đã được review/approve.

---

Repository này là hồ sơ học tập xuyên suốt khóa học. Hãy giữ cấu trúc rõ ràng, dễ chạy lại và dễ review.
