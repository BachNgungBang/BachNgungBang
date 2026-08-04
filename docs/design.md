# Concept thiết kế: `Neural Nightshift`

## Mục tiêu

`Neural Nightshift` là concept GitHub Profile README theo hướng **Cyber Gaming × AI Hacker × Anime Tech**. Đây không phải giao diện dashboard, template badge wall hay bản sao của các profile phổ biến. Nó là một portfolio đọc theo nhịp cinematic: người xem thấy định vị nghề nghiệp ngay trong vài giây đầu, sau đó đi từ năng lực hiện tại đến bằng chứng dự án và hành trình phát triển.

Đối tượng chính là nhà tuyển dụng và technical reviewer. Vì vậy visual chỉ làm nhiệm vụ tăng nhận diện; nội dung phải trả lời được bốn câu hỏi: ứng viên là ai, đang xây gì, dùng công nghệ nào và có thể tạo giá trị gì.

## Art direction

| Thành phần | Định hướng |
|---|---|
| Không khí | Không gian đêm, phòng điều khiển AI, màn hình gaming sci-fi; tinh gọn và có khoảng thở. |
| Màu nền | Black/navy gần đen: `#070A12`, `#0D1020`. |
| Màu chủ đạo | Purple điện: `#A855F7`; blue neon: `#38BDF8`; điểm nhấn trắng lạnh: `#E6F7FF`. |
| Chất liệu | Grid mờ, terminal line, scanline rất nhẹ, glow có kiểm soát; không dùng texture dày hoặc gradient cầu vồng. |
| Typography | Mono/terminal cho nhãn kỹ thuật; sans hiện đại cho nội dung. Không dùng quá hai họ chữ trong asset SVG. |
| Hình tượng | Một avatar anime-tech hoặc silhouette được cấp phép/tự tạo, chip AI, đường dữ liệu và node. Không dùng nhân vật anime có bản quyền. |
| Motion | Chỉ một điểm motion mạnh ở Hero và một micro-animation ở Footer; ưu tiên SVG tĩnh có thể đọc tốt nếu GitHub không phát animation. |

### Nguyên tắc “minimal nhưng cinematic”

- Một visual hero lớn, còn lại dùng block chữ, đường neon và card giới hạn.
- Mỗi section chỉ có một thông điệp chính và tối đa một điểm nhấn thị giác.
- Không đặt hàng dài logo/badge. Công nghệ được nhóm theo năng lực và vai trò.
- Glow chỉ xuất hiện trên yếu tố tương tác/thông tin quan trọng: tên, current mission, CTA và key metric.
- Mọi ảnh SVG phải có alt text; mọi nội dung quan trọng phải tồn tại dưới dạng Markdown, không bị giấu trong ảnh.

## Kịch bản đọc

```text
Hero → Identity → Capability → Current mission → Proof of work
     → Evidence → Growth paths → Personality → Contact → Exit signal
```

Hero bán “định vị”. About Me và Tech Stack làm rõ “năng lực”. Current Learning, AI Journey và Backend Journey thể hiện “động lực phát triển”. Projects và GitHub Stats cung cấp “bằng chứng”. Quote, Fun Facts và Footer tạo cá tính nhưng không cạnh tranh với portfolio.

## Section blueprint

### 1. Hero — `BOOT SEQUENCE`

**Mục đích:** tạo ấn tượng trong 3–5 giây và nêu giá trị nghề nghiệp rõ ràng.

Hero là một SVG/ảnh wide ratio khoảng 3:1: nền black/navy, một dải grid xanh lam rất mờ, silhouette AI core/terminal window ở mép phải và phần chữ ở trái. Tên là yếu tố lớn nhất; dưới đó là một statement ngắn dạng “Building [loại sản phẩm] with [lợi thế]”. Không dùng nhiều slogan luân phiên.

Ngay dưới hero là một dòng terminal tĩnh hoặc typing animation rất chậm: `STATUS: shipping AI-assisted commerce systems`. Chỉ có 2–3 link hành động: portfolio, email/contact và GitHub/repository nổi bật. Có thể dùng một badge trạng thái nhỏ, không dùng profile-view counter.

**Tín hiệu tuyển dụng:** định vị công việc, lĩnh vực quan tâm và CTA được nhìn thấy trước bất kỳ hiệu ứng nào.

### 2. About Me — `OPERATOR PROFILE`

**Mục đích:** chuyển từ phong cách sang con người và chuyên môn.

Layout hai cột nhẹ bằng bảng Markdown hoặc HTML tối giản: cột trái là 3–4 bullet “operator profile” (vai trò, focus, cách làm việc); cột phải là mini card “What I optimize for” gồm product thinking, execution và user value. Trên mobile, nội dung phải xếp một cột tự nhiên.

Nội dung nên cụ thể, tránh mô tả chung như “passionate developer”. Ví dụ cấu trúc: nền tảng hiện tại → hướng chuyên môn → phương pháp làm việc → loại vấn đề muốn giải.

