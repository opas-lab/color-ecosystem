# ColorEcosystem
[![Python: 3.13](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Code: Github](https://img.shields.io/badge/Code-Github-blue?logo=github)](https://github.com/opas-lab/color-ecosystem)
[![Paper: ColorEcosystem](https://img.shields.io/badge/Paper-Arxiv-green?logo=arxiv)](http://arxiv.org/abs/2510.21566)

<p style="color:red"><b>(To download source code, please see the below `Quick Start`)</b></p>

<h2 align="center">ColorEcosystem: Powering Personalized, Standardized, and Trustworthy Agentic Service in massive-agent Ecosystem</h2>

<p><b>The Blueprint of ColorEcosystem</b></p>

![](https://arxiv.org/html/2510.21566v1/figures/framework.png)

<p></p>
<p><b>A demo video for social task between assistant agents</b></p>
<img src="docs/assets/calendar.gif" title="Scheduling a calender event with a friend's assistant agent" />

<p></p>
<p><b>A demo video for tool call on mobile device</b></p>
<img src="docs/assets/phone.gif" title="Making an emergency phone call from my assistant agent to family doctor" />


## 🎉 News
- **[2025/10/24]**: ColorEcosystem is released! We have also opened source code of [ColorEcosystem](https://github.com/opas-lab/color-ecosystem)!


## ✨ Key Features
- **Agent Store**: Developers can publish remote A2A agents or MCP tools into Agent Store.
- **Agent Carrier**: Users can enable agents or tools in the store, and chat with their own assistant agent to complete a task by leveraging these tools, and even can talk to friends' assistant agents.
- **Agent Audit**: Users can authorize which data could be accessed by their personal assistant agent.


## 🚀 Quick Start
### 1. Introduction of repositories
The implementation of part of `ColorEcosystem`'s functionality consists of 6 repositories:
```
|- Backend Services                 Micro-services for backend services
|  |- color-gateway-service         API gateway for other backend services
|  |- color-store-service           API for Agent/MCPTool and user management
|  |- color-social-service          API for friend and user online management
|  |- color-assistant-service       API for assistant and tool call management
|
|- Frontend Service                 Web service for frontend web pages
|  |- color-store-portal            Web portal for developers' management console
|
|- Client App                       Client app for end users
|  |- color-store-android           Android client app
```

**Note**: You don't need to clone all repositories.
It's necessary to clone the 4 backend services (`color-*-service`) if you want to deploy them locally, and clone the frontend service (`color-store-portal`) if you want to publish remote servers of A2A agents or MCP tools as a developer.
We provided the prebuilt APK of Android client app, so you don't need to build it from the source code.

You may clone all repositories at the first time with:
```
git clone --recursive https://github.com/opas-lab/color-ecosystem.git
```

later you may update all repositories with:
```
git submodule update --remote --recursive
```

### 2. Usage
#### 2.1. Run Backend Services
Clone the 4 repositories of backend services, and follow the README.md of each repository to run them with the below order:
- [`color-gateway-service`](https://github.com/opas-lab/color-gateway-service)
- [`color-store-service`](https://github.com/opas-lab/color-store-service)
- [`color-social-service`](https://github.com/opas-lab/color-social-service)
- [`color-assistant-service`](https://github.com/opas-lab/color-assistant-service)

#### 2.2. Run Frontend Service
Follow the README.md of repository [`color-store-portal`](https://github.com/opas-lab/color-store-portal) to run the frontend service.

#### 2.3. Run Android App
Follow the README.md of repository [`color-store-android`](https://github.com/opas-lab/color-store-android) to run the Android client app.


## 🌱Contributing
We welcome all forms of contributions!


## 📜 License
This project is licensed under the MIT License, which permits free use and modification of the code but requires retaining the original copyright notice.


## 📚 Citation
If you have used this project in your research or work, please cite:
```
@article{wu2025colorecosystem,
  title={ColorEcosystem: Powering Personalized, Standardized, and Trustworthy Agentic Service in massive-agent Ecosystem},
  author={Wu, Fangwen and Wu, Zheng and Wang, Jihong and Chen, Yunku and Pei, Ruiguang and Huang, Heyuan and Liao, Xin and Lou, Xingyu and Deng, Huarong and Fu, Zhihui and Liu, Weiwen and Zhang, Zhuosheng and Zhang, Weinan and Wang, Jun},
  journal={arXiv preprint arXiv:2510.21566},
  year={2025},
  url={https://arxiv.org/abs/2510.21566}
}
```
