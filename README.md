# Achernar Desktop — Internal Beta

**This repository is not the source code.** It exists only to distribute internal beta installers and to power the in-app auto-updater.

> **The source will be released as open source in the near future.** Until then, Achernar Desktop is available to internal testers only. Please do not redistribute the installers outside the test group.

## Copyright and permitted use

**Copyright © 2026 JiuYue0820. All rights reserved for original proprietary portions of Achernar Desktop that are not already covered by another license.**

- Public availability of installers and plans to open-source the project do not, by themselves, grant an open-source license. A future source release will identify its license separately.
- Except where permitted by applicable law, GitHub's Terms of Service, an existing license or written authorization, do not copy, redistribute, resell or publish modified versions of those proprietary portions. Preserve required copyright, author and license notices; do not misrepresent authorship or official affiliation.
- Third-party components and previously licensed code, including MIT-licensed portions, remain governed by their respective licenses. This notice does not revoke or restrict existing permissions.
- This notice concerns copyrightable original expression; it does not claim exclusive rights over general ideas, functionality or independently created implementations. For permission requests or suspected infringement, [open an issue](../../issues) with relevant links and evidence. The rights holder reserves the right to seek remedies available under applicable law.

---

## Download

Grab the latest installer from the [**Releases**](../../releases/latest) page:

| File | Description |
| --- | --- |
| `Achernar-Setup-<version>.exe` | Windows installer (x64). The only file you need. |
| `latest.yml` | Update manifest. Used by the app, not by people. |

**Requirements:** Windows 10 1809 or newer, 64-bit. 4 GB RAM minimum; 8 GB recommended. A dedicated GPU is not required — the app detects low-end hardware and reduces animation cost automatically.

## Installation

1. Download `Achernar-Setup-<version>.exe` from Releases.
2. Run it. Windows SmartScreen will warn about an unknown publisher because the build is not code-signed yet — choose **More info → Run anyway**.
3. Pick an install folder (or accept the default) and finish.
4. Launch **Achernar** from the Start menu or desktop shortcut.

Your settings, sessions and provider keys stay in `%APPDATA%\Achernar` and survive both upgrades and uninstalls.

## Automatic updates

Every packaged build checks this repository for a newer release a few seconds after startup, and again every six hours while the app is running.

- A new version is downloaded in the background and announced in-app.
- Click the notice to restart into the new build.
- If a task is running, the restart waits until it finishes so nothing is lost.
- Updates are served from GitHub Releases with a SHA-512 checksum verified by the updater.

You can disable update checks by setting the environment variable `ACHERNAR_DISABLE_UPDATES=1`.

## Reporting problems

Send the version number shown in **Settings → About** along with:

- What you did, what you expected, what happened.
- A screenshot if the issue is visual.
- Logs from `%APPDATA%\Achernar` when the app fails to start or crashes.

## Version scheme

Internal builds use `0.2.x` for the current beta line. Every published tag is an installable build; there are no source archives here.

---

# Achernar Desktop — 内部测试版

**本仓库不是源代码仓库。** 它只用于分发内测安装包，并为应用内的自动更新提供支持。

> **源代码将在不久后开源。** 在此之前，Achernar Desktop 仅供内部测试人员使用，请不要把安装包转发到测试组之外。

## 版权与使用声明

**版权所有 © 2026 JiuYue0820。Achernar Desktop 尚未通过其他许可证授权的原创专有部分，保留所有权利。**

- 安装包公开可下载、源码计划未来开源，并不等于已经授予开源许可；后续开源以明确发布的许可证为准。
- 除适用法律、GitHub 服务条款、既有许可证或书面授权允许的情形外，不得擅自复制、再分发、转售上述专有部分或发布其修改版本。应保留必要的版权、作者署名和许可声明，不得冒充原创作者或官方发布方。
- 第三方组件及已经按 MIT 等许可证授权的内容，继续遵循各自许可证；本声明不撤销或限制任何既有授权。
- 本声明针对受著作权保护的原创表达，不主张对通用想法、功能或独立创作实现的专有权。授权咨询或疑似侵权反馈，请在本仓库 [提交 Issue](../../issues)，提供相关链接与证据；权利人保留依法寻求救济的权利。

## 下载

从 [**Releases**](../../releases/latest) 页面下载最新安装包：

| 文件 | 说明 |
| --- | --- |
| `Achernar-Setup-<版本号>.exe` | Windows 安装程序（x64），你只需要这一个文件。 |
| `latest.yml` | 更新清单，供应用读取，不需要手动下载。 |

**系统要求：** Windows 10 1809 及以上，64 位。内存最低 4 GB，推荐 8 GB。不要求独立显卡——应用会自动检测低配环境并降低动画开销。

## 安装

1. 在 Releases 页面下载 `Achernar-Setup-<版本号>.exe`。
2. 双击运行。因为当前版本尚未进行代码签名，Windows SmartScreen 会提示"未知发布者"，请选择 **更多信息 → 仍要运行**。
3. 选择安装目录（或使用默认值）并完成安装。
4. 从开始菜单或桌面快捷方式启动 **Achernar**。