**Tín hiệu tuyển dụng:** ứng viên có định hướng, giao tiếp tốt và hiểu tác động sản phẩm ngoài code.

### 3. Tech Stack — `LOADOUT`

**Mục đích:** cho thấy công cụ đang dùng một cách có ngữ cảnh.

Thiết kế một “loadout matrix” 4 nhóm: `Interface`, `Application`, `Data & API`, `Workflow`. Mỗi nhóm chỉ ghi công nghệ thực sự dùng/đủ tự tin, kèm vai trò ngắn; icon nếu dùng phải đồng nhất một nguồn và cùng kích thước. Ví dụ: React/Next.js để UI, TypeScript để độ tin cậy, API/database cho application flow, Git/AI tooling cho delivery.

Không xếp công nghệ đã học thành logo collection. Công nghệ nền hoặc đang học nên đưa vào section learning.

**Tín hiệu tuyển dụng:** biết chọn công cụ theo hệ thống, không chỉ tích lũy keyword.

### 4. Current Learning — `ACTIVE QUESTS`

**Mục đích:** chứng minh quá trình phát triển có kế hoạch.

Dùng ba quest ngắn, mỗi quest gồm `mục tiêu`, `lý do thực tế` và `output kế tiếp`. Ví dụ: xây API có authentication để hoàn chỉnh product flow; học testing để giảm lỗi regression; nghiên cứu AI integration để đưa vào tính năng có ích. Một progress bar giả không có bằng chứng không nên dùng.

Visual là ba node nối bởi đường neon mảnh, hoặc ba bullet có mã quest `Q-01` đến `Q-03`, không cần card lớn.

**Tín hiệu tuyển dụng:** tự học có ưu tiên, gắn việc học với deliverable.

### 5. Projects — `MISSION ARCHIVE`

**Mục đích:** là bằng chứng quan trọng nhất của profile.

Chọn 2–3 dự án mạnh nhất. Mỗi dự án là một mission card gọn, có: tên/link, một câu nêu vấn đề người dùng, vai trò cá nhân, stack then chốt và 1–2 outcome có thể kiểm chứng. Có link repository, demo hoặc case study khi tồn tại.

Không dùng mô tả chung chung như “a modern web app”. Dùng format: `Problem → Build → Result`. Một thumbnail tự tạo tối giản hoặc screenshot sản phẩm thật có giá trị hơn ảnh minh hoạ sci-fi.

**Tín hiệu tuyển dụng:** khả năng biến công nghệ thành sản phẩm, ownership và chất lượng trình bày.

### 6. GitHub Stats — `SIGNAL TELEMETRY`

**Mục đích:** bổ sung dữ liệu hoạt động, không thay thế portfolio.

Chỉ hiển thị tối đa hai visual: một profile summary card và một language/activity card trong cùng tone purple/blue. Thêm dòng chú thích dưới card giải thích con số liên quan đến loại công việc đang làm. Tránh trophies, streaks, snake graph và nhiều service khác nhau vì chúng tạo cảm giác gamification hơn là professional proof.

Cards phải được cập nhật bằng workflow riêng và chỉ commit theme đang dùng. Nếu dữ liệu không phản ánh chính xác công việc (private repo, thời gian học, đóng góp tổ chức), hãy giản lược section thay vì cố làm đầy.

**Tín hiệu tuyển dụng:** có hoạt động thực nhưng không phô trương số liệu.

### 7. AI Journey — `NEURAL PATH`

**Mục đích:** cho thấy AI là năng lực triển khai có trách nhiệm, không chỉ là buzzword.

Thể hiện hành trình ba tầng: `AI-assisted workflow` → `AI-integrated feature` → `AI product/system thinking`. Mỗi tầng nêu ví dụ thật: dùng AI để research/prototype/test; xây feature có AI API; thiết kế guardrail, evaluation hoặc UX cho AI output. Dùng đường node phát sáng nhẹ thay vì minh họa não/cyborg sáo rỗng.

Nêu rõ phần con người giữ quyền quyết định: problem framing, kiến trúc, kiểm thử và đánh giá đầu ra.

**Tín hiệu tuyển dụng:** dùng AI để nâng năng suất nhưng vẫn có năng lực kỹ thuật và tư duy sản phẩm độc lập.

### 8. Backend Journey — `SYSTEMS UNLOCKED`

**Mục đích:** diễn đạt roadmap backend theo năng lực có thể kiểm chứng.

Chia thành ba tầng theo hệ thống: `Foundation` (HTTP, REST, auth, validation), `Persistence` (schema, database, query, migration), `Reliability` (testing, logging, error handling, deployment). Mỗi tầng chỉ đánh dấu những gì đã làm hoặc đang xây, và link đến mini-project/commit khi có.

