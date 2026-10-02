# TripMaster Releases

TripMaster is a Windows AI travel-planning app. Download **0.2.1** from the [latest release](https://github.com/SamChengYo/TripMaster-Releases/releases/latest).

## Windows download

- [Windows x64 installer](https://github.com/SamChengYo/TripMaster-Releases/releases/download/v0.2.1/TripMaster-0.2.1-Windows-x64.exe)
- [Release notes and checksums](https://github.com/SamChengYo/TripMaster-Releases/releases/tag/v0.2.1)

This is an unsigned public development build. The app checks for updates on startup; you choose when to download and install them. Existing provider keys, journeys and preferences are retained.

## 0.2.1 changes

Budgets explicitly cover the whole trip and can be entered per person or for the whole party. Flights and accommodation can be included independently, and existing journeys can edit these settings.

Model calls go directly through **TripMaster → LiteLLM Proxy → model provider**. There is no extra TripMaster Gateway. Configure your LiteLLM URL, its access key when authentication is enabled, and your own provider API key. Obtain LiteLLM access from your service administrator or [deploy LiteLLM](https://docs.litellm.ai/docs/proxy/docker_quick_start). A shared TripMaster-hosted LiteLLM service is not yet available. Desktop users do not need Python.

When updating from 0.2.0, enter the actual LiteLLM URL and access key; old Gateway credentials are not reused. Saved provider keys are retained. Provider keys are encrypted on your computer and sent to the LiteLLM service you configure for model calls.

This public repository contains installers, release notes and update metadata. Source code is maintained in a private repository. A GitHub account or token is not needed to download releases.

---

TripMaster **0.2.1** 已提供 Windows x64 安裝包。這是未簽署的公開開發版；可從上方連結下載，或在 App 內選擇下載並安裝更新。

- 預算可選每人／全員整趟，機票與住宿各自選擇是否包含；既有旅程可修改預算。
- 模型呼叫直接交給 LiteLLM，已移除額外的 TripMaster Gateway。
- 更新會保留供應商 Key、行程與偏好；舊 Gateway 網址／存取碼需改為實際 LiteLLM 連線資訊。

LiteLLM 網址與存取金鑰由既有服務管理者提供，或由你自行部署。目前尚未提供 TripMaster 共用線上 LiteLLM 服務。供應商 Key 在本機加密保存，模型呼叫時會交給你設定的 LiteLLM 服務。
