<div align="right">
  <b>Language / 语言:</b> 
  <a href="#chinese"> 中文</a> | 
  <a href="#english"> English</a>
</div>

<span id="chinese"></span>

# 隐私政策

**版本生效日期：** 2025年12月9日  
**最近更新日期：** 2026年11月10日  
**开发者：** yokodev（以下简称“我们”）

---

### 导言
PrecisEQ 是一款由 yokodev 独立研发的音频数字信号处理（DSP）与均衡工具应用。我们深知个人信息对您的重要性，并始终致力于保护用户的隐私安全。

**【特别提示】**  
1. **本应用为纯本地音频 DSP 处理工具，所有音频均衡、卷积及空间音频运算均 100% 在您的设备本地即时处理完成。本应用绝不录音、绝不离线保存、绝不上传任何您的音频流或通话内容。**
2. 本应用不强制要求注册账号，不收集您的真实姓名、身份证号、通讯录或精确地理位置等敏感个人身份信息。

请您在使用我们的服务前仔细阅读并理解本《隐私政策》。如您使用或继续使用我们的服务，即意味着同意我们按照本政策处理您的相关信息。

---

### 1. 我们如何收集和使用信息

为了向您提供稳定的音频增强服务，我们仅在以下合法、正当、必要的范围内收集和使用信息：

#### 1.1 音频处理与敏感系统权限说明（重要）
* **录制音频权限（RECORD_AUDIO）**：仅用于通过系统底层接口捕获其他正在播放音频的应用的本地数字音频流，以便进行 DSP 均衡滤波处理。**本应用绝不会启用硬件麦克风进行环境录音，绝不录制、缓存或上传任何用户声音数据。**
* **媒体投影权限（MediaProjection）**：部分工作模式下需要通过媒体投影前台服务获取音频捕获授权。**在此郑重声明：本应用仅利用该服务获取音频捕获通道，绝不截取、录制、存储或上传您的屏幕图像、操作轨迹或显示画面。**
* **通知权限（POST_NOTIFICATIONS）**：用于在系统通知栏展示前台音频处理服务的实时运行状态与快捷控制开关。

#### 1.2 崩溃统计与基础设备信息
* 为排查应用崩溃问题、提升音频引擎稳定性，我们会通过第三方统计工具收集匿名化的设备信息（包括设备型号、操作系统版本、应用包名及版本、崩溃堆栈日志）。此类信息无法识别特定自然人身份。

#### 1.3 支付与订单信息
* 当您购买高级版时，支付流程通过第三方支付渠道完成。我们仅会记录并校验支付服务商返回的**订单流水号（Order ID）与支付状态**，用于激活并向您提供高级版功能。**我们不会也无法获取您的银行卡号、支付密码等任何敏感金融信息。**

#### 1.4 无广告业务承诺
* **本应用不包含任何商业广告业务，不收集广告标识符，亦不会因广告目的向任何广告主或营销机构共享您的信息。**

---

### 2. 第三方 SDK 目录及数据共享说明

为了保障本应用特定功能的实现，我们会接入由具备资质的第三方提供的 SDK。接入的 SDK 清单及数据处理规则如下：

