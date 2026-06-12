# 202606071709 e4770cd3 — USER_INPUT 序列（真實使用者輸入）

> 總 USER_INPUT 步驟: 49
> 真實使用者輸入（>50 字、非純 UUID）: 21

---

## Step 0

請用 MCP 讀取 ChatMelius/agyIDE/20260607_STLS_DaemonMode_FullReview/handoff_prompt_02.md 並繼續執行未完成任務。第一個任務就是看你的 System Prompt。

## Step 27

file://$HOME/...

## Step 80

$680b2cdc-cee5-4ee2-9a3b-0857fcce1326P "$e4770cd3-114c-41ae-8410-a7eae3d76b4d

## Step 192

但他是基於 cdp 方法，應該也不能有效作用了⋯⋯欸，先繼續搞 STLS 吧，全任務繼續，忽略這部分提示詞

## Step 236

找到兩個不同用途的 Debug.command：

AntiGeinese Debug.command（1231 行）— 主控腳本，管理整個 DeusEx 生態（CDP + MCP + STLS + agent-rs）


這個，搞到目前最能用的樣子就好。然後繼續地惡潤

## Step 242

不是，這個當然是拿來啟動 AntiGeinese.app 的，算是古早味實作
然後最新的 SakiAntiGeinese 會包含這裡面的 logger 等等

## Step 252

file://$HOME/...

## Step 277

-------------------------------------
Translated Report (Full Report Below)
-------------------------------------
Process:             AntiGeinese [3605]
Path:                /Applications/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
Identifier:          tw.com.saki-store.SakiAntiGeinese
Version:             2.0.11 (2.0.11)
Code Type:           ARM-64 (Native)
Role:                Background
Parent Process:      launchd [1]
Coalition:           tw.com.saki-store.SakiAntiGeinese [31314]
User ID:             503

Date/Time:           2026-06-07 16:19:29.3718 +0800
Launch Time:         2026-06-07 16:19:29.1672 +0800
Hardware Model:      iMac21,1
OS Version:          macOS 26.6 (25G5028f)
Release Type:        User

Crash Reporter Key:  328A513C-FB9E-63DF-7D77-FD036139EBD6
Incident Identifier: 673910D4-56B2-403B-A5B1-26A574EDA0F2

Time Awake Since Boot: 130000 seconds

System Integrity Protection: disabled

Triggered by Thread: 0, Dispatch Queue: com.apple.main-thread

Exception Type:    EXC_BREAKPOINT (SIGTRAP)
Exception Codes:   0x0000000000000001, 0x000000011500c858

Termination Reason:  Namespace SIGNAL, Code 5, Trace/BPT trap: 5
Terminating Process: exc handler [3605]


Thread 0 Crashed::  Dispatch queue: com.apple.main-thread
0   Electron Framework            	       0x11500c858 ares_dns_rr_get_ttl + 3407436
1   Electron Framework            	       0x11500c794 ares_dns_rr_get_ttl + 3407240
2   Electron Framework            	       0x110bb4c50 v8::Script::GetCompileHintsCollector() const + 101476
3   Electron Framework            	       0x11500c910 ares_dns_rr_get_ttl + 3407620
4   Electron Framework            	       0x111125204 v8::Object::WrapGlobal(v8::Isolate*, v8::Local<v8::Object> const&, v8::Object::Wrappable*, v8::CppHeapPointerTag) + 198764
5   Electron Framework            	       0x11260c86c node::PrincipalRealm::tick_callback_function() const + 627504
6   Electron Framework            	       0x11243e934 ElectronMain + 84
7   dyld                          	       0x18fafbe00 start + 6992


Thread 0 crashed with ARM Thread State (64-bit):
    x0: 0x000000011a263370   x1: 0x0000012000130760   x2: 0x0000000000000009   x3: 0x000000018fec0a10
    x4: 0x000000016b1f6bc0   x5: 0x0000000000000010   x6: 0x000000016b1f5930   x7: 0x00000000000000b0
    x8: 0x0000000000000000   x9: 0x0000000000000000  x10: 0x0000000000000000  x11: 0x0000000000000002
   x12: 0x0000000000000000  x13: 0x0000000000000000  x14: 0x0000000000000000  x15: 0x00000001fc9ae208
   x16: 0x000000018feb4944  x17: 0x00000001fc9a9ec0  x18: 0x0000000000000000  x19: 0x0000000000000068
   x20: 0x000000016b1f7198  x21: 0x000000016b1f6f98  x22: 0x000000011a185000  x23: 0x000000016b1f6fd0
   x24: 0x0000000000000002  x25: 0x00000001fc9ac680  x26: 0x0000000000000011  x27: 0x0000000000000041
   x28: 0x0000012000130700   fp: 0x000000016b1f6f80   lr: 0x000000011500c794
    sp: 0x000000016b1f6b50   pc: 0x000000011500c858 cpsr: 0x60001000
   far: 0x0000000000000000  esr: 0xf2000000 (Breakpoint) brk 0

