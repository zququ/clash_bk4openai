# clash_bk4openai
```
proxy-groups:
-
  name: '🧠 OpenAI'
    type: select
    proxies:
      - '🚀 节点选择'
      - '🔑 手动选择'
      - ⚡️IPLC/IEPL
      - 🎠Trojan
      - 🇭🇰香港节点
      - 🇯🇵日本节点
      - 🇺🇸美国节点
      - 🇨🇳台湾节点
      - 🇸🇬新加坡节点
      - 🇪🇺欧洲节点
      - 🍁其他地区
      - DIRECT
  -

rule-providers:
  OpenAI:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Providers/Ruleset/OpenAi.yaml"
    path: ./Rules/OpenAI.yaml
    interval: 259200   

rules:
  - DOMAIN-SUFFIX,sentry.io,REJECT
  - RULE-SET,OpenAI,🧠 OpenAI
```
