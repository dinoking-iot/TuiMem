🚀 TuiMem — Android Performance Monitor & Optimizer powered by Rust Core & On-Device AI!
🚀 TuiMem — Ứng dụng Giám sát & Tối ưu Hiệu năng Android với Lõi Rust và AI On-Device!
Looking for a lightweight, battery-friendly tool to keep your Android device smooth without requiring Root? Meet TuiMem (tuimem.apk) — a next-generation memory management app inspired by Samsung Memory Guardian's architecture, supercharged with an ultra-fast Rust core and real-time on-device Artificial Intelligence.
Bạn đang tìm kiếm một công cụ nhẹ nhàng, tiết kiệm pin giúp điện thoại Android luôn mượt mà mà không cần Root? Hãy trải nghiệm TuiMem (tuimem.apk) — giải pháp quản lý bộ nhớ thế hệ mới lấy cảm hứng từ kiến trúc Samsung Memory Guardian, được nâng cấp toàn diện với lõi Rust siêu tốc và trí tuệ nhân tạo chạy trực tiếp trên thiết bị.

✨ Key Features / Điểm nổi bật

🦀 Pure Rust Core (libtuimem_core.so) / Sức mạnh từ Lõi Rust thuần túy
• EN: Instead of relying on restricted, resource-heavy Android APIs, TuiMem's Rust core reads system metrics directly from /proc (/proc/meminfo, /proc/stat, /proc/<pid>). This delivers blazing speed, pinpoint accuracy, and minimal battery drain in a tiny ~1.7 MB package.
• VI: Thay vì phụ thuộc vào các API Android truyền thống vốn bị giới hạn và tốn tài nguyên, lõi Rust của TuiMem đọc trực tiếp thông số hệ thống từ /proc (/proc/meminfo, /proc/stat, /proc/<pid>). Điều này mang lại tốc độ xử lý cực nhanh, độ chính xác cao và tiết kiệm pin tối đa với dung lượng siêu nhẹ chỉ ~1.7 MB.
🧠 Smart On-Device AI — Fully Automated / AI On-Device thông minh — Tự động hóa hoàn toàn
• EN: Zero internet required, zero lag. TuiMem uses an on-device linear regression AI model analyzing 7 real-time system features (RAM usage, RAM rising trend, CPU load, Swap, background processes, etc.) to calculate a 0–100 performance score. Since v1.1.0, the AI automatically determines the optimal optimization level to keep your phone smooth and RAM safe while conserving battery — just flip the switch and let AI handle the rest.
• VI: Không cần mạng, không độ trễ. TuiMem tích hợp mô hình AI tuyến tính phân tích 7 đặc trưng hệ thống theo thời gian thực (mức RAM, xu hướng tăng RAM, tải CPU, Swap, tiến trình nền...) để chấm điểm hiệu năng từ 0–100. Từ bản v1.1.0, AI tự động tính toán mức tối ưu phù hợp nhất để giữ máy mượt mà, an toàn cho RAM và tiết kiệm pin — bạn chỉ cần bật công tắc và để AI lo phần còn lại.
🛡️ Multi-Layer Anti-Kill Protection / Công nghệ chống bị OEM "Kill" đa tầng
• EN: Aggressive background app killing on Xiaomi, OPPO, vivo, Samsung, and Huawei is a major headache. TuiMem solves this with:
	• 3 Independent Keep-Alive Layers: Foreground Service (START_STICKY), WorkManager (15-min periodic check), and a hidden Account Sync channel. If one is stopped, the others wake it right back up.
	• Notification Safety Net: Automatically restores the foreground service and notification within seconds if accidentally dismissed.
	• OEM-Specific Assistant (AntiKillManager): Auto-detects your device manufacturer to provide tailored step-by-step guides and one-tap shortcuts to "Ignore Battery Optimizations" and "Auto-Start" settings.
• VI: Việc các hãng (Xiaomi, OPPO, vivo, Samsung, Huawei) tự động đóng ứng dụng chạy ngầm là nỗi ám ảnh lớn nhất với các app tối ưu. TuiMem giải quyết triệt để nhờ:
	• 3 lớp giữ sống độc lập: Kết hợp Foreground Service (START_STICKY), WorkManager (kiểm tra định kỳ 15 phút) và kênh đồng bộ ẩn Account Sync. Bất kỳ lớp nào còn sống đều sẽ đánh thức các lớp khác.
	• Lưới an toàn Notification: Tự động khôi phục trạng thái chạy ngầm và thông báo chỉ sau vài giây nếu vô tình bị vuốt tắt.
	• Trợ lý cấu hình theo hãng (AntiKillManager): Tự động nhận diện hãng máy để đưa ra hướng dẫn chi tiết và nút mở nhanh trang cài đặt "Bỏ tối ưu pin" & "Tự khởi động" chuẩn xác nhất.
🔒 Safe, Transparent & Root-Free / An toàn, Minh bạch & Không cần Root
• EN: 100% Non-Root using standard Android APIs (KILL_BACKGROUND_PROCESSES). Smart whitelist protects System UI, Google Play Services, your Launcher, and active heavy apps. Features a modern Jetpack Compose UI with built-in EN/VI language switching.
• VI: 100% không cần Root, chỉ dùng API chuẩn của Android (KILL_BACKGROUND_PROCESSES). Whitelist thông minh bảo vệ tuyệt đối System UI, Google Play Services, Launcher và các app đang chạy tác vụ nặng. Giao diện Jetpack Compose hiện đại, hỗ trợ chuyển đổi song ngữ Anh/Việt trực tiếp trong app.

📱 Specs & Installation / Thông số & Cài đặt

• Compatibility / Tương thích: Android 8.0 (SDK 26) – Android 14 (Target SDK 34)
• Architectures / Kiến trúc: arm64-v8a & armeabi-v7a
• Current Version / Phiên bản hiện tại: v1.2.1
• How to install / Cách cài đặt: Download tuimem.apk, allow installation from unknown sources, and open the app. On first launch, follow the one-tap setup prompt to grant Battery & Auto-Start permissions for 24/7 protection. / Tải tuimem.apk, cho phép cài đặt từ nguồn không xác định và mở app. Ở lần mở đầu tiên, hãy làm theo hướng dẫn 1 chạm để cấp quyền Pin & Tự khởi động giúp TuiMem bảo vệ máy 24/7.
Design by dinoking — facebook.com/biglinuxviet
