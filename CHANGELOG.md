# CHANGELOG

## [v1.9.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.9.0) - 2025-07-07 18:22:25

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.9.0

### Feature

- general:
  - add PR comment if scan is clean ([370d8a0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/370d8a085f04a49ec5f8e55a5478feb569fa273e))

### Bug Fixes

- general:
  - revert back to v1.6.3 ([9493657](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/9493657f7cfb75c6677993f40d358e518907612a))
  - change findings to a file instead of env variable ([1be9151](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/1be915185304eafbf7e30f735c2c0dae2f872f6d))
  - add logic to email on failed scan ([5ddf619](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/5ddf61984473511e529b91049424c1ab82a3bdb6))
  - allow notifications on different scans ([ce41b1e](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/ce41b1eda5b7d01eaf8cea26743e7669bced39f3))
  - add notification step on supplemtary scans ([8a9c8f1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/8a9c8f15168fc34843e9ef88523aa325f00f46c4))
  - fix the alert environment variable ([c30e5f0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/c30e5f0717e7da7c8372ea59b84ed3512344ff1c))
  - fix error on main scan ([c04373d](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/c04373db6172cae01858e9ed8c52fa97552590e0))
  - add filescan to help pickup more obscure secrets ([ef29e23](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/ef29e23d4d98ee89fe1294b390425ab0df387beb))
  - remove regex patterns ([f33c500](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/f33c500b60b0dbe36f68e54e4d337ddd8e26ac21))
  - add more depth to main push scans ([b2aab9d](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/b2aab9daf9ffdcaa8e93f61e8f178854a7d31b48))

### Miscellaneous


- bot:
  - update files for Release v1.8.0. ([b92f701](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/b92f7016a79ec0f4c76ecdf5961f1e321e208c35))

## [v1.8.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.8.0) - 2025-07-03 13:52:45

## [v1.7.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.7.0) - 2025-07-02 19:35:40

## [v1.6.6](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.6.6) - 2025-07-02 19:33:33

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.6.6

### Bug Fixes

- general:
  - remove include-patterns command ([3829c50](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/3829c50bc180e74b77097c400d5dc020e74024c3))

### Miscellaneous


- bot:
  - update files for Release v1.6.5. ([d76b892](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/d76b8926e7184f70cc135f99c5c6b50f45944a11))

## [v1.6.5](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.6.5) - 2025-07-02 19:30:56

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.6.5

### Bug Fixes