| SDK 名称 | 所属机构 | 使用目的 | 收集的数据类型 | 官网/隐私政策链接 |
| :--- | :--- | :--- | :--- | :--- |
| **支付宝客户端 SDK**<br>*(官方分发渠道)* | 蚂蚁科技集团股份有限公司 | 提供高级版安全支付能力，校验订单结果 | 设备型号、MAC 地址、网络状态、BSSID/SSID、系统参数（用于支付风控） | [支付宝隐私政策](https://opendocs.alipay.com/open/54/01g6qm) |
| **Google Play Billing**<br>*(仅限 Google Play 渠道)* | Google LLC | 提供海外应用内购买及恢复购买服务 | 购买凭证、订单号、Google 账户匿名标识 | [Google 隐私政策](https://policies.google.com/privacy) |
| **Firebase Analytics** | Google LLC | 收集匿名异常崩溃日志，分析应用稳定性 | 匿名设备标识、崩溃堆栈信息、操作系统版本 | [Firebase 隐私政策](https://firebase.google.com/support/privacy) |

除上述因实现支付、崩溃统计所必需的第三方 SDK 外，我们**不会主动将您的个人信息共享、转让或公开披露给任何第三方**。

---

### 3. 信息的存储与安全

1. **存储地点**：我们在中华人民共和国境内运营中收集的信息，原则上存储于中国境内。因使用 Google Firebase 进行崩溃统计分析，部分去标识化的系统日志可能传输至境外 Google 服务器进行计算处理。
2. **存储期限**：我们仅在实现服务目的所必需的最短期限内保留信息（如高级版订单凭据在提供服务期间持续保留）。
3. **安全防护**：我们采用业界通行的安全防护标准（包括本地数据沙盒隔离、数据传输 HTTPS 加密等）保障信息安全，防止未经授权的访问、泄露或篡改。

---

### 4. 您的权利（查询、更新、数据撤回与注销）

1. **权限撤回**：您可以随时在 Android 系统“设置 - 应用权限管理”中关闭录音、通知等授权。关闭后相应功能将停止，但不影响其他独立功能使用。
2. **数据清除**：由于本应用不设用户注册体系，所有均衡器配置、自定曲线数据均存储于本地。您可通过 Android 系统“应用管理 - 清除数据/清除缓存”或直接卸载本应用来彻底删除所有本地数据。
3. **退订与客服响应**：如您对已绑定的订单有任何疑问或需要协助注销相关订单记录，可通过本政策公布的邮箱与我们联系，我们将在 15 个工作日内予以核查并答复。

---

### 5. 未成年人保护

1. 我们非常重视对未成年人个人信息的保护。本应用主要面向具备完全民事行为能力的成年人，若您为未成年人，请在监护人指导下阅读本政策。
2. 未成年人未经监护人同意，不得在应用内进行高级版充值或购买操作。

---

### 6. 隐私政策的更新

我们可能会适时对本《隐私政策》进行修订。当条款发生重大变更时，我们将在应用版本更新时向您展示弹窗或在关于页面展示更新后的内容。若您在变更生效后继续使用本服务，即表示您已充分理解并同意最新政策。

---

### 7. 联系我们

如果您对本隐私政策、个人信息保护有任何疑问、意见、投诉或建议，请通过以下方式联系开发者：

* **联系邮箱：** yokodev.pro@gmail.com  
* **响应时限：** 我们将在收到您的邮件并在验证身份后的 15 个工作日内给予答复与处理。

---
<br>

<span id="english"></span>

<div align="right">
  <b>Language / 语言:</b> 
  <a href="#chinese"> 中文</a> | 
  <a href="#english"> English</a>
</div>

# Privacy Policy

**Effective Date:** December 9, 2025  
**Last Updated:** November 10, 2026  
**Developer:** yokodev ("we", "us", or "our") 

---

### Introduction
PrecisEQ is a professional digital signal processing (DSP) and audio equalization tool independently engineered by yokodev. We understand the paramount importance of your personal information and are committed to safeguarding your privacy.

**【SPECIAL NOTICE】**  
1. **100% Local On-Device Audio DSP Processing**: All audio equalization, convolution filters, and spatial acoustic processing are executed strictly on your local device in real-time. This Application NEVER records environmental audio, NEVER caches audio recordings locally, and NEVER uploads or streams your audio or call content.  
2. **No Mandatory Account Registration**: The Application requires no sign-up or user account, and does not collect sensitive personally identifiable information such as legal names, national ID numbers, contacts, or precise GPS locations.

Please read and understand this Privacy Policy before utilizing our services. Using or continuing to use the Application constitutes your acceptance of the data handling practices outlined herein.

---

### 1. Information Collection and Usage

To deliver stable and reliable audio enhancement capabilities, we collect and process information only within a legitimate, lawful, and necessary scope:

#### 1.1 Audio Processing & Sensitive System Permissions (Important)
* **Audio Recording Permission (`RECORD_AUDIO`)**: Requested strictly to capture internal digital audio playback from media apps via standard Android OS routing APIs. **The Application NEVER activates the hardware microphone for ambient recording, nor does it record, store, or transmit your voice or sound data.**
* **Media Projection Permission (`MediaProjection`)**: Required in select operational modes to acquire audio loopback authorization from the OS via a foreground service. **Solemn Statement: The Application strictly uses this service for audio capture authorization only. It NEVER screenshots, records, stores, or uploads your screen graphics, display contents, or user interactions.**
* **Notification Permission (`POST_NOTIFICATIONS`)**: Used to display the ongoing real-time operational status and quick controls of the foreground audio processing service in your system notification drawer.

#### 1.2 Crash Diagnostics & Basic Device Telemetry
* To diagnose system crashes and enhance DSP engine stability, we collect anonymized technical logs via reputable third-party analytics (including device model, OS version, package version, and crash stack traces). This data cannot be utilized to identify any specific individual.

#### 1.3 In-App Purchases & Order Tokens
* When upgrading to the Pro Edition, payments are handled directly by authenticated payment gateways. We verify only the **Order ID and payment completion status** returned by payment providers to unlock Pro entitlements. **We neither receive nor store sensitive financial credentials such as credit card numbers or payment passwords.**

#### 1.4 No Advertising Commitment
* **The Application is completely ad-free. We do not gather advertising identifiers (e.g., GAID) and do not disclose or monetize any user data with ad brokers or marketing networks.**

---

### 2. Third-Party SDK Integrations & Data Sharing

To facilitate secure transactions and crash diagnostics, we integrate trusted third-party SDKs. The SDK directory and their respective data practices are detailed below:

| SDK Name | Provider | Purpose | Data Processed | Privacy Policy / Official Documentation |
| :--- | :--- | :--- | :--- | :--- |
| **Alipay Client SDK**<br>*(Domestic Distribution)* | Ant Group Co., Ltd. | Secure payment processing and order status verification | Device model, MAC address, network state, BSSID/SSID, system parameters (for anti-fraud risk control) | [Alipay Privacy Policy](https://opendocs.alipay.com/open/54/01g6qm) |
| **Google Play Billing**<br>*(Google Play Distribution)* | Google LLC | Global in-app purchases and license restoration | Purchase token, Order ID, anonymized Google account identifier | [Google Privacy Policy](https://policies.google.com/privacy) |
| **Firebase Analytics** | Google LLC | Crash stack diagnostics and application stability analysis | Anonymous instance ID, crash stack traces, OS release | [Firebase Privacy Policy](https://firebase.google.com/support/privacy) |

Apart from the indispensable SDKs listed above for payment and crash analytics, **we do not sell, share, transfer, or publicly disclose personal data to any external parties.**

---

### 3. Data Storage & Security Measures

1. **Storage Location**: Data collected within the operational scope in Mainland China is hosted domestically. For crash diagnostics handled via Google Firebase, de-identified diagnostics logs may be processed across secure Google server infrastructure globally.
2. **Retention Period**: We retain information only for the minimum duration strictly necessary to fulfill the service objectives (e.g., active purchase tokens are maintained throughout the service lifecycle).
3. **Security Protection**: We implement industry-standard protective safeguards, including Android app sandbox isolation and mandatory HTTPS/TLS cryptographic protocols for all remote network transmissions, ensuring protection against unauthorized interception or data breach.

---

### 4. Your Rights (Access, Deletion, and Revocation)

1. **Permission Revocation**: You may revoke permissions (`RECORD_AUDIO`, notifications, etc.) at any time via Android "Settings > Apps > Permissions". Revoking permissions disables dependent DSP features without impacting unaffected operations.
2. **Data Erasure**: Because the Application maintains no server-side user accounts, all EQ configurations, impulse response files, and custom presets reside exclusively in local device storage. You can permanently erase all local application state by selecting "Clear Storage / Clear Cache" in Android system settings or by uninstalling the Application.
3. **Inquiries & Order Assistance**: If you have questions concerning purchase binding or require assistance regarding order records, please contact us via our official email. We will process and respond to verified inquiries within 15 business days.

---

### 5. Protection of Minors

1. We place immense priority on safeguarding minors. This Application is designed for users with full civil capacity. Minors should review this policy under the supervision of a legal guardian.
2. Minors are strictly prohibited from executing in-app purchases or Pro upgrades without prior explicit authorization from their legal guardians.

---

### 6. Changes to this Privacy Policy

We may update this Privacy Policy periodically to reflect legal or technical changes. Material modifications will be notified via in-app prompts or version release notes. Continued use of our Application following an update signifies your acceptance of the revised terms.

---

### 7. Governing Language

This Privacy Policy is executed in Chinese and translated into English for convenience. In the event of any discrepancies or ambiguities between the Chinese version and any translated edition, the **Chinese version shall prevail**.

---

### 8. Contact Us

If you have questions, feedback, or complaints regarding this Privacy Policy or personal data practices, please reach out via:

* **Email:** yokodev.pro@gmail.com  
* **Response Window:** We review and reply within 15 business days upon identity verification.
