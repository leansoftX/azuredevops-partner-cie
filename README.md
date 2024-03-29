# Azure DevOps Partner CIE

所有参训人员需要具备以下条件：

- 预先完成 Azure DevOps 账号注册
- 预先完成 Azure 免费账号注册 [注册说明](./GlobalAzureUSD200FreeAccount.pdf)

讲师需要完成以下准备：

- 使用Demo Generator创建PartsUnlimited项目
- 在PartsUnlimited项目中完成
  - Build: PartsUnlimitedE2E 的触发，确保构建成功完成
  - Release: PartsUnlimitedE2E的配置和触发，确保Dev/QA/Production环境全部部署成功
  - Branch Policy：在master分支上启用以下分支策略
    - Require a minimum number of reviewers (允许 Requestors can approve their own changes)
    - Check for linked work items
    - Check for comment resolution
    - Build validation
      - 选择：PartsUnlimitedE2E

## 培训日程

- 1.1 9:00-10:00 Azure DevOps简单介绍及微软Azure DevOps案例分享，GitHub讲解。
  - 演讲：
    - 02-AzureDevOpsOverview-v1.pptx
  - 介绍Azure DevOps现状及主要功能简介。
  - Github介绍, Github集成Azure Pipeline
- 1.2 10:00-11:00 Azure DevOps 看板及代码管理功能展示
  - 演示
    - 02-AzureDevOpsOverview-v1.pptx 最后的基于Git的特定分支模式一页完成以下演示
  - 端到端广义流水线：演示看板功能，从看板卡片创建分支，在分支上提交代码并创建PR，通过PR触发构建并完成Dev-QA-PROD环境的部署
  - 参考资源（学员无需做实验）
    - <https://almvm.devopshub.cn/labs/azuredevops/git/>
    - <https://almvm.devopshub.cn/labs/azuredevops/pullrequests/>

- 1.3 11:00 – 12:00 Azure DevOps Service 看板管理练习
  - 练习
  - 学员使用自己的Azure DevOps Service根据练习指导手册完成看板及源代码管理练习
  - <https://almvm.devopshub.cn/labs/azuredevops/agile/>

午休

- 1.4 14:00-15:30	Azure Pipeline的搭建介绍及AKS集群部署
  - 演示如何在Azure DevOps Service中配置自动化编译及自动化部署
    - 03-Build-v1.pptx
    - 04-ReleaseMangement-v1.pptx
  - 如何基于看板、Git等功能创建广义交付流水线
    - 动手实验-Azure DevOps Service广义流水线
  - 如何持续部署应用到AKS集群环境
    - 动手实验-AKS搭建Azure DevOps流水线

- 1.5 14:00-15:00 Azure Pipeline搭建及运行练习
  - 练习
  - 学员根据练习指导手册自行创建并运行Azure Pipeline，完成自动化构建
  - <https://almvm.devopshub.cn/labs/vsts/continuousintegration/>
  - <https://almvm.devopshub.cn/labs/vsts/continuousdeployment/>

茶歇 10 分钟

- 1.6 15:10-16:00 Azure DevOps测试管理
  - 演讲 + 演示
    - 05-TestManagement-v1.pptx
  - 演示如何使用Azure DevOps进行测试

- 1.7 16:00-17:00 Azure DevOps 测试管理
  - 练习
  - 完成样例项目的测试计划、测试用例的编写及运行。
  - <https://almvm.devopshub.cn/labs/vsts/testmanagement/>

## 相关资料

- Azure Pipeline Build Agent Source <https://github.com/microsoft/azure-pipelines-agent>
- Azure Pipeline Build Tasks <https://github.com/Microsoft/azure-devops-extension-tasks>
- Marketplace <https://marketplace.visualstudio.com/azuredevops>
- Azure DevOps Extension Development Guide <https://docs.microsoft.com/en-us/azure/devops/extend/get-started/node?view=azure-devops>
- Azure Pipline Built-in Variables <https://docs.microsoft.com/en-us/azure/devops/pipelines/build/variables?view=azure-devops&tabs=yaml>