- general:
  - add common base64 key headers to parameters (#7) ([77c9ca6](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/77c9ca60602520641c82c1c6a39678e88747fc22)) ([#7](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/pull/7))

### Miscellaneous


- bot:
  - update files for Release v1.6.4. ([7df7916](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/7df7916cfac0b80c67008b5e5638f6312d17203d))
  - update files for Release v1.6.3. ([45567c8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/45567c86207890884d2de9130c28968afe42a9f1))

## [v1.6.3](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.6.3) - 2025-06-19 18:14:45

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.6.3

### Bug Fixes

- general:
  - change error handling for reversed commits ([e42b2c8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/e42b2c8c327c8ec9a59bf09aa56743b5fe0759bb))

### Miscellaneous


- bot:
  - update files for Release v1.6.2. ([eae1011](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/eae10116e917e6601df84bb7d475200713b7776d))

## [v1.6.2](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.6.2) - 2025-06-19 18:11:08

## [v1.6.1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.6.1) - 2025-06-18 17:40:59

## [v1.6.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.6.0) - 2025-06-05 15:29:08

## [v1.5.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.5.0) - 2025-06-04 14:41:43

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.5.0

### Feature

- general:
  - add action annotations ([59aa950](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/59aa950b53061e4302c1443560686f0c1108d47c))
  - scan whole branch and add readme ([f93abd8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/f93abd81b4d225f74417433830498d951008679b))

### Bug Fixes

- general:
  - populate email with findings on main push ([14790a2](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/14790a24aa17ecd7a59fb5c9fbc11510fa91ab96))
  - fix not sending alerts when finding found ([3324593](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/3324593f25a7fb3647008673fbc350361a7d74f4))
  - fix details passed to email when unverified secret ([d981148](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/d9811483fd34bc9612b78d9e655f2edba8e4d49f))
  - scan deeper in commits on main push ([98e94cb](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/98e94cbe5b4b82c7234fb554b51439e262162ff5))
  - fix yaml formatting ([18d2d11](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/18d2d11f057a6d6bbf8ed0b1dd8a156a55c79f26))
  - only alert if we did not delete the finding ([76dbd8d](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/76dbd8dd22c48d3b33c52201fe92ceecc6f91bce))
  - fix no line number when only 1 finding ([47d98cf](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/47d98cfda8a1fbcbc6a38286e005ce88e0d266dc))
  - change to only scan current files on PR ([a3c85ba](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/a3c85baa842e3ba946adbe945ff67097418ba02c))
  - remove duplicate args ([e5b7c25](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/e5b7c25d751115636e6e80c2fe95a37ba9a96670))
  - remove since commit flag ([1472293](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/14722937748eb153e980d0c19b6fed475d79e9c3))
  - only scan changed files on the PR ([2e682e4](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/2e682e4a2d428bf1f91521927dcf7923c5a74200))
  - scan entire branch ([b817359](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/b817359f8fd739bffe1b273fef58a6da8fa9a1bf))
  - make links a list on email ([8780d31](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/8780d3178e9770d36575ec684920f4fabd63facb))
  - ternary operator #3 ([c854204](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/c85420446bc145c92f492c2f05af530e5e193be7))
  - ternary operator again ([2b4e189](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/2b4e18997e1c22958646f94a2494f1995cae1010))
  - fix ternary operator in email ([80f0d96](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/80f0d969c5141f2d6039946798dca2d2184ecfe5))

### Miscellaneous


- general:
  - update usage on readme ([aab024f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/aab024f4ebc42391412d9ed0f674498678c711fb))
  - update Readme ([d593e2c](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/d593e2c64a922ac2ea8a66a44c8d15755998ebfb))
  - add commit date to annotations on main push ([5f913f9](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/5f913f97da4fd1fbafc7d073893d6feae194daaf))
  - change error annotation to warning ([95c17c0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/95c17c0474c64cc648dd7d2696b9fb51863d32ff))
  - move commit details to finding details ([7ae8124](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/7ae8124f164ed18d03cb11e6e9ea76f0313730f6))
  - add more details about commits to email ([8e2f96f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/8e2f96f766102ee079046deccab39ee4072487ae))
  - replace official github action with docker version ([1ebec50](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/1ebec503058cfce1ed1fe190b289a0c98fdb3efe))
  - make important links section look less blocky ([7720629](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/7720629287f8d484f04d4d2aeb158fa060624825))
  - revert to original template for email ([907302d](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/907302dfa610cd5fe256527c6d6356ec8e6f1337))
  - make email more modern ([4aea74d](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/4aea74d1cce3197b530ac8ab62cd198bee437734))

- bot:
  - update files for Release v1.4.1. ([1a0df43](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/1a0df43708153d003242fd2e38000c21e0526910))

## [v1.4.1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.4.1) - 2025-06-03 17:39:22

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.4.1

### Feature

- general:
  - add more detail about type of run to email ([12cc7ce](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/12cc7ced6ad135a3a78ecbf994568cd3a8d25113))

### Bug Fixes

- general:
  - fix reference in email for type ([706ae0c](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/706ae0c8a5cf508e046f1328c0699740a80836f2))

### Miscellaneous


- general:
  - change formatting ([1160cd8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/1160cd8d9462361193dfcebdc039c6e42819e146))

- bot:
  - update files for Release v1.4.0. ([6f8151b](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/6f8151b08f2327e73fc40e91f91f69a4d2fcdcd9))

## [v1.4.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.4.0) - 2025-06-03 15:53:45

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.4.0

### Feature

- general:
  - add more deatil to email ([53ee6c8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/53ee6c86d77068e41d5b7db67dd6be8b554f9362))
  - add more details to message ([ab7a2a1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/ab7a2a12233426dc1bf280e25135bad15665b2f5))

### Bug Fixes

- general:
  - make action run with normal github action output ([2e4a8da](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/2e4a8da33b3c7b35455e242d51b234b9c0654705))
  - add more details to logs ([93342dd](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/93342dd79a043ee53ffe4635b6f91f626412c91c))
  - change heredoc formatting ([284676c](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/284676cb4b7c6aa90a2371ba83974931b7c58395))
  - remove second run of trufflehog ([41cce9f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/41cce9f1bfed33cbad7b9be1be4197386ec5cf4a))
  - change for url error again ([9f4c82f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/9f4c82f11c34692c5d0ebc8a24996d9c488dfc25))
  - change for github url error ([f2f73f2](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/f2f73f28446b6fc94be65f1f4c0cc84f42e846f0))
  - change extra arugments for cli run ([5ecfeab](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/5ecfeab8824ff80353275e264c9a48a1668d3d6d))
  - run local install of trufflehog if action find secret ([ac1777e](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/ac1777ea4be72eb94ff6ee3128ac9dead0ad17a9))
  - change to grab output better ([cbdb504](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/cbdb504191651c70c9b0d239168e90b7dd287417))
  - fix grabbing outputted found secrets ([dfd4ab9](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/dfd4ab9cec88679a5407d2fddfb87c6c65563228))
  - fix grabbing secret output ([2c5dd4e](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/2c5dd4e8ad575555141c4eadf9f7304a4197839a))

### Miscellaneous


- bot:
  - update files for Release v1.3.3. ([98fa066](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/98fa066905d671696005261c7f5ce565ef5f65a9))

## [v1.3.3](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.3.3) - 2025-06-03 14:26:42

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.3.3

### Bug Fixes

- general:
  - continue on error ([e05f33e](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/e05f33e3ab279f131fe57343e1cc2028d98c3467))

### Miscellaneous


- bot:
  - update files for Release v1.3.2. ([9a23b1c](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/9a23b1cf79bed4582072dc1a0b008e51b3e1d07a))

## [v1.3.2](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.3.2) - 2025-06-03 14:17:36

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.3.2

### Miscellaneous


- bot:
  - update files for Release v1.3.1. ([5b99395](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/5b9939554cc03cf213072920d0b750433855136e))

## [v1.3.1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.3.1) - 2025-06-03 14:15:00

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.3.1

### Bug Fixes

- general:
  - remove > from extra_args ([5da6199](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/5da6199c75c5f3c250a71afec8283fe922d8ee80))

### Miscellaneous


- bot:
  - update files for Release v1.3.0. ([cb736c8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/cb736c8c38c8ad8166a33bd2b91b9dc3e5c291a7))

## [v1.3.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.3.0) - 2025-06-03 14:06:12

## [v1.2.1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.2.1) - 2025-06-03 13:38:12

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.2.1

### Miscellaneous


- bot:
  - update files for Release v1.2.0. ([310defc](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/310defccbbb72b5e530b13ae6244be53557e572e))

## [v1.2.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.2.0) - 2025-06-03 13:21:53

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.2.0

### Feature

- general:
  - add shallow cloning and github actions arguments ([6f776b8](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/6f776b8e3ecb9cc43f1b6996581b414a41ec6732))

### Miscellaneous


- bot:
  - update files for Release v1.1.5. ([9e8456d](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/9e8456dbf79820e5302a739ad7965becddd20f78))

## [v1.1.5](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.1.5) - 2025-06-02 19:06:24

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.1.5

### Bug Fixes

- general:
  - replace html code ([469651a](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/469651afcf8400f4ed7963cc032eb798c6d98560))

### Miscellaneous


- bot:
  - update files for Release v1.1.4. ([bab45a0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/bab45a0a7626e506c187fd530f9c50cafea4ff60))

## [v1.1.4](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.1.4) - 2025-06-02 18:42:16

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.1.4

### Bug Fixes

- general:
  - manually create file ([c6de00b](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/c6de00b1c71e5ee099d3349465f1d9f89a52ee1e))

### Miscellaneous


- bot:
  - update files for Release v1.1.3. ([8ba779f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/8ba779f79884ab893c3755e6711d463fe5099f62))

## [v1.1.3](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.1.3) - 2025-06-02 18:37:30

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.1.3

### Miscellaneous


- bot:
  - update files for Release v1.1.2. ([921b47f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/921b47f46792ec914360e345bfc08225cf204209))

## [v1.1.2](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.1.2) - 2025-06-02 18:34:10

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.1.2

### Miscellaneous


- bot:
  - update files for Release v1.1.1. ([30fb2b1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/30fb2b14635f5ab8cdf5591645a8cc144bef2259))

## [v1.1.1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.1.1) - 2025-06-02 18:32:07

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.1.1

### Miscellaneous


- bot:
  - update files for Release v1.1.0. ([58acdf9](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/58acdf930bd105b6b0fe230c818319bd99e65cc0))

## [v1.1.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.1.0) - 2025-06-02 18:31:05

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.1.0

### Feature

- general:
  - add html email format ([4d60987](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/4d609874a4aac6078959f17525bf5c70c46b506d))

### Miscellaneous


- bot:
  - update files for Release v1.0.5. ([f0e1a87](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/f0e1a8749134a8bb48dd01755f3b46fe8fa0c94e))

## [v1.0.5](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.0.5) - 2025-06-02 15:48:23

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.0.5

### Bug Fixes

- general:
  - change from email ([5466501](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/54665011bf99898ec91442b99d04fb3d97584938))

### Miscellaneous


- bot:
  - update files for Release v1.0.4. ([b039fa5](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/b039fa501b85567e4dc20f25dd12b0a16dc17322))

## [v1.0.4](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.0.4) - 2025-06-02 14:59:42

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.0.4

### Bug Fixes

- general:
  - remove base and head inputs ([54a9491](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/54a94915752fa4d00e767a8972b8e7dbddcd873a))

### Miscellaneous


- bot:
  - update files for Release v1.0.3. ([b50f6f0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/b50f6f066690eb19ec378721b6ebf974ffa71df6))

## [v1.0.3](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.0.3) - 2025-06-02 14:43:30

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.0.3

### Bug Fixes

- general:
  - change action url to use ([704c451](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/704c45128733b273cdcce279d8757fe4b370c792))

### Miscellaneous


- bot:
  - update files for Release v1.0.2. ([04d7d0f](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/04d7d0fb859b1d0b9f46c250b15ad51a7b47c232))

## [v1.0.2](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.0.2) - 2025-06-02 14:38:13

## [v1.0.1](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.0.1) - 2025-06-02 14:31:22

**Full Changelog**: https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/compare/v1...v1.0.1

### Bug Fixes

- general:
  - properly spell FOUNDATION ([f88a979](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/f88a97910687d0dd818961da591bc90194b43d5b))
  - change readme ([370fd3e](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/370fd3e50975b9df388b0c0c6bb1de5dfa1b61d9))

### Miscellaneous


- bot:
  - update files for Release v1.0.0. ([1c4d8cd](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/commit/1c4d8cdf483073b3a9f0b020b60f04a69b616d18))

## [v1.0.0](https://github.com/sdi-one-foundation/trufflehog-secret-sniffer-action/releases/tag/v1.0.0) - 2025-06-02 14:23:20

\* *This CHANGELOG was automatically generated by [auto-generate-changelog](https://github.com/BobAnkh/auto-generate-changelog)*
