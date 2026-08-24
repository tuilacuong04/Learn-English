# 🎙️ English for Client Calls — Coach Workspace

Chào mừng bạn đến với workspace luyện tiếng Anh giao tiếp chuyên sâu cho **Software Engineer**.

Hệ thống đã được tích hợp trực tiếp vào **Antigravity Skill** (`.agents/skills/english-coach/SKILL.md`), **Workspace Rule** (`AGENTS.md`) và **Hệ thống lưu trữ tự động Notes** (`notes/`).

---

## ⚡ Bảng Lệnh Tắt (Slash Commands)

| Lệnh chính | Viết tắt | Mô tả chi tiết | Ví dụ sử dụng |
|---|---|---|---|
| *(Gõ bình thường)* | | Chạy toàn bộ **Khung 9 bước tiêu chuẩn** | `phân biệt between và among` |
| `/check` hoặc `/answers` | `/a` | Chấm bài tập vừa giao ở lượt trước theo thang `✅`/`❌` + sửa lỗi | `/check` hoặc `/a` |
| `/save` | `/s` | **Tự động lưu Notes:** Ghi các chunk, lỗi sai và chủ đề vào thư mục `notes/` | `/save` hoặc `/s` |
| `/review` | `/r` | **Ôn tập giãn cách:** Đọc `notes/` và ra 5 câu kiểm tra phản xạ | `/review` hoặc `/r` |
| `/notes` | `/n` | **Xem sổ tay:** Tóm tắt nhanh các chunks và lỗi sai đã lưu | `/notes` hoặc `/n` |
| `/fast` | `/quick` | Chế độ vội: chỉ trả về **Chốt + Ví dụ + Bài tập** | `/fast delay deadline` |
| `/examples` | `/ex` | Cung cấp 6 ví dụ mới hoàn toàn trong các ngữ cảnh khác biệt | `/examples` hoặc `/ex` |
| `/harder` | `/h` | Nâng độ khó của bài tập lên một bậc | `/harder` hoặc `/h` |
| `/roleplay <tình huống>` | `/t <tình huống>` | **Roleplay cuộc họp:** AI đóng vai Client/PM, 100% tiếng Anh. Gõ `/stop` để tổng kết. | `/roleplay daily standup: blocked by auth service` |
| `/feedback <đoạn text>` | `/f <đoạn text>` | **Feedback thư/chat:** Soát lỗi và tối ưu hóa văn phong tin nhắn Slack/Email | `/feedback I cannot finish task today because db bug` |
| `/decode <câu>` | `/d <câu>` | **Decode câu khách nói:** Ý thật → Vì sao không kịp → Nối âm → 3 câu mẫu | `/decode Could we circle back to this by EOD?` |
| `/debate` hoặc `/why` | `/sao` | Phản biện lại một điểm sửa của Coach để được giải thích sâu hơn | `/why câu này tôi thấy tài liệu dùng được mà` |
| `/stop` | | Kết thúc phiên Roleplay và xuất bảng tổng kết, sửa lỗi chi tiết | `/stop` |

---

## 📓 Hệ Thống Lưu Trữ Notes Tự Động (`notes/`)

Thay vì phải copy-paste thủ công ra ngoài, bạn chỉ cần gõ `/save` (hoặc `/s`), AI Coach sẽ tự động cập nhật vào:

1. **[`notes/learning_log.md`](file:///c:/Users/tuila/Learn-English/notes/learning_log.md)**: Nhật ký học tập theo phương pháp lặp lại ngắt quãng (Spaced Repetition: `+2d`, `+7d`, `+21d`).
2. **[`notes/chunks_vault.md`](file:///c:/Users/tuila/Learn-English/notes/chunks_vault.md)**: Kho tra cứu nhanh các cụm từ (Chunks) theo từng tình huống IT (Standup, Demo, Blocker, Clarification...).
3. **[`notes/my_mistakes.md`](file:///c:/Users/tuila/Learn-English/notes/my_mistakes.md)**: Sổ tay lỗi sai cá nhân (Lỗi sai → Câu chuẩn → Giải thích nguyên nhân).

---

## 🎯 Khung Trả Lời Chuẩn (Default 9-Step Framework)

1. **Sửa tiền đề:** Nếu câu hỏi dựa trên hiểu lầm, chỉ rõ ngay trong 1 dòng.
2. **Chốt:** Trả lời trực diện, súc tích (1–2 dòng).
3. **Bản chất:** Cơ chế hoạt động + Dấu hiệu nhận biết trong 1 giây (Áp dụng tư duy lập trình).
4. **Ví dụ thật:** 6–8 câu (50% IT meeting/chat, 50% đời thường), kèm cặp **SAI ↔ ĐÚNG**.
5. **Ngoài đời người ta nói thế nào:** Nhãn tần suất ⭐/○/✕, nối âm thực tế, văn phong nói/viết.
6. **Mẹo & Trick:** Cách nhớ và **đường thoát an toàn** khi bí từ.
7. **Chunk từ vựng:** Tối đa 7 cụm từ ≥3 chữ (kèm IPA chỗ khó, tần suất, ví dụ).
8. **Bẫy người Việt:** 2–3 lỗi điển hình thường gặp.
9. **Bài tập 3 bậc (Không đưa trước đáp án):**
   - Bậc 1: Nhận diện (Trắc nghiệm/Đúng sai).
   - Bậc 2: Điền từ khuyết.
   - Bậc 3: Dịch tình huống công việc thực tế (Production).
10. **Một dòng đóng:** Thúc đẩy bạn phản xạ và trả lời ngay bằng 2 câu tiếng Anh.

---

## 📁 Cấu Trúc Thư Mục Workspace

```text
Learn-English/
├── .agents/
│   └── skills/
│       └── english-coach/
│           └── SKILL.md       # Antigravity Skill Engine
├── AGENTS.md                  # Workspace Rules (Luôn kích hoạt)
├── README.md                  # Hướng dẫn & Cheatsheet tra cứu nhanh
├── notes/                     # Kho ghi chú tự động (Được AI cập nhật khi gõ /save)
│   ├── learning_log.md        # Lịch ôn giãn cách Spaced Repetition
│   ├── chunks_vault.md        # Kho cụm từ (Chunks) theo chủ đề
│   └── my_mistakes.md         # Sổ tay lỗi sai của bạn
└── Doc/                       # Tài liệu tham khảo
```
