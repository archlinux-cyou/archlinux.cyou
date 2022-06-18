name: Start get your own free ArchLinux.cyou subdomain
description: Choose this if you are applying for a free ArchLinux.cyou subdomain for the first time
labels: ["Applying"]
assignees:
  - linlinzzo
body:
  - type: markdown
    attributes:
      value: |
        请在标题写“网站名称”！
  - type: input
    id: name
    attributes:
      label: 网站名称
      description: 会在 Readme 中展示
      placeholder: ex. 开往
    validations:
      required: true
  - type: input
    id: website
    attributes:
      label: 网站网址
      description: |
        必须是 http**s** 网站；
        `bar, best, cloud, digital, guru, life, live, miami, online, rest, shop, site, store, surf, today, website, world, sapce, fun` 这些域名往往购买时便宜，但第二年续费会在 100 元以上，你会坚持用这个域名吗？如果你更新了域名，记得打开 issues 更新信息。
      placeholder: ex. https://travellings.link
    validations:
      required: true
  - type: input
    id: place
    attributes:
      label: 徽标位置
      description: |
        只放在“网页底部”，或只放在“默认收起的菜单里”，审核通过率较低。请放在打开网页后能**直接看到的地方**（顶栏或固定的侧栏是不错的选择，可参见 Readme 或已收录的网站）；
      placeholder: ex. 侧栏
    validations:
      required: true
  - type: textarea
    id: content
    attributes:
      label: 内容方向
      description: |
        不会展示在 Readme ；
        你想与网络世界分享什么？
    validations:
      required: false
  - type: checkboxes
    id: checkagain
    attributes:
      label: 请确认一下事项
      description: |
        1. 我已阅读要求且满足收录条件，其中博客网站要求至少有 20 篇文章。
        2. 我的信息填写正确，如有错误会通知及时修改。
        3. 博客网站已经同步提交(同意被提交)至 https://zhblogs.ohyee.cc/ 。
        4. 允许开往社区对贵站可用性检查，爬取文章链接包括未来添加的其他协议
      options:
        - label: 我已确认以上事项
          required: true