- [Blog 绑定Git Pull Request和部署目标环境](https://devopshub.cn/2018/05/03/git-pull-request-binding-to-target-environment/)

- [视频：中国农业银行敏捷转型和看板秘籍分享](https://mp.weixin.qq.com/s?__biz=MzA5NzU3Njc5Mw==&mid=2651203177&idx=1&sn=85aef93f6d2f94dbf5157562983f7f63&chksm=8b6c345fbc1bbd494ac8f8e048e4fd105567fbb5078469f9c528e5f823cb4a4e91099b4b833f&mpshare=1&scene=1&srcid=1027QlkAX6kV93FxFIpgTqMf&sharer_sharetime=1572148802075&sharer_shareid=0c3fa1c9154ead4beb54fbbaad0db1d0&key=ffa2fa9c0f0d785dbfad1869589618ba4779be923b34d8f5fe7307b6259aed07e077f70fef2fb2fa036deeae1703260cf1da21cad0bef206d22a59df2ba3f6fa3bbf079171e405a0b0d69d9554b95ff0&ascene=1&uin=MzgwNjc5MDk1&devicetype=Windows+10&version=62070152&lang=zh_CN&pass_ticket=XKVG3HeaMs%2FwKBsPzpgWGAK4SKEkdXbuc88z2c09OkyjqvSkkPi9El2tz6hI0%2Fq5)

- [C3端到端全流程敏捷研发转型之路大揭秘](https://mp.weixin.qq.com/s?__biz=MzA5NzU3Njc5Mw==&mid=2651203249&idx=1&sn=694137ffa07b2049aff364c1146d9704&chksm=8b6c3487bc1bbd9101147a19c53b8fb6e4240dd30143e38deb12299e5883c74d48624869eb7e&mpshare=1&scene=1&srcid=1027AF6eyBMIG5ezR62ulVrJ&sharer_sharetime=1572148819899&sharer_shareid=0c3fa1c9154ead4beb54fbbaad0db1d0&key=e224974e93afb4ccf53e1fb64b59631375020a93d43b1de7eabe89b53aa42fbed84d9e0b54a0f441d290f4c5a830a9fdafba79f91603da909b4dce088c8717281f5b320972a15d5e6e815922a8467a12&ascene=1&uin=MzgwNjc5MDk1&devicetype=Windows+10&version=62070152&lang=zh_CN&pass_ticket=XKVG3HeaMs%2FwKBsPzpgWGAK4SKEkdXbuc88z2c09OkyjqvSkkPi9El2tz6hI0%2Fq5)

- [一种适用于大规模应用系统双模研发的GIT分支模型（上篇）](https://mp.weixin.qq.com/s?__biz=MzA5NzU3Njc5Mw==&mid=2651202659&idx=1&sn=656942ce084d0a6dcabfdfdec3c4635a&chksm=8b6c3655bc1bbf431d19eb5500758b830e612124367db59b32d228822a1d81853f8ee833163f&mpshare=1&scene=1&srcid=1027dkBB5YtxHsGyTL6meKn6&sharer_sharetime=1572148833518&sharer_shareid=0c3fa1c9154ead4beb54fbbaad0db1d0&key=3ea340d47a674ce8c5143f81676e3f637c581f63b8b43f3aee32e29aabc869d5e36f86bc3b47ad025de2346ef929891186169a014023191c61c2bdd5eea6b1a0b0eecfc800c9219dd0a9a2802c8b387f&ascene=1&uin=MzgwNjc5MDk1&devicetype=Windows+10&version=62070152&lang=zh_CN&pass_ticket=XKVG3HeaMs%2FwKBsPzpgWGAK4SKEkdXbuc88z2c09OkyjqvSkkPi9El2tz6hI0%2Fq5)

- [一种适用于大规模应用系统双模研发的GIT分支模型（下篇）](https://mp.weixin.qq.com/s?__biz=MzA5NzU3Njc5Mw==&mid=2651202676&idx=1&sn=96a3df0184621b69ee45aa420ce606a2&chksm=8b6c3642bc1bbf54d19823de63f0f0bdd3a5d6902968eb716e8fdf935da2acafe85a22f0655a&mpshare=1&scene=1&srcid=1027FQiElD3SBIvaRuMi8LIs&sharer_sharetime=1572148843660&sharer_shareid=0c3fa1c9154ead4beb54fbbaad0db1d0&key=ffa2fa9c0f0d785d50406532457ba9fd068a1159c207da20a9108ee1f9cac975bc8da81021c306cc169c54be92d7816eea106923a26723fb6f742c903e354bd303e77a9914eb996e8e4b0ee8f38268ca&ascene=1&uin=MzgwNjc5MDk1&devicetype=Windows+10&version=62070152&lang=zh_CN&pass_ticket=XKVG3HeaMs%2FwKBsPzpgWGAK4SKEkdXbuc88z2c09OkyjqvSkkPi9El2tz6hI0%2Fq5)
