---
title: NFC Studio 支持 / Support
description: NFC Studio 扫码、NFC、文件、权限、历史记录和 Pro 订阅的使用帮助与联系方式。
lang: zh-CN
---

# NFC Studio 支持 / Support

[简体中文](#zh-hans) · [English](#english) · [隐私政策 / Privacy Policy](PrivacyPolicy.html)

更新日期 / Updated: **2026-10-11**

支持邮箱 / Support email: [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com)

<a id="zh-hans"></a>

## 简体中文

NFC Studio 帮助你扫描和创建二维码、条形码，读取兼容 NFC 标签、编辑 NDEF 消息，并管理本地历史。App 需要 **iOS / iPadOS 17.0 或更新版本**；NFC 标签功能需要支持 Core NFC 的实体 iPhone，iPad 可使用二维码、条形码和其他不依赖 NFC 硬件的功能。

### 1. 联系支持

请发送邮件至 [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com)，并尽量提供：

- NFC Studio 版本、iOS / iPadOS 版本和设备型号。
- 使用的页面或功能、操作步骤，以及预期结果和实际结果。
- 显示的错误提示；如提供截图，请遮盖个人信息。
- NFC 问题请补充标签型号或技术类型、是否已格式化为 NDEF、是否可写，以及失败发生在读取、写入还是回读校验阶段。
- 订阅问题可补充月度或年度方案、购买时间及系统显示的订阅状态。

请勿发送 Apple 账户密码、完整支付卡信息、验证码、Wi-Fi 密码、标签保护密码或含敏感内容的完整 `.ndef` 文件。通常不需要提供完整付款凭证。

### 2. 扫码与创建

**扫描二维码或条形码：**打开“扫描”，选择相机扫描，按系统提示允许相机访问，将完整的码放入取景区域并保持稳定。也可以选择从照片导入，使用系统照片选择器识别图片中的码。

**创建内容：**打开“创建”，选择文本、网址、邮箱、电话、联系人、Wi-Fi、条形码、短信或位置类型，填写内容后生成。结果页可分享、保存到照片，或在历史开启时选择保存到历史。条形码创建使用 Code 128；二维码的样式和纠错选项不适用于条形码。

相机扫描支持 QR、Micro QR、Aztec、Data Matrix、PDF417、MicroPDF417、EAN、UPC-E、Code 39 / 93 / 128、Codabar、ITF 和 GS1 DataBar 等格式；具体可用类型取决于设备和系统。图片识别结果也取决于格式、清晰度和图片内容。

| 问题 | 可以尝试的操作 |
| --- | --- |
| 相机无法使用 | 在系统设置中检查 NFC Studio 的相机权限，返回 App 后重试；也可使用照片识别入口。设备限制或相机硬件不可用时，相机扫描可能无法启动。 |
| 扫描不到码 | 确保码完整、清晰、光线足够且没有强反光；调整距离与对焦，或改用清晰的原始图片。 |
| 图片中没有识别结果 | 选择能看清整个码的图片，避免模糊、遮挡或裁切。并非每张图片或每种码都能被识别。 |
| 图片无法保存 | 在系统设置中允许 NFC Studio 向照片添加图片，检查设备剩余空间，再返回结果页重试。 |
| 打开网址、邮件、电话或短信失败 | 核对内容格式和设备是否具备相应 App 或通信能力；结果内容也可以复制后手动处理。 |

### 3. NFC 读取、写入与标签兼容性

**读取：**在“扫描”中选择 NFC，启动读取，并将标签靠近 iPhone 的 NFC 感应区域，保持位置直到操作结束。普通 NDEF 读取适合日常消息；标签详情模式用于查看技术类型、标签标识和可用元数据。

**写入：**使用快速写入或 NDEF 编辑器准备内容，核对记录后开始写入。标签必须兼容、可写且容量足够。写入与校验期间保持标签位置稳定。NFC 写入和专业标签操作需要 Pro。

兼容性取决于标签技术、型号、格式、锁定或密码状态，以及 iPhone 和 iOS。App 的普通 NDEF 读取使用 NFC Forum 标签接口，标签详情涉及 ISO 14443 / MIFARE、ISO 15693、ISO 7816 和 FeliCa。原始存储区及密码工具仅对 App 能明确识别并提供对应工具的型号开放，不能据此认定同一技术类别下所有标签都兼容。

常见情况：

- **无法读取或没有 NDEF 内容：**确认使用支持 Core NFC 的实体 iPhone，并主动启动读取。保持单个标签靠近手机，尝试调整位置或移除会影响通信的外壳。未格式化、受保护或不兼容的标签可能无法读取 NDEF。
- **可读取但不可写入：**查看只读、锁定、密码保护和剩余容量状态。能读取不代表能写入；永久只读无法由 App 撤销。
- **写入中断或校验失败：**标签可能已被部分修改。重新读取并核对当前内容后，再决定下一步操作；失败提示不表示已经自动回滚。
- **高级工具不可用：**未知型号、保护状态不明或不支持的布局不会开放对应写入工具。请提供标签型号和错误提示联系支持。
- **想复制门禁卡、支付卡或 UID：**NFC Studio 不提供 UID 克隆、门禁或支付卡复制、MIFARE Classic / Crypto1 解密、手机卡模拟或绕过密码保护的功能。

清空 NDEF 不等于擦除全部物理存储，也不会取消密码或硬件锁。清除、密码修改和永久只读会改变标签状态；请先核对操作对象及 App 的确认说明。

### 4. NDEF 文件与历史记录

NDEF 编辑器可通过系统“文件”导入或导出单个 `.ndef` 消息，最大 **128 KiB**。导入前可预览并选择追加或替换。导入失败时，确认文件是完整、合法的 NDEF 消息，而不是多个拼接消息、截断数据或任意芯片存储镜像。

`.ndef` 导出保留完整消息，可能包含 Wi-Fi 密码、联系人或二进制数据。它不包含 UID 克隆、硬件锁或标签密码保护配置。分享前请检查内容。

本地历史支持搜索、来源筛选、收藏和删除。Pro 支持 JSON / CSV 历史导入导出，也可导出所选记录。历史文件是历史记录交换格式，不等同于 `.ndef` 消息或完整芯片备份。

- 在 **设置 → 历史 → 保存历史记录** 关闭新记录保存；已有记录仍保留。
- 在 **历史** 页面删除记录或清除全部历史。
- 二维码历史可能包含完整 Wi-Fi 密码。NFC 读取历史会隐藏可识别的 Wi-Fi 凭证及完整二进制 Payload；NDEF 写入历史只保存操作摘要，因此不能从该摘要还原完整写入消息。
- App 不提供自建云端历史同步。恢复购买只恢复有效的 Pro 权益，不会恢复已删除的本地历史。
- 删除历史不会删除导出文件、照片、已写入的标签内容或其他副本，请在对应位置另行管理。

### 5. Pro、恢复购买、取消与退款

基础扫码、照片识别、二维码和 Code 128 创建、经典二维码样式、普通 NDEF 读取及本地历史可免费使用。Pro 提供 NFC 写入和专业标签操作、高级二维码样式，以及历史 JSON / CSV 导入导出。其他入口以当前 App 显示的权益要求为准。

月度和年度为 App Store 自动续期订阅选项。实际可购买的方案、价格、试用期限和资格以 App Store 展示为准；免费试用并非每个 Apple 账户都可重复使用。

**已购买但 Pro 未解锁：**

1. 确认设备的 App Store 使用购买时的 Apple 账户。
2. 检查网络及系统订阅列表中的订阅状态。
3. 打开 **NFC Studio → 设置 → NFC Studio Pro → 恢复购买**。
4. 如果有效订阅仍未解锁，请将 App 版本、方案和错误提示发给支持邮箱。

**管理或取消订阅：**打开系统 **设置 → 你的姓名 / Apple 账户 → 订阅 → NFC Studio**，按系统说明操作。App 中有有效订阅时也提供管理订阅入口。删除 App 不会取消订阅；如不希望试用续订，Apple 建议至少在试用结束前 24 小时取消。详见 [Apple 取消订阅说明](https://support.apple.com/en-us/118428)。

**退款：**可通过 [Apple 问题报告页面](https://reportaproblem.apple.com/) 申请，是否符合条件及处理结果由 Apple 根据相关规则决定。详见 [Apple 退款说明](https://support.apple.com/en-us/118223)。

购买条款使用 [Apple 标准最终用户许可协议](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)。

### 6. 权限与隐私

照片识别通过系统照片选择器读取你选中的图片；保存图片只请求添加照片的权限。联系人卡片通过系统新建联系人界面保存。位置内容使用输入或扫描到的坐标，App 不请求读取当前定位。NFC 需要兼容 iPhone 和主动启动的读取或写入会话，无需寻找单独的 NFC 权限开关。

App 的扫描、识别与编码在设备上处理，历史保存在本地；主动分享、导出、写入标签及调用外部服务会交出相应内容，Apple 订阅服务和本网站托管也涉及外部服务。完整说明见 [NFC Studio 隐私政策](PrivacyPolicy.html)。

<a id="english"></a>

## English

NFC Studio helps you scan and create QR codes and barcodes, read compatible NFC tags, edit NDEF messages, and manage local history. It requires **iOS / iPadOS 17.0 or later**. NFC tag features require a physical iPhone that supports Core NFC. iPad can use QR, barcode, and other features that do not require NFC hardware.

### 1. Contact support

Email [nalonpeng@foxmail.com](mailto:nalonpeng@foxmail.com) and, where possible, include:

- NFC Studio version, iOS / iPadOS version, and device model.
- The page or feature, steps to reproduce, expected result, and actual result.
- Any error message. Redact personal information in screenshots.
- For NFC issues, the tag model or technology, whether it is NDEF-formatted and writable, and whether the failure occurred during reading, writing, or read-back verification.
- For subscription issues, the monthly or yearly plan, purchase time, and subscription status shown by the system.

Do not send Apple Account passwords, full payment-card information, verification codes, Wi-Fi passwords, tag-protection passwords, or full `.ndef` files containing sensitive information. A complete payment receipt is usually unnecessary.

### 2. Scanning and creating codes

**Scan a QR code or barcode:** Open Scan, select camera scanning, allow camera access when prompted, and keep the complete code in the viewfinder. You can also import a photo using the system photo picker.

**Create content:** Open Create, choose text, URL, email, phone, contact, Wi-Fi, barcode, message, or location, complete the fields, and generate the result. Share it, save it to Photos, or choose Save to History when history is enabled. Barcode creation uses Code 128; QR styles and error-correction options do not apply to barcodes.

Camera scanning includes QR, Micro QR, Aztec, Data Matrix, PDF417, MicroPDF417, EAN, UPC-E, Code 39 / 93 / 128, Codabar, ITF, and GS1 DataBar formats. Available types depend on the device and system. Recognition from photos also depends on the format, image clarity, and content.

| Issue | Suggested action |
| --- | --- |
| Camera unavailable | Check NFC Studio's camera permission in system settings, return to the app, and retry. You can also use photo recognition. Device restrictions or unavailable camera hardware can prevent camera scanning. |
| Code not recognized | Keep the whole code visible, improve lighting, avoid reflections, and adjust distance and focus. Try a clear original image. |
| No result from a photo | Choose a sharp image with the complete code visible, without cropping or obstruction. Not every image or format can be recognized. |
| Cannot save an image | Allow NFC Studio to add images to Photos, check free storage, and retry from the result page. |
| URL, email, call, or message action fails | Check the content format and whether the device has the relevant app or communication capability. You can copy the result and handle it manually. |

### 3. NFC reading, writing, and compatibility

**Read:** Choose NFC in Scan, start reading, and hold the tag near the iPhone's NFC reading area until the operation completes. Standard NDEF reading is intended for everyday messages; tag detail mode shows technology, identifiers, and available metadata.

**Write:** Prepare content using quick write or the NDEF editor, review the records, and start writing. The tag must be compatible, writable, and large enough. Keep it in position during writing and verification. NFC writing and professional tag operations require Pro.

Compatibility depends on tag technology, model, formatting, locks or passwords, and the iPhone and iOS version. Standard NDEF reading uses NFC Forum tag interfaces. Tag detail mode covers ISO 14443 / MIFARE, ISO 15693, ISO 7816, and FeliCa. Raw memory and password tools are available only where the app identifies a supported model and offers the corresponding tool; this does not establish compatibility with every tag in a technology family.

Common situations:

- **Cannot read, or no NDEF content:** Use a physical iPhone that supports Core NFC and start a reading session. Hold one tag close to the phone, adjust its position, or remove a case that interferes with communication. Unformatted, protected, or incompatible tags may not expose readable NDEF content.
- **Readable but not writable:** Check read-only status, locks, password protection, and capacity. Successful reading does not establish write access. The app cannot reverse a permanent read-only lock.
- **Interrupted write or verification failure:** The tag may have been partially changed. Read it again and review its current content before deciding what to do next. A failure does not imply automatic rollback.
- **Advanced tool unavailable:** Unknown models, uncertain protection states, and unsupported layouts do not expose the relevant write tools. Contact support with the tag model and error message.
- **Copying access cards, payment cards, or UIDs:** NFC Studio does not provide UID cloning, access or payment card copying, MIFARE Classic / Crypto1 decryption, phone card emulation, or password-protection bypass.

Clearing NDEF does not erase all physical memory or remove passwords or hardware locks. Erasing data, changing passwords, or permanently locking a tag changes its state; review the target and the app's confirmation before proceeding.

### 4. NDEF files and local history

The NDEF editor imports or exports a single `.ndef` message through the system Files interface, up to **128 KiB**. You can preview an import and choose to append or replace records. If importing fails, check that the file is one complete valid NDEF message rather than concatenated messages, truncated data, or an arbitrary chip-memory image.

An exported `.ndef` file preserves the full message and may contain Wi-Fi passwords, contact details, or binary data. It does not clone a UID or include hardware-lock or tag-password configuration. Review it before sharing.

Local history supports search, source filters, favorites, and deletion. Pro supports JSON / CSV history import and export, including exporting selected records. These are history exchange formats, not `.ndef` messages or full chip backups.

- Turn off **Settings → History → Save History** to stop saving new records. Existing records remain.
- Delete records or clear all history from the **History** page.
- QR history may contain full Wi-Fi passwords. NFC read history redacts recognized Wi-Fi credentials and full binary payloads. NDEF write history stores only an operation summary, which cannot reconstruct the complete written message.
- The app does not provide its own cloud history sync. Restore Purchases restores valid Pro access, not deleted local history.
- Deleting history does not erase exported files, photos, content on tags, or other copies. Manage these separately.

### 5. Pro, purchase restoration, cancellation, and refunds

Basic scanning, photo recognition, QR and Code 128 creation, the classic QR style, standard NDEF reading, and local history are free. Pro adds NFC writing and professional tag operations, advanced QR styles, and JSON / CSV history import and export. Other entry points follow the entitlement requirements shown by the current app.

Monthly and yearly options are App Store auto-renewable subscriptions. Available plans, prices, trial duration, and eligibility are those shown by the App Store. A free trial is not repeatedly available to every Apple Account.

**Purchased but Pro is still locked:**

1. Confirm that the App Store uses the Apple Account that made the purchase.
2. Check the network connection and the subscription status in system settings.
3. Open **NFC Studio → Settings → NFC Studio Pro → Restore Purchases**.
4. If an active subscription still does not unlock Pro, email support with the app version, plan, and error message.

**Manage or cancel:** Open system **Settings → your name / Apple Account → Subscriptions → NFC Studio** and follow the system instructions. The app also offers subscription management when a subscription is active. Deleting the app does not cancel a subscription. Apple recommends canceling at least 24 hours before a trial ends if you do not want it to renew. See [Apple's cancellation instructions](https://support.apple.com/en-us/118428).

**Refunds:** You can submit a request through [Apple's Report a Problem website](https://reportaproblem.apple.com/). Apple determines eligibility and the outcome under the applicable rules. See [Apple's refund instructions](https://support.apple.com/en-us/118223).

Purchase terms use [Apple's Standard End User License Agreement](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/).

### 6. Permissions and privacy

Photo recognition reads images you select through the system photo picker. Saving images requests add-only photo access. Contact cards are saved through the system new-contact interface. Location content uses entered or scanned coordinates; the app does not request your current location. NFC requires a compatible iPhone and a reading or writing session you start, rather than a separate NFC permission switch.

Scanning, recognition, and encoding are processed on the device, and history is stored locally. Sharing, exporting, writing tags, and opening external services pass the relevant content to those destinations. Apple subscription services and website hosting also involve external services. See the complete [NFC Studio Privacy Policy](PrivacyPolicy.html).