Binary Images:
       0x104c08000 -        0x104c0bfff tw.com.saki-store.SakiAntiGeinese (2.0.11) <4c4c4450-5555-3144-a175-a5a5eb513df3> /Applications/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
       0x10fa60000 -        0x119ae7fff com.github.Electron.framework (*) <4c4c4403-5555-3144-a1a9-c4d1d783e6a0> /Applications/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Electron Framework
       0x104c4c000 -        0x104c63fff com.github.Squirrel (1.0) <4c4c44b8-5555-3144-a15d-f194c9417c2d> /Applications/SakiAntiGeinese.app/Contents/Frameworks/Squirrel.framework/Versions/A/Squirrel
       0x104cd4000 -        0x104d17fff com.electron.reactive (3.1.0) <4c4c445a-5555-3144-a166-7a5e68cf5b14> /Applications/SakiAntiGeinese.app/Contents/Frameworks/ReactiveObjC.framework/Versions/A/ReactiveObjC
       0x104c74000 -        0x104c7ffff org.mantle.Mantle (1.0) <4c4c44f8-5555-3144-a17c-b3f84b6f3c3b> /Applications/SakiAntiGeinese.app/Contents/Frameworks/Mantle.framework/Versions/A/Mantle
       0x105088000 -        0x10525bfff libffmpeg.dylib (*) <4c4c444b-5555-3144-a15c-da7f1e4e481b> /Applications/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Libraries/libffmpeg.dylib
       0x18fadc000 -        0x18fb822ab dyld (*) <e1c380d2-7409-3641-84e4-0a44aa2f0460> /usr/lib/dyld
               0x0 - 0xffffffffffffffff ??? (*) <00000000-0000-0000-0000-000000000000> ???
       0x18fec0000 -        0x18fec8963 libsystem_platform.dylib (*) <40fe7c10-0df9-3730-b0e7-f761093207e7> /usr/lib/system/libsystem_platform.dylib
       0x18feb3000 -        0x18febfb3b libsystem_pthread.dylib (*) <3aa5cdeb-79d9-3bb0-b5a3-906b7283e492> /usr/lib/system/libsystem_pthread.dylib

External Modification Summary:
  Calls made by other processes targeting this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
 

## Step 304

