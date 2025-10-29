# ColorEcosystem
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.txt)
[![Code: GitHub](https://img.shields.io/badge/Code-GitHub-blue?logo=github)](https://github.com/opas-lab/color-ecosystem)
[![Paper: ColorEcosystem](https://img.shields.io/badge/Paper-ArXiv-green?logo=arxiv)](http://arxiv.org/abs/2510.21566)

<h2 align="center">ColorEcosystem: Powering Personalized, Standardized, and Trustworthy Agentic Service in massive agent Ecosystem</h2>

<h3>The Blueprint of ColorEcosystem</h3>

![](https://arxiv.org/html/2510.21566v1/figures/framework.png)

<h3>Demo 1: Social task between assistant agents</h3>
<img src="docs/assets/calendar.gif" title="Scheduling a calendar event with a friend's assistant agent" />

<h3>Demo 2: Tool call on a mobile device</h3>
<img src="docs/assets/phone.gif" title="Making an emergency phone call from my assistant agent to a family doctor" />

## 🎉 News
- **[2025/10/24]**: ColorEcosystem is released! We have open-sourced the ColorEcosystem code on GitHub.

## ✨ Key Features
- **Agent Store**: Developers can publish remote A2A agents or MCP tools to the Agent Store.
- **Agent Carrier**: Users can enable agents or tools from the store, chat with their personal assistant agent to complete tasks by leveraging these tools, and even interact with friends' assistant agents.
- **Agent Audit**: Users can control and authorize which data their personal assistant agent is allowed to access.

## 🚀 Quick Start
### 1. Repository overview
ColorEcosystem is implemented across several repositories:

Backend Services (microservices)
- color-gateway-service — API gateway for other backend services
- color-store-service — API for Agent/MCPTool and user management
- color-social-service — API for friend and user online management
- color-assistant-service — API for assistant and tool call management

Frontend Service
- color-store-portal — Web portal for developers' management console

Client App
- color-store-android — Android client app (prebuilt APK is provided)

Note: You do not need to clone all repositories. To deploy locally you should clone the four backend services (`color-*-service`). Clone the frontend service (`color-store-portal`) if you want to run the web portal. A prebuilt APK for the Android client is provided, so building the Android app from source is optional.

You can clone all repositories at once with:
```
git submodule update --init --recursive
```

To update all submodules later:
```
git submodule update --remote --recursive
```


### 2. Usage
#### 2.1 Run backend services
Clone the four backend service repositories and follow each repository's README to run them in the following order:
- [`color-gateway-service`](https://github.com/opas-lab/color-gateway-service.git)
- [`color-store-service`](https://github.com/opas-lab/color-store-service.git)
- [`color-social-service`](https://github.com/opas-lab/color-social-service.git)
- [`color-assistant-service`](https://github.com/opas-lab/color-assistant-service.git)

#### 2.2 Run frontend service
Follow the README of [`color-store-portal`](https://github.com/opas-lab/color-store-portal.git) to run the frontend service.

#### 2.3 Run Android app
Follow the README of [`color-store-android`](https://github.com/opas-lab/color-store-android.git) to run the Android client app, or use the provided prebuilt APK.

## 🌱 Contributing
We welcome contributions of all kinds! Please open issues or pull requests in the appropriate repositories.

## 📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

## 📚 Citation
If you use this project in your research or work, please cite:
```
@article{wu2025colorecosystem,
  title={ColorEcosystem: Powering Personalized, Standardized, and Trustworthy Agentic Service in massive agent Ecosystem},
  author={Wu, Fangwen and Wu, Zheng and Wang, Jihong and Chen, Yunku and Pei, Ruiguang and Huang, Heyuan and Liao, Xin and Lou, Xingyu and Deng, Huarong and Fu, Zhihui and Liu, Weiwen and Zhang, Zhuosheng and Zhang, Weinan and Wang, Jun},
  journal={arXiv preprint arXiv:2510.21566},
  year={2025},
  url={https://arxiv.org/abs/2510.21566}
}
```
