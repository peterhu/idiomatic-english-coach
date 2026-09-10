# Example 2 — 技术排障（UART 乱码）

**Before**（原文，未修改）：

> We received a lpddr5 board from supplier recently. we didn't some basic function test, In general the functions looks alright, but there's one thing bothered me, the uart debug for BIOS doesn't work. this is the only way for BIOS debug so It's very import to me. the symptom is the putty is 乱码 while I tried to capture it during BIOS boot. after synced with the supply It seems the cable we used doesn't the 3000000 baud rate which is setted in current BIOS. since we don't have the cable, we tried to capture it by protocol analyzer, after 折腾 for serveral times, and eventually, 黄天不负苦心人，we can captuer the log porperly. I feel so happy when I saw the BIOS debug log.

**After**（日常口语版）：

> We just **got an LPDDR5 board** from the supplier. We **ran through some basic tests**, and everything looked okay overall — but **one thing bugged me**: the BIOS UART debug doesn't work. And that's **our only way to debug the BIOS**, so it's **a big deal**. The symptom is, **PuTTY just shows garbage** when I try to capture the output during boot. After **checking with the supplier**, it turns out our cable **can't handle the 3M baud rate** the BIOS is set to. Since we didn't have the right cable, we tried **a protocol analyzer instead**. After **messing around with it a bunch**, it finally **paid off** — we **got the log captured cleanly**. I was so happy when I finally saw the BIOS debug log.

**Key fixes**：

| 生硬 | 地道 |
|------|------|
| we didn't some basic function test | we ran some basic function tests |
| the putty is 乱码 | PuTTY shows garbage / garbled text |
| doesn't the 3000000 baud rate | doesn't support / can't handle the baud rate |
| after 折腾 for several times | after messing around with it several times |
| 皇天不负有心人 | it finally paid off |

**可迁移表达**：`run through some tests` · `bug me` · `garbled text / mojibake` · `sync up with` · `mess around with` · `pay off` · `manage to`