-------------------------------------
Translated Report (Full Report Below)
-------------------------------------
Process:             AntiGeinese [4069]
Path:                /Users/USER/*/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
Identifier:          tw.com.saki-store.SakiAntiGeinese
Version:             2.0.11 (2.0.11)
Code Type:           ARM-64 (Native)
Role:                Unspecified
Parent Process:      zsh [4063]
Coalition:           com.AlphaDelta.antigravity [1359]
Responsible Process: AntiGeinese [2897]
User ID:             503

Date/Time:           2026-06-07 16:26:10.1331 +0800
Launch Time:         2026-06-07 16:26:10.0054 +0800
Hardware Model:      iMac21,1
OS Version:          macOS 26.6 (25G5028f)
Release Type:        User

Crash Reporter Key:  328A513C-FB9E-63DF-7D77-FD036139EBD6
Incident Identifier: 3CB9EDA6-C935-4C02-8988-788E0E44080D

Time Awake Since Boot: 130000 seconds

System Integrity Protection: disabled

Triggered by Thread: 0, Dispatch Queue: com.apple.main-thread

Exception Type:    EXC_BREAKPOINT (SIGTRAP)
Exception Codes:   0x0000000000000001, 0x00000001109e0858

Termination Reason:  Namespace SIGNAL, Code 5, Trace/BPT trap: 5
Terminating Process: exc handler [4069]


Thread 0 Crashed::  Dispatch queue: com.apple.main-thread
0   Electron Framework            	       0x1109e0858 ares_dns_rr_get_ttl + 3407436
1   Electron Framework            	       0x1109e0794 ares_dns_rr_get_ttl + 3407240
2   Electron Framework            	       0x10c588c50 v8::Script::GetCompileHintsCollector() const + 101476
3   Electron Framework            	       0x1109e0910 ares_dns_rr_get_ttl + 3407620
4   Electron Framework            	       0x10caf9204 v8::Object::WrapGlobal(v8::Isolate*, v8::Local<v8::Object> const&, v8::Object::Wrappable*, v8::CppHeapPointerTag) + 198764
5   Electron Framework            	       0x10dfe086c node::PrincipalRealm::tick_callback_function() const + 627504
6   Electron Framework            	       0x10de12934 ElectronMain + 84
7   dyld                          	       0x18fafbe00 start + 6992


Thread 0 crashed with ARM Thread State (64-bit):
    x0: 0x0000000115c37370   x1: 0x00000138001308b0   x2: 0x0000000000000009   x3: 0x000000018fec0a10
    x4: 0x000000016f775fc0   x5: 0x0000000000000020   x6: 0x000000000000000a   x7: 0x0000000000000300
    x8: 0x0000000000000000   x9: 0x0000000000000000  x10: 0x0000000000000000  x11: 0x0000000000000002
   x12: 0x0000000000000000  x13: 0x0000000000000000  x14: 0x0000000000000000  x15: 0x0000000000000000
   x16: 0x000000018feb4944  x17: 0x00000001fc9a9ec0  x18: 0x0000000000000000  x19: 0x0000000000000068
   x20: 0x000000016f776598  x21: 0x000000016f776398  x22: 0x0000000115b59000  x23: 0x000000016f7763d0
   x24: 0x0000000000000002  x25: 0x000000000000004f  x26: 0x0000000113d5f65d  x27: 0x0000000000000041
   x28: 0x0000013800130850   fp: 0x000000016f776380   lr: 0x00000001109e0794
    sp: 0x000000016f775f50   pc: 0x00000001109e0858 cpsr: 0x60001000
   far: 0x0000000000000000  esr: 0xf2000000 (Breakpoint) brk 0

Binary Images:
       0x100688000 -        0x10068bfff tw.com.saki-store.SakiAntiGeinese (2.0.11) <4c4c4450-5555-3144-a175-a5a5eb513df3> /Users/USER/*/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
       0x10b434000 -        0x1154bbfff com.github.Electron.framework (*) <4c4c4403-5555-3144-a1a9-c4d1d783e6a0> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Electron Framework
       0x1006cc000 -        0x1006e3fff com.github.Squirrel (1.0) <4c4c44b8-5555-3144-a15d-f194c9417c2d> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Squirrel.framework/Versions/A/Squirrel
       0x100754000 -        0x100797fff com.electron.reactive (3.1.0) <4c4c445a-5555-3144-a166-7a5e68cf5b14> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/ReactiveObjC.framework/Versions/A/ReactiveObjC
       0x1006f4000 -        0x1006fffff org.mantle.Mantle (1.0) <4c4c44f8-5555-3144-a17c-b3f84b6f3c3b> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Mantle.framework/Versions/A/Mantle
       0x100a5c000 -        0x100c2ffff libffmpeg.dylib (*) <4c4c444b-5555-3144-a15c-da7f1e4e481b> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Libraries/libffmpeg.dylib
       0x18fadc000 -        0x18fb822ab dyld (*) <e1c380d2-7409-3641-84e4-0a44aa2f0460> /usr/lib/dyld
               0x0 - 0xffffffffffffffff ??? (*) <00000000-0000-0000-0000-000000000000> ???
       0x18fec0000 -        0x18fec8963 libsystem_platform.dylib (*) <40fe7c10-0df9-3730-b0e7-f761093207e7> /usr/lib/system/libsystem_platform.dylib
       0x18feb3000 -        0x18febfb3b libsystem_pthread.dylib (*) <3aa5cdeb-79d9-3bb0-b5a3-906b7283e492> /usr/lib/system/libsystem_pthread.dylib

External Modification Summary:
  Calls made by other processes targeting this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by this process:
    task_for_pid: 0
    thread_create: 

## Step 309

Apple Development 證書只能用於從 Xcode 調試啟動的 app，直接從 Finder/CLI 啟動會被 macOS 拒絕。需要用 Developer ID Application 或者其他方式繞過。

有，你做一個 xcode.project 我送 archive 這是已知的千法

## Step 316

