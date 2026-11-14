
🚀 TuiMem (tuimem.apk)

Android Performance Monitor & Optimizer powered by Pure Rust Core & On-Device AI
Ứng dụng Giám sát & Tối ưu Hiệu năng Android với Lõi Rust thuần túy & AI On-Device
🌐 Language / Ngôn ngữ: English • Tiếng Việt

🇬🇧 English


📖 Overview

Inspired by Samsung Memory Guardian's architecture, TuiMem is a next-generation Android memory monitor and optimizer re-engineered with an ultra-fast Rust core (libtuimem_core.so) and an on-device AI scoring engine. Built to keep your device smooth and battery-friendly without requiring Root access.

✨ Key Highlights

• 🦀 Blazing-Fast Rust Core: Reads system metrics directly from /proc (/proc/meminfo, /proc/stat, /proc/<pid>) instead of heavy Android APIs — delivering near-zero overhead, pinpoint accuracy, and minimal battery drain in a tiny ~1.7 MB APK.
• 🧠 Fully Automated On-Device AI: Analyzes 7 real-time system features (RAM usage, RAM rising trend, CPU load, Swap, process count, top RSS) via linear regression to compute a 0–100 performance score. Since v1.1.0, the AI automatically calculates the safest, smoothest optimization level — just toggle it on and let AI handle the rest.
• 🛡️ Multi-Layer Anti-Kill Defense: Engineered to survive aggressive OEM background killers (Xiaomi, OPPO, vivo, Samsung, Huawei):
	• 3 Independent Keep-Alive Layers: Foreground Service (START_STICKY) + WorkManager (15-min periodic check) + Hidden Account Sync channel.
	• Notification Safety Net: Automatically revives the foreground service and notification within seconds if accidentally dismissed.
	• Smart OEM Assistant (AntiKillManager): Auto-detects your device brand and provides tailored setup steps with one-tap shortcuts to Ignore Battery Optimizations & Auto-Start settings.
• 🔒 Safe, Transparent & Root-Free: Uses strictly standard Android APIs (KILL_BACKGROUND_PROCESSES). Built-in smart whitelist protects System UI, Google Play Services, your Launcher, and active heavy apps. Supports instant EN / VI UI switching.

🇻🇳 Tiếng Việt


📖 Tổng quan

Lấy cảm hứng từ kiến trúc của Samsung Memory Guardian, TuiMem là ứng dụng giám sát và tối ưu bộ nhớ Android thế hệ mới, được tái thiết kế với lõi xử lý viết bằng Rust (libtuimem_core.so) siêu tốc và mô hình AI chạy trực tiếp trên thiết bị. Giúp điện thoại luôn mượt mà, tiết kiệm pin mà hoàn toàn không cần Root.

✨ Điểm nổi bật

• 🦀 Lõi Rust thuần túy siêu nhẹ: Đọc trực tiếp thông số hệ thống từ /proc (/proc/meminfo, /proc/stat, /proc/<pid>) thay vì phụ thuộc vào các API Android nặng nề — mang lại tốc độ phản hồi tức thì, độ chính xác cao và tiết kiệm pin tối đa trong bộ cài chỉ ~1.7 MB.
• 🧠 AI On-Device tự động hóa hoàn toàn: Phân tích 7 đặc trưng hệ thống theo thời gian thực (mức RAM, xu hướng tăng RAM, tải CPU, Swap, số lượng tiến trình, top RSS) để chấm điểm hiệu năng từ 0–100. Từ bản v1.1.0, AI tự động tính toán mức tối ưu cân bằng nhất giữa độ mượt, độ an toàn RAM và thời lượng pin — chỉ cần bật công tắc và để AI tự vận hành.
• 🛡️ Công nghệ chống bị OEM "Kill" đa tầng: Giải quyết triệt để tình trạng đóng app ngầm trên Xiaomi, OPPO, vivo, Samsung, Huawei:
	• 3 lớp giữ sống độc lập: Foreground Service (START_STICKY) + WorkManager (kiểm tra mỗi 15 phút) + kênh đồng bộ ẩn Account Sync.
	• Lưới an toàn Notification: Tự động khôi phục dịch vụ chạy ngầm và thông báo chỉ sau vài giây nếu vô tình bị vuốt tắt.
	• Trợ lý cấu hình theo hãng (AntiKillManager): Tự động nhận diện hãng máy để hiển thị hướng dẫn từng bước cùng nút mở nhanh cài đặt Bỏ tối ưu pin & Tự khởi động.
• 🔒 An toàn, Minh bạch & Không cần Root: Chỉ sử dụng API chuẩn của Android (KILL_BACKGROUND_PROCESSES). Whitelist thông minh bảo vệ tuyệt đối System UI, Google Play Services, Launcher và các ứng dụng nặng đang hoạt động. Hỗ trợ chuyển đổi song ngữ Anh / Việt ngay trên giao diện chính.

📱 Technical Specs & Quick Start / Thông số & Cài đặt


Specification / Thông số	Details / Chi tiết
Latest Version / Phiên bản	v1.2.1
Android Support / Hỗ trợ	Android 8.0 (minSdk 26) – Android 14 (targetSdk 34)
Architectures / Kiến trúc	arm64-v8a, armeabi-v7a
Tech Stack / Công nghệ	Kotlin, Jetpack Compose, Rust (rustc 1.100), JNI, DataStore, WorkManager
 Download here https://github.com/dinoking-iot/TuiMem/releases/tag/TuiMem
 
Installation / Cài đặt nhanh:
1. Download tuimem.apk from the Releases section (or install via adb install -r tuimem.apk).
Tải file tuimem.apk tại mục Releases (hoặc cài qua lệnh adb install -r tuimem.apk).
2. Open TuiMem and follow the one-tap setup prompt to grant Ignore Battery Optimizations & Auto-Start permissions for uninterrupted 24/7 protection.
Mở TuiMem và làm theo hướng dẫn 1 chạm để cấp quyền Bỏ tối ưu pin & Tự khởi động giúp ứng dụng bảo vệ máy 24/7.
Design by dinoking • Facebook.com/biglinuxviet
