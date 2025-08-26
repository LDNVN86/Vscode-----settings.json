# VS Code — `settings.json` (Compact Folders & Explorer Tweaks)
[English](#english) • [Tiếng Việt](#tiếng-việt)


---

## English

### Overview
This repository provides a ready-to-use **VS Code `settings.json`** focused on a cleaner Explorer: it **compacts single-child folders** so paths like `src/components/Button` display in one line. It keeps your tree tidy and improves navigation in large projects.

### Features
- **Compact single-child folders** in Explorer (`a/b/c` on one line).
- Clean, shareable **JSON configuration** for both global and workspace scopes.
- Optional Explorer/UI niceties (commented in the snippet).

### Repository Structure
```
.
├─ settings.json        # Main VS Code settings
└─ assets/              # Images referenced in README (add your own)
   ├─ cover.png
   ├─ before.png
   └─ after.png
```

### Quick Start

**Option A — Apply for all projects (User Settings)**
1. Open VS Code → press `Ctrl/Cmd + Shift + P` → **Open Settings (JSON)**.
2. Paste the contents of [`settings.json`](./settings.json) and save.

**Option B — Apply per project (Workspace)**
1. In your project, create: `.vscode/settings.json`.
2. Paste the contents of [`settings.json`](./settings.json) and save.

> Tip: Workspace settings override User settings for that project.

### Core Settings (excerpt)
```jsonc
{
  // Show single-child folders as a compact path "a/b/c"
  "explorer.compactFolders": true,

  // Optional suggestions — safe to remove if you don't need them
  "explorer.autoReveal": true,
  "workbench.iconTheme": "vs-seti"
}
```

### Screenshots

- Before enabling compact folders:  
  ![Before](./assets/before.png)

- After enabling compact folders:  
  ![After](./assets/after.png)


### FAQ
- **Team use?**  
  Yes. Commit `.vscode/settings.json` to your repo so teammates get the same Explorer behavior.

- **Conflicts with other settings?**  
  Minimal. Workspace settings take precedence over User settings.

### Contributing
PRs and issues are welcome for additional Explorer/Editor tweaks.

---

## Tiếng Việt

### Tổng quan
Repo này cung cấp **file `settings.json` cho VS Code** với mục tiêu làm Explorer gọn gàng hơn: **gộp/nén các thư mục chỉ có 1 mục con** để đường dẫn như `src/components/Button` hiển thị trên một dòng. Việc duyệt cây thư mục trở nên nhanh và rõ ràng hơn, nhất là với dự án lớn.

### Tính năng
- **Gộp thư mục 1-con** trong Explorer (hiển thị kiểu `a/b/c`).
- Cấu hình **JSON** dễ chia sẻ, dùng được cho cả phạm vi người dùng lẫn từng workspace.
- Một vài tinh chỉnh Explorer/UI (được comment trong snippet, tuỳ chọn dùng).

### Cấu trúc repo
```
.
├─ .vscode/settings.json	    # Cài đặt chính cho VS Code
└─ assets/              	# Ảnh dùng trong README (bạn tự thêm)
   ├─ cover.png
   ├─ before.png
   └─ after.png
```

### Bắt đầu nhanh

**Cách A — Áp dụng cho mọi dự án (User Settings)**
1. Mở VS Code → nhấn `Ctrl/Cmd + Shift + P` → **Open Settings (JSON)**.
2. Dán nội dung từ [`settings.json`](./settings.json) và lưu.

**Cách B — Áp dụng theo từng dự án (Workspace)**
1. Trong thư mục dự án, tạo: `.vscode/settings.json`.
2. Dán nội dung từ [`settings.json`](./settings.json) và lưu.

> Lưu ý: Workspace Settings **ưu tiên** hơn User Settings trong dự án đó.

### Thiết lập cốt lõi (trích)
```jsonc
{
  // Hiển thị thư mục chỉ có 1 mục con theo dạng "a/b/c"
  "explorer.compactFolders": true,

  // Gợi ý thêm (tuỳ chọn) — có thể xoá nếu không dùng
  "explorer.autoReveal": true,
  "workbench.iconTheme": "vs-seti"
}
```

### Ảnh minh hoạ

- Trước khi bật gộp thư mục:  
  ![Trước](./assets/before.png)

- Sau khi bật gộp thư mục:  
  ![Sau](./assets/after.png)


### Hỏi nhanh — đáp gọn
- **Dùng cho cả team?**  
  Được. Commit `.vscode/settings.json` vào repo để mọi người dùng chung cấu hình.

- **Có xung đột cài đặt khác?**  
  Hiếm. Nếu có, VS Code sẽ ưu tiên `Workspace Settings`.

### Đóng góp
Chào mừng issue/PR để bổ sung các tinh chỉnh Explorer/Editor hữu ích.

---