Translated Report (Full Report Below)
-------------------------------------
Process:             AntiGeinese [4315]
Path:                /private/tmp/*/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
Identifier:          tw.com.saki-store.SakiAntiGeinese
Version:             2.0.11 (2.0.11)
Code Type:           ARM-64 (Native)
Role:                Unspecified
Parent Process:      zsh [4240]
Coalition:           com.AlphaDelta.antigravity [1359]
Responsible Process: AntiGeinese [2897]
User ID:             503

Date/Time:           2026-06-07 16:27:40.1251 +0800
Launch Time:         2026-06-07 16:27:39.8677 +0800
Hardware Model:      iMac21,1
OS Version:          macOS 26.6 (25G5028f)
Release Type:        User

Crash Reporter Key:  328A513C-FB9E-63DF-7D77-FD036139EBD6
Incident Identifier: 547C01FB-9B28-4E93-BEB6-02DF2E8D6432

Time Awake Since Boot: 130000 seconds

System Integrity Protection: disabled

Triggered by Thread: 0, Dispatch Queue: com.apple.main-thread

Exception Type:    EXC_BREAKPOINT (SIGTRAP)
Exception Codes:   0x0000000000000001, 0x0000000110b34858

Termination Reason:  Namespace SIGNAL, Code 5, Trace/BPT trap: 5
Terminating Process: exc handler [4315]


Thread 0 Crashed::  Dispatch queue: com.apple.main-thread
0   Electron Framework            	       0x110b34858 ares_dns_rr_get_ttl + 3407436
1   Electron Framework            	       0x110b34794 ares_dns_rr_get_ttl + 3407240
2   Electron Framework            	       0x10c6dcc50 v8::Script::GetCompileHintsCollector() const + 101476
3   Electron Framework            	       0x110b34910 ares_dns_rr_get_ttl + 3407620
4   Electron Framework            	       0x10cc4d204 v8::Object::WrapGlobal(v8::Isolate*, v8::Local<v8::Object> const&, v8::Object::Wrappable*, v8::CppHeapPointerTag) + 198764
5   Electron Framework            	       0x10e13486c node::PrincipalRealm::tick_callback_function() const + 627504
6   Electron Framework            	       0x10df66934 ElectronMain + 84
7   dyld                          	       0x18fafbe00 start + 6992


Thread 0 crashed with ARM Thread State (64-bit):
    x0: 0x0000000115d8b370   x1: 0x00000130001307d0   x2: 0x0000000000000009   x3: 0x000000018fec0a10
    x4: 0x000000016f671840   x5: 0x0000000000000020   x6: 0x000000000000000a   x7: 0x0000000000000300
    x8: 0x0000000000000000   x9: 0x0000000000000000  x10: 0x0000000000000000  x11: 0x0000000000000002
   x12: 0x0000000000000000  x13: 0x0000000000000000  x14: 0x0000000000000000  x15: 0x0000000000000000
   x16: 0x000000018feb4944  x17: 0x00000001fc9a9ec0  x18: 0x0000000000000000  x19: 0x0000000000000068
   x20: 0x000000016f671e18  x21: 0x000000016f671c18  x22: 0x0000000115cad000  x23: 0x000000016f671c50
   x24: 0x0000000000000002  x25: 0x000000000000004f  x26: 0x0000000113eb365d  x27: 0x0000000000000041
   x28: 0x0000013000130770   fp: 0x000000016f671c00   lr: 0x0000000110b34794
    sp: 0x000000016f6717d0   pc: 0x0000000110b34858 cpsr: 0x60001000
   far: 0x0000000000000000  esr: 0xf2000000 (Breakpoint) brk 0

Binary Images:
       0x10078c000 -        0x10078ffff tw.com.saki-store.SakiAntiGeinese (2.0.11) <4c4c4450-5555-3144-a175-a5a5eb513df3> /private/tmp/*/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
       0x10b588000 -        0x11560ffff com.github.Electron.framework (*) <4c4c4403-5555-3144-a1a9-c4d1d783e6a0> /private/tmp/*/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Electron Framework
       0x1007d0000 -        0x1007e7fff com.github.Squirrel (1.0) <4c4c44b8-5555-3144-a15d-f194c9417c2d> /private/tmp/*/SakiAntiGeinese.app/Contents/Frameworks/Squirrel.framework/Versions/A/Squirrel
       0x100858000 -        0x10089bfff com.electron.reactive (3.1.0) <4c4c445a-5555-3144-a166-7a5e68cf5b14> /private/tmp/*/SakiAntiGeinese.app/Contents/Frameworks/ReactiveObjC.framework/Versions/A/ReactiveObjC
       0x1007f8000 -        0x100803fff org.mantle.Mantle (1.0) <4c4c44f8-5555-3144-a17c-b3f84b6f3c3b> /private/tmp/*/SakiAntiGeinese.app/Contents/Frameworks/Mantle.framework/Versions/A/Mantle
       0x100cd8000 -        0x100eabfff libffmpeg.dylib (*) <4c4c444b-5555-3144-a15c-da7f1e4e481b> /private/tmp/*/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Libraries/libffmpeg.dylib
       0x18fadc000 -        0x18fb822ab dyld (*) <e1c380d2-7409-3641-84e4-0a44aa2f0460> /usr/lib/dyld
               0x0 - 0xffffffffffffffff ??? (*) <00000000-0000-0000-0000-000000000000> ???
       0x18fec0000 -        0x18fec8963 libsystem_platform.dylib (*) <40fe7c10-0df9-3730-b0e7-f761093207e7> /usr/lib/system/libsystem_platform.dylib
       0x18feb3000 -        0x18febfb3b libsystem_pthread.dylib (*) <3aa5cdeb-79d9-3bb0-b5a3-906b7283e492> /usr/lib/system/libsystem_pthread.dylib

External Modification Summary:
  Calls made by other processes targeting this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Cal

## Step 319

All Identifiers
Edit your App ID Configuration

Remove
Save

Platform
iOS, iPadOS, macOS, tvOS, watchOS, visionOS
App ID Prefix
36HPTNN8NU (Team ID)
Description

You cannot use special characters such as @, &, *, "
Bundle ID
tw.com.saki-store.SakiAntiGeinese (explicit)

請照著填

## Step 326

In-App Purchase
	
Increased Debugging Memory Limit
	
Manage Thread Network Credentials (development)
	
MDM Managed Associated Domains
	
Network Extensions
	
Personal VPN

## Step 333

<Command PhaseScriptExecution failed with a nonzero exit code

## Step 346

T參考：：$HOME/...

## Step 358

file://$HOME/...

## Step 364

還是沒圖
'$HOME/... 2026-06-07 16-35-43'

## Step 368

沒圖。
警告只有No App Category is set for target 'SakiAntiGeinese'. Set a category by using the General tab for your target, or by adding an appropriate LSApplicationCategory value to your Info.plist.

## Step 371

整個 resourse 就一行字
// SakiAntiGeinese — Xcode Archive 用 placeholder
// 實際 app 內容由 build-nosign.sh 組裝（Post Build Script）
import Foundation
// This file exists only so Xcode has a compilation target.
// The real app is the Electron-based AntiGeinese, assembled by the post-build script.


你他媽的是會有圖

## Step 435

我知道你們在想什麼狗屁，沒用
opening $HOME/... No such file or directory

## Step 470

Last login: Sun Jun  7 16:05:18 on ttys003
/Applications/SakiAntiGeinese.app/Contents/MacOS/SakiAntiGeinese ; exit;

╭─ OPERATOR at WorkHome in ~ 
╰─❯ /Applications/SakiAntiGeinese.app/Contents/MacOS/SakiAntiGeinese ; exit;                                                   17:05:40 

Saving session...completed.

[程序完成]


-------------------------------------
Translated Report (Full Report Below)
-------------------------------------
Process:             AntiGeinese [13743]
Path:                /Users/USER/*/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
Identifier:          tw.com.saki-store.SakiAntiGeinese
Version:             2.0.11 (2.0.11)
Code Type:           ARM-64 (Native)
Role:                Unspecified
Parent Process:      zsh [13740]
Coalition:           com.AlphaDelta.antigravity [1359]
Responsible Process: AntiGeinese [13493]
User ID:             503

