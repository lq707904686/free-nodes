# free-nodes

免费外网节点订阅（公开节点合集），每小时级更新的源 + 逐节点 TLS 握手验证后精选。

## 订阅链接（直接导入）

- **Clash / Clash Meta**：`https://cdn.jsdelivr.net/gh/lq707904686/free-nodes@main/clash.yaml`
  备用直链：`https://raw.githubusercontent.com/lq707904686/free-nodes/main/clash.yaml`
- **NekoBox / sing-box**：`https://cdn.jsdelivr.net/gh/lq707904686/free-nodes@main/singbox.json`
  备用直链：`https://raw.githubusercontent.com/lq707904686/free-nodes/main/singbox.json`
- **通用分享链接（base64）**：`https://cdn.jsdelivr.net/gh/lq707904686/free-nodes@main/links.txt`

> 优先用 jsDelivr 链接导入：国内直连 raw.githubusercontent.com 常常失败，jsDelivr 稳得多。

## 这一版（2026-11-15）

- 130 个节点：100 个 TLS 节点（VLESS Reality 为主，99 VLESS + 1 VMess）+ 15 个 Hysteria2 + 15 个 Shadowsocks
- **全部非 Cloudflare 出口**：有意避开 CF 线，只补 VPS 直连节点，和现有 CF 订阅互补
- 来源：Au1rxx/free-vpn-subscriptions（每小时刷新、逐节点探活）90 个 + TelegaVPN/free-vpn-keys（15–30 分钟探活）10 个 + 同源 hy2/ss 30 个
- 验证口径：100 个 TLS 节点逐个做过 TLS 握手 + 证书校验（全部通过）；hy2/ss 只验证了源头探活状态，未做端到端握手
- 已过滤：私网 IP、假 SNI、弱加密（rc4-md5 等）、无证书节点

## 诚实说明

- 公开免费节点没有隐私可言，**不要用它登录重要账号**。
- 节点存活按小时计，导入后请在客户端跑自动测速（url-test），以手机实测排名为准；沙盒里测不了真实速度。
- 文件按周刷新（源头挂了或节点大面积失效会提前换源）。

## 来源

- https://github.com/Au1rxx/free-vpn-subscriptions
- https://github.com/TelegaVPN/free-vpn-keys
- 另参考：chengaopan/AutoMergePublicNodes、free18/v2ray、mahdibland/V2RayAggregator