Không dùng thanh level 0–100% không có tiêu chí. Hình tượng “skill tree” nên rất tiết chế: ba tầng thẳng, node chưa mở khoá dùng outline mờ.

**Tín hiệu tuyển dụng:** roadmap rõ ràng từ frontend/product vào system thinking, không tạo kỳ vọng sai về seniority.

### 9. Quote — `CORE DIRECTIVE`

**Mục đích:** tạo nhịp nghỉ trước phần cá nhân.

Một câu ngắn do cá nhân viết hoặc trích dẫn có nguồn. Đặt trên nền terminal strip cực mảnh, không dùng blockquote dài hay ảnh lớn. Quote phải củng cố triết lý làm việc, ví dụ trọng tâm vào shipping, học bằng xây dựng hoặc giải quyết vấn đề người dùng.

**Tín hiệu tuyển dụng:** cá tính có định hướng, không làm gián đoạn luồng thông tin.

### 10. Fun Facts — `SIDE CHANNEL`

**Mục đích:** thêm dấu hiệu con người sau khi portfolio chính đã hoàn tất.

Tối đa ba fact: sở thích tạo ảnh hưởng tích cực đến cách làm sản phẩm, một game/creative interest, hoặc nghi thức học/làm việc. Dùng icon line nhỏ hoặc bullet terminal; không dùng GIF lớn, meme hay nội dung khiến trang dài thêm mà không mang giá trị.

**Tín hiệu tuyển dụng:** dễ kết nối và có cá tính, nhưng vẫn giữ professional boundary.

### 11. Contact — `OPEN COMMS`

**Mục đích:** biến sự quan tâm thành hành động đơn giản.

Đặt một CTA rõ: “Open to internships / collaboration / product conversations” tùy tình trạng thực tế. Có 2–3 link: email/contact form, LinkedIn/website và portfolio. Dùng text link hoặc icon có accessible label; tránh nhúng email thô vào badge nếu không muốn bị bot thu thập.

**Tín hiệu tuyển dụng:** người xem biết chính xác cách và lý do liên hệ.

### 12. Footer — `END TRANSMISSION`

**Mục đích:** kết thúc gọn và để lại tín hiệu thương hiệu.

Footer là một line SVG mảnh hoặc Markdown divider cùng chữ ngắn: `END TRANSMISSION · built with intent`. Micro-animation có thể là một chấm blue neon pulse; phải có bản tĩnh tương đương. Không thêm quote thứ hai, counter hay các badge dư thừa.

**Tín hiệu tuyển dụng:** đóng trang chuyên nghiệp, nhất quán với concept mà không kéo dài không cần thiết.

## Hệ thống layout và responsive

- Chiều rộng nội dung theo chuẩn GitHub; asset SVG dùng `viewBox`, `width="100%"` và không khóa chiều rộng desktop quá lớn.
- Section dùng Markdown heading cấp `##` và identifier (`## Projects — Mission Archive`) để outline có thể quét và liên kết được.
- Mỗi section ngăn bởi khoảng trắng nhất quán; chỉ dùng divider giữa những hồi nội dung lớn: identity, proof, growth, contact.
- HTML chỉ dành cho căn hàng/card mà Markdown không làm được. Không phụ thuộc HTML phức tạp vì GitHub có sanitization.
- Asset có phiên bản dark-first, độ tương phản đủ khi GitHub dark mode; không kỳ vọng control toàn bộ background của trang profile.

## Quy tắc asset và workflow khi triển khai

- Tạo asset riêng trong `assets/` theo mục đích, ví dụ `hero-neural-nightshift.svg`, `neural-path.svg` và `footer-signal.svg`; không đặt tên theo phiên bản mơ hồ như `v2`.
- Giữ source editable (SVG rõ cấu trúc) và chỉ commit các asset được README tham chiếu.
- Animation dùng SMIL tối giản, không script, không nhấp nháy nhanh; nội dung chữ quan trọng luôn có bản Markdown hoặc alt text.
- Workflow GitHub Stats chỉ sinh theme cần dùng, chạy thủ công và theo lịch hợp lý; pin action theo SHA, dùng quyền tối thiểu và tránh tạo commit khi output không đổi.
- Thực hiện kiểm tra cuối: render desktop/mobile, dark/light, link integrity, alt text, tương phản và tính chính xác của mọi project/skill claim.

## Tiêu chí thành công

1. Trong 5 giây, người xem hiểu tên, định vị và loại giá trị ứng viên đang xây.
2. Trong một lần cuộn, người xem thấy dự án và bằng chứng cụ thể trước các hiệu ứng/metrics phụ.
3. Màu neon tạo nhận diện nhưng nội dung vẫn đọc được khi không có animation hoặc ảnh không tải.
4. Profile có cá tính AI hacker/anime-tech riêng nhưng tránh motif template phổ biến như trophy wall, snake contribution và badge wall.
5. Mọi section đều hỗ trợ quyết định tuyển dụng hoặc tạo điểm kết nối thực sự.