Date/Time:           2026-06-07 17:06:01.1626 +0800
Launch Time:         2026-06-07 17:06:01.0274 +0800
Hardware Model:      iMac21,1
OS Version:          macOS 26.6 (25G5028f)
Release Type:        User

Crash Reporter Key:  328A513C-FB9E-63DF-7D77-FD036139EBD6
Incident Identifier: 59E74E69-5E4D-445F-842E-C596DCEA3781

Time Awake Since Boot: 130000 seconds

System Integrity Protection: disabled

Triggered by Thread: 0, Dispatch Queue: com.apple.main-thread

Exception Type:    EXC_BREAKPOINT (SIGTRAP)
Exception Codes:   0x0000000000000001, 0x0000000112484858

Termination Reason:  Namespace SIGNAL, Code 5, Trace/BPT trap: 5
Terminating Process: exc handler [13743]


Thread 0 Crashed::  Dispatch queue: com.apple.main-thread
0   Electron Framework            	       0x112484858 ares_dns_rr_get_ttl + 3407436
1   Electron Framework            	       0x112484794 ares_dns_rr_get_ttl + 3407240
2   Electron Framework            	       0x10e02cc50 v8::Script::GetCompileHintsCollector() const + 101476
3   Electron Framework            	       0x112484910 ares_dns_rr_get_ttl + 3407620
4   Electron Framework            	       0x10e59d204 v8::Object::WrapGlobal(v8::Isolate*, v8::Local<v8::Object> const&, v8::Object::Wrappable*, v8::CppHeapPointerTag) + 198764
5   Electron Framework            	       0x10fa8486c node::PrincipalRealm::tick_callback_function() const + 627504
6   Electron Framework            	       0x10f8b6934 ElectronMain + 84
7   dyld                          	       0x18fafbe00 start + 6992


