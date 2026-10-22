# Hive browser account admission

<!-- 561-group-standards:badges:start -->
[![Red Cup Engineering](https://img.shields.io/badge/561%20Group-Red%20Cup%20Engineering-c0392b)](https://github.com/red-cup-engineering)
[![License: MIT](https://img.shields.io/badge/license-MIT-c0392b)](LICENSE)
[![Indigenous data: CARE](https://img.shields.io/badge/Indigenous%20data-CARE-4b6f44)](https://github.com/red-cup-engineering/.github/blob/main/GOVERNANCE.md)
[![Tips welcome](https://img.shields.io/badge/tips-welcome-d4a017)](https://github.com/561-group/.github/blob/main/TIPS.md)
<!-- 561-group-standards:badges:end -->

`createHiveLoginApp` supplies login and callback resources for a host's existing browser session. The host supplies its representations, registry, cookies and state directory. The signed challenge binds application, account and nonce; the persisted nonce is consumed once, and valid account-key proof does not bypass the host registry.

This is Hive account admission, not canonical Actor association, Board budget admission, hiring authority or transaction authorization. Signature verification currently checks live key membership across two RPC nodes; it does not establish a general weighted or delegated Hive authority evaluation.

Source recovered from Bare Cedar Fog at c677e9999ea05bf577f9355660687e56dffd3da9. The browser admission demonstration uses a disposable signing key, two fixture RPC responses and an actual temporary nonce file. It exercises refusal of an unadmitted account, admitted session establishment and replay refusal. Live host migration remains unfinished.