你的设置、会话和模型密钥保存在 `%APPDATA%\Achernar`，升级和卸载都不会删除。

## 自动更新

打包版本会在启动几秒后检查本仓库是否有新版本，运行期间每六小时再检查一次。

- 新版本在后台下载完成后会在应用内提示。
- 点击提示即可重启并切换到新版本。
- 如果有任务正在执行，重启会等任务结束后再进行，不会中断。
- 更新包从 GitHub Releases 下载，并经过 SHA-512 校验。

设置环境变量 `ACHERNAR_DISABLE_UPDATES=1` 可以关闭更新检查。

## 反馈问题

请附上 **设置 → 关于** 中显示的版本号，以及：

- 你做了什么、期望的结果、实际发生了什么。
- 如果是界面问题，附上截图。
- 启动失败或崩溃时，附上 `%APPDATA%\Achernar` 中的日志。

## 版本号规则

当前内测线使用 `0.2.x`。每个发布的 tag 都是可安装的构建，本仓库不提供源码压缩包。

---

# Achernar Desktop — 内部ベータ版

**このリポジトリはソースコードではありません。** 内部ベータ版インストーラーの配布と、アプリ内自動アップデートのためだけに存在します。

> **ソースコードは近いうちにオープンソース化されます。** それまでは内部テスター限定です。インストーラーをテストグループ外へ再配布しないでください。

## 著作権と利用に関する声明

**Copyright © 2026 JiuYue0820. Achernar Desktop の独自の専有部分のうち、他のライセンスで既に許諾されていない部分について、すべての権利を留保します。**

- インストーラーの公開や将来のオープンソース化の予定だけでは、オープンソースライセンスは付与されません。ソースを公開する際にライセンスを別途明示します。
- 適用法、GitHub の利用規約、既存のライセンスまたは書面による許諾で認められる場合を除き、上記の専有部分の複製、再配布、転売、改変版の公開は認められません。必要な著作権・著作者・ライセンス表示を保持し、著作者や公式配布元を偽らないでください。
- 第三者のコンポーネントおよび MIT などで既に許諾された部分には、それぞれのライセンスが引き続き適用されます。本声明は既存の許諾を撤回・制限しません。
- 対象は著作権で保護される独自の表現であり、一般的なアイデア、機能、独立して作成された実装の独占権を主張するものではありません。許諾の相談や侵害の疑いは、関連リンクと証拠を添えて [Issue](../../issues) でお知らせください。権利者は適用法に基づく救済を求める権利を留保します。

## ダウンロード

[**Releases**](../../releases/latest) ページから最新のインストーラーを取得してください。

| ファイル | 説明 |
| --- | --- |
| `Achernar-Setup-<バージョン>.exe` | Windows インストーラー（x64）。必要なのはこのファイルだけです。 |
| `latest.yml` | アップデートマニフェスト。アプリが読み取るもので、手動でダウンロードする必要はありません。 |

**動作環境：** Windows 10 1809 以降（64 ビット）。メモリは最低 4 GB、8 GB 推奨。専用 GPU は不要です。アプリが低スペック環境を検出し、アニメーションの負荷を自動で下げます。

## インストール

1. Releases から `Achernar-Setup-<バージョン>.exe` をダウンロードします。
2. 実行します。コード署名がまだ行われていないため、Windows SmartScreen が「不明な発行元」と警告します。**詳細情報 → 実行** を選んでください。
3. インストール先を選択（または既定のまま）して完了します。
4. スタートメニューまたはデスクトップのショートカットから **Achernar** を起動します。

設定・セッション・API キーは `%APPDATA%\Achernar` に保存され、アップデートやアンインストールでも削除されません。

## 自動アップデート

パッケージ版は起動から数秒後にこのリポジトリを確認し、その後も 6 時間ごとに新しいリリースを確認します。

- 新しいバージョンはバックグラウンドでダウンロードされ、アプリ内で通知されます。
- 通知をクリックすると再起動して新しいビルドに切り替わります。
- タスク実行中は、処理が終わるまで再起動を待機するため、作業内容は失われません。
- 更新ファイルは GitHub Releases から取得され、SHA-512 で検証されます。

環境変数 `ACHERNAR_DISABLE_UPDATES=1` を設定すると、アップデート確認を無効にできます。

## 問題の報告

**設定 → バージョン情報** に表示されるバージョン番号と、以下を添えてください。

- 行った操作、期待した結果、実際に起きたこと。
- 表示の問題であればスクリーンショット。
- 起動失敗やクラッシュの場合は `%APPDATA%\Achernar` 内のログ。

## バージョン規則

現在の内部ベータは `0.2.x` 系列です。公開されるタグはすべてインストール可能なビルドで、ソースアーカイブは含まれません。

---

<sub>Achernar Desktop · internal beta channel · installers only, source withheld until public release</sub>
