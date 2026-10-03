# 測試人員感謝套裝發放

[English](README.md) | **繁體中文**

發放給測試人員的紀念套裝：全附魔下界合金裝備、鞘翅與感謝勳章，並提供管理員回收與查詢功能。

> 本儲存庫包含同一個腳本的兩個版本：**繁體中文（zh-TW）** 是作者伺服器實際使用的原始版本；**English** 為完整英文翻譯版（指令、訊息與變數名稱皆為英文），功能相同。

## 功能特色

- 下界合金頭盔、胸甲、護腿、靴子與鞘翅，附上所有保護類附魔、荊棘、耐久、經驗修補及對應的額外附魔（水下呼吸、親水性、迅捷潛行、輕盈、深海漫遊、靈魂疾行、冰霜行者）
- 附說明文字的感謝勳章（下界之星）
- 可發給指定玩家或全體在線玩家
- 可回收單一玩家或全體玩家的套裝（裝備欄與背包），並查詢誰還持有

## 需求

- [Paper](https://papermc.io/) 伺服器（開發環境 Paper 26.2 / Minecraft 26.2）
- [Skript](https://github.com/SkriptLang/Skript)（開發環境 2.16.2）

## 安裝

1. 先安裝[需求](#需求)中列出的插件。
2. 下載**其中一個**版本：

   | 版本 | 檔案 |
   |---|---|
   | 繁體中文（原始版本） | [`zh-TW/測試人員感謝套裝發放.sk`](zh-TW/%E6%B8%AC%E8%A9%A6%E4%BA%BA%E5%93%A1%E6%84%9F%E8%AC%9D%E5%A5%97%E8%A3%9D%E7%99%BC%E6%94%BE.sk) |
   | English（英文） | [`en/tester-thank-you-kit.sk`](en/tester-thank-you-kit.sk) |

3. 把 `.sk` 檔案放進伺服器的 `plugins/Skript/scripts/`。
4. 執行 `/sk reload 測試人員感謝套裝發放`（請換成你放入的檔名），或重新啟動伺服器。

> [!IMPORTANT]
> **只能安裝其中一個版本。** 兩個版本是同一個腳本的不同語言，同時載入會互相衝突或重複執行。

## 指令

| 指令（中文版） | 英文版 | 說明 | 權限 |
|---|---|---|---|
| `/發放感謝套裝 [玩家]` | `/givethankskit [player]` | 發放給指定玩家；省略時發給全體在線玩家 | OP |
| `/回收感謝套裝 <玩家>` | `/recallthankskit <player>` | 回收指定玩家的套裝 | OP |
| `/回收全部感謝套裝` | `/recallallthankskits` | 回收全體在線玩家的套裝 | OP |
| `/查看感謝套裝` | `/checkthankskits` | 列出持有套裝的在線玩家 | OP |

## 設定

- 依你的活動修改 `options:` 的 `armor_name` / `medal_name` 與說明文字中的日期（`2026/4/27`）。物品是以完整名稱辨識，請確保名稱獨一無二。

## 注意事項

- 回收與查詢只對在線玩家有效。

## 相關專案

- [skript-test-gear-distribution](https://github.com/Im-Tim-mI/skript-test-gear-distribution)－測試裝備發放系統
- [skript-special-item-lock](https://github.com/Im-Tim-mI/skript-special-item-lock)－特殊物品封鎖系統

## 授權

**MIT + Commons Clause**，完整條款請見 [LICENSE](LICENSE)。

- ✅ 可自由使用、複製、修改與分享本腳本。
- ✅ 本授權明確允許在收費或營利的 Minecraft 伺服器上安裝與運行本插件（含修改版）。
- ❌ 禁止的僅限於直接或間接販售本插件本體、修改版本，或以付費方式取得其檔案或原始碼。

Copyright (c) 2026 廷廷小教室、廷廷的家（Tim945）
