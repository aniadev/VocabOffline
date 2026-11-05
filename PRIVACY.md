# Privacy Policy — Vocab Handbook (VocabOffline)

**Effective date:** 5 November 2026
**App:** Vocab Handbook (bundle ID `com.hai.VocabOffline`), iOS
**Developer:** Ania (aniadev) — contact: aniadev.99@gmail.com

*Tiếng Việt ở phía dưới — [Chính sách quyền riêng tư (Tiếng Việt)](#chính-sách-quyền-riêng-tư--vocab-handbook)*

---

## 1. Summary

Vocab Handbook is an offline vocabulary notebook. **We do not collect, store, or sell any personal data.** The app has no user accounts, no analytics, no advertising, no tracking, and no server operated by the developer. Everything you create in the app stays on your device.

The only time data leaves your device is when **you explicitly choose** to use the optional "add words from a photo" feature, which sends one photo to Google's Gemini API using **your own API key**. This is described in section 4.

## 2. Data stored on your device

The app keeps the following data locally, inside the app's private sandbox on your iPhone or iPad:

| Data | Where | Purpose |
|---|---|---|
| Vocabulary list and conjunction list | App Documents folder (JSON files) | Core function of the app |
| An optional reference photo you take or choose | App Documents folder (JPEG) | Shown as a zoomable reference image |
| Your Google Gemini API key (optional) | iOS Keychain | Used only to call the Gemini API on your behalf |
| Gemini model name, your consent choice, and AI usage counters (requests / tokens) | UserDefaults | App settings and a local usage estimate |

This data is **never transmitted to the developer** and is not backed up to any developer-controlled service. Standard iOS device backups (iCloud or Finder/iTunes) may include the app's data according to your own device settings.

## 3. Device permissions

- **Camera** — used only when you tap to take a photo of a book page (to extract words or save a reference image). Photos are not uploaded anywhere unless you use the AI feature described below.
- **Photos** — the app uses the system photo picker, which lets you choose a single image without granting access to your whole library.
- **Files** — the app uses the system file picker to let you import vocabulary from Excel (`.xlsx`) files. Files are parsed on-device.
- **Text-to-speech** — pronunciation is generated on-device with Apple's speech synthesizer. No audio or text is sent to any server.

## 4. Optional AI feature (Google Gemini)

The "add words from a photo" feature is **off by default** and requires two deliberate steps from you:

1. You paste your own Google Gemini API key into the app's AI settings.
2. You accept an in-app consent screen before the first photo is sent. You can withdraw this consent at any time in AI settings.

When you use the feature, the app sends **only** the following to Google's Gemini API (`generativelanguage.googleapis.com`):

- the single photo you just took or chose, including the highlight marks you drew, downscaled to at most 1600 px on the longest side;
- a fixed text instruction asking the model to read the highlighted words;
- your API key, as an authentication header.

The app does **not** send your vocabulary list, your device identifiers, your location, or any other information. The developer never sees the photo, the key, or the response: the request goes directly from your device to Google.

Google processes this data under its own terms and privacy policy. Please note that on the free tier of the Gemini API, Google may use submitted content to improve its services. **Avoid photographing pages that contain personal or confidential information.** See:

- Gemini API Terms: https://ai.google.dev/gemini-api/terms
- Google Privacy Policy: https://policies.google.com/privacy

## 5. Data we collect

**None.** The developer does not collect, receive, or process any personal data, usage data, crash reports, or device identifiers through this app. There are no third-party analytics or advertising SDKs. The app does not use tracking as defined by Apple's App Tracking Transparency framework.

## 6. Data retention and deletion

All data lives on your device. You can:

- delete individual words, lists, or the reference image inside the app;
- remove your API key by clearing it in AI settings;
- delete **all** app data at once by uninstalling the app.

Because the developer holds no copy of your data, there is nothing for us to delete on our side.

## 7. Children

The app is a general-audience educational tool and is not directed at children under 13. It does not knowingly collect personal information from anyone, including children.

## 8. Security

Your API key is stored in the iOS Keychain, which is encrypted by the operating system. Network requests to Google are made over HTTPS only.

## 9. Changes to this policy

If the app's data practices change (for example, a new online feature), this document will be updated and the effective date revised. The current version is always available at the URL where you are reading it.

## 10. Contact

Questions about privacy: **aniadev.99@gmail.com**

---
---

# Chính sách quyền riêng tư — Vocab Handbook

**Ngày hiệu lực:** 5 tháng 11 năm 2026
**Ứng dụng:** Vocab Handbook (bundle ID `com.hai.VocabOffline`), iOS
**Nhà phát triển:** Ania (aniadev) — liên hệ: aniadev.99@gmail.com

## 1. Tóm tắt

Vocab Handbook là sổ từ vựng hoạt động offline. **Chúng tôi không thu thập, lưu trữ hay bán bất kỳ dữ liệu cá nhân nào.** Ứng dụng không có tài khoản người dùng, không analytics, không quảng cáo, không theo dõi (tracking) và nhà phát triển không vận hành máy chủ nào. Mọi thứ bạn tạo trong ứng dụng đều nằm trên thiết bị của bạn.

Dữ liệu chỉ rời khỏi thiết bị khi **bạn chủ động chọn** dùng tính năng tùy chọn "thêm từ từ ảnh". Tính năng này gửi một tấm ảnh tới Gemini API của Google bằng **API key của chính bạn**. Chi tiết ở mục 4.

## 2. Dữ liệu lưu trên thiết bị

Ứng dụng lưu các dữ liệu sau trong vùng sandbox riêng của ứng dụng trên iPhone/iPad của bạn:

| Dữ liệu | Nơi lưu | Mục đích |
|---|---|---|
| Danh sách từ vựng và danh sách liên từ | Thư mục Documents của ứng dụng (file JSON) | Chức năng chính của ứng dụng |
| Một ảnh tham khảo tùy chọn do bạn chụp hoặc chọn | Thư mục Documents của ứng dụng (JPEG) | Hiển thị làm ảnh tham khảo có thể phóng to |
| Gemini API key của bạn (tùy chọn) | iOS Keychain | Chỉ dùng để gọi Gemini API thay cho bạn |
| Tên model Gemini, lựa chọn đồng ý của bạn, bộ đếm lượt dùng AI (số request / token) | UserDefaults | Cài đặt ứng dụng và ước tính mức sử dụng cục bộ |

Dữ liệu này **không bao giờ được gửi tới nhà phát triển** và không được sao lưu lên bất kỳ dịch vụ nào do nhà phát triển kiểm soát. Sao lưu thiết bị tiêu chuẩn của iOS (iCloud hoặc Finder/iTunes) có thể bao gồm dữ liệu ứng dụng tùy theo cài đặt thiết bị của bạn.

## 3. Quyền truy cập trên thiết bị

- **Camera** — chỉ dùng khi bạn bấm chụp trang sách (để trích từ mới hoặc lưu ảnh tham khảo). Ảnh không được tải lên bất kỳ đâu trừ khi bạn dùng tính năng AI mô tả bên dưới.
- **Ảnh** — ứng dụng dùng bộ chọn ảnh của hệ thống, cho phép bạn chọn một ảnh mà không cần cấp quyền truy cập toàn bộ thư viện.
- **Tệp** — ứng dụng dùng bộ chọn tệp của hệ thống để nhập từ vựng từ file Excel (`.xlsx`). File được xử lý ngay trên thiết bị.
- **Đọc văn bản** — phát âm được tạo trên thiết bị bằng bộ tổng hợp giọng nói của Apple. Không có âm thanh hay văn bản nào được gửi lên máy chủ.

## 4. Tính năng AI tùy chọn (Google Gemini)

Tính năng "thêm từ từ ảnh" **mặc định tắt** và cần hai bước chủ động từ bạn:

1. Bạn dán Gemini API key của chính mình vào Cài đặt AI trong ứng dụng.
2. Bạn chấp nhận màn hình xin đồng ý trong ứng dụng trước khi ảnh đầu tiên được gửi. Bạn có thể rút lại đồng ý bất cứ lúc nào trong Cài đặt AI.

Khi bạn dùng tính năng này, ứng dụng **chỉ** gửi những thứ sau tới Gemini API của Google (`generativelanguage.googleapis.com`):

- một tấm ảnh bạn vừa chụp hoặc chọn, kèm các nét tô bạn đã vẽ, được thu nhỏ còn tối đa 1600 px cạnh dài;
- một đoạn hướng dẫn cố định yêu cầu model đọc các từ đã tô;
- API key của bạn, dưới dạng header xác thực.

Ứng dụng **không** gửi danh sách từ vựng, định danh thiết bị, vị trí hay bất kỳ thông tin nào khác. Nhà phát triển không bao giờ thấy ảnh, key hay kết quả trả về: yêu cầu đi thẳng từ thiết bị của bạn tới Google.

Google xử lý dữ liệu này theo điều khoản và chính sách quyền riêng tư của họ. Lưu ý rằng với gói miễn phí của Gemini API, Google có thể dùng nội dung gửi lên để cải thiện dịch vụ. **Tránh chụp những trang có thông tin cá nhân hoặc bảo mật.** Xem:

- Điều khoản Gemini API: https://ai.google.dev/gemini-api/terms
- Chính sách quyền riêng tư của Google: https://policies.google.com/privacy

## 5. Dữ liệu chúng tôi thu thập

**Không có.** Nhà phát triển không thu thập, nhận hay xử lý bất kỳ dữ liệu cá nhân, dữ liệu sử dụng, báo cáo sự cố hay định danh thiết bị nào thông qua ứng dụng này. Không có SDK analytics hay quảng cáo của bên thứ ba. Ứng dụng không theo dõi người dùng theo định nghĩa của Apple App Tracking Transparency.

## 6. Lưu giữ và xóa dữ liệu

Toàn bộ dữ liệu nằm trên thiết bị của bạn. Bạn có thể:

- xóa từng từ, từng danh sách hoặc ảnh tham khảo ngay trong ứng dụng;
- xóa API key bằng cách xóa trống trong Cài đặt AI;
- xóa **toàn bộ** dữ liệu ứng dụng bằng cách gỡ cài đặt ứng dụng.

Vì nhà phát triển không giữ bản sao dữ liệu của bạn nên không có gì để chúng tôi xóa ở phía mình.

## 7. Trẻ em

Ứng dụng là công cụ học tập dành cho mọi đối tượng, không hướng tới trẻ em dưới 13 tuổi. Ứng dụng không cố ý thu thập thông tin cá nhân của bất kỳ ai, kể cả trẻ em.

## 8. Bảo mật

API key của bạn được lưu trong iOS Keychain, được hệ điều hành mã hóa. Các yêu cầu mạng tới Google chỉ đi qua HTTPS.

## 9. Thay đổi chính sách

Nếu cách ứng dụng xử lý dữ liệu thay đổi (ví dụ thêm tính năng online mới), tài liệu này sẽ được cập nhật và ngày hiệu lực được sửa lại. Phiên bản hiện hành luôn có tại URL bạn đang đọc.

## 10. Liên hệ

Câu hỏi về quyền riêng tư: **aniadev.99@gmail.com**
