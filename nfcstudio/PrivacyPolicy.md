---
title: NFC Studio 隐私政策 / Privacy Policy
description: NFC Studio 的数据处理、系统权限、订阅、数据删除与隐私联系方式。
lang: zh-CN
---

# NFC Studio 隐私政策 / Privacy Policy

[简体中文](#zh-hans) · [English](#en) · [支持 / Support](support.html)

生效及更新日期 / Effective and updated: **2026-10-11**

隐私联系 / Privacy contact: [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com)

<a id="zh-hans"></a>

## 简体中文

### 1. 适用范围

本政策说明 NFC Studio 如何处理信息，以及你如何管理相关数据。NFC Studio 是一款用于扫描和创建二维码、条形码，以及读取和操作兼容 NFC 标签的 iPhone / iPad 工具。NFC 标签功能需要支持 Core NFC 的 iPhone。

本政策中的“我们”指 NFC Studio 的开发与支持方，你可以通过本页的邮箱联系开发者。当前 App 不提供自建账号或登录系统，不内置广告、广告跟踪或第三方行为分析 SDK，也不提供将扫描内容或历史记录上传至开发者服务器的功能。

### 2. 在设备上处理与保存的信息

扫描、图片识别、内容编码和 NFC 数据解析在设备上进行。根据你使用的功能和历史设置，App 会处理或保存下列信息：

| 信息 | 处理方式与用途 |
| --- | --- |
| 相机画面与所选照片 | 用于识别其中的二维码和条形码。App 不将相机画面或所选原始照片上传至开发者服务器，也不将其保存为历史照片。 |
| 二维码与条形码内容 | 开启历史记录时，识别结果会保存到本地历史；创建的内容可通过“保存到历史记录”保存。历史可包含完整文字、网址、联系人、电话、短信、位置坐标或 Wi-Fi 信息，包括内容中存在的 Wi-Fi 密码。 |
| NFC 标签与 NDEF 内容 | 读取时处理标签标识（如 UID）、技术类型、可用元数据和消息内容。本地读取历史可包含可读文字及格式、长度、标签信息；可识别的 Wi-Fi 凭证和二进制 Payload 不作为完整内容保存。任意普通文字中的敏感信息不会自动识别并全部隐藏。NDEF 写入历史保存记录数量和字节数等操作摘要，不保存写入消息的完整内容。 |
| App 偏好与收藏 | 外观、语言、触觉、历史开关和收藏标记保存在本机，用于保留你的设置。 |
| 购买与权益信息 | App 使用 Apple StoreKit 返回的商品、交易验证结果、订阅状态和到期信息，判断是否可以使用 Pro 功能。 |

当前 App 不提供自建云端历史同步。设备备份、恢复，以及照片或文件的云同步可能由你的 iOS、iPadOS、iCloud 或文件服务设置触发，相关数据由你选择的系统服务管理。

### 3. 系统能力与权限

| 功能 | 使用的数据或权限 |
| --- | --- |
| 相机扫描 | 使用相机识别二维码和条形码；在使用相机扫描时请求授权。 |
| 从照片识别 | 使用系统照片选择器，读取你主动选择的图片；不需要授予 App 整个照片图库的读取权限。 |
| 保存生成的图片 | 在你选择保存时，请求向照片图库添加图片的权限。 |
| NFC 读写与标签工具 | 在你主动启动操作后，使用 Core NFC 与附近的兼容标签通信。NFC 可用性取决于设备、系统和标签。 |
| 保存联系人卡片 | 在你选择添加联系人时，打开系统的新建联系人界面，由你确认是否保存；App 不遍历整个通讯录。 |
| 位置内容 | 使用你填写或扫描到的坐标生成内容；你选择地图操作时将相应坐标交给地图服务。App 不通过定位权限读取你当前的位置。 |

你可以在系统设置中管理可用的相机、照片和联系人权限。拒绝某项权限会影响对应功能；例如拒绝相机权限后，仍可使用系统照片选择器识别图片中的码。NFC 不是本 App 提供的独立系统权限开关。

### 4. 你主动选择的分享、导出和外部操作

当你选择分享、导出、复制、保存图片、写入 NFC 标签、打开网址、撰写邮件或短信、拨打电话、打开地图或保存联系人时，相应内容会按你的操作交给目标标签、剪贴板、系统 App、文件位置、服务或接收方。接收方和相关服务按各自的隐私规则处理这些内容。

二维码图片、历史 JSON / CSV 文件及 `.ndef` 消息文件可能包含个人信息或凭证。**`.ndef` 文件保留完整消息内容，可能包含 Wi-Fi 密码及二进制数据；NFC 历史中的隐藏处理不会同步应用于 `.ndef` 导出。**请在分享或写入标签前核对内容，并选择合适的接收方和保存位置。

### 5. 订阅与付款

NFC Studio Pro 的购买、试用资格、续订和付款通过 Apple App Store 处理。App 使用 StoreKit 的购买和权益信息验证 Pro 状态，不通过本 App 获取你的支付卡号码或 Apple 账户密码。

你可以在 App 中恢复购买，并通过 Apple 账户的订阅设置管理或取消订阅。实际价格、试用期限和续订条件以 App Store 购买确认页为准。Apple 对其处理的信息适用 [Apple 隐私政策](https://www.apple.com/legal/privacy/)。

### 6. 本地数据保留与删除

本地历史会保留至你删除相应记录、清空历史或删除 App。App 没有按时间自动清理历史的机制。

- 在 **NFC Studio → 设置 → 历史 → 保存历史记录** 关闭新记录保存。关闭开关不会删除已有记录。
- 在 **历史** 页面删除指定记录，或使用清除全部历史的操作。
- 在系统设置中撤销适用权限。撤销权限不会自动删除已经保存的记录。
- 在系统中选择**删除 App**，可移除 App 容器内的数据；“卸载 App”保留文稿与数据，不能代替删除。

清空历史或删除 App 不会删除已经写入 NFC 标签的内容、保存到照片的图片、导出文件、剪贴板或其他 App 中的副本、系统备份，也不会取消订阅。请在对应标签、照片、文件服务、备份位置或 Apple 订阅设置中另行管理。Apple 的交易记录由 Apple 管理。开发者不能远程查看或删除你设备上的本地历史。

### 7. 支持联系

如果你主动发送支持邮件，我们会收到你的邮件地址、问题描述，以及你选择提供的设备信息、截图或附件，并用这些信息回复和处理请求。App 不自动向支持邮箱发送扫描内容、照片、NFC 消息或诊断附件。

支持邮件及附件保存在支持邮箱及其邮件服务中，用于处理请求、必要的后续沟通及适用的记录保留要求；相关处理不再需要这些信息时予以删除。你可以向 [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com) 提出访问、更正或删除支持邮件中个人信息的请求。邮件服务的存储及备份同时受其自身规则管理。

请仅提供排查所需的信息，并遮盖截图中的个人信息。不要发送 Apple 账户密码、支付卡号码、验证码、标签保护密码或 Wi-Fi 密码。

### 8. 政策与支持网站

本政策及支持页面托管于 GitHub Pages。页面本身未添加分析脚本、广告或跟踪 Cookie。GitHub 作为托管服务商会处理访问网站所需的技术信息；GitHub Pages 访问者的 IP 地址会为安全目的被记录，因此本政策不作“网站不产生访问日志”的承诺。相关处理见 [GitHub Pages 说明](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages) 和 [GitHub 隐私声明](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)。

### 9. 隐私请求与政策变更

有关本政策、本地数据控制或你发送给支持方的信息，请联系 [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com)。如监护人认为儿童在支持邮件中提供了不应保留的个人信息，也可通过该邮箱提出处理请求。

若 App 的功能或数据处理方式发生变化，我们会在本页更新政策和日期，并在适用时更新商店披露、提供说明或请求授权。

<a id="en"></a>

## English

### 1. Scope

This policy explains how NFC Studio handles information and how you can manage your data. NFC Studio is an iPhone / iPad utility for scanning and creating QR codes and barcodes, and for reading and operating compatible NFC tags. NFC tag features require an iPhone that supports Core NFC.

“We” means the developer and support provider of NFC Studio, whom you can contact using the email address on this page. The current app has no developer-operated account or sign-in system, ads, advertising tracking, or third-party behavioral analytics SDKs. It does not provide a service that uploads scanned content or history to a developer server.

### 2. Information processed and stored on your device

Scanning, image recognition, content encoding, and NFC data parsing take place on the device. Depending on the features you use and your history settings, the app processes or stores the following information:

| Information | Handling and purpose |
| --- | --- |
| Camera frames and selected photos | Used to recognize QR codes and barcodes. The app does not upload these frames or original photos to a developer server or save them as history photos. |
| QR code and barcode content | Recognized results are saved locally when history is enabled. Created content can be saved using “Save to History.” History can contain full text, URLs, contact details, phone numbers, messages, coordinates, or Wi-Fi information, including any Wi-Fi passwords in the content. |
| NFC tags and NDEF content | Reading processes identifiers such as a tag UID, technology, available metadata, and message content. Local read history may contain readable text, format and length summaries, and tag information. Recognized Wi-Fi credentials and binary payloads are not stored in full. Sensitive information embedded in arbitrary plain text is not automatically detected and fully redacted. NDEF write history stores an operation summary such as record and byte counts, rather than the full written message. |
| Preferences and favorites | Appearance, language, haptics, history settings, and favorite markers are stored on the device to remember your choices. |
| Purchase and entitlement information | The app uses product information, transaction verification results, subscription status, and expiration information returned by Apple StoreKit to determine access to Pro features. |

The current app does not provide its own cloud history sync. Device backup, restore, and photo or file syncing may occur through your iOS, iPadOS, iCloud, or file-service settings and are managed by those services.

### 3. System features and permissions

| Feature | Data or permission used |
| --- | --- |
| Camera scanning | Uses the camera to recognize QR codes and barcodes, with authorization requested when you use camera scanning. |
| Recognizing codes in photos | Uses the system photo picker to read images you select. It does not require permission to read your entire photo library. |
| Saving generated images | Requests permission to add images to Photos when you choose to save an image. |
| NFC reading, writing, and tag tools | Uses Core NFC to communicate with nearby compatible tags after you start an operation. Availability depends on the device, system, and tag. |
| Saving contact cards | Opens the system new-contact interface when you choose to add a contact, allowing you to confirm saving. The app does not enumerate your address book. |
| Location content | Encodes coordinates you enter or scan, and passes them to Maps when you choose a map action. The app does not request location permission to read your current position. |

You can manage available camera, photo, and contact permissions in system settings. Denying a permission affects the related feature; for example, you can still recognize codes using the system photo picker if camera access is denied. The app does not offer a separate system NFC permission switch.

### 4. Sharing, exporting, and external actions you choose

When you choose to share, export, copy, save an image, write to an NFC tag, open a URL, compose email or a message, make a call, open Maps, or save a contact, the relevant content is passed to the tag, clipboard, system app, file location, service, or recipient you select. Their privacy practices apply to their handling of that content.

QR images, history JSON / CSV files, and `.ndef` message files may contain personal information or credentials. **A `.ndef` file preserves the complete message, including any Wi-Fi passwords and binary data. Redaction in NFC history does not apply to `.ndef` exports.** Review the content before sharing it or writing it to a tag, and choose an appropriate recipient and storage location.

### 5. Subscriptions and payments

Apple's App Store handles NFC Studio Pro purchases, trial eligibility, renewals, and payments. The app uses StoreKit purchase and entitlement information to verify Pro access. It does not receive your payment-card number or Apple Account password through the app.

You can restore purchases in the app and manage or cancel a subscription in your Apple Account subscription settings. Prices, trial duration, and renewal terms are those shown in the App Store purchase confirmation. Apple's handling of information is covered by the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).

### 6. Local retention and deletion

Local history remains until you delete individual records, clear history, or delete the app. The app does not automatically remove history based on its age.

- Turn off **NFC Studio → Settings → History → Save History** to stop saving new records. Existing records remain.
- Delete selected records or clear all history from the **History** page.
- Revoke applicable permissions in system settings. This does not automatically delete previously saved records.
- Choose **Delete App** in system settings to remove data in the app container. **Offload App** keeps documents and data and does not replace deletion.

Clearing history or deleting the app does not erase content written to NFC tags, images saved to Photos, exported files, clipboard contents, copies in other apps, or system backups, and does not cancel a subscription. Manage those separately on the tag, in Photos, in the relevant file or backup service, or in Apple subscription settings. Apple manages its transaction records. The developer cannot remotely view or delete local history on your device.

### 7. Support correspondence

If you email support, we receive your email address, issue description, and any device information, screenshots, or attachments you choose to provide. We use this information to respond to and handle your request. The app does not automatically email scanned content, photos, NFC messages, or diagnostic attachments to support.

Support emails and attachments are stored in the support mailbox and its email service for handling your request, necessary follow-up, and applicable recordkeeping requirements, and are deleted when no longer needed for those purposes. You can request access, correction, or deletion of personal information in support correspondence by emailing [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com). The email service's own rules also govern its storage and backups.

Include only information needed to investigate the issue and redact personal information in screenshots. Do not send Apple Account passwords, payment-card numbers, verification codes, tag-protection passwords, or Wi-Fi passwords.

### 8. Policy and support website

This policy and the support page are hosted on GitHub Pages. The pages do not add analytics scripts, ads, or tracking cookies. GitHub processes technical information needed to serve the website. GitHub Pages logs visitors' IP addresses for security purposes, so this policy does not claim that website access produces no logs. See the [GitHub Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages) and [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

### 9. Privacy requests and changes

For questions about this policy, local data controls, or information you send to support, contact [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com). A parent or guardian who believes that a child supplied personal information in a support email that should not be retained can also contact this address.

If app features or information handling change, we will update this page and its date, and update store disclosures, provide explanations, or request authorization when applicable.