Thread 0 crashed with ARM Thread State (64-bit):
    x0: 0x00000001176db370   x1: 0x00000128001308b0   x2: 0x0000000000000009   x3: 0x000000018fec0a10
    x4: 0x000000016da56180   x5: 0x0000000000000020   x6: 0x000000000000000a   x7: 0x0000000000000300
    x8: 0x0000000000000000   x9: 0x0000000000000000  x10: 0x0000000000000000  x11: 0x0000000000000002
   x12: 0x0000000000000000  x13: 0x0000000000000000  x14: 0x0000000000000000  x15: 0x0000000000000000
   x16: 0x000000018feb4944  x17: 0x00000001fc9a9ec0  x18: 0x0000000000000000  x19: 0x0000000000000068
   x20: 0x000000016da56768  x21: 0x000000016da56568  x22: 0x00000001175fd000  x23: 0x000000016da565a0
   x24: 0x0000000000000002  x25: 0x000000000000004f  x26: 0x000000011580365d  x27: 0x0000000000000041
   x28: 0x0000012800130850   fp: 0x000000016da56550   lr: 0x0000000112484794
    sp: 0x000000016da56120   pc: 0x0000000112484858 cpsr: 0x60001000
   far: 0x0000000000000000  esr: 0xf2000000 (Breakpoint) brk 0

Binary Images:
       0x1023a8000 -        0x1023abfff tw.com.saki-store.SakiAntiGeinese (2.0.11) <4c4c4450-5555-3144-a175-a5a5eb513df3> /Users/USER/*/SakiAntiGeinese.app/Contents/MacOS/AntiGeinese
       0x10ced8000 -        0x116f5ffff com.github.Electron.framework (*) <4c4c4403-5555-3144-a1a9-c4d1d783e6a0> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Electron Framework
       0x1023ec000 -        0x102403fff com.github.Squirrel (1.0) <4c4c44b8-5555-3144-a15d-f194c9417c2d> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Squirrel.framework/Versions/A/Squirrel
       0x102500000 -        0x102543fff com.electron.reactive (3.1.0) <4c4c445a-5555-3144-a166-7a5e68cf5b14> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/ReactiveObjC.framework/Versions/A/ReactiveObjC
       0x102414000 -        0x10241ffff org.mantle.Mantle (1.0) <4c4c44f8-5555-3144-a17c-b3f84b6f3c3b> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Mantle.framework/Versions/A/Mantle
       0x102780000 -        0x102953fff libffmpeg.dylib (*) <4c4c444b-5555-3144-a15c-da7f1e4e481b> /Users/USER/*/SakiAntiGeinese.app/Contents/Frameworks/Electron Framework.framework/Versions/A/Libraries/libffmpeg.dylib
       0x18fadc000 -        0x18fb822ab dyld (*) <e1c380d2-7409-3641-84e4-0a44aa2f0460> /usr/lib/dyld
               0x0 - 0xffffffffffffffff ??? (*) <00000000-0000-0000-0000-000000000000> ???
       0x18fec0000 -        0x18fec8963 libsystem_platform.dylib (*) <40fe7c10-0df9-3730-b0e7-f761093207e7> /usr/lib/system/libsystem_platform.dylib
       0x18feb3000 -        0x18febfb3b libs
