# Changelog

## [2.5.0](https://github.com/YuanYuYuan/toggleterm.nvim/compare/v2.10.0...v2.5.0) (2024-04-07)


### ⚠ BREAKING CHANGES

* switch persist_mode to false ([#410](https://github.com/YuanYuYuan/toggleterm.nvim/issues/410))
* **colors:** use api.nvim_get_hl_by_name
* this increases the minimum versions required to nvim 0.7
* allow global config of on_exit(), on_stdout(), on_stderr() ([#162](https://github.com/YuanYuYuan/toggleterm.nvim/issues/162))
* Replace 2 toggleterm command i.e. ToggleTermOpenAll and ToggleTermCloseAll with a single command that toggle all terminal.

### Features

* "row" and "col" can be given as function ([#343](https://github.com/YuanYuYuan/toggleterm.nvim/issues/343)) ([#347](https://github.com/YuanYuYuan/toggleterm.nvim/issues/347)) ([8c12749](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8c12749d74b9ce27197ec659dc54869a09ddff60))
* add "float" display option ([#23](https://github.com/YuanYuYuan/toggleterm.nvim/issues/23)) ([5bb328f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5bb328f139f7bd43cbecd2158d9e60f6c2ff56ef))
* add `Terminal.find` function ([#486](https://github.com/YuanYuYuan/toggleterm.nvim/issues/486)) ([01a84bc](https://github.com/YuanYuYuan/toggleterm.nvim/commit/01a84bc642484681933140537c3ff99b10b8a866))
* add a terminal select command ([#429](https://github.com/YuanYuYuan/toggleterm.nvim/issues/429)) ([c8574d7](https://github.com/YuanYuYuan/toggleterm.nvim/commit/c8574d7a7d2e5682de4479463ddba794390c0e40))
* add api to spawn tasks without opening a window ([#218](https://github.com/YuanYuYuan/toggleterm.nvim/issues/218)) ([b82ef23](https://github.com/YuanYuYuan/toggleterm.nvim/commit/b82ef23b2b4172e0ced173f5d12d4ee1edada7d1))
* add close on exit ([#32](https://github.com/YuanYuYuan/toggleterm.nvim/issues/32)) ([1a52426](https://github.com/YuanYuYuan/toggleterm.nvim/commit/1a52426c2f9bb9cdb587dc32fe06a68e570806cb))
* add close_on_exit field to the Terminal class ([#72](https://github.com/YuanYuYuan/toggleterm.nvim/issues/72)) ([4dcdca2](https://github.com/YuanYuYuan/toggleterm.nvim/commit/4dcdca29cc6d7c83f09f3669ab83358ef29e79b3))
* add command completion to TermExec and ToggleTerm ([#256](https://github.com/YuanYuYuan/toggleterm.nvim/issues/256)) ([b8bb778](https://github.com/YuanYuYuan/toggleterm.nvim/commit/b8bb778192285d9f5bcab6d4cc464fa5d53ea766))
* add desc property to key mappings ([#337](https://github.com/YuanYuYuan/toggleterm.nvim/issues/337)) ([3ba6838](https://github.com/YuanYuYuan/toggleterm.nvim/commit/3ba683827c623affb4d9aa518e97b34db2623093))
* add name param to ToggleTerm and TermExec ([#479](https://github.com/YuanYuYuan/toggleterm.nvim/issues/479)) ([81ea9f7](https://github.com/YuanYuYuan/toggleterm.nvim/commit/81ea9f71a3fd7621fd02b2c74861595378a3c938))
* add option to always open terminal in insert ([d3b57e9](https://github.com/YuanYuYuan/toggleterm.nvim/commit/d3b57e915315ed3c3f42ab079a600730c8b4f6fb))
* add shortcut for opening terminal at git dir ([200ab54](https://github.com/YuanYuYuan/toggleterm.nvim/commit/200ab543c90bbe8e99f4e8c845db5caac81b6685))
* add single toggle all command ([#107](https://github.com/YuanYuYuan/toggleterm.nvim/issues/107)) ([de9a2ef](https://github.com/YuanYuYuan/toggleterm.nvim/commit/de9a2ef88e18e109744b94ea230bcc26c7232ffa))
* add terminal_mappings option ([#149](https://github.com/YuanYuYuan/toggleterm.nvim/issues/149)) ([882489f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/882489f4ebe4f8379016a453f508965f08ce1a86))
* add ToggleTerm{Open|Close}All commands ([#49](https://github.com/YuanYuYuan/toggleterm.nvim/issues/49)) ([0ea3484](https://github.com/YuanYuYuan/toggleterm.nvim/commit/0ea34845668065e34db785109253f76cea373375))
* add ToggleTermSetName command ([#272](https://github.com/YuanYuYuan/toggleterm.nvim/issues/272)) ([9db6f98](https://github.com/YuanYuYuan/toggleterm.nvim/commit/9db6f98af4f700945cff0f4f34b92ec80ab67a2b))
* allow changing terminal dir in background ([#438](https://github.com/YuanYuYuan/toggleterm.nvim/issues/438)) ([f5cf0b1](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f5cf0b1eebd95ba4edc69e2fbd13e1a289048d5d))
* allow expanding vim wildcards in cmd ([#38](https://github.com/YuanYuYuan/toggleterm.nvim/issues/38)) ([5bf694f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5bf694fce51f0711e3e005e105992178d87a86c6))
* allow global config of on_exit(), on_stdout(), on_stderr() ([#162](https://github.com/YuanYuYuan/toggleterm.nvim/issues/162)) ([a3f4235](https://github.com/YuanYuYuan/toggleterm.nvim/commit/a3f4235453b7b53c7037baac7eb4124af3e8d0b4))
* allow operator mapping to send to terminal ([#507](https://github.com/YuanYuYuan/toggleterm.nvim/issues/507)) ([5b84866](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5b848664989b6deb2c28dad5135c89720915675a))
* **config:** allow `shell` parameter to be a function ([#423](https://github.com/YuanYuYuan/toggleterm.nvim/issues/423)) ([a7857b6](https://github.com/YuanYuYuan/toggleterm.nvim/commit/a7857b6cbfdfc98df2a7b61591be16e1020c7a82))
* delay module requires ([c9c09be](https://github.com/YuanYuYuan/toggleterm.nvim/commit/c9c09bea3ffbafd3f837ddc675cfcb1d3c41929b))
* dynamic resize float terms([#186](https://github.com/YuanYuYuan/toggleterm.nvim/issues/186)) ([6dfe443](https://github.com/YuanYuYuan/toggleterm.nvim/commit/6dfe4438c59f57e0cbefad52eeb73f0d03661baf))
* enable auto-scroll on stdout/stderr ([#285](https://github.com/YuanYuYuan/toggleterm.nvim/issues/285)) ([8719396](https://github.com/YuanYuYuan/toggleterm.nvim/commit/871939685275f3ba4ad9c4a7479858f60c6e4bd4))
* enable title for floating terminals ([#534](https://github.com/YuanYuYuan/toggleterm.nvim/issues/534)) ([d3aa6e8](https://github.com/YuanYuYuan/toggleterm.nvim/commit/d3aa6e88c2dcbefd240ffb77a2c77b486a19fa5f))
* expand `self.dir` before opening a `Terminal` ([#58](https://github.com/YuanYuYuan/toggleterm.nvim/issues/58)) ([8271a10](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8271a10cfe6a0e666f2b571338c69c873972c7e2))
* Force close terminals via ToggleTermToggleAll ([#113](https://github.com/YuanYuYuan/toggleterm.nvim/issues/113)) ([265bbff](https://github.com/YuanYuYuan/toggleterm.nvim/commit/265bbff68fbb8b2a5fb011272ec469850254ec9f))
* hide numbers in terminal buffer ([2c54f8c](https://github.com/YuanYuYuan/toggleterm.nvim/commit/2c54f8c73c4d2c9a115691a9518262dcdaac0c71))
* **highlights:** allow adding custom highlights ([#166](https://github.com/YuanYuYuan/toggleterm.nvim/issues/166)) ([37b2527](https://github.com/YuanYuYuan/toggleterm.nvim/commit/37b2527b4c79704639922d7c11a8c8134a3593fa))
* open last toggled term on smart toggle ([#397](https://github.com/YuanYuYuan/toggleterm.nvim/issues/397)) ([42438b3](https://github.com/YuanYuYuan/toggleterm.nvim/commit/42438b30421035753ea86d5ec1a36d88019d5bac))
* pass on_close option from setup ([#137](https://github.com/YuanYuYuan/toggleterm.nvim/issues/137)) ([f2239cb](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f2239cb5e3a31d5e38a1fe65887c87934d502e31))
* pass on_open option from setup ([#131](https://github.com/YuanYuYuan/toggleterm.nvim/issues/131)) ([ed319ba](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ed319baf2552687f1d959202986042c11abb0788))
* persist terminal mode ([#245](https://github.com/YuanYuYuan/toggleterm.nvim/issues/245)) ([ce755e3](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ce755e3a07f2464287dc60ed448fdbbe6ea157f5))
* restore terminal view on smart toggle ([#399](https://github.com/YuanYuYuan/toggleterm.nvim/issues/399)) ([a5638b2](https://github.com/YuanYuYuan/toggleterm.nvim/commit/a5638b2206c3930a16a24e5c184dddd572f8cd34))
* send line(s) to the terminal ([#185](https://github.com/YuanYuYuan/toggleterm.nvim/issues/185)) ([d0ae5de](https://github.com/YuanYuYuan/toggleterm.nvim/commit/d0ae5de89fbe744a5f89f027fe2ae13e761f0231))
* support both cmd and powershell(pwsh) for windows ([#96](https://github.com/YuanYuYuan/toggleterm.nvim/issues/96)) ([8a56b0b](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8a56b0bb6047d1fb0d5bb5f0b3cfffbff87328b3))
* support sending commands without opening window ([#87](https://github.com/YuanYuYuan/toggleterm.nvim/issues/87)) ([08744f8](https://github.com/YuanYuYuan/toggleterm.nvim/commit/08744f8bd46b3f6dd5cbfa8ed6287cbe32af29ab))
* support z-index option for floating windows ([#418](https://github.com/YuanYuYuan/toggleterm.nvim/issues/418)) ([0aa9364](https://github.com/YuanYuYuan/toggleterm.nvim/commit/0aa936445b895cd5d3387860f96ce424ce32b072))
* switch persist_mode to false ([#410](https://github.com/YuanYuYuan/toggleterm.nvim/issues/410)) ([98e15df](https://github.com/YuanYuYuan/toggleterm.nvim/commit/98e15df2c838fe5c3cae1efa36fa5c255fc75aa8))
* **term:** add autochdir to track nvim's CWD ([6dcdad0](https://github.com/YuanYuYuan/toggleterm.nvim/commit/6dcdad0b9815f28b6e6299767edd4fbefa7e5d9a)), closes [#304](https://github.com/YuanYuYuan/toggleterm.nvim/issues/304)
* **terminal:** add `on_create` function ([#335](https://github.com/YuanYuYuan/toggleterm.nvim/issues/335)) ([fa5646f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/fa5646fd35b15d5aa741733a8991a84978bd5d60))
* **terminal:** add mechanism to fetch last focused terminal ([#411](https://github.com/YuanYuYuan/toggleterm.nvim/issues/411)) ([bfb7a72](https://github.com/YuanYuYuan/toggleterm.nvim/commit/bfb7a7254b5d897a5b889484c6a5142951a18b29))
* **terms:** delete internal term resources on shutdown. ([#234](https://github.com/YuanYuYuan/toggleterm.nvim/issues/234)) ([5bf839a](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5bf839a558bf313fdbbe44824bcf3c4fe60502d0))
* **toggleterm:** add a simple winbar to show terminal data ([#229](https://github.com/YuanYuYuan/toggleterm.nvim/issues/229)) ([9150581](https://github.com/YuanYuYuan/toggleterm.nvim/commit/91505816335a93b10f026409228aef5e8d48e6d9))
* **ui:** fix leaking winhighlight (on nightly) ([00d2645](https://github.com/YuanYuYuan/toggleterm.nvim/commit/00d26454e2fe0d7f5a8e90ea62b50e029aeb9be7))
* update send visual selection ([#239](https://github.com/YuanYuYuan/toggleterm.nvim/issues/239)) ([50f88d3](https://github.com/YuanYuYuan/toggleterm.nvim/commit/50f88d316261bfe56854cb75b9d092061c38b21e))
* **utils:** add notify helper ([3dc3ef8](https://github.com/YuanYuYuan/toggleterm.nvim/commit/3dc3ef8b802b6423f63123b45ea8b90b3a2bf8ec))


### Bug Fixes

* **#487:** avoid terminal id collisions in __add ([#490](https://github.com/YuanYuYuan/toggleterm.nvim/issues/490)) ([6bec54e](https://github.com/YuanYuYuan/toggleterm.nvim/commit/6bec54e73807919b15fc92824fb48be32fb7e8ea))
* add missing self:on_create() to Terminal:spawn() ([#378](https://github.com/YuanYuYuan/toggleterm.nvim/issues/378)) ([a54e6c4](https://github.com/YuanYuYuan/toggleterm.nvim/commit/a54e6c471ce1cd8ef8357e34598a28a955297131))
* allow specifying size and cmd for TermExec ([5d7b24e](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5d7b24ecf9c95dddab59dbcaee7cdd8fe5d736a2))
* allow tab direction in empty buffers ([5f9ba91](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5f9ba91157a25be5ee7395fbc11b1a8f25938365)), closes [#95](https://github.com/YuanYuYuan/toggleterm.nvim/issues/95)
* change predicate and reassign table of available ids ([802e258](https://github.com/YuanYuYuan/toggleterm.nvim/commit/802e258d576dfa2b6d95cf640088d1715738e556))
* check that a directory is valid before using it ([#293](https://github.com/YuanYuYuan/toggleterm.nvim/issues/293)) ([6673a8f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/6673a8f2fd2a9c0ed09b9951298093d14ba0445a))
* **ci:** move ignore comments ([db8392f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/db8392f3c1df47de08ce3779aa171ebac12cdbb0))
* close float windows on WinLeave ([8f2e78d](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8f2e78d0256eba4896c8514aa150e41e63f7d5b2)), closes [#246](https://github.com/YuanYuYuan/toggleterm.nvim/issues/246)
* **colors:** apply terminal highlights more consistently ([#231](https://github.com/YuanYuYuan/toggleterm.nvim/issues/231)) ([c525442](https://github.com/YuanYuYuan/toggleterm.nvim/commit/c525442a03b7bb229c48874abf53168eb38c5b9b))
* **commandline.lua:** improve shellslash check ([981e207](https://github.com/YuanYuYuan/toggleterm.nvim/commit/981e207e17ecd8bf065b5b9201c1d6d2395e9338)), closes [#110](https://github.com/YuanYuYuan/toggleterm.nvim/issues/110)
* **commands:** call ToggleTermSetName with count ([#497](https://github.com/YuanYuYuan/toggleterm.nvim/issues/497)) ([ef1bbff](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ef1bbff59c9ab5b468062c33ca183541a3849547)), closes [#496](https://github.com/YuanYuYuan/toggleterm.nvim/issues/496)
* **config:** config.highlights should respect prefs ([#197](https://github.com/YuanYuYuan/toggleterm.nvim/issues/197)) ([e62008f](https://github.com/YuanYuYuan/toggleterm.nvim/commit/e62008fe5879eaecb105eb81e393f87d4607164c))
* **config:** only set winbar winhighlight on nightly ([0c1dc87](https://github.com/YuanYuYuan/toggleterm.nvim/commit/0c1dc87fa9779a3de8d33acf1253b1ca88be25d5))
* **config:** set default float winblend to 0 ([ef7a882](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ef7a882a818d1bf2598bc58ca0bc158d097d499d))
* **config:** use correct colours for terminal hls ([3c79039](https://github.com/YuanYuYuan/toggleterm.nvim/commit/3c7903924d7e3f16375a760d1db0a7829ae036a9))
* create terminal with called ID if not found ([#163](https://github.com/YuanYuYuan/toggleterm.nvim/issues/163)) ([a568cd4](https://github.com/YuanYuYuan/toggleterm.nvim/commit/a568cd4defb710dfb41e427b936f2e7e6e63bbd7))
* delay getting term directory till spawn ([ffe9a7e](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ffe9a7e44d888f6f745e532a5aace8547e176ef0))
* delete buffer on process exit ([#44](https://github.com/YuanYuYuan/toggleterm.nvim/issues/44)) ([9215c19](https://github.com/YuanYuYuan/toggleterm.nvim/commit/9215c1955c30b08779bcf1043964a49a9aaf0da8))
* determine custom terminal ids on spawn ([#488](https://github.com/YuanYuYuan/toggleterm.nvim/issues/488)) ([8572917](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8572917413dd039d1a53b007df5c571e2a3b8ad7))
* don't return a table if no config key found ([863ac0b](https://github.com/YuanYuYuan/toggleterm.nvim/commit/863ac0b85221b29b5ddbc3d8ebe113850d548e06))
* don't throw window error on bufdelete ([d92c01d](https://github.com/YuanYuYuan/toggleterm.nvim/commit/d92c01d4371fd2be106a2086039e5e8fe201981d)), closes [#64](https://github.com/YuanYuYuan/toggleterm.nvim/issues/64)
* don't try to close the last tab ([#267](https://github.com/YuanYuYuan/toggleterm.nvim/issues/267)) ([ce1dbb4](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ce1dbb49ff64219a2fccf8566a36974f83be495d))
* ensure terminals are deleted correctly when multiple open ([#264](https://github.com/YuanYuYuan/toggleterm.nvim/issues/264)) ([8e6f938](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8e6f938ed8eec7f988dc07aec2af148ad57c6d95))
* ensure window/buffer before validity check ([46c1eee](https://github.com/YuanYuYuan/toggleterm.nvim/commit/46c1eee4bbee55d1a739b322a0f32ae9176bd006))
* **exec:** don't presume that the start id is 1 ([53134b0](https://github.com/YuanYuYuan/toggleterm.nvim/commit/53134b08a5a5e66f343c4e431966a0a19ce2d162))
* **float:** close window if it loses focus ([7e13134](https://github.com/YuanYuYuan/toggleterm.nvim/commit/7e13134c7e252746586ccb35a535c42a1c3b07c4))
* **float:** ensure sidescroll is zero ([43b75f4](https://github.com/YuanYuYuan/toggleterm.nvim/commit/43b75f43aa7590228d88945525c737f0ddc05c22))
* guess the direction of resurrected terms ([8c4da4a](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8c4da4a877a0eb49d40fed30c4a928f011d242de))
* handle errors when switching buffer [#453](https://github.com/YuanYuYuan/toggleterm.nvim/issues/453) ([#454](https://github.com/YuanYuYuan/toggleterm.nvim/issues/454)) ([029ad96](https://github.com/YuanYuYuan/toggleterm.nvim/commit/029ad968fd5a06ac5e29afe083d0a61be68e792b))
* **highlights:** add EndOfBuffer highlight ([46ffb28](https://github.com/YuanYuYuan/toggleterm.nvim/commit/46ffb283c490f96b31d699b766471f83da0bc0cf))
* include double colon pattern for autocmds on Windows ([#351](https://github.com/YuanYuYuan/toggleterm.nvim/issues/351)) ([b02a167](https://github.com/YuanYuYuan/toggleterm.nvim/commit/b02a1674bd0010d7982b056fd3df4f717ff8a57a))
* incorrect merge of formatting ([b6f6a2a](https://github.com/YuanYuYuan/toggleterm.nvim/commit/b6f6a2afd05b6399ba67974ad3dc47d003b72f25))
* **mappings:** respect insert mapping in terminal ([4751476](https://github.com/YuanYuYuan/toggleterm.nvim/commit/4751476fcf7ab24a3179812ac983927fd365dd09))
* **next_id:** Terminal IDs should be unique. ([#240](https://github.com/YuanYuYuan/toggleterm.nvim/issues/240)) ([aaeed9e](https://github.com/YuanYuYuan/toggleterm.nvim/commit/aaeed9e02167c5e8f00f25156895a6fd95403af8))
* **parse:** correct quotes matching for TermExec commands ([#52](https://github.com/YuanYuYuan/toggleterm.nvim/issues/52)) ([28c40c9](https://github.com/YuanYuYuan/toggleterm.nvim/commit/28c40c908d0edacda1fb2422a31d00d12878d1fb))
* prevent window closing error ([895f8e2](https://github.com/YuanYuYuan/toggleterm.nvim/commit/895f8e2485267640ccd11fe3fbf1ab5fe178bc4c))
* replace vim.wo with nvim_set_option_value ([#449](https://github.com/YuanYuYuan/toggleterm.nvim/issues/449)) ([7da102a](https://github.com/YuanYuYuan/toggleterm.nvim/commit/7da102a9c2fa1dd190c11faea03ee1c47af03d02))
* **resurrect:** use correct reference to terminal ([66a7ea3](https://github.com/YuanYuYuan/toggleterm.nvim/commit/66a7ea31fb571fddbfab9244d343612c83ae40f0))
* send_lines_to_terminal now honours ID variable when trim_spaces = false ([#541](https://github.com/YuanYuYuan/toggleterm.nvim/issues/541)) ([63ac4c8](https://github.com/YuanYuYuan/toggleterm.nvim/commit/63ac4c8529604ad247d9426644128de6ebb1f43a))
* **send_lines:** place cursor back in the original window ([#201](https://github.com/YuanYuYuan/toggleterm.nvim/issues/201)) ([93a7c59](https://github.com/YuanYuYuan/toggleterm.nvim/commit/93a7c59230f5dad60061318fefec35d431dec67f))
* separator on windows with powershell ([#192](https://github.com/YuanYuYuan/toggleterm.nvim/issues/192)) ([5733b24](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5733b24c684d202f978ccedca4a8c7571889bf28))
* shade_color ([#224](https://github.com/YuanYuYuan/toggleterm.nvim/issues/224)) ([ea21c3e](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ea21c3ef51868a564eeace357f4a3d429f93efb1))
* some auto commands don't fire on Windows ([#144](https://github.com/YuanYuYuan/toggleterm.nvim/issues/144)) ([f23866b](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f23866b8fbb0703be4e15d50c814ffe496242a67))
* **tabs:** allow persisting mode for tab terminals ([8d44db6](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8d44db6923d49088d33101650c0eef3e5a9e2084)), closes [#286](https://github.com/YuanYuYuan/toggleterm.nvim/issues/286)
* TermExec cmd with config.shell as function ([#467](https://github.com/YuanYuYuan/toggleterm.nvim/issues/467)) ([83871e3](https://github.com/YuanYuYuan/toggleterm.nvim/commit/83871e3c34837117644d83f422ee6c869b61891f))
* **terminal:** allow resizing hidden terminals ([bacbaa7](https://github.com/YuanYuYuan/toggleterm.nvim/commit/bacbaa7480344e4cfcebdf46fdfc058b3cb04648)), closes [#459](https://github.com/YuanYuYuan/toggleterm.nvim/issues/459)
* **terminal:** clear correctly on windows ([#513](https://github.com/YuanYuYuan/toggleterm.nvim/issues/513)) ([0731e99](https://github.com/YuanYuYuan/toggleterm.nvim/commit/0731e99de590fb7451eb4fee99470506e012b34d))
* **terminal:** fix conditional when focusing terminal ([f494c61](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f494c61024ffa25ee407d55b04d8b28ba9e839cb))
* **terminal:** fix scroll_bottom ([#307](https://github.com/YuanYuYuan/toggleterm.nvim/issues/307)) ([#319](https://github.com/YuanYuYuan/toggleterm.nvim/issues/319)) ([2a787c4](https://github.com/YuanYuYuan/toggleterm.nvim/commit/2a787c426ef00cb3488c11b14f5dcf892bbd0bda))
* **terminal:** improve nil dir check ([62683d9](https://github.com/YuanYuYuan/toggleterm.nvim/commit/62683d927dfd30dc68441a5811fdcb6c9f176c42))
* **terminal:** keep focus in current on TermExec ([40cab5d](https://github.com/YuanYuYuan/toggleterm.nvim/commit/40cab5df71a9ceb8d3952c2c0ebfec02d21f96d9))
* **terminal:** keep focus in current on TermExec in 'float' orientation ([01110d9](https://github.com/YuanYuYuan/toggleterm.nvim/commit/01110d99ea1ee13c30ebbe61141f53783492a8e2))
* **terminal:** only scroll to bottom if valid ([05c52fc](https://github.com/YuanYuYuan/toggleterm.nvim/commit/05c52fc249804893ce8a4994da81940c67994c85))
* toggle floating windows properly ([#165](https://github.com/YuanYuYuan/toggleterm.nvim/issues/165)) ([e97d0c1](https://github.com/YuanYuYuan/toggleterm.nvim/commit/e97d0c1046512e975a9f3fa95afe98f312752b1c))
* **toggleterm:** convert cmd args to a number ([9f05033](https://github.com/YuanYuYuan/toggleterm.nvim/commit/9f050333629308c80540bfa88631c9eccacbd282))
* **toggleterm:** ensure persist mode called at correct points ([5478abd](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5478abd611bc795a92a67415ff7a7ba4aca3e468))
* **toggleterm:** use correct arg for getting lines ([1e80c28](https://github.com/YuanYuYuan/toggleterm.nvim/commit/1e80c282f4b78964cd45068083a93471db0b5483))
* typo in readme ([#1](https://github.com/YuanYuYuan/toggleterm.nvim/issues/1)) ([e57deb1](https://github.com/YuanYuYuan/toggleterm.nvim/commit/e57deb1eebbe8c96f4439b10cb3f09f30058fe1e))
* **ui:** allow specifying only one float highlight ([5230dde](https://github.com/YuanYuYuan/toggleterm.nvim/commit/5230dde400fd5ef743be7ffcee290012cf5ee6fb)), closes [#250](https://github.com/YuanYuYuan/toggleterm.nvim/issues/250)
* **ui:** check all tabs for current terminal's window ([#309](https://github.com/YuanYuYuan/toggleterm.nvim/issues/309)) ([1be9b5a](https://github.com/YuanYuYuan/toggleterm.nvim/commit/1be9b5aadac71f7c3c9ed7799e0363f2b4427761))
* **ui:** handle highlighting unknown terminals ([#204](https://github.com/YuanYuYuan/toggleterm.nvim/issues/204)) ([1a608cc](https://github.com/YuanYuYuan/toggleterm.nvim/commit/1a608cc9ab269ec2877e617696cd2cf84f4a0e08))
* update error message to explicitly state compatible versions ([#159](https://github.com/YuanYuYuan/toggleterm.nvim/issues/159)) ([4e35034](https://github.com/YuanYuYuan/toggleterm.nvim/commit/4e350340e2fce27465fa9cc6b6a9f94c7f1e60de))
* use proper newline characters on windows ([#157](https://github.com/YuanYuYuan/toggleterm.nvim/issues/157)) ([f984519](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f9845199f1d647890ca47f6185f7ac935991b442))
* use resolve size when resizing a split ([8cafb2c](https://github.com/YuanYuYuan/toggleterm.nvim/commit/8cafb2c021175515d7b577c6236ac9428260222b))
* use self when applying terminal highlight ([f9ffba6](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f9ffba63cc77837edaceae61a5b9de6e77c88e7f))
* use smaller ignore comments to fix docs ([a16e636](https://github.com/YuanYuYuan/toggleterm.nvim/commit/a16e6366463b32ef5bf98c63b866cd0834e2a69b))
* use specified shell on windows ([#182](https://github.com/YuanYuYuan/toggleterm.nvim/issues/182)) ([36704dd](https://github.com/YuanYuYuan/toggleterm.nvim/commit/36704ddf3883842f3354e11da968d4c1201f0831))


### Reverts

* determine custom terminal ids on spawn ([#488](https://github.com/YuanYuYuan/toggleterm.nvim/issues/488)) ([0e4dcb8](https://github.com/YuanYuYuan/toggleterm.nvim/commit/0e4dcb8f0914bd191f732cae826df59f174359fe))
* **mappings:** use &lt;c-\&gt;<c-n> for terminal mode ([7127f4b](https://github.com/YuanYuYuan/toggleterm.nvim/commit/7127f4b686108ec5468ab79ff5fdd778adcdf5a6))


### Miscellaneous Chores

* release 2.5.0 ([f14cbfd](https://github.com/YuanYuYuan/toggleterm.nvim/commit/f14cbfd3141ce35d2738084e40bccf2176a474b2))


### Code Refactoring

* **colors:** use api.nvim_get_hl_by_name ([87e757e](https://github.com/YuanYuYuan/toggleterm.nvim/commit/87e757e1a8da9870f89e77c1515048ea0500b7d9)), closes [#276](https://github.com/YuanYuYuan/toggleterm.nvim/issues/276)
* use 0.7 autocommand api ([ba79cb4](https://github.com/YuanYuYuan/toggleterm.nvim/commit/ba79cb4fe9861130bdeb93a90c59efa461908950))

## [2.10.0](https://github.com/akinsho/toggleterm.nvim/compare/v2.9.0...v2.10.0) (2024-02-12)


### Features

* enable title for floating terminals ([#534](https://github.com/akinsho/toggleterm.nvim/issues/534)) ([d3aa6e8](https://github.com/akinsho/toggleterm.nvim/commit/d3aa6e88c2dcbefd240ffb77a2c77b486a19fa5f))


### Bug Fixes

* send_lines_to_terminal now honours ID variable when trim_spaces = false ([#541](https://github.com/akinsho/toggleterm.nvim/issues/541)) ([63ac4c8](https://github.com/akinsho/toggleterm.nvim/commit/63ac4c8529604ad247d9426644128de6ebb1f43a))

## [2.9.0](https://github.com/akinsho/toggleterm.nvim/compare/v2.8.0...v2.9.0) (2023-12-06)


### Features

* allow operator mapping to send to terminal ([#507](https://github.com/akinsho/toggleterm.nvim/issues/507)) ([5b84866](https://github.com/akinsho/toggleterm.nvim/commit/5b848664989b6deb2c28dad5135c89720915675a))


### Bug Fixes

* **commands:** call ToggleTermSetName with count ([#497](https://github.com/akinsho/toggleterm.nvim/issues/497)) ([ef1bbff](https://github.com/akinsho/toggleterm.nvim/commit/ef1bbff59c9ab5b468062c33ca183541a3849547)), closes [#496](https://github.com/akinsho/toggleterm.nvim/issues/496)
* **terminal:** clear correctly on windows ([#513](https://github.com/akinsho/toggleterm.nvim/issues/513)) ([0731e99](https://github.com/akinsho/toggleterm.nvim/commit/0731e99de590fb7451eb4fee99470506e012b34d))

## [2.8.0](https://github.com/akinsho/toggleterm.nvim/compare/v2.7.1...v2.8.0) (2023-09-11)


### Features

* add `Terminal.find` function ([#486](https://github.com/akinsho/toggleterm.nvim/issues/486)) ([01a84bc](https://github.com/akinsho/toggleterm.nvim/commit/01a84bc642484681933140537c3ff99b10b8a866))
* add name param to ToggleTerm and TermExec ([#479](https://github.com/akinsho/toggleterm.nvim/issues/479)) ([81ea9f7](https://github.com/akinsho/toggleterm.nvim/commit/81ea9f71a3fd7621fd02b2c74861595378a3c938))


### Bug Fixes

* **#487:** avoid terminal id collisions in __add ([#490](https://github.com/akinsho/toggleterm.nvim/issues/490)) ([6bec54e](https://github.com/akinsho/toggleterm.nvim/commit/6bec54e73807919b15fc92824fb48be32fb7e8ea))
* determine custom terminal ids on spawn ([#488](https://github.com/akinsho/toggleterm.nvim/issues/488)) ([8572917](https://github.com/akinsho/toggleterm.nvim/commit/8572917413dd039d1a53b007df5c571e2a3b8ad7))
* TermExec cmd with config.shell as function ([#467](https://github.com/akinsho/toggleterm.nvim/issues/467)) ([83871e3](https://github.com/akinsho/toggleterm.nvim/commit/83871e3c34837117644d83f422ee6c869b61891f))


### Reverts

* determine custom terminal ids on spawn ([#488](https://github.com/akinsho/toggleterm.nvim/issues/488)) ([0e4dcb8](https://github.com/akinsho/toggleterm.nvim/commit/0e4dcb8f0914bd191f732cae826df59f174359fe))

## [2.7.1](https://github.com/akinsho/toggleterm.nvim/compare/v2.7.0...v2.7.1) (2023-07-10)


### Bug Fixes

* handle errors when switching buffer [#453](https://github.com/akinsho/toggleterm.nvim/issues/453) ([#454](https://github.com/akinsho/toggleterm.nvim/issues/454)) ([029ad96](https://github.com/akinsho/toggleterm.nvim/commit/029ad968fd5a06ac5e29afe083d0a61be68e792b))
* replace vim.wo with nvim_set_option_value ([#449](https://github.com/akinsho/toggleterm.nvim/issues/449)) ([7da102a](https://github.com/akinsho/toggleterm.nvim/commit/7da102a9c2fa1dd190c11faea03ee1c47af03d02))
* **terminal:** allow resizing hidden terminals ([bacbaa7](https://github.com/akinsho/toggleterm.nvim/commit/bacbaa7480344e4cfcebdf46fdfc058b3cb04648)), closes [#459](https://github.com/akinsho/toggleterm.nvim/issues/459)

## [2.7.0](https://github.com/akinsho/toggleterm.nvim/compare/v2.6.0...v2.7.0) (2023-05-22)


### Features

* add a terminal select command ([#429](https://github.com/akinsho/toggleterm.nvim/issues/429)) ([c8574d7](https://github.com/akinsho/toggleterm.nvim/commit/c8574d7a7d2e5682de4479463ddba794390c0e40))
* allow changing terminal dir in background ([#438](https://github.com/akinsho/toggleterm.nvim/issues/438)) ([f5cf0b1](https://github.com/akinsho/toggleterm.nvim/commit/f5cf0b1eebd95ba4edc69e2fbd13e1a289048d5d))


### Bug Fixes

* **float:** ensure sidescroll is zero ([43b75f4](https://github.com/akinsho/toggleterm.nvim/commit/43b75f43aa7590228d88945525c737f0ddc05c22))

## [2.6.0](https://github.com/akinsho/toggleterm.nvim/compare/v2.5.0...v2.6.0) (2023-04-09)


### Features

* **config:** allow `shell` parameter to be a function ([#423](https://github.com/akinsho/toggleterm.nvim/issues/423)) ([a7857b6](https://github.com/akinsho/toggleterm.nvim/commit/a7857b6cbfdfc98df2a7b61591be16e1020c7a82))

## [2.5.0](https://github.com/akinsho/toggleterm.nvim/compare/2.4.0...v2.5.0) (2023-03-31)


### ⚠ BREAKING CHANGES

* switch persist_mode to false ([#410](https://github.com/akinsho/toggleterm.nvim/issues/410))

### Features

* support z-index option for floating windows ([#418](https://github.com/akinsho/toggleterm.nvim/issues/418)) ([0aa9364](https://github.com/akinsho/toggleterm.nvim/commit/0aa936445b895cd5d3387860f96ce424ce32b072))
* switch persist_mode to false ([#410](https://github.com/akinsho/toggleterm.nvim/issues/410)) ([98e15df](https://github.com/akinsho/toggleterm.nvim/commit/98e15df2c838fe5c3cae1efa36fa5c255fc75aa8))
* **terminal:** add mechanism to fetch last focused terminal ([#411](https://github.com/akinsho/toggleterm.nvim/issues/411)) ([bfb7a72](https://github.com/akinsho/toggleterm.nvim/commit/bfb7a7254b5d897a5b889484c6a5142951a18b29))


### Miscellaneous Chores

* release 2.5.0 ([f14cbfd](https://github.com/akinsho/toggleterm.nvim/commit/f14cbfd3141ce35d2738084e40bccf2176a474b2))
