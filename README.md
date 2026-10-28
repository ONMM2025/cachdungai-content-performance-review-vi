# Đánh giá hiệu quả nội dung

> **Một repository, một skill.** Workflow độc lập bằng tiếng Việt cho AI Agent.
>
> **Watermark:** [https://cachdungai.blog/](https://cachdungai.blog/)

## Giới thiệu

Phân tích số liệu website và mạng xã hội để đề xuất thử nghiệm nội dung đo được. Dùng khi có dữ liệu theo thời gian và mục tiêu rõ; không suy diễn nguyên nhân từ tương quan yếu.

Mở **SKILL.md** để xem đầu vào, quy trình, đầu ra, giới hạn và prompt mẫu. Gói cài đặt chứa SKILL.md và giấy phép MIT, không kèm script thực thi.

## Tải gói cài đặt

Tải ZIP sẵn dùng: [content-performance-review-vi.zip](content-performance-review-vi.zip). ZIP có thư mục gốc tên **content-performance-review-vi** và chứa **SKILL.md**, phù hợp để tải lên như một skill riêng.

## Cách cài

### Claude.ai

1. Nếu Skills chưa hiện, kiểm tra Settings > Capabilities và bật code execution nếu tài khoản/workspace hỗ trợ.
2. Mở **Customize > Skills**, bấm **+ > Create skill > Upload a skill**.
3. Chọn tệp **content-performance-review-vi.zip** vừa tải và bật skill sau khi upload.

Khả năng tạo và dùng skill phụ thuộc gói tài khoản, bật code execution và chính sách workspace.

### Claude Code

Chép **SKILL.md** vào **.claude/skills/content-performance-review-vi/SKILL.md** trong dự án hoặc **~/.claude/skills/content-performance-review-vi/SKILL.md** để dùng cá nhân. Gọi bằng **/content-performance-review-vi** hoặc mô tả yêu cầu để Claude tự chọn khi phù hợp.

### ChatGPT

Skills chỉ xuất hiện ở các tài khoản/workspace đủ điều kiện; hiện trang trợ giúp OpenAI nêu Business, Enterprise, Healthcare và Edu, tùy thiết lập workspace.

1. Mở **Plugins > Plugin Directory > Skills**.
2. Chọn **Create > Upload from your computer**.
3. Chọn **content-performance-review-vi.zip**.

Nếu không có mục Skills, mở **SKILL.md** rồi dán nội dung vào yêu cầu hoặc Project instructions nếu có. Đây là cách dùng thủ công, không phải cài skill tự động.

### Codex

Trong repo dự án, chép **SKILL.md** vào **.agents/skills/content-performance-review-vi/SKILL.md**, rồi yêu cầu Codex dùng skill này.

## Prompt mẫu

“So sánh 12 bài Facebook trong tháng này với 12 bài tháng trước. Mục tiêu là kéo click về blog. Hãy tính CTR nếu có impressions và link clicks, nêu điểm chưa đủ dữ liệu, rồi đề xuất ba thử nghiệm cho tháng tới.”

Gửi thêm mục tiêu, độc giả, tài liệu đầu vào, nền tảng và giới hạn cần giữ để kết quả sát hơn. Kiểm tra dữ kiện và duyệt nội dung trước khi xuất bản.

## Giấy phép

MIT License — xem file **LICENSE** trong repository.

---

**Watermark:** [https://cachdungai.blog/](https://cachdungai.blog/)
