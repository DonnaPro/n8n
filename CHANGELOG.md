## [1.97.1](https://github.com/n8n-io/n8n/compare/n8n@1.97.0...n8n@1.97.1) (2025-06-04)



# [1.97.0](https://github.com/n8n-io/n8n/compare/n8n@1.96.0...n8n@1.97.0) (2025-06-02)


### Bug Fixes

* **core:** Allow dotfiles in sendFile to fix WorkFlow settings 404 error ([#14744](https://github.com/n8n-io/n8n/issues/14744)) ([7928a9b](https://github.com/n8n-io/n8n/commit/7928a9b3c26e676dd77e24aae98054e1ecbbb37b))
* **core:** Honor absolute paths for `N8N_LOG_FILE_LOCATION` ([#15873](https://github.com/n8n-io/n8n/issues/15873)) ([1e5b905](https://github.com/n8n-io/n8n/commit/1e5b90571d380bb674071d988147d3e854728e41))
* **core:** Normalize trailing slash when setting CORS headers for test webhooks ([#15906](https://github.com/n8n-io/n8n/issues/15906)) ([61d0c6a](https://github.com/n8n-io/n8n/commit/61d0c6a6e7f1ad5dd1795a0e1f910425d6e2fc8f))


### Performance Improvements

* **core:** Lazyload LDAP during bootup ([#15907](https://github.com/n8n-io/n8n/issues/15907)) ([31b6f32](https://github.com/n8n-io/n8n/commit/31b6f32a363da2b199eff135f4f1fbe227ef47c6))



# [1.96.0](https://github.com/n8n-io/n8n/compare/n8n@1.95.0...n8n@1.96.0) (2025-06-02)


### Bug Fixes

* **API:** Allow `false` as a dependant value for public api json schema validation ([#15858](https://github.com/n8n-io/n8n/issues/15858)) ([5a8899c](https://github.com/n8n-io/n8n/commit/5a8899c4c980cbb6276c96199e20cc160c775038))
* Check if form trigger URL is live before oppening pop-up ([#15800](https://github.com/n8n-io/n8n/issues/15800)) ([041ada1](https://github.com/n8n-io/n8n/commit/041ada1fd6b15fc43ceb78a52e9a4b8bb05344d8))
* **core:** Don't allow creating more projects than allowed by exploiting a race condition ([#15218](https://github.com/n8n-io/n8n/issues/15218)) ([6466e76](https://github.com/n8n-io/n8n/commit/6466e76c06723d181e984d2c185c67eafea68f8a))
* **core:** Fix sorting of executions not working on postgres and mysql ([#15423](https://github.com/n8n-io/n8n/issues/15423)) ([eca282d](https://github.com/n8n-io/n8n/commit/eca282d09c1641eaa2937acbab40249752d6bb38))
* **core:** Fix timezone-dependent test failures in Insights weekly compaction ([#15680](https://github.com/n8n-io/n8n/issues/15680)) ([096806a](https://github.com/n8n-io/n8n/commit/096806af154dfb3be8c4724cb054beba4b777792))
* **core:** Simplify Websocket origin security checks ([#15761](https://github.com/n8n-io/n8n/issues/15761)) ([bbe2b12](https://github.com/n8n-io/n8n/commit/bbe2b12bf2cca1a73e332ace349279f214f1f236))
* **core:** Solve memory leak in `TaskRequester` ([#15768](https://github.com/n8n-io/n8n/issues/15768)) ([0398505](https://github.com/n8n-io/n8n/commit/039850514387d4966845e6646e2a3e1562a0fc6d))
* **core:** Support `helpers.request` in task runners ([#15859](https://github.com/n8n-io/n8n/issues/15859)) ([7f8b943](https://github.com/n8n-io/n8n/commit/7f8b943c1ae805807134205eae8ebb24cef5511e))
* **editor:** Deactivate workflow on save if trigger is missing ([#15642](https://github.com/n8n-io/n8n/issues/15642)) ([3ba6419](https://github.com/n8n-io/n8n/commit/3ba6419710887456a4a6ecc04146721ffce4dcb5))
* **editor:** Delete all connections of nodes with multiple ones when removed from canvas ([#15713](https://github.com/n8n-io/n8n/issues/15713)) ([c4ea757](https://github.com/n8n-io/n8n/commit/c4ea7578fe3dddc8d480f3abb8cb5f2d064120c0))
* **editor:** Fix Execute workflow button hover state  ([#15518](https://github.com/n8n-io/n8n/issues/15518)) ([57d7b5e](https://github.com/n8n-io/n8n/commit/57d7b5e35edac78caffd27e29108272f0e995969))
* **editor:** Handle Insights calculations to prevent Infinity numbers ([#15727](https://github.com/n8n-io/n8n/issues/15727)) ([d1a39d9](https://github.com/n8n-io/n8n/commit/d1a39d96bbac78bb5b305e3760a2030311f6d732))
* **editor:** Move focus to search input in RLC ([#15741](https://github.com/n8n-io/n8n/issues/15741)) ([fee10da](https://github.com/n8n-io/n8n/commit/fee10da95b9444931915146f50a614411d8350bb))
* **editor:** Set deterministic width for sidebar ([#15753](https://github.com/n8n-io/n8n/issues/15753)) ([3f9a271](https://github.com/n8n-io/n8n/commit/3f9a271e69c0ab6ec1a4f35f57e736e566877adb))
* **editor:** Simplifying empty project deletion ([#15834](https://github.com/n8n-io/n8n/issues/15834)) ([6bf2d8a](https://github.com/n8n-io/n8n/commit/6bf2d8a4d4a62c3a20129a5e79bf18efa6de80ca))
* **editor:** Update copy for debug modal paywall ([#15905](https://github.com/n8n-io/n8n/issues/15905)) ([d0ff662](https://github.com/n8n-io/n8n/commit/d0ff66226fdd5af0bab2286360da397367b653a2))
* **editor:** Use last task data for calculating the current state ([#15546](https://github.com/n8n-io/n8n/issues/15546)) ([1daf0ff](https://github.com/n8n-io/n8n/commit/1daf0ff169468c9afde1ab3f37b241426cfd1db3))
* **GitHub Node:** Update auth urls for enterprise server ([#15533](https://github.com/n8n-io/n8n/issues/15533)) ([bc66d9f](https://github.com/n8n-io/n8n/commit/bc66d9fb7d757c308fe10b85c1b43913d3cc738a))
* **Jina AI Node:** Default value for "Output format" option ([#15683](https://github.com/n8n-io/n8n/issues/15683)) ([e125854](https://github.com/n8n-io/n8n/commit/e1258547ad7b0fe50bd5001b52eea0042eb5c4d5))
* **Microsoft SharePoint Node:** Add back the support for cred only node ([#15806](https://github.com/n8n-io/n8n/issues/15806)) ([0fdeba5](https://github.com/n8n-io/n8n/commit/0fdeba52bb171111d311f6d8bbb1b348ad08ebc9))
* **n8n Form Node:** Use execution.mode instead of hard coding webhook ([#15647](https://github.com/n8n-io/n8n/issues/15647)) ([636e9f4](https://github.com/n8n-io/n8n/commit/636e9f463fd7ee600e529649e31fdbbfc30234e2))
* Run evaluations loop manually always from first row ([#15794](https://github.com/n8n-io/n8n/issues/15794)) ([b8ab4b6](https://github.com/n8n-io/n8n/commit/b8ab4b6a5e1adfb9b582d0186b5238b487b5ce5b))
* Skip subworkflow input test temporarily ([#15803](https://github.com/n8n-io/n8n/issues/15803)) ([ba70cab](https://github.com/n8n-io/n8n/commit/ba70cab9d508405e0c24ac29ad4ea5d585b5482a))


### Features

* **API:** Add user management endpoints to the Projects Public API ([#12329](https://github.com/n8n-io/n8n/issues/12329)) ([4459c7e](https://github.com/n8n-io/n8n/commit/4459c7e7b10e7e1cd30a8885dd03ad452f846b96))
* **core:** Allow specifying Content-Security-Policy-Report-Only ([#15805](https://github.com/n8n-io/n8n/issues/15805)) ([c127846](https://github.com/n8n-io/n8n/commit/c12784600fb5acd42fcce10c72f73168d3d2948d))
* **core:** Start listening to IPv6 addresses as well by default ([#15810](https://github.com/n8n-io/n8n/issues/15810)) ([9f44f40](https://github.com/n8n-io/n8n/commit/9f44f407459cb656a697a8d44a129d1d4cbbbc17))
* **editor:** Add ability to extract sub-workflows to canvas context menu ([#15538](https://github.com/n8n-io/n8n/issues/15538)) ([5985df6](https://github.com/n8n-io/n8n/commit/5985df6e5166e59e77193cba49607a7d3110deac))
* **editor:** Combine 'Move to Folder' and 'Change owner' modals ([#15756](https://github.com/n8n-io/n8n/issues/15756)) ([e860dd6](https://github.com/n8n-io/n8n/commit/e860dd6d2eb6a2dac5126bc60006d53b53115a68))
* **editor:** Support pasting an expression into a number parameter ([#15722](https://github.com/n8n-io/n8n/issues/15722)) ([2a1475d](https://github.com/n8n-io/n8n/commit/2a1475d67125d111b0f2ed602e597fae83d65b56))
* **MCP Server Trigger Node:** Cleanup MCP server management, use sanitized trigger node's name as name for the MCP server ([#15751](https://github.com/n8n-io/n8n/issues/15751)) ([07a636e](https://github.com/n8n-io/n8n/commit/07a636eed6cb4d1f487018b34632810d24d99824))
* **Perplexity Node:** New node  ([#13604](https://github.com/n8n-io/n8n/issues/13604)) ([6d3e6ee](https://github.com/n8n-io/n8n/commit/6d3e6eef00ed3acf35d376b88ce6586692ae641b))
* **Respond to Webhook Node:** Setting to configure outputs  ([#15619](https://github.com/n8n-io/n8n/issues/15619)) ([be5f14e](https://github.com/n8n-io/n8n/commit/be5f14e31623174b66ef3062aa8f780970c5689f))


### Performance Improvements

* **core:** Shorten bootup for all instance types ([#15856](https://github.com/n8n-io/n8n/issues/15856)) ([73c9a52](https://github.com/n8n-io/n8n/commit/73c9a529dd5ee8f5e461edfe815a88bb97d86275))



# [1.95.0](https://github.com/n8n-io/n8n/compare/n8n@1.94.0...n8n@1.95.0) (2025-05-26)


### Bug Fixes

* **Chat Trigger Node:** Don't continue when action is load previous session and option is not set ([#15438](https://github.com/n8n-io/n8n/issues/15438)) ([8fd0738](https://github.com/n8n-io/n8n/commit/8fd0738191f87f5762f23c763f64e86fdd444830))
* **core:** Add support for proxy using forward headers ([#15006](https://github.com/n8n-io/n8n/issues/15006)) ([b1687c6](https://github.com/n8n-io/n8n/commit/b1687c6be2cbeda0989505f67be3c2a64489c5d0))
* **core:** Fix community package installation on windows ([#15685](https://github.com/n8n-io/n8n/issues/15685)) ([647cb85](https://github.com/n8n-io/n8n/commit/647cb851e5e7f7b206bede8ac858f6c506b7a8c7))
* **core:** Fix license reloading flow in scaling mode ([#15650](https://github.com/n8n-io/n8n/issues/15650)) ([c2449ee](https://github.com/n8n-io/n8n/commit/c2449ee2c8fec784e16620eebf936ce008598765))
* **core:** Use destination node to select the correct pinned trigger to start from ([#15633](https://github.com/n8n-io/n8n/issues/15633)) ([dc0802b](https://github.com/n8n-io/n8n/commit/dc0802bbd1034812a7061d0610acb62986e1f3bf))
* **editor:** Add type definition for $getWorkflowStaticData to code node ([#15544](https://github.com/n8n-io/n8n/issues/15544)) ([bca03ca](https://github.com/n8n-io/n8n/commit/bca03ca7392b00ce2edd7d829bc23b6d999a0e37))
* **editor:** Don't mark node as dirty when NDV is opened ([#15222](https://github.com/n8n-io/n8n/issues/15222)) ([8d1170e](https://github.com/n8n-io/n8n/commit/8d1170e3ddc179a6ac1e6efe584cbbce702e11ab))
* **editor:** Fix how deviation percentage is calculated in Insights summary ([#15526](https://github.com/n8n-io/n8n/issues/15526)) ([26de979](https://github.com/n8n-io/n8n/commit/26de97976aed4d5f11f7e37ca55fc5c1fe283099))
* **editor:** Fix notification toast offset outside of NodeView if chat/logs were opened ([#15622](https://github.com/n8n-io/n8n/issues/15622)) ([70ea7a8](https://github.com/n8n-io/n8n/commit/70ea7a88594026479a934341b5c149661e75973b))
* **editor:** Fix schema view showing incorrect data on loop node done branch ([#15635](https://github.com/n8n-io/n8n/issues/15635)) ([f762c59](https://github.com/n8n-io/n8n/commit/f762c59fb353dd334e4239b545ae44503b6e78d4))
* **editor:** Fix update panel icon display. Fix title on insights dashboard ([#15593](https://github.com/n8n-io/n8n/issues/15593)) ([075b035](https://github.com/n8n-io/n8n/commit/075b035d64d462e84e35c2e3b73afee0fca592b8))
* **editor:** Handle Loop node execution data preview correctly when inserting a node  ([#15351](https://github.com/n8n-io/n8n/issues/15351)) ([5967c13](https://github.com/n8n-io/n8n/commit/5967c131654d5d8e87633fba9181af5ed571539b))
* **editor:** Make deleting Call n8n Workflow Tool fromAI workflow input descriptions work ([#15459](https://github.com/n8n-io/n8n/issues/15459)) ([0e708dd](https://github.com/n8n-io/n8n/commit/0e708ddb54a2487ce48776b6470a7bc71998b845))
* Fix jobs for secrets inherit ([#15532](https://github.com/n8n-io/n8n/issues/15532)) ([cf29b5f](https://github.com/n8n-io/n8n/commit/cf29b5f188c83f02ea3d1f8cb9a064dfebaca3eb))
* **Google Drive Node:** Incorrect MIME type when uploading files on cloud ([#15478](https://github.com/n8n-io/n8n/issues/15478)) ([2060498](https://github.com/n8n-io/n8n/commit/20604983cd007fc041da6b9dd084264c8977bb68))
* **HTTP Request Node:** Fix prototype pollution vulnerability ([#15463](https://github.com/n8n-io/n8n/issues/15463)) ([1ffc33d](https://github.com/n8n-io/n8n/commit/1ffc33dcc63dfcc0dc27905a9c0a01de33da4160))
* **Information Extractor Node:** Improve error handling for empty inputs ([#15590](https://github.com/n8n-io/n8n/issues/15590)) ([bb2f675](https://github.com/n8n-io/n8n/commit/bb2f675817ccfc2e11ce9b758c4f9dd80a992cd5))
* **Jira Software Node:** Use old endpoints to get all issues on self-hosted instances ([#15591](https://github.com/n8n-io/n8n/issues/15591)) ([e23ffcc](https://github.com/n8n-io/n8n/commit/e23ffccca8248aa76435be9d20cc3df6bd6c3773))
* **MongoDB Node:** Stop overwriting nested values on update ([#15543](https://github.com/n8n-io/n8n/issues/15543)) ([3ee15a8](https://github.com/n8n-io/n8n/commit/3ee15a833128cac63a767f13aaaaad7ebd960501))
* **Summarize Node:** Convert v1 split by values to string ([#15525](https://github.com/n8n-io/n8n/issues/15525)) ([4d037ca](https://github.com/n8n-io/n8n/commit/4d037ca68abe4660b3815da3b99e8b65e2b80c43))
* **Telegram Node:** Include error message in output when continueOnFail is set ([#15540](https://github.com/n8n-io/n8n/issues/15540)) ([b8ee275](https://github.com/n8n-io/n8n/commit/b8ee275f0beeaf054cd0ef52e987c73bc211ec27))


### Features

* **Airtop Node:** Add File operations and scroll micro-interaction ([#15089](https://github.com/n8n-io/n8n/issues/15089)) ([86885a7](https://github.com/n8n-io/n8n/commit/86885a7d0e035a480960600a20303ebcda508870))
* **Anthropic Chat Model Node:** Set the new Claude 4 Sonnet model to be the default ([#15609](https://github.com/n8n-io/n8n/issues/15609)) ([cf8b611](https://github.com/n8n-io/n8n/commit/cf8b611d14528b3a898a1b89d6c817a0b7e63575))
* **core:** Add logs for insights flushing and compaction ([#15519](https://github.com/n8n-io/n8n/issues/15519)) ([3743a8c](https://github.com/n8n-io/n8n/commit/3743a8c33dfc77295e743bf8606e45850be21579))
* **core:** Invalidate all sessions when MFA is enabled/disabled ([#15524](https://github.com/n8n-io/n8n/issues/15524)) ([2a35c19](https://github.com/n8n-io/n8n/commit/2a35c19ef971bd9a2612a43471e6f87dd4c43f7b))
* **core:** Scope getStatus for environments for project admin role ([#15404](https://github.com/n8n-io/n8n/issues/15404)) ([f9f9597](https://github.com/n8n-io/n8n/commit/f9f9597bbd20a8a97c0100f20586e9c1a8acd4d9))
* **editor:** "Executing" state in the output panel ([#15470](https://github.com/n8n-io/n8n/issues/15470)) ([7e3bcd3](https://github.com/n8n-io/n8n/commit/7e3bcd389546a8b85a9a81e0ce76f5aeb4df3e7c))
* **editor:** Add an option to sync canvas with log view ([#15391](https://github.com/n8n-io/n8n/issues/15391)) ([9938e63](https://github.com/n8n-io/n8n/commit/9938e63a666cb37461ce642836c427f05a44ebc9))
* **editor:** Distinguish official verified nodes from community built nodes ([#15630](https://github.com/n8n-io/n8n/issues/15630)) ([7f0c6d6](https://github.com/n8n-io/n8n/commit/7f0c6d62e6a1b9a1b2fc92ad05d4c47d3a9393d6))
* **editor:** Save new project on Enter in name field ([#15535](https://github.com/n8n-io/n8n/issues/15535)) ([fbf7083](https://github.com/n8n-io/n8n/commit/fbf7083062488d1b7e2e69b8ed7f5bcded417baf))
* **editor:** Show informative message in NDV when AI tools have no parameters ([#15515](https://github.com/n8n-io/n8n/issues/15515)) ([a426ecd](https://github.com/n8n-io/n8n/commit/a426ecd2f13208ac80ddcbabbc8ac8fdbd268ab0))
* **editor:** Use resource locator at Simple Vector Store memory key, allow cross workflow use ([#15421](https://github.com/n8n-io/n8n/issues/15421)) ([e5c2aea](https://github.com/n8n-io/n8n/commit/e5c2aea6fe770698c0f8d6986b6b4662e89f90b4))
* **Merge Node:** Option in combineBySql operation to return either confirmation of succes or empty result ([#15509](https://github.com/n8n-io/n8n/issues/15509)) ([a86bc43](https://github.com/n8n-io/n8n/commit/a86bc43f50185f0aa647a63dfe04d147fad62256))
* Migrate Test Workflows to Main Repo ([#15504](https://github.com/n8n-io/n8n/issues/15504)) ([867842d](https://github.com/n8n-io/n8n/commit/867842d4735a73ce117ae418ea49db4f1f567c94))



# [1.94.0](https://github.com/n8n-io/n8n/compare/n8n@1.93.0...n8n@1.94.0) (2025-05-19)


### Bug Fixes

* **AI Agent Node:** Fix tool calling when tools run in a loop ([#15250](https://github.com/n8n-io/n8n/issues/15250)) ([cd1d6c9](https://github.com/n8n-io/n8n/commit/cd1d6c9dfc5491a10b4c522b664949b46c58ea45))
* **Azure OpenAI Chat Model Node:** Simplify Azure Entra ID Authentication and Auto-Refresh token ([#15335](https://github.com/n8n-io/n8n/issues/15335)) ([e750d53](https://github.com/n8n-io/n8n/commit/e750d5366ec51b09278ed75f2c07bf9946488645))
* **Basic LLM Chain Node:** Use JSON parsing for Claude 3.7 with thinking enabled ([#15381](https://github.com/n8n-io/n8n/issues/15381)) ([c8b9a7f](https://github.com/n8n-io/n8n/commit/c8b9a7fdebc902b6d68ed1356e79ee976ab1cee7))
* **core:** Allow strings starting with numbers in alphanumeric string validator ([#15425](https://github.com/n8n-io/n8n/issues/15425)) ([64b3fa3](https://github.com/n8n-io/n8n/commit/64b3fa3d1771a69d62814977d3ac3782a35aeb35))
* **core:** Load config early to fix `N8N_CONFIG_FILES` ([#15406](https://github.com/n8n-io/n8n/issues/15406)) ([ec63a61](https://github.com/n8n-io/n8n/commit/ec63a616523221ec2216782845e508a59c6d0a05))
* **core:** Load insights module on webhook instance to save insights on webhook workflows ([#15433](https://github.com/n8n-io/n8n/issues/15433)) ([bf5551d](https://github.com/n8n-io/n8n/commit/bf5551d711bb15af3ac104046219abb4686ef1c1))
* **core:** Make the Insights by time datetime parsing more robust ([#15413](https://github.com/n8n-io/n8n/issues/15413)) ([d9fdef3](https://github.com/n8n-io/n8n/commit/d9fdef3bf9ca2f0bca564493cbae851b7a97bd8e))
* **core:** Upgrade formidable to address CVE-2025-46653 ([#15341](https://github.com/n8n-io/n8n/issues/15341)) ([d612d7b](https://github.com/n8n-io/n8n/commit/d612d7ba32d2cea093a6ebf149b93c5e9a4bcbe6))
* **core:** Upgrade snowflake-sdk to address CVE-2025-46328 ([#15345](https://github.com/n8n-io/n8n/issues/15345)) ([eb634ea](https://github.com/n8n-io/n8n/commit/eb634eacf4b82f00cc44f4328150e9a0d22b791f))
* **editor:** Correctly show Workflow Breadcrumbs in MainHeader on Registered Community ([#15457](https://github.com/n8n-io/n8n/issues/15457)) ([5c38405](https://github.com/n8n-io/n8n/commit/5c3840583dc8993e76fb9324aa4fe766aff60cb7))
* **editor:** Don't render `now` when `startedAt` is `null` ([#15283](https://github.com/n8n-io/n8n/issues/15283)) ([44ecad5](https://github.com/n8n-io/n8n/commit/44ecad58831cca5fd411b1f943a74910283b77c7))
* **editor:** FE fixes to insights ([#15228](https://github.com/n8n-io/n8n/issues/15228)) ([3eb1c1c](https://github.com/n8n-io/n8n/commit/3eb1c1c783a45a150fa7229d8f2590d3786f58ad))
* **editor:** Fix node renaming in pinned data ([#15482](https://github.com/n8n-io/n8n/issues/15482)) ([fc17cde](https://github.com/n8n-io/n8n/commit/fc17cdece2fdaf4ee31c77f38a2b4fc2416b762d))
* **editor:** Fix paired items after renaming a node ([#15440](https://github.com/n8n-io/n8n/issues/15440)) ([7d3cae5](https://github.com/n8n-io/n8n/commit/7d3cae5639b26b32d170e516b72dbe782e25f4bb))
* **editor:** Fix partial chat executions ([#15379](https://github.com/n8n-io/n8n/issues/15379)) ([b6370fb](https://github.com/n8n-io/n8n/commit/b6370fb2ec97e4533ec24f712019227f7f47b253))
* **editor:** Fix resizing NDV output panel when closing assistant ([#15313](https://github.com/n8n-io/n8n/issues/15313)) ([d7d3d33](https://github.com/n8n-io/n8n/commit/d7d3d33d1a072372a7930290eb060371e0b466e8))
* **editor:** Fix switching between connected SQL/HTML editors ([#15297](https://github.com/n8n-io/n8n/issues/15297)) ([bb2cfc2](https://github.com/n8n-io/n8n/commit/bb2cfc209c96cc4ed3335ecff878d5d40346a8da))
* **editor:** Hide evaluation trigger ([#15471](https://github.com/n8n-io/n8n/issues/15471)) ([b53bd17](https://github.com/n8n-io/n8n/commit/b53bd173d0a26b0662053e8c95505cbab3dc6963))
* **editor:** Make `AI Agent` appear before `Magento 2` when typing `agent` ([#15302](https://github.com/n8n-io/n8n/issues/15302)) ([d683a54](https://github.com/n8n-io/n8n/commit/d683a54da0e1f43cb9ef9bdb54ba49551839a640))
* **editor:** Normalize credential data from source control ([#15434](https://github.com/n8n-io/n8n/issues/15434)) ([840a3be](https://github.com/n8n-io/n8n/commit/840a3bee4bc41e4b94bd571ef2899e24c7fa7afe))
* **editor:** Show error toast for failed executions ([#15388](https://github.com/n8n-io/n8n/issues/15388)) ([e68149b](https://github.com/n8n-io/n8n/commit/e68149bbc7760b2c1f311803f51588fbb0704fbd))
* **editor:** Tag styling issues ([#15336](https://github.com/n8n-io/n8n/issues/15336)) ([807084e](https://github.com/n8n-io/n8n/commit/807084e75d63d76115448e1b21d29ec8c7fd3854))
* Ensure diagnostics stay disabled in e2e even when enabled by environment variable ([#15322](https://github.com/n8n-io/n8n/issues/15322)) ([c026962](https://github.com/n8n-io/n8n/commit/c02696241bcce356aa5ff774226e1fd223069ee0))
* **Execute Workflow Trigger Node:** Show helpful error message when passing array to JSON Example ([#15458](https://github.com/n8n-io/n8n/issues/15458)) ([06e9386](https://github.com/n8n-io/n8n/commit/06e938687584d4f3a57a444171396152b0491c59))
* **n8n Evaluation Trigger Node:** Fix tweaks ([#15473](https://github.com/n8n-io/n8n/issues/15473)) ([3985387](https://github.com/n8n-io/n8n/commit/398538720429c061d9df3374bffa711cc4d9aa20))
* **n8n Form Node:** Limit the max width for text area ([#15508](https://github.com/n8n-io/n8n/issues/15508)) ([9936186](https://github.com/n8n-io/n8n/commit/99361869a3e8eaf0c228bbc923d45e844f9f6ac5))
* **OpenAI Node:** Hide the option to return URL for gpt-image-1 model ([#15392](https://github.com/n8n-io/n8n/issues/15392)) ([027a479](https://github.com/n8n-io/n8n/commit/027a479172351b0af8b2e596eb4f3e9a76859437))
* **PostBin Node:** Update base URL for postbin node ([#15358](https://github.com/n8n-io/n8n/issues/15358)) ([0cddc95](https://github.com/n8n-io/n8n/commit/0cddc9576f6c77b6b5813fe6f3aa649df45c2ce9))
* **RabbitMQ Node:** Support RabbitMQ v.4.1.0 by updating amqplib ([#15418](https://github.com/n8n-io/n8n/issues/15418)) ([cf05c33](https://github.com/n8n-io/n8n/commit/cf05c3341ed81ab343c656ddbbcf14486add8f20))
* Set `tournament` for nodes test harness ([#15346](https://github.com/n8n-io/n8n/issues/15346)) ([0699925](https://github.com/n8n-io/n8n/commit/069992524d3a45b0f10183379cc0168c67f661fb))
* **Text Classifier Node:** Return error for empty inputText ([#15390](https://github.com/n8n-io/n8n/issues/15390)) ([71e5584](https://github.com/n8n-io/n8n/commit/71e5584d28771400b7d8478d9c519de65c35ee6f))
* **YouTube Node:** Chunk file content before uploading ([#15405](https://github.com/n8n-io/n8n/issues/15405)) ([3e855b4](https://github.com/n8n-io/n8n/commit/3e855b4485244549c1cbe46e7e23a73fa6292460))


### Features

* Add HTTP proxy for supported LLM nodes ([#15449](https://github.com/n8n-io/n8n/issues/15449)) ([907485d](https://github.com/n8n-io/n8n/commit/907485d01692f004ea289dcd2d6af2d0900e1b49))
* **API:** Add Public API endpoint for updating variables ([#15315](https://github.com/n8n-io/n8n/issues/15315)) ([52bf920](https://github.com/n8n-io/n8n/commit/52bf9203f009d7ffc586f87fdd642d431acdca8f))
* **AWS IAM Node:** Add new AWS IAM Node ([#11963](https://github.com/n8n-io/n8n/issues/11963)) ([ab1047e](https://github.com/n8n-io/n8n/commit/ab1047ebde4ce0bdbf9ef25cae1503ef147eb89e))
* **editor:** Add "Go to Sub-workflow" menu context action to `Workflow Tool` ([#15396](https://github.com/n8n-io/n8n/issues/15396)) ([2b05dbe](https://github.com/n8n-io/n8n/commit/2b05dbea8c416c1edd88801f711d4c4f6c43a4d7))
* **editor:** Add user info on relations to enhance design of project users list ([#15420](https://github.com/n8n-io/n8n/issues/15420)) ([435d43f](https://github.com/n8n-io/n8n/commit/435d43fc5b2307a966e44fc71d2e1ec71c0ce694))
* **editor:** Improve canvas node insertion position ([#14289](https://github.com/n8n-io/n8n/issues/14289)) ([102c676](https://github.com/n8n-io/n8n/commit/102c67628c67da19c54eeca8bfe1703616a016c9))
* **editor:** Improve manual description in nodes as tools ([#15373](https://github.com/n8n-io/n8n/issues/15373)) ([726438d](https://github.com/n8n-io/n8n/commit/726438d95ef3a58095b46bb17d2ce88209c5ceec))
* **editor:** Include pending users for project users search ([#15389](https://github.com/n8n-io/n8n/issues/15389)) ([f906dba](https://github.com/n8n-io/n8n/commit/f906dbaf6337764297de4fd7afaf96e1baebd4a5))
* **editor:** Keyboard shortcuts for the log view ([#15378](https://github.com/n8n-io/n8n/issues/15378)) ([1935e62](https://github.com/n8n-io/n8n/commit/1935e62adfba1cd2b3bea6122bd88fc01f9f5bb7))
* **editor:** Rollout improved log view (2nd attempt) ([#15382](https://github.com/n8n-io/n8n/issues/15382)) ([4657e34](https://github.com/n8n-io/n8n/commit/4657e348f4a262a14b8c4060ff2d9538222e13da))
* **editor:** Show sub workflow runs in the log view ([#15163](https://github.com/n8n-io/n8n/issues/15163)) ([0c4398f](https://github.com/n8n-io/n8n/commit/0c4398fd2f72ad473a38f925e99cc524c4ad2038))
* **Execute Workflow Trigger Node:** Reintroduce binary data on Workflow Triggers ([#15259](https://github.com/n8n-io/n8n/issues/15259)) ([218007e](https://github.com/n8n-io/n8n/commit/218007e625ca52256548fc3f5b01debb1f2bbfb3))
* **Microsoft SharePoint Node:** New node ([#13727](https://github.com/n8n-io/n8n/issues/13727)) ([954b662](https://github.com/n8n-io/n8n/commit/954b66218fa045c4784c29a2d3a805f51fea9924))
* **n8n Evaluation Trigger Node:** Add Evaluation Trigger and Evaluation Node ([#15194](https://github.com/n8n-io/n8n/issues/15194)) ([570d1e7](https://github.com/n8n-io/n8n/commit/570d1e7aadd5ba1d77ab95432bed0c9fcbe812a5))
* **n8n Evaluation Trigger Node:** Add link to dataset template in trigger ([#15455](https://github.com/n8n-io/n8n/issues/15455)) ([1f023db](https://github.com/n8n-io/n8n/commit/1f023db531ce019163e479c1c1340a0c0041b4b5))
* **n8n Evaluation Trigger Node:** Add telemetry events ([#15465](https://github.com/n8n-io/n8n/issues/15465)) ([9834a49](https://github.com/n8n-io/n8n/commit/9834a49bd344f74be0280afbf4a0ed03b5816708))
* **n8n Microsoft Teams Node:** New trigger node ([#12875](https://github.com/n8n-io/n8n/issues/12875)) ([870940b](https://github.com/n8n-io/n8n/commit/870940b54393ab4a836c6ca4325af4f97c16dfbd))
* Optimise langchain calls in batching mode ([#15243](https://github.com/n8n-io/n8n/issues/15243)) ([ff15693](https://github.com/n8n-io/n8n/commit/ff156930c5f1b75da59bc27b424925a5535cd908))
* **Respond to Webhook Node:** Additional output branch - Response ([#13734](https://github.com/n8n-io/n8n/issues/13734)) ([40fb4a2](https://github.com/n8n-io/n8n/commit/40fb4a2efc6201539d765358db536ca243cb140f))
* **Snowflake Node:** Add support for Key-Pair authentication ([#14833](https://github.com/n8n-io/n8n/issues/14833)) ([4302c5f](https://github.com/n8n-io/n8n/commit/4302c5f474e96412f7a1c5d724b1d1c05acc2068))


### Performance Improvements

* **editor:** Avoid deep watch on execution result data ([#15304](https://github.com/n8n-io/n8n/issues/15304)) ([cd2e2dc](https://github.com/n8n-io/n8n/commit/cd2e2dc8d93632479ff4a38600ddd76cdcd5c957))



# [1.93.0](https://github.com/n8n-io/n8n/compare/n8n@1.92.0...n8n@1.93.0) (2025-05-12)


### Bug Fixes

* Center circular element in Milvus logo ([#15078](https://github.com/n8n-io/n8n/issues/15078)) ([2202264](https://github.com/n8n-io/n8n/commit/22022642bf182b7f35a7446ef15465a201665bb0))
* **Code Node:** Update pyodide sandbox context to fix micropip regressions ([#15181](https://github.com/n8n-io/n8n/issues/15181)) ([63cbf86](https://github.com/n8n-io/n8n/commit/63cbf8681a85b2b4ac1bbf69bf13a91f0c40ea4a))
* Community nodes - setting page empty state ([#15305](https://github.com/n8n-io/n8n/issues/15305)) ([e7c095d](https://github.com/n8n-io/n8n/commit/e7c095d047759349ddb970537de2575b25d47ca1))
* **core:** Add mechanism to prevent concurrent compaction on Insights ([#14988](https://github.com/n8n-io/n8n/issues/14988)) ([392e914](https://github.com/n8n-io/n8n/commit/392e91480a8e1508faced838854d2215c3ae6139))
* **core:** Do not cache dynamic webhooks ([#15176](https://github.com/n8n-io/n8n/issues/15176)) ([0659ba9](https://github.com/n8n-io/n8n/commit/0659ba957cf741feabef32445a3a2f96c7e59006))
* **core:** Fix Insights concurrency issues for legacy sqlite ([#15028](https://github.com/n8n-io/n8n/issues/15028)) ([e34bca7](https://github.com/n8n-io/n8n/commit/e34bca779bdbae13477990e61a8cb088f65af40f))
* **core:** Fix task runner logging to browser console ([#15111](https://github.com/n8n-io/n8n/issues/15111)) ([e86edf5](https://github.com/n8n-io/n8n/commit/e86edf536f647b2c215bcf8f289c7127d975e7eb))
* **core:** Fix task runner validation error on array of arrays ([#15106](https://github.com/n8n-io/n8n/issues/15106)) ([75c1a4c](https://github.com/n8n-io/n8n/commit/75c1a4c5b3d7debfabdee83f4dd6b1d732aa0185))
* **core:** Prioritize workflow execution with existing execution data on worker ([#15165](https://github.com/n8n-io/n8n/issues/15165)) ([12b681f](https://github.com/n8n-io/n8n/commit/12b681fc41035619a9684df97dd4c676a365e54c))
* **core:** Support task runner in `execute` and `execute-batch` commands ([#15147](https://github.com/n8n-io/n8n/issues/15147)) ([985f554](https://github.com/n8n-io/n8n/commit/985f5545012d07622c9632e26aaeba1e39484b18))
* **editor:** Close Workflow URL Import Modal after import ([#15177](https://github.com/n8n-io/n8n/issues/15177)) ([d14fb4d](https://github.com/n8n-io/n8n/commit/d14fb4dde3123548c477803e5da066544ed0ecb2))
* **editor:** Ensure no running node when execution finished ([#15299](https://github.com/n8n-io/n8n/issues/15299)) ([d12c7ee](https://github.com/n8n-io/n8n/commit/d12c7ee87f6d4087ed1d875dd72ca636f163b7a6))
* **editor:** Fix AI Node Logs View to Filter Duplicate Executions ([#15049](https://github.com/n8n-io/n8n/issues/15049)) ([8680797](https://github.com/n8n-io/n8n/commit/86807978c1c7a8f934b23132a99052f07313fef1))
* **editor:** Fix context menu behaviour and rename shortcut indicator ([#15116](https://github.com/n8n-io/n8n/issues/15116)) ([73a4a33](https://github.com/n8n-io/n8n/commit/73a4a33da0b36eb9fd40e9f3dc9a7f39fc1b892e))
* **editor:** Fix Paired item error message ([#15171](https://github.com/n8n-io/n8n/issues/15171)) ([be72f73](https://github.com/n8n-io/n8n/commit/be72f736ac6e3246ea52da92124be26585f0ac9e))
* **editor:** Fix sticky button disappearing on window resize ([#15105](https://github.com/n8n-io/n8n/issues/15105)) ([dcf3267](https://github.com/n8n-io/n8n/commit/dcf32679c3462f5dc3012667dfc2e2de3f96cd80))
* **editor:** Increase hover delay and hit area for canvas toolbar edge ([#15125](https://github.com/n8n-io/n8n/issues/15125)) ([cdcd059](https://github.com/n8n-io/n8n/commit/cdcd0592484e479e2b1aee140d912b22c055ad5e))
* **editor:** Issue with context menu disabling most options when importing template ([#15185](https://github.com/n8n-io/n8n/issues/15185)) ([abb8225](https://github.com/n8n-io/n8n/commit/abb822594453a594d306327817d435771779fad1))
* **editor:** Sort start start nodes for manual execution by Y position ([#15254](https://github.com/n8n-io/n8n/issues/15254)) ([ab27f91](https://github.com/n8n-io/n8n/commit/ab27f91944d6cb27e69f972e52f054a827290608))
* **Google Sheets Node:** Return single row in read operation if combine conditions is OR and 'Return only First Matching Row' ([#15095](https://github.com/n8n-io/n8n/issues/15095)) ([e0f5ba2](https://github.com/n8n-io/n8n/commit/e0f5ba2c67796883a8f284bc3de74caba89270b5))
* **Microsoft Entra ID Node:** Change Micosoft typo with Microsoft ([#14452](https://github.com/n8n-io/n8n/issues/14452)) ([af92117](https://github.com/n8n-io/n8n/commit/af92117e767cad160edfab141001e7f69ce0792d))
* Revert AI nodes batching ([#15129](https://github.com/n8n-io/n8n/issues/15129)) ([939ff97](https://github.com/n8n-io/n8n/commit/939ff97ec4248e610d560c9aea876ad43b147399))


### Features

* Community Nodes in the Nodes Panel ([#13923](https://github.com/n8n-io/n8n/issues/13923)) ([2463842](https://github.com/n8n-io/n8n/commit/24638420bd6183939dfd6ff7f008c225fedb49f9))
* **core:** Archive workflows when removing folders without transfer ([#15057](https://github.com/n8n-io/n8n/issues/15057)) ([403f08b](https://github.com/n8n-io/n8n/commit/403f08b6e36eecc45b734f4e6c594753c1a816b3))
* **core:** Change workflow deletions to soft deletes ([#14894](https://github.com/n8n-io/n8n/issues/14894)) ([3a13139](https://github.com/n8n-io/n8n/commit/3a13139f78891afd14cb585ca26e8f4c9847393d))
* **core:** Check license config for insights max retention ([#15256](https://github.com/n8n-io/n8n/issues/15256)) ([3be0555](https://github.com/n8n-io/n8n/commit/3be05556f9fe11c6b81f89bc94e3c09b7c838078))
* **core:** Implement Insights pruning system ([#14468](https://github.com/n8n-io/n8n/issues/14468)) ([ae27b48](https://github.com/n8n-io/n8n/commit/ae27b48ee7b5d3156b4ea1662826ad2a94c24263))
* **core:** Implement partial execution for all tool nodes ([#15168](https://github.com/n8n-io/n8n/issues/15168)) ([8b467e3](https://github.com/n8n-io/n8n/commit/8b467e3f569514787fc865789fd4bf2387051120))
* **core:** Improve nodeNameToToolName special characters normalization ([#15126](https://github.com/n8n-io/n8n/issues/15126)) ([07e6c7e](https://github.com/n8n-io/n8n/commit/07e6c7e13f1ddac9abaa484f7ee502cd049d49ef))
* **editor:** Allow jumping into sub-workflow with shortkey  ([#15200](https://github.com/n8n-io/n8n/issues/15200)) ([e2b9ada](https://github.com/n8n-io/n8n/commit/e2b9ada4b562426fbe8deeaefe657c1ed2b83362))
* **editor:** Implement 'Shared with you' section in the main navigation ([#15140](https://github.com/n8n-io/n8n/issues/15140)) ([1c65e82](https://github.com/n8n-io/n8n/commit/1c65e82b38b78da73a038e2e43743311c6a0ef12))
* **editor:** Preserve workflow list sort & page size preferences ([#15101](https://github.com/n8n-io/n8n/issues/15101)) ([cf03a28](https://github.com/n8n-io/n8n/commit/cf03a28774ebf495c0762ce4f7ea2a1922f569c4))
* **editor:** Rollout improved log view ([#15202](https://github.com/n8n-io/n8n/issues/15202)) ([8229b0b](https://github.com/n8n-io/n8n/commit/8229b0bcc20f6170d652a06789a9b586ba7a6315))
* **Jina AI Node:** Add Jina AI node ([#15094](https://github.com/n8n-io/n8n/issues/15094)) ([e9ef193](https://github.com/n8n-io/n8n/commit/e9ef193eaa52089da640c6d40f882dd42137efc5))
* **MCP Server Trigger Node:** Handle multiple tool calls in mcp server trigger ([#15064](https://github.com/n8n-io/n8n/issues/15064)) ([59ba162](https://github.com/n8n-io/n8n/commit/59ba162bd9fe9967d0b0733c3955d65256e062f5))
* **n8n AWS Cognito Node:** New node ([#11767](https://github.com/n8n-io/n8n/issues/11767)) ([f6e5efc](https://github.com/n8n-io/n8n/commit/f6e5efc2e0ae7b08d0b9f45948d78af06a9b2e6b))



# [1.92.0](https://github.com/n8n-io/n8n/compare/n8n@1.91.0...n8n@1.92.0) (2025-05-05)


### Bug Fixes

* **core:** Don't create additional `nodeExecuteBefore` message ([#14958](https://github.com/n8n-io/n8n/issues/14958)) ([a33e3a8](https://github.com/n8n-io/n8n/commit/a33e3a807a9dd4c2df6f44b1107c41b949dfe331))
* **core:** Error in partial execution of vector stores ([#15019](https://github.com/n8n-io/n8n/issues/15019)) ([5fa41bd](https://github.com/n8n-io/n8n/commit/5fa41bd73ae57fa0d957541643f0bf9c64a53d8f))
* **core:** Manual execution defaults to Manual trigger ([#15052](https://github.com/n8n-io/n8n/issues/15052)) ([c176063](https://github.com/n8n-io/n8n/commit/c1760631cf86942a8da19d0bf647d2eb70fc0477))
* **core:** Revert back to the extended query-parser on express 5 ([#15016](https://github.com/n8n-io/n8n/issues/15016)) ([9541b5b](https://github.com/n8n-io/n8n/commit/9541b5bb07de0e359159f5fcffbc48e5c6a08162))
* **core:** Use manual tool description if neither resources or operations exist  ([#15093](https://github.com/n8n-io/n8n/issues/15093)) ([1d4f639](https://github.com/n8n-io/n8n/commit/1d4f63985b6802fe0af6fe7862d4215611552d71))
* **editor:**  Close saving modal when workflow is new ([#14836](https://github.com/n8n-io/n8n/issues/14836)) ([48f0c91](https://github.com/n8n-io/n8n/commit/48f0c91a474dda995b5dbd89cdb51905b84ecbd9))
* **editor:** "Trigger node not found" error when chat message is entered ([#14954](https://github.com/n8n-io/n8n/issues/14954)) ([8981e22](https://github.com/n8n-io/n8n/commit/8981e22dd4df2c182fe4d845e7d0cc2677ff2d36))
* **editor:** Hide $fromAI button for exact type matches only ([#14996](https://github.com/n8n-io/n8n/issues/14996)) ([8613521](https://github.com/n8n-io/n8n/commit/8613521aabb95128d762076d15323bb1aa8e9deb))
* **editor:** Import form data with special characters from curl command correctly ([#14898](https://github.com/n8n-io/n8n/issues/14898)) ([3e43f9f](https://github.com/n8n-io/n8n/commit/3e43f9f8bc8542534a17f55e32634034c174a9d8))
* **editor:** Only prompt for MFA code when email is updated ([#15065](https://github.com/n8n-io/n8n/issues/15065)) ([aa4607e](https://github.com/n8n-io/n8n/commit/aa4607e7b5c15f8a6f69b3c900e656f317ebb784))
* **HTTP Request Node:** Add support for Bearer Auth in HttpRequest node ([#15043](https://github.com/n8n-io/n8n/issues/15043)) ([31003aa](https://github.com/n8n-io/n8n/commit/31003aacd15d7219fa87c919dedca7c8be09b1c2))
* **Summarize Node:** Fix spaces in Fields to Split By values converted to underscores ([#15020](https://github.com/n8n-io/n8n/issues/15020)) ([154153d](https://github.com/n8n-io/n8n/commit/154153d86f59552cffe33a1a746cbaf28fc8886f))


### Features

* **Anthropic Chat Model Node:** Add configurable base URL for Anthropic API ([#15063](https://github.com/n8n-io/n8n/issues/15063)) ([4b5f045](https://github.com/n8n-io/n8n/commit/4b5f045281837e7cc29a57a1b9360e87cc3805f7))
* **Azure OpenAI Chat Model Node:** Implement Azure Entra ID OAuth2 Authentication ([#15003](https://github.com/n8n-io/n8n/issues/15003)) ([cf00085](https://github.com/n8n-io/n8n/commit/cf0008500cafd94582720a1445d0468898e71184))
* **Calendly Trigger Node:** Deprecation notice for apiKey authentication ([#15048](https://github.com/n8n-io/n8n/issues/15048)) ([40d0702](https://github.com/n8n-io/n8n/commit/40d0702ed33ef7ffea303957b06e1e953023b559))
* **core:** Add production root executions ([#14845](https://github.com/n8n-io/n8n/issues/14845)) ([7f89244](https://github.com/n8n-io/n8n/commit/7f89244304855748bcd70f495914373369a89cbe))
* **editor:** Add "Rendered" display mode to the logs view ([#14994](https://github.com/n8n-io/n8n/issues/14994)) ([c0b5483](https://github.com/n8n-io/n8n/commit/c0b54832b3e7e7daafcc65c73c15a4cb90d3172a))
* **editor:** Support partial executions of tool nodes ([#14945](https://github.com/n8n-io/n8n/issues/14945)) ([54dcded](https://github.com/n8n-io/n8n/commit/54dcdedecedb0a480caa17f8d6f0447535a2995a))
* **Google Workspace Admin Node:** Google Admin Node Overhaul implementation ([#12271](https://github.com/n8n-io/n8n/issues/12271)) ([8a30c35](https://github.com/n8n-io/n8n/commit/8a30c35c33ad1175a3ee216c86a75ddd786d9887))
* **Jira Software Node:** Migrate from soon deprecated endpoints to get issues ([#14821](https://github.com/n8n-io/n8n/issues/14821)) ([216bdd1](https://github.com/n8n-io/n8n/commit/216bdd15fd94f9a427a86aaf0a9291e7d4df4056))
* Only show workflows shared with you in the overview page ([#14773](https://github.com/n8n-io/n8n/issues/14773)) ([eb46576](https://github.com/n8n-io/n8n/commit/eb465763cf31e1b24e0b2737e15cd1a0478658d9))
* Optimize langchain calls in batching mode ([#15011](https://github.com/n8n-io/n8n/issues/15011)) ([f3e29d2](https://github.com/n8n-io/n8n/commit/f3e29d25ed767d29aebed02a040f57a1cbc05f8d))



# [1.91.0](https://github.com/n8n-io/n8n/compare/n8n@1.90.0...n8n@1.91.0) (2025-04-28)


### Bug Fixes

* **AI Agent Node:** Prevent adding empty binary message ([#14871](https://github.com/n8n-io/n8n/issues/14871)) ([897338b](https://github.com/n8n-io/n8n/commit/897338bd245e33f26fe54bdd4659c8e3a58f1ff3))
* Bring back TidyUp button's icon and fix Easy AI button size ([#14818](https://github.com/n8n-io/n8n/issues/14818)) ([1e5c1fc](https://github.com/n8n-io/n8n/commit/1e5c1fceb70feeae2affdaa1256c018124da07a2))
* **Code Node:** Upgrade pyodide, sandbox it, and prevent JS sandbox escape ([#14356](https://github.com/n8n-io/n8n/issues/14356)) ([6c9c720](https://github.com/n8n-io/n8n/commit/6c9c720ae9496d5f1ea9817241fe257d6be5a10f))
* **core:** Disable insights for sqlite legacy ([#14824](https://github.com/n8n-io/n8n/issues/14824)) ([27f223d](https://github.com/n8n-io/n8n/commit/27f223d294f375a8f5af69557a5c2995e9004486))
* **core:** Error when multiple nodes return items with multiple paired items ([#14883](https://github.com/n8n-io/n8n/issues/14883)) ([ddb688b](https://github.com/n8n-io/n8n/commit/ddb688ba300b231e53a024a190cb7fc4bec3a9e7))
* **core:** Fix task runner's task timeout and heartbeat interval ([#14889](https://github.com/n8n-io/n8n/issues/14889)) ([cdf421e](https://github.com/n8n-io/n8n/commit/cdf421e80f6a8cca276a015e8cb8cb12660b8ee1))
* **core:** Handle infinite max history for insights date range ([#14794](https://github.com/n8n-io/n8n/issues/14794)) ([e83a64b](https://github.com/n8n-io/n8n/commit/e83a64b84a516181f62add011bb763840e5d8f20))
* **core:** Hide task runner warning if Code node is disabled ([#14801](https://github.com/n8n-io/n8n/issues/14801)) ([a217611](https://github.com/n8n-io/n8n/commit/a217611b2a146a0febbb6811e245ec60fb38494c))
* **core:** ID quoting in add scopes migration ([#14788](https://github.com/n8n-io/n8n/issues/14788)) ([f835c66](https://github.com/n8n-io/n8n/commit/f835c66d98abb1b93120e4d624498c40ba410d98))
* **Customer.io Node:** Allow EU customer.io domains in credential ([#14880](https://github.com/n8n-io/n8n/issues/14880)) ([0c7f7b3](https://github.com/n8n-io/n8n/commit/0c7f7b33cb45e39bec481cf731d5206ddd1486fa))
* **editor:** Changes to workflow after execution should not affect logs ([#14703](https://github.com/n8n-io/n8n/issues/14703)) ([84cee1d](https://github.com/n8n-io/n8n/commit/84cee1d12de19755154d415df117117225b7d941))
* **editor:** Data in input/output panel incorrectly mapped ([#14878](https://github.com/n8n-io/n8n/issues/14878)) ([0a2b740](https://github.com/n8n-io/n8n/commit/0a2b740063d4a78592e349ef75e61b3ef5fa9f61))
* **editor:** Fix insights summary banner empty state on time saved tab ([#14838](https://github.com/n8n-io/n8n/issues/14838)) ([2920381](https://github.com/n8n-io/n8n/commit/29203819031b80110259f15415caec9806e27c60))
* **editor:** Fix schema view bugs ([#14734](https://github.com/n8n-io/n8n/issues/14734)) ([022f475](https://github.com/n8n-io/n8n/commit/022f4755c2fe34a5ff446bfa7acb1e5324104740))
* **editor:** Handle if nodes are undefined/null in InputNodeSelect ([#14860](https://github.com/n8n-io/n8n/issues/14860)) ([67240ee](https://github.com/n8n-io/n8n/commit/67240ee069e55f09563f994c7c7729a1399c62db))
* **editor:** Ignore unconnected nodes when executing workflow ([#14683](https://github.com/n8n-io/n8n/issues/14683)) ([f743915](https://github.com/n8n-io/n8n/commit/f743915cc9940b2cc49a7cb617a84c8cb78a4070))
* **editor:** Only show previews if the param is an expression ([#14720](https://github.com/n8n-io/n8n/issues/14720)) ([db887b6](https://github.com/n8n-io/n8n/commit/db887b6f29ca627683c55b497f7410e435d47c3d))
* **editor:** Open NDV from logs view with correct run index ([#14779](https://github.com/n8n-io/n8n/issues/14779)) ([82b7be5](https://github.com/n8n-io/n8n/commit/82b7be5d2964ca7fc610aa7ff4f9b10c513fe2fc))
* **editor:** Place duplicated WFs always to correct parent folders ([#14713](https://github.com/n8n-io/n8n/issues/14713)) ([6c91e7e](https://github.com/n8n-io/n8n/commit/6c91e7e1b797e242afabe7e0ef4f9188b2d71cc6))
* **editor:** Show Transform Node in Panel only if available ([#14830](https://github.com/n8n-io/n8n/issues/14830)) ([92e2a8e](https://github.com/n8n-io/n8n/commit/92e2a8e61a4189025e5d4bac8be81576b624fe85))
* **editor:** Styling/UX improvements on the new logs view ([#14789](https://github.com/n8n-io/n8n/issues/14789)) ([454e5c7](https://github.com/n8n-io/n8n/commit/454e5c77ade0d412eb2de1719a58a07fffcc4649))
* **editor:** Use redirect url also with SSO login ([#14893](https://github.com/n8n-io/n8n/issues/14893)) ([6145790](https://github.com/n8n-io/n8n/commit/614579026dca75efbf1026a7017931f6971760b5))
* **Google Sheets Trigger Node:** Filter by first data row on `rowAdded` event  ([#14731](https://github.com/n8n-io/n8n/issues/14731)) ([1593fe3](https://github.com/n8n-io/n8n/commit/1593fe3de51b337d25fd35876202f71503006f8d))
* **Jira Software Node:** 403 when getting a list of items from Jira Cloud ([#14782](https://github.com/n8n-io/n8n/issues/14782)) ([1cbbcf4](https://github.com/n8n-io/n8n/commit/1cbbcf4a7726f38936a8fceeee8d635a212b0764))
* **n8n Form Node:** Use binary response from latest node in execution ([#14842](https://github.com/n8n-io/n8n/issues/14842)) ([9672a6d](https://github.com/n8n-io/n8n/commit/9672a6db0a3211ea27b658c9a2ab55053b1c3475))
* **n8n Split In Batches Node:** Rewrite hint for reset ([#14844](https://github.com/n8n-io/n8n/issues/14844)) ([9029f34](https://github.com/n8n-io/n8n/commit/9029f34bfdba79a5970b1ec680c3ebea11b6a7e4))
* **Text Classifier Node:** Validate inputText parameter ([#14832](https://github.com/n8n-io/n8n/issues/14832)) ([9021e19](https://github.com/n8n-io/n8n/commit/9021e195fa945ce92822d0afb0654808b2ff67b7))


### Features

* **core:** Add insights date ranges option to frontend settings ([#14792](https://github.com/n8n-io/n8n/issues/14792)) ([65d6b23](https://github.com/n8n-io/n8n/commit/65d6b2382df8d4382bcb9aac7e2e7d2192e457c0))
* **core:** Add InstanceRole auth support for AWS external secrets ([#14799](https://github.com/n8n-io/n8n/issues/14799)) ([8c4b9f7](https://github.com/n8n-io/n8n/commit/8c4b9f73f1bfc1d4e28ef0a38efe02627e15ac2f))
* **core:** Add InstanceRole auth support for binary-data object- storage backend ([#14800](https://github.com/n8n-io/n8n/issues/14800)) ([271024d](https://github.com/n8n-io/n8n/commit/271024ded0d55aa97daaf52cb8051abee36ad474))
* **core:** Allow setting folder destination when transferring workflow ownership ([#14935](https://github.com/n8n-io/n8n/issues/14935)) ([dbffcdc](https://github.com/n8n-io/n8n/commit/dbffcdc2ff4bf795995f53bc1a5166c4901b3320))
* **core:** Enable insights for sqlite legacy ([#14606](https://github.com/n8n-io/n8n/issues/14606)) ([88ed7be](https://github.com/n8n-io/n8n/commit/88ed7beff2bf3aaa00258dd06715d52ac129f1ca))
* **core:** Export new dto and schemas ([#14828](https://github.com/n8n-io/n8n/issues/14828)) ([9082adf](https://github.com/n8n-io/n8n/commit/9082adf89a821ab318d4767598275dac755b0918))
* **core:** Implement granularity and date range filtering on insights ([#14841](https://github.com/n8n-io/n8n/issues/14841)) ([28596a6](https://github.com/n8n-io/n8n/commit/28596a633ec336178409c0604dcfe69f13d2c869))
* **core:** Split insights service ([#14469](https://github.com/n8n-io/n8n/issues/14469)) ([eaf6783](https://github.com/n8n-io/n8n/commit/eaf6783eb54216aa3ba0f4d6871cc1d52095c5d7))
* **editor:** Add support for automatic expression switching to RLC ([#14735](https://github.com/n8n-io/n8n/issues/14735)) ([6b344f8](https://github.com/n8n-io/n8n/commit/6b344f8a7e74d6ac902457953cc1dcdfb2435da3))
* **editor:** Add time range selector to Insights ([#14877](https://github.com/n8n-io/n8n/issues/14877)) ([bfd85dd](https://github.com/n8n-io/n8n/commit/bfd85dd3c9afc02b427c16fa0241db5be1b3a6c4))
* **editor:** Include NodeDetailsView in URL ([#14349](https://github.com/n8n-io/n8n/issues/14349)) ([5ff073b](https://github.com/n8n-io/n8n/commit/5ff073bd7be80dcb857fd80f9637545e058397bb))
* **editor:** Show workflow breadcrumbs in canvas ([#14710](https://github.com/n8n-io/n8n/issues/14710)) ([46df8b4](https://github.com/n8n-io/n8n/commit/46df8b47d6ee2ad685a51c8b805ceeb230e4fe25))
* Group memory nodes into section in nodes panel ([#14826](https://github.com/n8n-io/n8n/issues/14826)) ([6197b0c](https://github.com/n8n-io/n8n/commit/6197b0cb6d668ac6b13e17c3765c7fa458cd0362))
* **OpenAI Node:** Filter available models by blacklisting rather than whitelisting ([#14780](https://github.com/n8n-io/n8n/issues/14780)) ([0e2eceb](https://github.com/n8n-io/n8n/commit/0e2eceb33f0a605173ba7e16fe9ac0b4cf8dcaa5))
* **OpenAI Node:** Support gpt-image-1 for image generation ([#14870](https://github.com/n8n-io/n8n/issues/14870)) ([11379bf](https://github.com/n8n-io/n8n/commit/11379bf656d50d30b8b1dfbeb03d9c64aaf8b26d))
* Prevent webhook url takeover ([#14783](https://github.com/n8n-io/n8n/issues/14783)) ([be53453](https://github.com/n8n-io/n8n/commit/be53453def4169a5598069218c8e58e6409d5a60))
* Refresh workflow name in workflows selector when updated ([#14705](https://github.com/n8n-io/n8n/issues/14705)) ([418a588](https://github.com/n8n-io/n8n/commit/418a588e8965c8b994051059a5ae8dbc2c87b860))


### Performance Improvements

* **editor:** Improve performance of the new logs view ([#14861](https://github.com/n8n-io/n8n/issues/14861)) ([40aadbf](https://github.com/n8n-io/n8n/commit/40aadbf880e525aedfbe8a89f0a2b78e298357bc))



# [1.90.0](https://github.com/n8n-io/n8n/compare/n8n@1.89.0...n8n@1.90.0) (2025-04-21)


### Bug Fixes

* AWS credential signing http request - convert form to body ([#14060](https://github.com/n8n-io/n8n/issues/14060)) ([652d0f5](https://github.com/n8n-io/n8n/commit/652d0f5428c1aecab25dcdb99487941310599a2a))
* **core:** Allow `$evaluateExpression` to resolve in task runners ([#14641](https://github.com/n8n-io/n8n/issues/14641)) ([7c1be05](https://github.com/n8n-io/n8n/commit/7c1be0584577621702e5ec39162881afee0cfd90))
* **core:** Fix missing encryption key check on workers ([#14603](https://github.com/n8n-io/n8n/issues/14603)) ([de03452](https://github.com/n8n-io/n8n/commit/de034526310639a4451f356b7a6ad0f01fb3fe51))
* **core:** Fix using secrets for credentials on oauth callback ([#14711](https://github.com/n8n-io/n8n/issues/14711)) ([09806c3](https://github.com/n8n-io/n8n/commit/09806c36ae0ae9f4b590999e83b90e9b42651eec))
* **core:** Handle task runner accept timeout error ([#14709](https://github.com/n8n-io/n8n/issues/14709)) ([a93dd53](https://github.com/n8n-io/n8n/commit/a93dd53a3b16118dbe7d5463d90f2406d0660134))
* **core:** Only check for folder changes when `parentFolderId` is present ([#14618](https://github.com/n8n-io/n8n/issues/14618)) ([08e73d3](https://github.com/n8n-io/n8n/commit/08e73d3aed5e706ebab9abb8895bbd9f5314c978))
* **core:** Prefer triggers with run data during partial executions ([#14691](https://github.com/n8n-io/n8n/issues/14691)) ([ddfe594](https://github.com/n8n-io/n8n/commit/ddfe594cf0486ed64d0ddc58e634ae6dbceb72e7))
* **core:** Propagate env to task runner ([#14638](https://github.com/n8n-io/n8n/issues/14638)) ([8e26d55](https://github.com/n8n-io/n8n/commit/8e26d5514d14e16e6f2777805dad372127b4a932))
* **core:** Reschedule Insights flushing after skipping for empty buffer ([#14637](https://github.com/n8n-io/n8n/issues/14637)) ([513f20a](https://github.com/n8n-io/n8n/commit/513f20a902c526ca8bd137f9c3189970e8b97243))
* **editor:** Account for `$evaluateExpression` in Codemirror ([#14643](https://github.com/n8n-io/n8n/issues/14643)) ([68a8761](https://github.com/n8n-io/n8n/commit/68a87619afa6ef1c0b1d4e9dcabe9fee9bb82321))
* **editor:** Allow long links on rendered markdown split to multiple lines ([#14635](https://github.com/n8n-io/n8n/issues/14635)) ([b80d753](https://github.com/n8n-io/n8n/commit/b80d7531d4cbc920950ff5445d821512dd5dd5ec))
* **editor:** Differentiate $fromAI overrides within lists ([#14696](https://github.com/n8n-io/n8n/issues/14696)) ([5aa6054](https://github.com/n8n-io/n8n/commit/5aa6054bc96fce1eb798d639d1a37ae2eff78455))
* **editor:** Fix expanding schema items with same names on NDV ([#14673](https://github.com/n8n-io/n8n/issues/14673)) ([ad386cd](https://github.com/n8n-io/n8n/commit/ad386cde31bf30084f49a8d0231ef49f50374fa7))
* **editor:** Fix Insights display time saved from minutes ([#14622](https://github.com/n8n-io/n8n/issues/14622)) ([6dd7756](https://github.com/n8n-io/n8n/commit/6dd7756191623e2d11f64d04ba21481505f923ad))
* **editor:** Fix same order of buttons in run data selector ([#14677](https://github.com/n8n-io/n8n/issues/14677)) ([74de403](https://github.com/n8n-io/n8n/commit/74de4037be7f46c9ce9f5fa844c8182f6f38ed16))
* **editor:** Fix updating of canvas node issue when credential is set-up ([#14633](https://github.com/n8n-io/n8n/issues/14633)) ([bc26923](https://github.com/n8n-io/n8n/commit/bc269234cf2b78f6887a272baa4563c482ed1597))
* **editor:** Highlight the suggested data type with bold in the Filter node ([#14707](https://github.com/n8n-io/n8n/issues/14707)) ([8325ca1](https://github.com/n8n-io/n8n/commit/8325ca1a4533ff8e5f79a19aafa89f9ed7d47e0d))
* **editor:** Improve handling of trailing 'Trigger' in NodeCreator search ([#14612](https://github.com/n8n-io/n8n/issues/14612)) ([8b3b474](https://github.com/n8n-io/n8n/commit/8b3b4749eaf5ff401f1d6499c95da00094e9c9d2))
* **editor:** Restrict what binary-data types can be viewed in the UI ([#14685](https://github.com/n8n-io/n8n/issues/14685)) ([11a36b7](https://github.com/n8n-io/n8n/commit/11a36b758df38e16a2c2c258628bf58a030a12d7))
* **editor:** Show `Execute previous Node` panel after disabled node in Schema view ([#14443](https://github.com/n8n-io/n8n/issues/14443)) ([a12c952](https://github.com/n8n-io/n8n/commit/a12c9522d5992a7fc2719644a9cfa4af5cdc3712))
* Fix issue with open router credential test ([#14440](https://github.com/n8n-io/n8n/issues/14440)) ([4362f37](https://github.com/n8n-io/n8n/commit/4362f37df2aed8f4aa8ef22cd8ab0df971ea9a9f))
* **Freshdesk Node:** Fix types issue ([#14730](https://github.com/n8n-io/n8n/issues/14730)) ([38eaef9](https://github.com/n8n-io/n8n/commit/38eaef97fe798037cac8e33455584639a03a531f))
* **HubSpot Node:** Include item index in error messages ([#14704](https://github.com/n8n-io/n8n/issues/14704)) ([e6f26b8](https://github.com/n8n-io/n8n/commit/e6f26b895de0dd3d204c88c10b47286ab63d5f64))
* **LinkedIn Node:** API version update ([#14697](https://github.com/n8n-io/n8n/issues/14697)) ([77e2ac6](https://github.com/n8n-io/n8n/commit/77e2ac64950c6dc7e8d61702e1fc1d66d4730990))
* **MCP Client Tool Node:** Stringify tool result ([#14554](https://github.com/n8n-io/n8n/issues/14554)) ([390c508](https://github.com/n8n-io/n8n/commit/390c5089463ed7aada32a32b1fb34ddf454f7faa))
* **n8n Form Trigger Node:** Remove relience on getWorkflowStaticData for passing query parameters ([#14728](https://github.com/n8n-io/n8n/issues/14728)) ([3feab31](https://github.com/n8n-io/n8n/commit/3feab31792fe4426f58af89009bf39a1bee0213a))
* **Postgres Node:** Fix inserting `null` or `undefined` in `type=json` columns ([#14672](https://github.com/n8n-io/n8n/issues/14672)) ([3add0b8](https://github.com/n8n-io/n8n/commit/3add0b82ba2e77a0416ea273184aceeabfae2a57))
* **Respond to Webhook Node:** Disable expressions in Respond With ([#14727](https://github.com/n8n-io/n8n/issues/14727)) ([fec2284](https://github.com/n8n-io/n8n/commit/fec2284a779917f4d53d05e9b107a977655999e4))
* **Wait Node:** Fix wait node tests by always using a future date ([#14733](https://github.com/n8n-io/n8n/issues/14733)) ([81d08ad](https://github.com/n8n-io/n8n/commit/81d08ad1de4ccfa56b020afc69da2b85f7b1149e))
* **Wait Node:** Validate datetime for specific time mode ([#14701](https://github.com/n8n-io/n8n/issues/14701)) ([3641c1f](https://github.com/n8n-io/n8n/commit/3641c1fb8738471c2ad68d2882ab299506fca4a1))


### Features

* **core:** Add scopes to API Keys ([#14176](https://github.com/n8n-io/n8n/issues/14176)) ([e1b9407](https://github.com/n8n-io/n8n/commit/e1b9407fe9c742c4f050a721f182dfe494101d84))
* **core:** Add support for signed URLs for binary data ([#14492](https://github.com/n8n-io/n8n/issues/14492)) ([7723a13](https://github.com/n8n-io/n8n/commit/7723a138a1f411566ddb0499ac0806ae2cac53e7))
* **editor:** Add drag n drop support for folders ([#14549](https://github.com/n8n-io/n8n/issues/14549)) ([57444d3](https://github.com/n8n-io/n8n/commit/57444d3a16d77aabf3bd4d3835d86eca7aeff8f7))
* **editor:** Align `DynamicStructuredTool` and `DynamicTool` name fields ([#14604](https://github.com/n8n-io/n8n/issues/14604)) ([302258d](https://github.com/n8n-io/n8n/commit/302258dda2d6bb9c8712cb5fbc5d36dd91c6c261))
* **editor:** Fix paywall for dashboard disabled licences ([#14617](https://github.com/n8n-io/n8n/issues/14617)) ([46d9b60](https://github.com/n8n-io/n8n/commit/46d9b6004984bec75687a1b5ffdb3c28868eedb6))
* **editor:** Log details panel ([#14409](https://github.com/n8n-io/n8n/issues/14409)) ([1e0853b](https://github.com/n8n-io/n8n/commit/1e0853b24aa3070805cf9cc7694faf30772ea7ef))
* **editor:** Show logs panel in execution history page ([#14477](https://github.com/n8n-io/n8n/issues/14477)) ([ed19f0f](https://github.com/n8n-io/n8n/commit/ed19f0f39b2a5d4daa67a0645bb82ce0e71968fb))
* **HTTP Request Node:** Replace HttpRequest Tool with tool version of standalone HttpRequest Node ([#14669](https://github.com/n8n-io/n8n/issues/14669)) ([a8fee9a](https://github.com/n8n-io/n8n/commit/a8fee9a4f3e80d9d651fe39927db14f261761648))
* Option to skip validation in getNodeParameter ([#14726](https://github.com/n8n-io/n8n/issues/14726)) ([b615e51](https://github.com/n8n-io/n8n/commit/b615e51f1319130c3a0f918e882aa3ae3bf5a4f2))
* Resolve `parentFolder` when retrieving workflow ([#14656](https://github.com/n8n-io/n8n/issues/14656)) ([bc12f66](https://github.com/n8n-io/n8n/commit/bc12f662e76c435bf385c62823259c626bcafe79))
* **Supabase Node:** Add support for database schema ([#13339](https://github.com/n8n-io/n8n/issues/13339)) ([23f25ce](https://github.com/n8n-io/n8n/commit/23f25cefbfcefbdb0cf74af384f9cda20ced518f))


### Performance Improvements

* **core:** Reuse context in `runOnceForEachItem` mode in task runner ([#14682](https://github.com/n8n-io/n8n/issues/14682)) ([ff47279](https://github.com/n8n-io/n8n/commit/ff47279b25b4a5dc3a224945cb05d53b5e80a7ed))



# [1.89.0](https://github.com/n8n-io/n8n/compare/n8n@1.88.0...n8n@1.89.0) (2025-04-14)


### Bug Fixes

* **AI Agent Node:** Allow removal of system message ([#14407](https://github.com/n8n-io/n8n/issues/14407)) ([2451ead](https://github.com/n8n-io/n8n/commit/2451ead9f3028ed290e5d76ac6fd5b203e4b51db))
* **core:** Restore run data value when offloading to workers ([#14516](https://github.com/n8n-io/n8n/issues/14516)) ([313cfec](https://github.com/n8n-io/n8n/commit/313cfec74da58dc2403d828a2a211c6c4004f7df))
* **core:** Schema parsing bypassing config key assignment ([#14556](https://github.com/n8n-io/n8n/issues/14556)) ([d390258](https://github.com/n8n-io/n8n/commit/d39025800106b4a406fa34332367775d20c54545))
* **core:** Validate task runner mode ([#14376](https://github.com/n8n-io/n8n/issues/14376)) ([52170f1](https://github.com/n8n-io/n8n/commit/52170f1bbc48f2b7ddcb05d7a6fb4f9c1762a3c6))
* **editor:** Add telemetry to Insights ([#14511](https://github.com/n8n-io/n8n/issues/14511)) ([2fb970a](https://github.com/n8n-io/n8n/commit/2fb970aaa1ed7cf588f9e52ee21814fb5fb4e07f))
* **editor:** Implement insight's design feedback 4 ([#14550](https://github.com/n8n-io/n8n/issues/14550)) ([cc089be](https://github.com/n8n-io/n8n/commit/cc089bebd4e12fd9c3690c53568cb0100c838be4))
* **editor:** Schema preview displays for some empty nodes ([#14488](https://github.com/n8n-io/n8n/issues/14488)) ([8c35229](https://github.com/n8n-io/n8n/commit/8c352293b576285d6b371efea72ed31ce274f9a2))
* Fix issue with Qdrant not always connecting ([#14328](https://github.com/n8n-io/n8n/issues/14328)) ([6748db9](https://github.com/n8n-io/n8n/commit/6748db9c3b104aae23c6c3f432e3ac61b5dbef1c))
* **Summarize Node:** Fix property key with dot notation ([#14528](https://github.com/n8n-io/n8n/issues/14528)) ([c890108](https://github.com/n8n-io/n8n/commit/c89010871d28e2cc4d5807fb7b3aa29968a0364c))
* **xAI Grok Chat Model Node:** Remove stream_options parameter ([#14496](https://github.com/n8n-io/n8n/issues/14496)) ([8c417d7](https://github.com/n8n-io/n8n/commit/8c417d7b1b7473cdca0f74bffa41aa87321d808e))


### Features

* Add nested search in folders ([#14372](https://github.com/n8n-io/n8n/issues/14372)) ([cade309](https://github.com/n8n-io/n8n/commit/cade309d3b972bb7be364c42869d2cd11a0e121a))
* **API:** Add user id information on push tracking when available ([#14519](https://github.com/n8n-io/n8n/issues/14519)) ([6195789](https://github.com/n8n-io/n8n/commit/61957899e1ca9c013dbd0c3385f9484d724df3a0))
* **API:** Match insights summary period with number of days filter in graphs and table ([#14500](https://github.com/n8n-io/n8n/issues/14500)) ([ec73958](https://github.com/n8n-io/n8n/commit/ec73958797d1a0a821eda9501507c849859d39a9))
* **core:** Add a new option to customize SSH tunnel idle timeout ([#14522](https://github.com/n8n-io/n8n/issues/14522)) ([965baae](https://github.com/n8n-io/n8n/commit/965baae093c22d2a67a1e4d76c85da9910806994))
* **core:** Handle disabled modules logic and db engine dependent default for insights ([#14243](https://github.com/n8n-io/n8n/issues/14243)) ([b568caa](https://github.com/n8n-io/n8n/commit/b568caa209c92cb3998243562f22706d7e0f235b))
* **core:** Make runtime prototype mutation protection configurable for task runner ([#14515](https://github.com/n8n-io/n8n/issues/14515)) ([d6ae388](https://github.com/n8n-io/n8n/commit/d6ae3889ca48e29469a372396550798678f7bd14))
* **editor:** Make logs applicable for all nodes ([#14397](https://github.com/n8n-io/n8n/issues/14397)) ([d24b684](https://github.com/n8n-io/n8n/commit/d24b684a9520ab8bf14d3496fa3d12adf92ad317))
* **editor:** Show specific content when 0 data on insights ([#14609](https://github.com/n8n-io/n8n/issues/14609)) ([296d5b4](https://github.com/n8n-io/n8n/commit/296d5b4a7f3c5740cdbd2208132124481274caf0))
* **editor:** Tweak nodes panel to update AI category name and highlight AI Transform node ([#14608](https://github.com/n8n-io/n8n/issues/14608)) ([9c34e3d](https://github.com/n8n-io/n8n/commit/9c34e3d534e46191a82d99b23786f0bba945a2fb))
* **Salesforce Node:** Add credentials test ([#14486](https://github.com/n8n-io/n8n/issues/14486)) ([6b2d31c](https://github.com/n8n-io/n8n/commit/6b2d31ca2b40869e1b16982db0a202a7b4e41eba))
* **SearXNG Node:** Add SearXNG tool ([#13218](https://github.com/n8n-io/n8n/issues/13218)) ([0b46055](https://github.com/n8n-io/n8n/commit/0b460552bae3feb1394fd62a0b977204246c4397))
* Update Easy AI workflow ([#14521](https://github.com/n8n-io/n8n/issues/14521)) ([53812a5](https://github.com/n8n-io/n8n/commit/53812a544f00ac71ab79c77bdc2c978bf801bec9))



# [1.88.0](https://github.com/n8n-io/n8n/compare/n8n@1.87.0...n8n@1.88.0) (2025-04-10)


### Bug Fixes

* **API:** Fix ratio tests on insights by workflow ([#14448](https://github.com/n8n-io/n8n/issues/14448)) ([6c73d7e](https://github.com/n8n-io/n8n/commit/6c73d7ed812521f64a4db9a5437f2596953f204d))
* **Code Node:** Use an explicit `indexURL` to load the pyodide runtime ([#14487](https://github.com/n8n-io/n8n/issues/14487)) ([860bb1e](https://github.com/n8n-io/n8n/commit/860bb1ef92bbe4e6fa6f8478dfde37c8e498af65))
* **core:** Fall back to regular mode for `execute` and `executeBatch` commands ([#14381](https://github.com/n8n-io/n8n/issues/14381)) ([84e85c9](https://github.com/n8n-io/n8n/commit/84e85c9469e0417de2d8960a5aa6a91807690e91))
* **core:** Fix routing for waiting webhooks and forms ([#14470](https://github.com/n8n-io/n8n/issues/14470)) ([b5d5b57](https://github.com/n8n-io/n8n/commit/b5d5b5711838fc5a1b63edce4f7fb8dc0a087883))
* **editor:** Fix race condition for updating node and workflow execution status ([#14353](https://github.com/n8n-io/n8n/issues/14353)) ([a495d81](https://github.com/n8n-io/n8n/commit/a495d81c13e9a2721d4900db94d4a9765b0795c2))
* **editor:** Improve node creator items typing and fix missing icons ([#14449](https://github.com/n8n-io/n8n/issues/14449)) ([ad6c83a](https://github.com/n8n-io/n8n/commit/ad6c83afd48dd4f75873231e20316d730a678fdc))
* **editor:** Inline expression previews are not displayed in NDV ([#14475](https://github.com/n8n-io/n8n/issues/14475)) ([aee83bf](https://github.com/n8n-io/n8n/commit/aee83bf3449f275a90d3e51e5bb10e59edd31135))
* **editor:** Prevent moving non owned workflows to folders ([#14474](https://github.com/n8n-io/n8n/issues/14474)) ([2a5c3d4](https://github.com/n8n-io/n8n/commit/2a5c3d49900e8e3e2dee5f19c3922ccc017bd1d7))
* Isolate license SDK proxy settings to avoid affecting unrelated requests ([#14451](https://github.com/n8n-io/n8n/issues/14451)) ([7463f0c](https://github.com/n8n-io/n8n/commit/7463f0c18a67e8e89144bd3e29bba21f245c7a94))


### Features

* **Azure Cosmos DB Node:** New node ([#14156](https://github.com/n8n-io/n8n/issues/14156)) ([b52f9f0](https://github.com/n8n-io/n8n/commit/b52f9f0f6cbd96005f6f81a522955a47379316e1))
* **Email Trigger (IMAP) Node:** IMAP trigger node returns message UIDs ([#13152](https://github.com/n8n-io/n8n/issues/13152)) ([4578709](https://github.com/n8n-io/n8n/commit/457870953aadb54578912abb234c9d546ccbaca2))
* **MCP Client Tool Node:** Add MCP Client Tool Node to connect to MCP servers over SSE ([#14464](https://github.com/n8n-io/n8n/issues/14464)) ([34252f5](https://github.com/n8n-io/n8n/commit/34252f53f9ca586c15f40713678074a358d877f1))
* **MCP Server Trigger Node:** Add MCP Server Trigger node to expose tools to MCP clients ([#14403](https://github.com/n8n-io/n8n/issues/14403)) ([8360283](https://github.com/n8n-io/n8n/commit/8360283c6f28f8d3e7cc60ae1a3982964954cf79))
* **Milvus Vector Store Node:** Add support for the Milvus vector db ([#14404](https://github.com/n8n-io/n8n/issues/14404)) ([048b9d7](https://github.com/n8n-io/n8n/commit/048b9d75890bf27e1dbfbd2862d7377a35e15434))


### Performance Improvements

* **core:** Batch raw insights save and add metadata cache ([#14261](https://github.com/n8n-io/n8n/issues/14261)) ([60afb46](https://github.com/n8n-io/n8n/commit/60afb46094ea11f2479130867ae2409f171e9f09))



# [1.87.0](https://github.com/n8n-io/n8n/compare/n8n@1.86.0...n8n@1.87.0) (2025-04-07)


### Bug Fixes

* **API:** Insights - round failure rate to 3 decimals ([#14325](https://github.com/n8n-io/n8n/issues/14325)) ([cf37ee3](https://github.com/n8n-io/n8n/commit/cf37ee3cedb60dc9bbf6c87c7f6212213c93c61e))
* **Code Node:** Ensure 'Generate Code' works with empty input object  ([#14352](https://github.com/n8n-io/n8n/issues/14352)) ([480b44d](https://github.com/n8n-io/n8n/commit/480b44d0245484fc1554051728a1cb34672a361f))
* **core:** Add cross-origin checks on push endpoints ([#14365](https://github.com/n8n-io/n8n/issues/14365)) ([178628a](https://github.com/n8n-io/n8n/commit/178628a59b322543ac05c0fdf9c62c59c72380b3))
* **core:** Detach workflow from parent folder in source project when transferring ownership ([#14414](https://github.com/n8n-io/n8n/issues/14414)) ([adbfb44](https://github.com/n8n-io/n8n/commit/adbfb44c26681f8ee6ca94867d3a778bfb2f10a1))
* **core:** Return correct trigger count for nodes with multiple webhooks ([#14300](https://github.com/n8n-io/n8n/issues/14300)) ([39e2d35](https://github.com/n8n-io/n8n/commit/39e2d35a710307b9e4d170c3a71eeccc34a08738))
* **core:** Sandbox HTML binary files in viewing mode ([#14350](https://github.com/n8n-io/n8n/issues/14350)) ([9c8a5f9](https://github.com/n8n-io/n8n/commit/9c8a5f9c57e65a56a3b7da5dfa805d23c55e5ee3))
* **core:** Upgrade swagger/openai setup to address CVE-2024-57083 ([#14314](https://github.com/n8n-io/n8n/issues/14314)) ([4a95035](https://github.com/n8n-io/n8n/commit/4a95035b3a46565d04d5c89879ed6f9fd0bb6923))
* Disable autocomplete expression for specialized editor types ([#14344](https://github.com/n8n-io/n8n/issues/14344)) ([0450542](https://github.com/n8n-io/n8n/commit/04505421709f12fda79d3e0eed50baada717cea1))
* **editor:** Autofocus Search in Move Folder Dialog ([#14378](https://github.com/n8n-io/n8n/issues/14378)) ([d60ed74](https://github.com/n8n-io/n8n/commit/d60ed746bb5477498ab29d5c8b6b7fc63e6065e5))
* **editor:** Change label for unexecuted nodes ([#14260](https://github.com/n8n-io/n8n/issues/14260)) ([08450b2](https://github.com/n8n-io/n8n/commit/08450b20af0535cf643dc945867602635ce21e6a))
* **editor:** Disable Drag and Drop for ResourceMapper 'attemptToConvertTypes' switch ([#14327](https://github.com/n8n-io/n8n/issues/14327)) ([64aeb37](https://github.com/n8n-io/n8n/commit/64aeb378140dd2e4f0ae7bfe499062403324c992))
* **editor:** Fix empty objects in schema view in output panel ([#14355](https://github.com/n8n-io/n8n/issues/14355)) ([2f0b5e4](https://github.com/n8n-io/n8n/commit/2f0b5e488ef70cd0ebec4bc2599c42da281265be))
* **editor:** Fix search highlights on node details view table schema ([#14379](https://github.com/n8n-io/n8n/issues/14379)) ([3d64d14](https://github.com/n8n-io/n8n/commit/3d64d140e9eb4cd9fc58c673a307cf1ac83654b5))
* **editor:** Hide node toolbar on `AddNodes` node type ([#14317](https://github.com/n8n-io/n8n/issues/14317)) ([a245a5c](https://github.com/n8n-io/n8n/commit/a245a5ca61fb33c86b2727fe8d1866bc6c4c868c))
* **editor:** Improve sub-workflow debugging for more node error types ([#14347](https://github.com/n8n-io/n8n/issues/14347)) ([9104743](https://github.com/n8n-io/n8n/commit/9104743a5fb4305eeccec55f35ea9555c0a9a979))
* **editor:** Insights FE fixes and improvements ([#14398](https://github.com/n8n-io/n8n/issues/14398)) ([e8a7acd](https://github.com/n8n-io/n8n/commit/e8a7acda6bf656b8e2da08a502cc6d4dc64895a6))
* **editor:** Make styling of search labels inline ([#14323](https://github.com/n8n-io/n8n/issues/14323)) ([8abbc30](https://github.com/n8n-io/n8n/commit/8abbc304f013bbbd63982f47fde22230592063a2))
* **editor:** Memory getting rendered in chat on workflow load ([#14346](https://github.com/n8n-io/n8n/issues/14346)) ([5382531](https://github.com/n8n-io/n8n/commit/538253197079e92117943a6e18021094ddda76fa))
* **editor:** Support 'View Execution' links with multiple branches ([#14345](https://github.com/n8n-io/n8n/issues/14345)) ([744e2da](https://github.com/n8n-io/n8n/commit/744e2da3f9e3af6e5d20827a965bcfb01acd7cdc))
* **Google Sheets Node:** Improve error message when row_number is null or undefined ([#14229](https://github.com/n8n-io/n8n/issues/14229)) ([c5e2d2d](https://github.com/n8n-io/n8n/commit/c5e2d2dddcea53c9896113e41eb66ca4d01e124b))
* **HTTP Request Tool Node:** Fix OAuth2 requests ([#14380](https://github.com/n8n-io/n8n/issues/14380)) ([7cef314](https://github.com/n8n-io/n8n/commit/7cef314535bbbf59f26916206a066bfe3d5591f9))
* **Jira Trigger Node:** Fix Jira webhook subscriptions on Jira v10+ ([#14333](https://github.com/n8n-io/n8n/issues/14333)) ([cd212e4](https://github.com/n8n-io/n8n/commit/cd212e4f78f6704a8b2f1a27f507dcc7784ef6a5))
* **Kafka Node:** Upgrade kafkajs and add tests ([#14326](https://github.com/n8n-io/n8n/issues/14326)) ([5c58e8e](https://github.com/n8n-io/n8n/commit/5c58e8e8cfe5d04917b29d3d7ab9c14c27d95fdf))
* **n8n Form Node:** Add doctype to page ([#14306](https://github.com/n8n-io/n8n/issues/14306)) ([df9ea09](https://github.com/n8n-io/n8n/commit/df9ea095fcc4b0fceb8a11c611396ef31a0c4fca))
* **n8n Form Node:** Remove field requirement and do not inherit description ([#14254](https://github.com/n8n-io/n8n/issues/14254)) ([4bc1c1a](https://github.com/n8n-io/n8n/commit/4bc1c1a547abd1bfff1c43c93f77c33aa1b2ccc7))
* **Pipedrive Trigger Node:** Add support for webhooks v2 ([#14220](https://github.com/n8n-io/n8n/issues/14220)) ([a39502f](https://github.com/n8n-io/n8n/commit/a39502f3bb28d566df284cebf5a12c99b41d103f))
* Show correct message on retry ([#14321](https://github.com/n8n-io/n8n/issues/14321)) ([501963f](https://github.com/n8n-io/n8n/commit/501963f568a6e0a5f9782fe10ad0c2e9aaf6756c))


### Features

* Add example `@n8n/n8n-extension-insights` extension package ([#14360](https://github.com/n8n-io/n8n/issues/14360)) ([b91be49](https://github.com/n8n-io/n8n/commit/b91be496c3c36a8bfe61b57943ea890554e0df3a))
* Add support for google vertex embeddings ([#14359](https://github.com/n8n-io/n8n/issues/14359)) ([85cbfb6](https://github.com/n8n-io/n8n/commit/85cbfb64c0a2645c833c73a03624fdfd0adf2dab))
* **Airtop Node:** Add Airtop node ([#13809](https://github.com/n8n-io/n8n/issues/13809)) ([a7a165d](https://github.com/n8n-io/n8n/commit/a7a165dda259e2626a94c220eb0ffab166544485))
* **API:** Add config to set age threshold for insights compaction ([#14221](https://github.com/n8n-io/n8n/issues/14221)) ([17a829f](https://github.com/n8n-io/n8n/commit/17a829f1a2da1aa0297c8f1f6b0e4af2fbb70c4b))
* **API:** Add insights config on frontend settings ([#14315](https://github.com/n8n-io/n8n/issues/14315)) ([837131f](https://github.com/n8n-io/n8n/commit/837131fc96b7d48d8a5d612d431706d5f8dea41a))
* **API:** Implement BE api for insights data ([#14064](https://github.com/n8n-io/n8n/issues/14064)) ([db38149](https://github.com/n8n-io/n8n/commit/db381492a94d664f5e2ccc42f8830b20c8c19852))
* **core:** Add special `[@tool](https://github.com/tool)` displayOption ([#14318](https://github.com/n8n-io/n8n/issues/14318)) ([73748e3](https://github.com/n8n-io/n8n/commit/73748e300ed4a7f57b9c01f72eba2fbaa24ceef9))
* **core:** Don't store insights for sub workflow executions ([#14384](https://github.com/n8n-io/n8n/issues/14384)) ([7379f44](https://github.com/n8n-io/n8n/commit/7379f44896e2a3e66fee9d547ba929928f93a104))
* **core:** Make detaching floatable entitlements on shutdown configurable ([#14266](https://github.com/n8n-io/n8n/issues/14266)) ([c9565fc](https://github.com/n8n-io/n8n/commit/c9565fc0beea2751ba316fc363a275ea28d20653))
* **core:** Upgrade to express 5 to address CVE-2024-52798 ([#14332](https://github.com/n8n-io/n8n/issues/14332)) ([4110f31](https://github.com/n8n-io/n8n/commit/4110f3188e557a5d8c6d7ee44fb9c23ce73ce751))
* **editor:** Display a notice for HTTP header auth credentials ([#14389](https://github.com/n8n-io/n8n/issues/14389)) ([ec4dd9f](https://github.com/n8n-io/n8n/commit/ec4dd9f762f02c6da6f1c7e1e7faa1fa89802092))
* **editor:** Hover actions on the logs overview ([#14386](https://github.com/n8n-io/n8n/issues/14386)) ([8f9ea23](https://github.com/n8n-io/n8n/commit/8f9ea23019241de47fdee3a1da120f7c05a5aadb))
* **editor:** Insights dashboard ([#13739](https://github.com/n8n-io/n8n/issues/13739)) ([90ba680](https://github.com/n8n-io/n8n/commit/90ba68063116cdca358d74bf3c392af46280a2f5))
* **editor:** Show error state in the logs overview ([#14248](https://github.com/n8n-io/n8n/issues/14248)) ([37e5349](https://github.com/n8n-io/n8n/commit/37e5349fe139d9f292145d06218aa235b51bab38))
* **GitHub Node:** GitHub Node Overhaul implementation [#12271](https://github.com/n8n-io/n8n/issues/12271) ([#13238](https://github.com/n8n-io/n8n/issues/13238)) ([33e265a](https://github.com/n8n-io/n8n/commit/33e265aaa8563225eb408fe7dcff8412784cf6f9))
* **MongoDB Chat Memory Node:** New MongoDB Chat Memory Node ([#14049](https://github.com/n8n-io/n8n/issues/14049)) ([0bac6ff](https://github.com/n8n-io/n8n/commit/0bac6ffac6e8b1db5c9167ef7954a83c9c2230a2))
* **Postgres Node:** Batching warning for executeQuery operation insert query ([#14287](https://github.com/n8n-io/n8n/issues/14287)) ([f85b851](https://github.com/n8n-io/n8n/commit/f85b85185109b0ebd3f2f0def8a7c4a0902c8014))
* **Think Tool Node:** ToolThink, a simple tool to force the AI agent to do some thinking ([#14351](https://github.com/n8n-io/n8n/issues/14351)) ([281b70b](https://github.com/n8n-io/n8n/commit/281b70be044b3fd70a26a16d14eebf38bab739a6))



# [1.86.0](https://github.com/n8n-io/n8n/compare/n8n@1.85.0...n8n@1.86.0) (2025-03-31)


### Bug Fixes

* **API:** Fix import config import ([#14137](https://github.com/n8n-io/n8n/issues/14137)) ([6f60d65](https://github.com/n8n-io/n8n/commit/6f60d657eb0dc6ec9e99fe91d5b5cd99662d7ef8))
* **API:** Summarize insights from current datetime instead of beginning of the day ([#14186](https://github.com/n8n-io/n8n/issues/14186)) ([bf274c0](https://github.com/n8n-io/n8n/commit/bf274c0a870eba3ff293ee6033289e2d2b39fae1))
* **Baserow Node:** Fix issue where database selection was returning other types ([#14115](https://github.com/n8n-io/n8n/issues/14115)) ([10f6c3b](https://github.com/n8n-io/n8n/commit/10f6c3b1d35db31376419da0e6e791f9f903d266))
* **Basic LLM Chain Node:** Prevent incorrect wrapping of output ([#14183](https://github.com/n8n-io/n8n/issues/14183)) ([b9030d4](https://github.com/n8n-io/n8n/commit/b9030d45dead945342be88726cde2d0043ff4ab7))
* **Basic LLM Chain Node:** Prevent stringifying of structured output on previous versions ([#14200](https://github.com/n8n-io/n8n/issues/14200)) ([bbd6e8e](https://github.com/n8n-io/n8n/commit/bbd6e8ee415f27f40929ec404f5dd6e4c216f423))
* **core:** Fix OAuth1 callback token request ([#14251](https://github.com/n8n-io/n8n/issues/14251)) ([4ea219b](https://github.com/n8n-io/n8n/commit/4ea219b1f783370c39be3e776e664f71348c67c9))
* Correct connections in SentimentAnalysis and TextClassifier ([#14155](https://github.com/n8n-io/n8n/issues/14155)) ([70764a0](https://github.com/n8n-io/n8n/commit/70764a02589c146bf8e863c9c652ac30858841af))
* **editor:** Adjust URL on lost change warning Cancel or failed save ([#13683](https://github.com/n8n-io/n8n/issues/13683)) ([fdcca1d](https://github.com/n8n-io/n8n/commit/fdcca1d0ed7f7c32aa6c40f4751f554826064619))
* **editor:** Change freeAiCredits success text size ([#14161](https://github.com/n8n-io/n8n/issues/14161)) ([ca01236](https://github.com/n8n-io/n8n/commit/ca01236dd11b3c021358671ed99cbada4a34e325))
* **editor:** Check for when to show the community+ modal for the folder's feature ([#14146](https://github.com/n8n-io/n8n/issues/14146)) ([9e3bfe2](https://github.com/n8n-io/n8n/commit/9e3bfe23f67dca8d31bcff8758ed5d076477f9f3))
* **editor:** Handle Leading Spaces in Workflow Search ([#13889](https://github.com/n8n-io/n8n/issues/13889)) ([8aad7db](https://github.com/n8n-io/n8n/commit/8aad7dbaf69d7e2826f8798b6682d269c6c6f37f))
* **editor:** Remove selection box when only one node selected using selection rectangle ([#14160](https://github.com/n8n-io/n8n/issues/14160)) ([acbaec5](https://github.com/n8n-io/n8n/commit/acbaec550f1ebf560262d6a6492651ebaf72d78d))
* **editor:** Remove title icon on Overview subpages ([#14128](https://github.com/n8n-io/n8n/issues/14128)) ([4bd42e2](https://github.com/n8n-io/n8n/commit/4bd42e2f3a8a79c33a20f992e2727f8bb3dae101))
* **editor:** Show left-hand NDV floating nodes in correct order ([#14126](https://github.com/n8n-io/n8n/issues/14126)) ([71f281b](https://github.com/n8n-io/n8n/commit/71f281b90da6f71db04c9b22dee9e5976b0abab4))
* **Microsoft SQL Node:** Fix maximum call stack on execute query ([#13940](https://github.com/n8n-io/n8n/issues/13940)) ([a082a16](https://github.com/n8n-io/n8n/commit/a082a16c5d785d87ea334bb2285000bd3f44c157))
* **n8n Form Node:** Hidden field fix ([#14219](https://github.com/n8n-io/n8n/issues/14219)) ([9bd72ea](https://github.com/n8n-io/n8n/commit/9bd72eaa139649811cb1114f3cf40f22d5dfe905))
* **n8n Form Node:** Show Form Complition after Form Complition page ([#14226](https://github.com/n8n-io/n8n/issues/14226)) ([af77730](https://github.com/n8n-io/n8n/commit/af777307b3fddcf553fb68786260dba79f32d87c))
* **OpenAI Node:** Show correct inputs for AI node ([#14142](https://github.com/n8n-io/n8n/issues/14142)) ([5bf10cd](https://github.com/n8n-io/n8n/commit/5bf10cdb4abe364a8f914362fb94841530aa02c9))
* **Slack Node:** Make sure paginated calls use the defined limits ([#14185](https://github.com/n8n-io/n8n/issues/14185)) ([24fad51](https://github.com/n8n-io/n8n/commit/24fad512da9bcd4fd002dfac3cff5935ed00204f))
* **Slack Trigger Node:** Fix issue with new user event not correctly working ([#14129](https://github.com/n8n-io/n8n/issues/14129)) ([5f4e56f](https://github.com/n8n-io/n8n/commit/5f4e56f75b6659fc21b3d18817f5afabc022b5b7))
* **Summarize Node:** Fix type casting of strings and numbers ([#14259](https://github.com/n8n-io/n8n/issues/14259)) ([4443a5f](https://github.com/n8n-io/n8n/commit/4443a5f53281064f9d474d61435c83e004d7a403))


### Features

* **API:** Add day to week compaction for insights dashboard ([#14165](https://github.com/n8n-io/n8n/issues/14165)) ([db99974](https://github.com/n8n-io/n8n/commit/db99974cca364d16391d00d5aec066b68cb8a4e6))
* **API:** Add failureRate as sort field for insights by workflow ([#14247](https://github.com/n8n-io/n8n/issues/14247)) ([877823d](https://github.com/n8n-io/n8n/commit/877823d887fe7d387a5bbe25a606de1f1d22daa5))
* **API:** Add fields to insight by time type and export types from index ([#14172](https://github.com/n8n-io/n8n/issues/14172)) ([3d332ab](https://github.com/n8n-io/n8n/commit/3d332ab04fa0de9873cd8944514afa4e2bf7907b))
* **API:** Create schema and dto types for insights dashboard query param and api responses ([#14163](https://github.com/n8n-io/n8n/issues/14163)) ([6eee081](https://github.com/n8n-io/n8n/commit/6eee081cf3f99e7cf925a0daef0728e5537e1e57))
* **API:** Return null deviation on insights summary if previous period has no data ([#14193](https://github.com/n8n-io/n8n/issues/14193)) ([ffc0a59](https://github.com/n8n-io/n8n/commit/ffc0a596e00d1cbf14ff2980894d52025bfc1187))
* **core:** Explicitly warn if tool passed binary data to Agent ([#14071](https://github.com/n8n-io/n8n/issues/14071)) ([88f5851](https://github.com/n8n-io/n8n/commit/88f58514e6d7b5fe11d91b7e524b3447c09474eb))
* **editor:** Improve schema view empty state when node has binary data ([#14044](https://github.com/n8n-io/n8n/issues/14044)) ([22ddf1b](https://github.com/n8n-io/n8n/commit/22ddf1b644dcddfff3a97bd7953823f63ab7c41a))
* **editor:** Logs overview panel ([#14045](https://github.com/n8n-io/n8n/issues/14045)) ([d1710a1](https://github.com/n8n-io/n8n/commit/d1710a1da375d13a687add4f48400faab62169d7))
* **Matrix Node:** Add audio and video media types ([#14057](https://github.com/n8n-io/n8n/issues/14057)) ([cb01f2d](https://github.com/n8n-io/n8n/commit/cb01f2dd0d018ef54fc63b255abc0a054d01b6ed))
* **SendGrid Node:** Add option to specify "reply to" email addresses ([#14282](https://github.com/n8n-io/n8n/issues/14282)) ([68d9460](https://github.com/n8n-io/n8n/commit/68d9460f2acece495671667cacf6faa2e9a70cbf))
* **Telegram Trigger Node:** Add options to restrict to chat and user IDs ([#14164](https://github.com/n8n-io/n8n/issues/14164)) ([f651766](https://github.com/n8n-io/n8n/commit/f6517664dd05878b0e5264668c52c74cbdd2d027))



# [1.85.0](https://github.com/n8n-io/n8n/compare/n8n@1.84.0...n8n@1.85.0) (2025-03-24)


### Bug Fixes

* Allow saved credenitals types of up to 64 characters instead of 32 ([#13985](https://github.com/n8n-io/n8n/issues/13985)) ([bc15bb1](https://github.com/n8n-io/n8n/commit/bc15bb18d9f33abdeed24e26826e7f3308d3eef2))
* Allow username to be set in Redis chat memory ([#13926](https://github.com/n8n-io/n8n/issues/13926)) ([b2e359a](https://github.com/n8n-io/n8n/commit/b2e359ac1c2dfdf79f8d50fe83998eda5fc34dd2))
* **core:** Allow running webhook servers in multi-main mode ([#13989](https://github.com/n8n-io/n8n/issues/13989)) ([e0fd505](https://github.com/n8n-io/n8n/commit/e0fd50554d48c873c8f77169d1a17438391dd973))
* **core:** Bring back the missing GMT and UTC timezone for workflow settings ([#13999](https://github.com/n8n-io/n8n/issues/13999)) ([bda0688](https://github.com/n8n-io/n8n/commit/bda068880ea7a44718e01a156e97f09c9ec2bc46))
* **core:** Do not use `url.includes` to check for domain names ([#13802](https://github.com/n8n-io/n8n/issues/13802)) ([d3bc80c](https://github.com/n8n-io/n8n/commit/d3bc80c22bbbf0ae39c88a6f085d5f80aa8a0e82))
* **core:** Don't fail partial execution when an unrelated node is dirty ([#13925](https://github.com/n8n-io/n8n/issues/13925)) ([918cc51](https://github.com/n8n-io/n8n/commit/918cc51abc79bbcfb6a333d5ecafa07a9e986b6f))
* **core:** Ensure frontend sentry releases also follow semver ([#14019](https://github.com/n8n-io/n8n/issues/14019)) ([401ed2c](https://github.com/n8n-io/n8n/commit/401ed2ce1194ad7ff238debff418f0db77eb06e6))
* **editor:** Add "time saved per execution" workflow setting ([#13369](https://github.com/n8n-io/n8n/issues/13369)) ([6992c36](https://github.com/n8n-io/n8n/commit/6992c36ebb3aa608ce31396f9b7ed0aa10c80299))
* **editor:** Add smart decimals directive ([#14054](https://github.com/n8n-io/n8n/issues/14054)) ([1a26fc2](https://github.com/n8n-io/n8n/commit/1a26fc2762dee366d2ce7ccf24e173cdc761c70c))
* **editor:** Fix routing between workflow editing and new workflow pages ([#14031](https://github.com/n8n-io/n8n/issues/14031)) ([6817abe](https://github.com/n8n-io/n8n/commit/6817abe47facd7ff0e42a66599827d42c4df757c))


### Features

* Add appendN8nAttribution option to sendAndWait operation ([#13697](https://github.com/n8n-io/n8n/issues/13697)) ([d6d5a66](https://github.com/n8n-io/n8n/commit/d6d5a66f5dc28d926755ca8153f91c7be0742cf5))
* Add xAiGrok Chat Model node and credentials ([#13670](https://github.com/n8n-io/n8n/issues/13670)) ([cc502fb](https://github.com/n8n-io/n8n/commit/cc502fb8c34b65d569b4abe4603cc8ef1eadc7a7))
* Allow custom scopes for Entra credential ([#13796](https://github.com/n8n-io/n8n/issues/13796)) ([7e10361](https://github.com/n8n-io/n8n/commit/7e1036187ff7bd5be990f191a3ac8ef002e7812a))
* **API:** Fix generation strategy for mysql/mariadb ([#14028](https://github.com/n8n-io/n8n/issues/14028)) ([24d8eac](https://github.com/n8n-io/n8n/commit/24d8eac85d8ce95671aabf8500139b3ef3e19a56))
* **API:** Implement compaction logic for insights ([#14062](https://github.com/n8n-io/n8n/issues/14062)) ([d8433d2](https://github.com/n8n-io/n8n/commit/d8433d289543c40854e59b0384be356a3d7b947d))
* Cat 720 improve pre merge ci ([#14116](https://github.com/n8n-io/n8n/issues/14116)) ([743b63e](https://github.com/n8n-io/n8n/commit/743b63e97a9a96dfaf35f138a79eddaad9bb2dbb))
* **core:** Add folder synchronization to environments feature ([#14005](https://github.com/n8n-io/n8n/issues/14005)) ([198f17d](https://github.com/n8n-io/n8n/commit/198f17dbcf0b21e579f9a68466494662257dbe44))
* **core:** Add tool to uninstall a community node ([#14026](https://github.com/n8n-io/n8n/issues/14026)) ([e0f9506](https://github.com/n8n-io/n8n/commit/e0f9506912aa6a129df332185063291f0627f9ca))
* **core:** Allow community nodes to be used as tools ([#14042](https://github.com/n8n-io/n8n/issues/14042)) ([9d698ed](https://github.com/n8n-io/n8n/commit/9d698edcebc8cdbf9fefc3bf89a13f9daa32f40b))
* **core:** Allow customizing auth cookie samesite attribute and CSP headers ([#13855](https://github.com/n8n-io/n8n/issues/13855)) ([17fc5c1](https://github.com/n8n-io/n8n/commit/17fc5c148b99b8f346abf2142a1d2bee567b2621))
* **core:** Enable folders feature via license server ([#13942](https://github.com/n8n-io/n8n/issues/13942)) ([fa7e7ac](https://github.com/n8n-io/n8n/commit/fa7e7ac2e7b38418619ebe1f3839d47c491419d2))
* **core:** Implement API to retrieve summary metrics ([#13927](https://github.com/n8n-io/n8n/issues/13927)) ([b616ceb](https://github.com/n8n-io/n8n/commit/b616ceb08b712ecd350114acc48a9a0f35843c0a))
* **core:** Support importing a singular workflow object ([#14041](https://github.com/n8n-io/n8n/issues/14041)) ([91b2796](https://github.com/n8n-io/n8n/commit/91b27964d80309ce493200289b31a83ef6051b4d))
* **core:** Update endpoint to update a workflow, to support updating the workflow parent folder (no-chagelog) ([#13906](https://github.com/n8n-io/n8n/issues/13906)) ([3a5cc4a](https://github.com/n8n-io/n8n/commit/3a5cc4ae957ea5f370472f08d2af4ac29c3b21b2))
* **editor:** Add variables and context section to schema view ([#13875](https://github.com/n8n-io/n8n/issues/13875)) ([c06ce76](https://github.com/n8n-io/n8n/commit/c06ce765f11dcde4731d3739e1aa5f27351c3cc2))
* **editor:** Always show collapsed panel at the bottom of canvas ([#13715](https://github.com/n8n-io/n8n/issues/13715)) ([2e9d3ad](https://github.com/n8n-io/n8n/commit/2e9d3ad3e14da7aa2f3b3b9577858791e9128908))
* **editor:** Insights summary banner ([#13424](https://github.com/n8n-io/n8n/issues/13424)) ([df474f3](https://github.com/n8n-io/n8n/commit/df474f3ccbc629a8e308359e6a4973cc00b86e17))
* **Extract from File Node:** Add relax_quote option ([#13607](https://github.com/n8n-io/n8n/issues/13607)) ([830d2c5](https://github.com/n8n-io/n8n/commit/830d2c5df53c5436f89868dfe23cf55c41585a46))
* **n8n Form Trigger Node:** Respond with File ([#13507](https://github.com/n8n-io/n8n/issues/13507)) ([8f46371](https://github.com/n8n-io/n8n/commit/8f46371d77262aa0a924e1c58cf9691327e0f193))
* **Salesforce Node:** Add support for PKCE ([#14082](https://github.com/n8n-io/n8n/issues/14082)) ([defeb2e](https://github.com/n8n-io/n8n/commit/defeb2e817dbc559844124f20e6bebf7717d878a))
* **SeaTable Node:** Update node with new options ([#11431](https://github.com/n8n-io/n8n/issues/11431)) ([d0fdb11](https://github.com/n8n-io/n8n/commit/d0fdb11499de2e5fb1602b7cc86f2b24543ce50f))
* **Simple Vector Store Node:** Implement store cleaning based on age/used memory ([#13986](https://github.com/n8n-io/n8n/issues/13986)) ([e06c552](https://github.com/n8n-io/n8n/commit/e06c552a6a0471ec60862247f6a597b8ab5f9cd3))



# [1.84.0](https://github.com/n8n-io/n8n/compare/n8n@1.83.0...n8n@1.84.0) (2025-03-17)


### Bug Fixes

* **AWS SES Node:** Encode template parameters properly ([#13570](https://github.com/n8n-io/n8n/issues/13570)) ([ca8d249](https://github.com/n8n-io/n8n/commit/ca8d249700e341ea79173a5d6d148205db0ff0ac))
* **core:** Avoid using structuredClone on node descriptions ([#13832](https://github.com/n8n-io/n8n/issues/13832)) ([d2df154](https://github.com/n8n-io/n8n/commit/d2df154b49ad4e89ac1b5e5b1b49df57a377175e))
* **core:** Clean run data for dirty nodes properly, including their children ([#13821](https://github.com/n8n-io/n8n/issues/13821)) ([b3f9cde](https://github.com/n8n-io/n8n/commit/b3f9cde3fd1a22d007d323785fa6ff09f945dd8a))
* **core:** Ensure worker stops picking up new jobs while shutting down ([#13714](https://github.com/n8n-io/n8n/issues/13714)) ([4fe2495](https://github.com/n8n-io/n8n/commit/4fe249580a57f167000c1cad294feb37170e5e8b))
* **core:** Find correct start nodes when the first node after that has no run data has pinned data ([#13784](https://github.com/n8n-io/n8n/issues/13784)) ([cbf2476](https://github.com/n8n-io/n8n/commit/cbf2476819402b273b55baf6e4eb91d6ce14dac5))
* **core:** License should ignore empty input on onFeatureChange ([#13912](https://github.com/n8n-io/n8n/issues/13912)) ([dedcdbd](https://github.com/n8n-io/n8n/commit/dedcdbd31496928d3cb8820fd0c2542d056bf7de))
* **core:** Log all command errors messages ([#13827](https://github.com/n8n-io/n8n/issues/13827)) ([e8334ee](https://github.com/n8n-io/n8n/commit/e8334eefa16d552e6ea8f915818928ae9de114ec))
* **core:** Update samlify and xml-crypto to address CVE-2025-29775 and CVE-2025-29774 ([#13951](https://github.com/n8n-io/n8n/issues/13951)) ([c91688d](https://github.com/n8n-io/n8n/commit/c91688d49404c5640c03a0238ea7bbc4d4b34fc2))
* Do not trigger sendAndWait response on bot visit if response type is approval ([#13792](https://github.com/n8n-io/n8n/issues/13792)) ([526a2e4](https://github.com/n8n-io/n8n/commit/526a2e4ca3a488ee1a6c48aa0dc7053f298da2f5))
* **editor:** Add disabled state with tooltip on project creation buttons if user lacks permission ([#13867](https://github.com/n8n-io/n8n/issues/13867)) ([e33d0d7](https://github.com/n8n-io/n8n/commit/e33d0d7466969c372b2ea82eb1b1ebf52ed5fe92))
* **editor:** Decrease notification max-height ([#13858](https://github.com/n8n-io/n8n/issues/13858)) ([1c2feb4](https://github.com/n8n-io/n8n/commit/1c2feb455aa26687b957499625c4f05243e6434c))
* **editor:** Disable `test step` option in context menu for sub-nodes ([#13816](https://github.com/n8n-io/n8n/issues/13816)) ([b6d5092](https://github.com/n8n-io/n8n/commit/b6d5092258a7f0d59adf38e89afd6534e21422fc))
* **editor:** Disable deactivated node execution ([#13643](https://github.com/n8n-io/n8n/issues/13643)) ([473f6d4](https://github.com/n8n-io/n8n/commit/473f6d48db4bcde28b1bb4bae7727f33073c8deb))
* **editor:** Fix logo alignment issues ([#13870](https://github.com/n8n-io/n8n/issues/13870)) ([d2e4706](https://github.com/n8n-io/n8n/commit/d2e4706b973af490fcdda507ef12b544bdf67c21))
* **editor:** Fix NDV panels size on narrow screens ([#13708](https://github.com/n8n-io/n8n/issues/13708)) ([899f6c9](https://github.com/n8n-io/n8n/commit/899f6c98243df2dc661be5ce7d9b242b62f9790f))
* **editor:** Fix options parameters that have extra displayName field ([#13928](https://github.com/n8n-io/n8n/issues/13928)) ([eec3251](https://github.com/n8n-io/n8n/commit/eec325127c075a0a0db429d5b41db5c2851fc187))
* **editor:** Increase contrast on hover for AI button ([#13920](https://github.com/n8n-io/n8n/issues/13920)) ([c239b8f](https://github.com/n8n-io/n8n/commit/c239b8f07a6951a3b5a0203b94e5c43d8707c769))
* **editor:** Tweak schema view empty state copy and styling ([#13819](https://github.com/n8n-io/n8n/issues/13819)) ([cfc7a14](https://github.com/n8n-io/n8n/commit/cfc7a14e18e1adc078579eff3c2eb3598f7096aa))
* Execute method should be assigned to a Routing node even if it has webhook defined ([#13910](https://github.com/n8n-io/n8n/issues/13910)) ([3a4247a](https://github.com/n8n-io/n8n/commit/3a4247a91c5ffef6a65cd1e28007f8961022fc03))
* **MySQL Node:** Fix potential sql injection ([#13818](https://github.com/n8n-io/n8n/issues/13818)) ([dd4f51c](https://github.com/n8n-io/n8n/commit/dd4f51cff5bec5f045fe549ffd9ab04367e543a9))
* **n8n Form Node:** Resolve expressions in HTML fields ([#13755](https://github.com/n8n-io/n8n/issues/13755)) ([de23ae5](https://github.com/n8n-io/n8n/commit/de23ae55585d2b43a338314cddbbf506ffd5daf6))
* **n8n Form Trigger Node:** Add back the query selector for multiselect ([#13987](https://github.com/n8n-io/n8n/issues/13987)) ([39208dc](https://github.com/n8n-io/n8n/commit/39208dcb7033b19fa2fdd20e16293fd5a6d6f19d))
* **OpenAI Chat Model Node:** Sort models alphabetically ([#13909](https://github.com/n8n-io/n8n/issues/13909)) ([3103748](https://github.com/n8n-io/n8n/commit/31037484a51ec0e41840e697f7427034c6274796))
* **Postgres Node:** RMC do not mark collumn as required if identity_generation is BY DEFAULT ([#13752](https://github.com/n8n-io/n8n/issues/13752)) ([b563254](https://github.com/n8n-io/n8n/commit/b5632545c5972d7716445b9337d6598d7b8b6dbd))
* **Structured Output Parser Node, Auto-fixing Output Parser Node, Tools Agent Node:** Structured output improvements ([#13908](https://github.com/n8n-io/n8n/issues/13908)) ([5b6b787](https://github.com/n8n-io/n8n/commit/5b6b78709efa5665e8fc7b260b8de71763b4d6ae))
* Update Sentry `rewriteFramesIntegration` prefix (no-changleog) ([#13900](https://github.com/n8n-io/n8n/issues/13900)) ([1eec246](https://github.com/n8n-io/n8n/commit/1eec246f4eecb7dbb9ec3130e0e460e720a2d42c))


### Features

* **editor:** Add toJsonString to string extensions ([#13798](https://github.com/n8n-io/n8n/issues/13798)) ([4e93ffd](https://github.com/n8n-io/n8n/commit/4e93ffda8bfa39e33120f76b5c2f4d393fcdfbfa))
* **editor:** Popping logs out into a new window ([#13788](https://github.com/n8n-io/n8n/issues/13788)) ([4d04c22](https://github.com/n8n-io/n8n/commit/4d04c227a988639bcbd6bcfd9e6df675afa12958))
* Hints for tools and agent ([#13386](https://github.com/n8n-io/n8n/issues/13386)) ([ec8a719](https://github.com/n8n-io/n8n/commit/ec8a719efaaf03f1269abdea567a41d404e212d8))
* **Merge Node:** Better pairedItem mapping in combineBySql operation if SELECT query ([#13849](https://github.com/n8n-io/n8n/issues/13849)) ([881d3f8](https://github.com/n8n-io/n8n/commit/881d3f8771b547adf6e4bfe060575b1992b1d34c))
* **MongoDB Atlas Vector Store Node:** Add Mongo db vector store Node ([#12924](https://github.com/n8n-io/n8n/issues/12924)) ([3d87228](https://github.com/n8n-io/n8n/commit/3d872287fbedb72ded1172b2fcbe0b82dc2b8fd6))
* **WhatsApp Trigger Node:** New option to opt-out from message status updates ([#13751](https://github.com/n8n-io/n8n/issues/13751)) ([9c040ee](https://github.com/n8n-io/n8n/commit/9c040ee5a533ab23f913614a4d56927956ac7a8a))



# [1.83.0](https://github.com/n8n-io/n8n/compare/n8n@1.82.0...n8n@1.83.0) (2025-03-10)


### Bug Fixes

* **Airtable Node:** Table RLC should depend on Base RLC ([#13735](https://github.com/n8n-io/n8n/issues/13735)) ([321fac2](https://github.com/n8n-io/n8n/commit/321fac2efa62d256b99e7ed6ea5b8706ef604ab1))
* **Call n8n Workflow Tool Node:** Return all items from subexecution ([#13393](https://github.com/n8n-io/n8n/issues/13393)) ([d9e3cfe](https://github.com/n8n-io/n8n/commit/d9e3cfe13fdd9c47474cd129db2f943871138331))
* **core:** Correct NODE_OPTIONS export syntax for custom certificates ([#13779](https://github.com/n8n-io/n8n/issues/13779)) ([080fc51](https://github.com/n8n-io/n8n/commit/080fc514e6a8485430028962cf8b29e5fa03a9d7))
* **core:** Do not validate email when LDAP is enabled ([#13605](https://github.com/n8n-io/n8n/issues/13605)) ([17738c5](https://github.com/n8n-io/n8n/commit/17738c50962d25ac34c8fd0248bd2b2e0863b429))
* **core:** Fix task runner error report from user-defined function ([#13706](https://github.com/n8n-io/n8n/issues/13706)) ([9bedd87](https://github.com/n8n-io/n8n/commit/9bedd87744bb21317c22b96dae902ebb3790bde2))
* **core:** Pass `NODE_PATH` to task runners ([#13652](https://github.com/n8n-io/n8n/issues/13652)) ([906770a](https://github.com/n8n-io/n8n/commit/906770a06aafc5814f8a7af543adfc0ec06361da))
* **editor:** Allow pinned data for Code node AI generation ([#13638](https://github.com/n8n-io/n8n/issues/13638)) ([6d7e346](https://github.com/n8n-io/n8n/commit/6d7e346e4f06c9f90cf1ca01de88cc84832e200f))
* **editor:** Apply html sanitization in right lifecycle ([#13703](https://github.com/n8n-io/n8n/issues/13703)) ([8ab3073](https://github.com/n8n-io/n8n/commit/8ab3073323b8b1c4d32ed541b1cb46b72aa0a80d))
* **editor:** Copy JSON from selected run if node has been multiple times ([#13673](https://github.com/n8n-io/n8n/issues/13673)) ([5eddf00](https://github.com/n8n-io/n8n/commit/5eddf00fa1bf9b4bcf15a05eec0050aba3d54a2f))
* **editor:** Don't flag uiStore as dirty on node selected ([#13641](https://github.com/n8n-io/n8n/issues/13641)) ([4f6d76c](https://github.com/n8n-io/n8n/commit/4f6d76cd25215e75e4b03eb84f0476b346cbedcd))
* **editor:** Enable pin data button to also un-pin ([#13642](https://github.com/n8n-io/n8n/issues/13642)) ([24681f8](https://github.com/n8n-io/n8n/commit/24681f843c906c6b83c8c686b5c11fa18d792fd7))
* **editor:** Expand error view to full output panel width ([#13688](https://github.com/n8n-io/n8n/issues/13688)) ([97ca702](https://github.com/n8n-io/n8n/commit/97ca702f8cb660224975e2eb956e2a513f753127))
* **editor:** Fix code node displays lint messages in wrong location ([#13664](https://github.com/n8n-io/n8n/issues/13664)) ([d3ead68](https://github.com/n8n-io/n8n/commit/d3ead6805981140decf7f26ccda40cc9c1248356))
* **editor:** Fix GCP icon size for external secrets modal ([#13672](https://github.com/n8n-io/n8n/issues/13672)) ([77425f0](https://github.com/n8n-io/n8n/commit/77425f04cf05e161eb82aea57d11b93dd489cc1f))
* **editor:** Fix opening 'Schema' view by default after opening binary nodes ([#13676](https://github.com/n8n-io/n8n/issues/13676)) ([3cd34b5](https://github.com/n8n-io/n8n/commit/3cd34b5af6da43d38c358b9cd23c8ea49b28e83d))
* **editor:** Fix RLC dropdown vanishing when focusing search input ([#13579](https://github.com/n8n-io/n8n/issues/13579)) ([5ac8691](https://github.com/n8n-io/n8n/commit/5ac869194656181ed93338199e07e682a8649afe))
* **editor:** Fix save keybind in expression editor and unfocused node details view ([#13640](https://github.com/n8n-io/n8n/issues/13640)) ([9ba9443](https://github.com/n8n-io/n8n/commit/9ba9443460529728404cf3be70b3aeb45c1768e6))
* **editor:** Fix sidebar logo container layout ([#13203](https://github.com/n8n-io/n8n/issues/13203)) ([850d458](https://github.com/n8n-io/n8n/commit/850d458858bee4dd88db081758a04932dc4aef54))
* **editor:** Ignore required module type declaration error in code node ([#13628](https://github.com/n8n-io/n8n/issues/13628)) ([2a5738a](https://github.com/n8n-io/n8n/commit/2a5738aebe617b9dabbdb77db48b0f5412cefe04))
* **editor:** Match nodes for autocomplete ([#13716](https://github.com/n8n-io/n8n/issues/13716)) ([8043a6c](https://github.com/n8n-io/n8n/commit/8043a6ce82cc539ddc88ec919ec86e52da1e18d9))
* **editor:** Render credential-only nodes when loading from the backend ([#13689](https://github.com/n8n-io/n8n/issues/13689)) ([c821f1c](https://github.com/n8n-io/n8n/commit/c821f1c532048c9afa0bc51e3566ae65bf9caf0a))
* **editor:** Show error details in resource locator dropdown ([#13679](https://github.com/n8n-io/n8n/issues/13679)) ([630608c](https://github.com/n8n-io/n8n/commit/630608c8bda85739196f51e32dc57efae88858a7))
* **editor:** Support pasting values that start with `=` ([#13699](https://github.com/n8n-io/n8n/issues/13699)) ([9e83ff5](https://github.com/n8n-io/n8n/commit/9e83ff51da3587f4525c6fdfeceaa85c79834510))
* **Elasticsearch Node:** Use POST instead of GET to allow request body in search API ([#13302](https://github.com/n8n-io/n8n/issues/13302)) ([783bf7b](https://github.com/n8n-io/n8n/commit/783bf7b3bc90a3a82169fb14e057640f45e656e3))
* **GitHub Node:** Fix workflow resource locator ([#13599](https://github.com/n8n-io/n8n/issues/13599)) ([b7f7121](https://github.com/n8n-io/n8n/commit/b7f7121cb8fd5e707f602e9f3ea18fffaf75d526))
* **Google Sheets Node:** Accommodate special characters when updating row ([#13589](https://github.com/n8n-io/n8n/issues/13589)) ([e633e91](https://github.com/n8n-io/n8n/commit/e633e91f69669dc01540aca8be7c3d43672dcea3))
* In addNodeToBeExecuted if stillDataMissing allow more then 2 inputs ([#13704](https://github.com/n8n-io/n8n/issues/13704)) ([e9a8a7f](https://github.com/n8n-io/n8n/commit/e9a8a7f8755980848bd5041d6a443c518b99ee18))
* **n8n Form Trigger Node:** Sanitize HTML for formNode ([#13595](https://github.com/n8n-io/n8n/issues/13595)) ([20dfaa3](https://github.com/n8n-io/n8n/commit/20dfaa3be6ee03498771ca0a62567e562bbab9da))
* **S3 Node:** Fix issue when connecting to Supabase storage ([#13667](https://github.com/n8n-io/n8n/issues/13667)) ([5fe33ef](https://github.com/n8n-io/n8n/commit/5fe33efc944a8adf07093badfe43773a34f79d6f))


### Features

* **editor:** Schema preview UI updates ([#13578](https://github.com/n8n-io/n8n/issues/13578)) ([8790a0d](https://github.com/n8n-io/n8n/commit/8790a0df3de2bc6a1909358017abf6734823faad))



# [1.82.0](https://github.com/n8n-io/n8n/compare/n8n@1.81.0...n8n@1.82.0) (2025-03-03)


### Bug Fixes

* **Call n8n Workflow Tool Node:** Support concurrent invocations of the tool ([#13526](https://github.com/n8n-io/n8n/issues/13526)) ([5334661](https://github.com/n8n-io/n8n/commit/5334661b76909f48aa4e45af889e6180c025eed6))
* **core:** Gracefully handle missing tasks metadata ([#13632](https://github.com/n8n-io/n8n/issues/13632)) ([999fb81](https://github.com/n8n-io/n8n/commit/999fb8174ae6bb34354cb8c6f85f769cb64e8ae4))
* **core:** Remove `index.html` caching entirely ([#13563](https://github.com/n8n-io/n8n/issues/13563)) ([afba8f9](https://github.com/n8n-io/n8n/commit/afba8f9ff89054d54e1cf70070ae5710bc9ddd37))
* **editor:** Add workflows to the store when fetching current page ([#13583](https://github.com/n8n-io/n8n/issues/13583)) ([c4f3293](https://github.com/n8n-io/n8n/commit/c4f329377828d80a54b71f5733ea7d9b4ee91f48))
* **editor:** Ai 672 minor UI fixes on evaluation creation ([#13461](https://github.com/n8n-io/n8n/issues/13461)) ([b791677](https://github.com/n8n-io/n8n/commit/b791677ffa8c82161c4c40b65bc62d93f2e7bc9e))
* **editor:** Ai 675 minor tweaks to tests list ([#13467](https://github.com/n8n-io/n8n/issues/13467)) ([5ad950f](https://github.com/n8n-io/n8n/commit/5ad950f60371546414ff17eb31171f2259e70f57))
* **editor:** Don't show duplicate logs when tree is deeply nested ([#13537](https://github.com/n8n-io/n8n/issues/13537)) ([d550382](https://github.com/n8n-io/n8n/commit/d550382a4a43c54cae47e9071236aa18efe38a5d))
* **editor:** Fix browser crash with large execution result ([#13580](https://github.com/n8n-io/n8n/issues/13580)) ([1c8c7e3](https://github.com/n8n-io/n8n/commit/1c8c7e34f9d2c8363c441aeb8c562ac91088a687))
* **editor:** Fix github star button layout ([#13630](https://github.com/n8n-io/n8n/issues/13630)) ([139b5b3](https://github.com/n8n-io/n8n/commit/139b5b378daba6df18639eeb4f326edce7752e11))
* **editor:** Fix icon color on 'Call n8n Workflow Tool' node ([#13568](https://github.com/n8n-io/n8n/issues/13568)) ([90d0943](https://github.com/n8n-io/n8n/commit/90d09431af97570a3a6adfb0470a18681af28001))
* **editor:** Fix icon spacing in accordion title ([#13539](https://github.com/n8n-io/n8n/issues/13539)) ([ebaaf0e](https://github.com/n8n-io/n8n/commit/ebaaf0e3d9602052f76f61b90fb073e390896cea))
* **editor:** Fix keyboard shortcuts no longer working after editing sticky note ([#13502](https://github.com/n8n-io/n8n/issues/13502)) ([ab41fc3](https://github.com/n8n-io/n8n/commit/ab41fc3fb5f15e9c7ce7279b46cec90a511d0e0d))
* **editor:** Fix workflows list status filter ([#13621](https://github.com/n8n-io/n8n/issues/13621)) ([4067fb0](https://github.com/n8n-io/n8n/commit/4067fb0b12d242c795c6598df6c4090d48cec7b1))
* **editor:** Hide fromAI button in old workflow tool ([#13552](https://github.com/n8n-io/n8n/issues/13552)) ([6ef8d34](https://github.com/n8n-io/n8n/commit/6ef8d34f969ddb9e80b82dc50b38698249089af2))
* **editor:** Parse out nodeType ([#13474](https://github.com/n8n-io/n8n/issues/13474)) ([1cd13b6](https://github.com/n8n-io/n8n/commit/1cd13b639efcfabf183740bb6634023c66d5ce99))
* **editor:** Show dropdown scrollbars only when appropriate ([#13562](https://github.com/n8n-io/n8n/issues/13562)) ([615a42a](https://github.com/n8n-io/n8n/commit/615a42afd52d0d95dd30ed9aa231b9921e0708fe))
* **editor:** Show JSON full-screen Editor Window in Full Height ([#13350](https://github.com/n8n-io/n8n/issues/13350)) ([46dcce3](https://github.com/n8n-io/n8n/commit/46dcce341fbfa1c2a44a08f3dc93f1f8f16808c8))
* **editor:** Show scrollbar in Element UI popup ([#13259](https://github.com/n8n-io/n8n/issues/13259)) ([c021a7e](https://github.com/n8n-io/n8n/commit/c021a7e4b2daccc59541bab25c1447339dd68c09))
* **editor:** Undo keybinding changes related to window focus/blur events ([#13559](https://github.com/n8n-io/n8n/issues/13559)) ([6ddcc1f](https://github.com/n8n-io/n8n/commit/6ddcc1f8c93f86b0d111cae1b24518d621d8fe84))
* **Odoo Node:** Model and fields dynamic fetching errors ([#13511](https://github.com/n8n-io/n8n/issues/13511)) ([294f019](https://github.com/n8n-io/n8n/commit/294f0194145ca4139d9d9cea0729bf83d0871c94))
* **Postgres Node:** Accommodate null values in query parameters for expressions ([#13544](https://github.com/n8n-io/n8n/issues/13544)) ([6c266ac](https://github.com/n8n-io/n8n/commit/6c266acced95500148532b4fc015fe5d9587db76))
* **QuickBooks Online Node:** Add qty to quickbooks invoice line details ([#13602](https://github.com/n8n-io/n8n/issues/13602)) ([7c4e2f0](https://github.com/n8n-io/n8n/commit/7c4e2f014c0b38935a4d661646e773ad26fc97e1))
* **seven Node:** Remove obsolete options and fix typos ([#13122](https://github.com/n8n-io/n8n/issues/13122)) ([d02c8b0](https://github.com/n8n-io/n8n/commit/d02c8b0d7dbd4144c954a66aa0e78e43122b6e9a))
* **Switch Node:** Fix an issue in ordering rules in Switch Node ([#13476](https://github.com/n8n-io/n8n/issues/13476)) ([0fb6607](https://github.com/n8n-io/n8n/commit/0fb66076ba6120a7cb2401102ff8d1d6220ae106))


### Features

* **Anthropic Chat Model Node:** Fetch models dynamically & support thinking ([#13543](https://github.com/n8n-io/n8n/issues/13543)) ([461df37](https://github.com/n8n-io/n8n/commit/461df371f76b9dee9916a985a2bd2197facbcf6b))
* **Azure Storage Node:** New node ([#12536](https://github.com/n8n-io/n8n/issues/12536)) ([727f6f3](https://github.com/n8n-io/n8n/commit/727f6f3c0e5cef2d0cd4cd1ef1c6fa8f4d3f69ec))
* **core:** Add metric for active workflow count ([#13420](https://github.com/n8n-io/n8n/issues/13420)) ([3aa679e](https://github.com/n8n-io/n8n/commit/3aa679e4ac411d0d34e039fa6c43bc98f2e3670f))
* **core:** Fix partial workflow execution with specific trigger data ([#13505](https://github.com/n8n-io/n8n/issues/13505)) ([9029dac](https://github.com/n8n-io/n8n/commit/9029dace5c682e4b5df4f18f2f51098dce6436e5))
* **core:** Make Tools Agent the default Agent type, deprecate other agent types ([#13459](https://github.com/n8n-io/n8n/issues/13459)) ([a60d106](https://github.com/n8n-io/n8n/commit/a60d106ebb4fb71e80f90a17965d7fb79d7806c6))
* **core:** Support executing single nodes not part of a graph as a partial execution ([#13529](https://github.com/n8n-io/n8n/issues/13529)) ([8a34f02](https://github.com/n8n-io/n8n/commit/8a34f027c531f0d37fc8088c13d7e289cd8897ce))
* **editor:** Add functionality to create folders ([#13473](https://github.com/n8n-io/n8n/issues/13473)) ([2cb9d9e](https://github.com/n8n-io/n8n/commit/2cb9d9e29fc961a417d06c1449b79d4a0a66658e))
* **editor:** Automatically tidy up workflows ([#13471](https://github.com/n8n-io/n8n/issues/13471)) ([f381a24](https://github.com/n8n-io/n8n/commit/f381a24145271f4df4fa5c9345bb12c984f6e1fc))
* **editor:** Indicate dirty nodes with yellow borders/connectors on canvas ([#13040](https://github.com/n8n-io/n8n/issues/13040)) ([75493ef](https://github.com/n8n-io/n8n/commit/75493ef6ef4ee47d0ccf217cd5c2e58754f60c12))
* **editor:** Rename 'In-Memory Vector Store' to 'Simple Vector Store' ([#13472](https://github.com/n8n-io/n8n/issues/13472)) ([35c00d0](https://github.com/n8n-io/n8n/commit/35c00d0c846e8a1e214aea3690ea60ff80d03eed))
* **editor:** Rename 'Window Buffer Memory' to 'Simple Memory' ([#13477](https://github.com/n8n-io/n8n/issues/13477)) ([819fc2d](https://github.com/n8n-io/n8n/commit/819fc2da63ce7f06d4702bce698d382eb64c45a3))
* Hackmation - automatically switch to expression mode ([#13213](https://github.com/n8n-io/n8n/issues/13213)) ([6953b0d](https://github.com/n8n-io/n8n/commit/6953b0d53a28448022c9de0a2f6294c9390a3b48))
* **n8n Form Trigger Node, Chat Trigger Node:** Allow to customize form and chat css ([#13506](https://github.com/n8n-io/n8n/issues/13506)) ([289041e](https://github.com/n8n-io/n8n/commit/289041e997eedb660356cdbd259660b7c3117194))
* **n8n Vertica credentials only Node:** New node ([#12256](https://github.com/n8n-io/n8n/issues/12256)) ([d3fe3de](https://github.com/n8n-io/n8n/commit/d3fe3dea32207dfdb2a43db0def96466a31daa66))
* Update AWS credential to support more regions ([#13524](https://github.com/n8n-io/n8n/issues/13524)) ([b50658c](https://github.com/n8n-io/n8n/commit/b50658cbc64c0a6fc000b11dca0cca49cc707471))
* WhatsApp Business Cloud Node - new operation sendAndWait ([#12941](https://github.com/n8n-io/n8n/issues/12941)) ([97defb3](https://github.com/n8n-io/n8n/commit/97defb3a833bb269a4a3fc573a8e250a0d0e0deb))



# [1.81.0](https://github.com/n8n-io/n8n/compare/n8n@1.80.0...n8n@1.81.0) (2025-02-24)


### Bug Fixes

* Always clear popupWindowState  before showing popup from form trigger ([#13363](https://github.com/n8n-io/n8n/issues/13363)) ([b7f1265](https://github.com/n8n-io/n8n/commit/b7f12650f1f42c0ff15c1da3e5ade350fb1e23d2))
* **Code Node:** Fix `$items` in Code node when using task runner ([#13368](https://github.com/n8n-io/n8n/issues/13368)) ([87b3c50](https://github.com/n8n-io/n8n/commit/87b3c508b3d5a7d6f3b9f8377de66567a04fa970))
* **core:** Avoid renewing the license on init to prevent excessive duplicate renewal calls ([#13347](https://github.com/n8n-io/n8n/issues/13347)) ([1e1f528](https://github.com/n8n-io/n8n/commit/1e1f52846641515ad4479ab1088e78a9266e452d))
* **core:** Ensure that 'workflow-post-execute' event has userId whenever it's available ([#13326](https://github.com/n8n-io/n8n/issues/13326)) ([f41e353](https://github.com/n8n-io/n8n/commit/f41e353887fef4269510d25fa87b73da4cf925f9))
* **core:** Fix DB migrations for MySQL ([#13261](https://github.com/n8n-io/n8n/issues/13261)) ([d0968a1](https://github.com/n8n-io/n8n/commit/d0968a10d56ac5c97974129742ba8f8a85997dac))
* **core:** Fix resuming executions on test webhooks from Wait forms ([#13410](https://github.com/n8n-io/n8n/issues/13410)) ([8ffd316](https://github.com/n8n-io/n8n/commit/8ffd3167d58d30f087fd31010e6f79f1398d8f49))
* **core:** Handle connections for missing nodes in a workflow ([#13362](https://github.com/n8n-io/n8n/issues/13362)) ([1e5feb1](https://github.com/n8n-io/n8n/commit/1e5feb195d50054939f85c9e1b5a32885c579901))
* **core:** Make sure middleware works with legacy API Keys ([#13390](https://github.com/n8n-io/n8n/issues/13390)) ([ca76ef4](https://github.com/n8n-io/n8n/commit/ca76ef4bc248a3bcde844bc8378d38eed269f032))
* **core:** Return original hooks errors to the frontend ([#13365](https://github.com/n8n-io/n8n/issues/13365)) ([5439181](https://github.com/n8n-io/n8n/commit/5439181e92f20fef1423575cabec7acbe1740b26))
* **editor:** Correctly close node creator when selecting/deselecting a node ([#13338](https://github.com/n8n-io/n8n/issues/13338)) ([c3dc66e](https://github.com/n8n-io/n8n/commit/c3dc66ee7372927fcfd6baac3b9d853690e39c99))
* **editor:** Do not show credential details popup for users without necessary scopes with direct link ([#13264](https://github.com/n8n-io/n8n/issues/13264)) ([a5401d0](https://github.com/n8n-io/n8n/commit/a5401d06a58ef026f44499d05b42a8d0dbe2520e))
* **editor:** Do not show project settings for users without permission with direct link ([#13246](https://github.com/n8n-io/n8n/issues/13246)) ([fa488f1](https://github.com/n8n-io/n8n/commit/fa488f15619f798a0360c96492f2928ac661d9ee))
* **editor:** Don't open form popup window if different trigger node is used ([#13391](https://github.com/n8n-io/n8n/issues/13391)) ([57a9a5b](https://github.com/n8n-io/n8n/commit/57a9a5b15f55aae0301851e93847ed87feb081e8))
* **editor:** Fix configurable node description margins and text alignment ([#13318](https://github.com/n8n-io/n8n/issues/13318)) ([c881ea2](https://github.com/n8n-io/n8n/commit/c881ea2c7b43a4fb610533dd553520a6de51f22d))
* **editor:** Fix workflow moving E2E tests ([#13396](https://github.com/n8n-io/n8n/issues/13396)) ([073b05b](https://github.com/n8n-io/n8n/commit/073b05b10c81e3a0451c310bc0bde25170e1591e))
* **editor:** Optionally share credentials used by the workflow when moving the workflow between projects ([#12524](https://github.com/n8n-io/n8n/issues/12524)) ([7bd83d7](https://github.com/n8n-io/n8n/commit/7bd83d7d330b6f01b5798461f2218254a9964d87))
* **editor:** Polyfill `Array.prototype.toSorted` (no-chanhelog) ([#13463](https://github.com/n8n-io/n8n/issues/13463)) ([f2b15ea](https://github.com/n8n-io/n8n/commit/f2b15ea086fcc541a5a584998985d712335210ec))
* **editor:** Register/unregister keybindings on window focus/blur ([#13419](https://github.com/n8n-io/n8n/issues/13419)) ([7a504dc](https://github.com/n8n-io/n8n/commit/7a504dc30fcf0c7641528ed469835811f82bb098))
* **editor:** Switch back to selection mode on window blur ([#13341](https://github.com/n8n-io/n8n/issues/13341)) ([415e25b](https://github.com/n8n-io/n8n/commit/415e25b5d524b0d3c391403f129468e57bbb918e))
* Prevent flicker during paginated workflow navigation ([#13348](https://github.com/n8n-io/n8n/issues/13348)) ([d277e0b](https://github.com/n8n-io/n8n/commit/d277e0ba0e5d87500457538b4b0f1363e267f071))


### Features

* **core:** Hackmation - Add last activity metric ([#13237](https://github.com/n8n-io/n8n/issues/13237)) ([272f55b](https://github.com/n8n-io/n8n/commit/272f55b80f1d4576d1675040bd2775210c4ab5e9))
* **editor:** Change rename node keyboard shortcut to Space on new canvas ([#11872](https://github.com/n8n-io/n8n/issues/11872)) ([c90d0d9](https://github.com/n8n-io/n8n/commit/c90d0d9161ec161cd1afd6aa5b56345c1611f9c9))
* **editor:** Implement breadcrumbs component ([#13317](https://github.com/n8n-io/n8n/issues/13317)) ([db297f1](https://github.com/n8n-io/n8n/commit/db297f107d81738d57e298135a9c279ad83345dc))
* **editor:** Implement folder navigation in workflows list ([#13370](https://github.com/n8n-io/n8n/issues/13370)) ([0eae14e](https://github.com/n8n-io/n8n/commit/0eae14e27ab4fab3229750d6b2a32868db1e8dd4))
* **editor:** Rename 'Text' fields on AI nodes to 'Prompt' ([#13416](https://github.com/n8n-io/n8n/issues/13416)) ([4fa666b](https://github.com/n8n-io/n8n/commit/4fa666b976423365299e915130384e10c8e12528))
* Enable partial exections v2 by default ([#13344](https://github.com/n8n-io/n8n/issues/13344)) ([29ae239](https://github.com/n8n-io/n8n/commit/29ae2396c99d54d8f3db71e6370516f0dc354d00))
* **n8n Form Node:** Limit wait time parameters ([#13160](https://github.com/n8n-io/n8n/issues/13160)) ([14b6f8b](https://github.com/n8n-io/n8n/commit/14b6f8b97275e38ba4a4c1819e8e32b711de21ba))



# [1.80.0](https://github.com/n8n-io/n8n/compare/n8n@1.79.0...n8n@1.80.0) (2025-02-17)


### Bug Fixes

* **AI Agent Node:** Move model retrieval into try/catch to fix continueOnFail handling ([#13165](https://github.com/n8n-io/n8n/issues/13165)) ([47c5688](https://github.com/n8n-io/n8n/commit/47c5688618001a51c9412c5d07fd25d85b8d1b8d))
* **Code Tool Node:** Fix Input Schema Parameter not hiding correctly ([#13245](https://github.com/n8n-io/n8n/issues/13245)) ([8e15ebf](https://github.com/n8n-io/n8n/commit/8e15ebf8333d06b5fe4d5bf8ee39f285b31332d7))
* **core:** Redact credentials ([#13263](https://github.com/n8n-io/n8n/issues/13263)) ([052f177](https://github.com/n8n-io/n8n/commit/052f17744d072cd16ce90ea94fa9873b4ea2ffed))
* **core:** Reduce risk of race condition during workflow activation loop ([#13186](https://github.com/n8n-io/n8n/issues/13186)) ([64c5b6e](https://github.com/n8n-io/n8n/commit/64c5b6e0604ce9da6b19dd5f04e61e38209b3153))
* **core:** Run full manual execution when a trigger is executed even if run data exists ([#13194](https://github.com/n8n-io/n8n/issues/13194)) ([66acb1b](https://github.com/n8n-io/n8n/commit/66acb1bcb68926526ed98a5fe5b89bdaa74148d6))
* Display correct editor URL ([#13251](https://github.com/n8n-io/n8n/issues/13251)) ([67a4ed1](https://github.com/n8n-io/n8n/commit/67a4ed18a13cb2bc54b3472b9a8beb2f274c2bd2))
* **editor:** Add template id to metadata when saving workflows from json ([#13172](https://github.com/n8n-io/n8n/issues/13172)) ([2a92032](https://github.com/n8n-io/n8n/commit/2a92032704ebc4e0cdd11aa59b6834a9d891ffb0))
* **editor:** Fix page size resetting when filters are reset on workflows page ([#13265](https://github.com/n8n-io/n8n/issues/13265)) ([b4380d0](https://github.com/n8n-io/n8n/commit/b4380d05087e1213641ee322875cf51bf706d2f5))
* **editor:** Open autocompletion when starting an expression ([#13249](https://github.com/n8n-io/n8n/issues/13249)) ([6377635](https://github.com/n8n-io/n8n/commit/6377635bf03387c8d0ae5d54848113258bbabacc))
* **editor:** Prevent pagination setting from being overwritten in URL ([#13266](https://github.com/n8n-io/n8n/issues/13266)) ([d1e65a1](https://github.com/n8n-io/n8n/commit/d1e65a1cd5841f1d4e815f8da36713cdb18281a4))
* **editor:** Propagate isReadOnly to ResourceMapper `Attempt to Convert Types` switch ([#13216](https://github.com/n8n-io/n8n/issues/13216)) ([617f841](https://github.com/n8n-io/n8n/commit/617f841e0d82f2b40fcf9ac4bf2cb6a8010b517f))
* **editor:** Render assignments without ID correctly ([#13252](https://github.com/n8n-io/n8n/issues/13252)) ([d116f12](https://github.com/n8n-io/n8n/commit/d116f121e351e3d81e1b5d6c52eb3e5c3b68ae43))


### Features

* **editor:** Add pagination to the workflows list ([#13100](https://github.com/n8n-io/n8n/issues/13100)) ([8e37088](https://github.com/n8n-io/n8n/commit/8e370882490d569ff85bba6b7f0a1320fab5eb91))



# [1.79.0](https://github.com/n8n-io/n8n/compare/n8n@1.78.0...n8n@1.79.0) (2025-02-13)


### Bug Fixes

* **Airtable Node:** Use item at correct index in base/getSchema ([#13174](https://github.com/n8n-io/n8n/issues/13174)) ([f2e3586](https://github.com/n8n-io/n8n/commit/f2e35869c143d15ea79017ec103370c4aa92a92f))
* **Basic LLM Chain Node:** Use correct mimetype for binary data ([#12978](https://github.com/n8n-io/n8n/issues/12978)) ([2b1eb04](https://github.com/n8n-io/n8n/commit/2b1eb049f2c639f054e7c5f671483e29fd600567))
* **Call n8n Sub-Workflow Tool Node:** Fix json type when using $fromAI ([#13102](https://github.com/n8n-io/n8n/issues/13102)) ([9e4e1ca](https://github.com/n8n-io/n8n/commit/9e4e1ca1f48b08143883668be037026075eddb25))
* **core:** Add an option to enable dual-stack lookup to support IPv6 for redis ([#13118](https://github.com/n8n-io/n8n/issues/13118)) ([be39d0a](https://github.com/n8n-io/n8n/commit/be39d0a0f11c0274d2be1d7e1579264a95b18f7b))
* **core:** Allow secrets manager secrets to be used in credentials ([#13110](https://github.com/n8n-io/n8n/issues/13110)) ([cae98e7](https://github.com/n8n-io/n8n/commit/cae98e733d4cac7b5082bae345be504d00876c4b))
* **core:** Do not save credential overwrites data into the database ([#13170](https://github.com/n8n-io/n8n/issues/13170)) ([298a7b0](https://github.com/n8n-io/n8n/commit/298a7b00386dcfb670c27e6e1cc374f73d00a7a5))
* **core:** Fix high volume of node operation errors in Sentry ([#13053](https://github.com/n8n-io/n8n/issues/13053)) ([e59d983](https://github.com/n8n-io/n8n/commit/e59d9830bfda51bcf43246e32bf88bd045f8b8ad))
* **core:** Fix resuming executions on test webhooks from Wait nodes ([#13168](https://github.com/n8n-io/n8n/issues/13168)) ([5dddf77](https://github.com/n8n-io/n8n/commit/5dddf772cf1704f65ed86cea1f4640e3b274b14e))
* **core:** Handle cancellation of waiting executions correctly ([#13051](https://github.com/n8n-io/n8n/issues/13051)) ([fc440eb](https://github.com/n8n-io/n8n/commit/fc440eb68bb6750dc096cdaeb50fed7cf0718b07))
* **core:** Handle credential decryption failures gracefully on the API ([#13166](https://github.com/n8n-io/n8n/issues/13166)) ([a4c5334](https://github.com/n8n-io/n8n/commit/a4c5334853cbc71eddbb035b86d3dda68c3ef81e))
* **core:** Handle missing `json` property on `nodeSuccessData` ([#13219](https://github.com/n8n-io/n8n/issues/13219)) ([aedea7a](https://github.com/n8n-io/n8n/commit/aedea7a76c1752410b8734d87a74bd870cd54e2d))
* **core:** Same version of merge node behaves differently after n8n update ([#13106](https://github.com/n8n-io/n8n/issues/13106)) ([df8f059](https://github.com/n8n-io/n8n/commit/df8f059504266667ffd30b5d706bad9dd7e09ab3))
* **editor:** Adjust project plus button color in dark mode ([#13175](https://github.com/n8n-io/n8n/issues/13175)) ([4c19bae](https://github.com/n8n-io/n8n/commit/4c19baea3dd232df67353e8637470c205c37bd92))
* **editor:** Correctly compare old parameter value for nested parameters ([#13179](https://github.com/n8n-io/n8n/issues/13179)) ([b6c0d96](https://github.com/n8n-io/n8n/commit/b6c0d96e4376e1b5fbc80227633eae57b1eff4c0))
* **editor:** Disable fromAI button for vector stores ([#13125](https://github.com/n8n-io/n8n/issues/13125)) ([bde8420](https://github.com/n8n-io/n8n/commit/bde84205f924d79c3eb2bd45d2e3745b53992a0d))
* **editor:** Don't show 'Test workflow' button if the canvas is read-only ([#13199](https://github.com/n8n-io/n8n/issues/13199)) ([56426e9](https://github.com/n8n-io/n8n/commit/56426e989ff4ca01efad0b6d525e12e68d25e87f))
* **editor:** Fix '=' handling in expressions ([#13129](https://github.com/n8n-io/n8n/issues/13129)) ([8f25a06](https://github.com/n8n-io/n8n/commit/8f25a06e6ca7d4d0a78b5aa379a8c124f55a0325))
* **editor:** Fix alignment in RMC component ([#13167](https://github.com/n8n-io/n8n/issues/13167)) ([78644b0](https://github.com/n8n-io/n8n/commit/78644b0ec7007cabd1a908cfd81ec1b3f06db63d))
* **editor:** Fix issues with push connect reconnection ([#13085](https://github.com/n8n-io/n8n/issues/13085)) ([fff98b1](https://github.com/n8n-io/n8n/commit/fff98b16bb7c86e08ec2b1a475eeb7b93bedf2de))
* **editor:** Fix prompt in easy ai template ([#13091](https://github.com/n8n-io/n8n/issues/13091)) ([2eabca5](https://github.com/n8n-io/n8n/commit/2eabca5613dece94231395a89e84c5e4433bb730))
* **editor:** Load only personal credentials when setting up a template ([#12826](https://github.com/n8n-io/n8n/issues/12826)) ([814e2a8](https://github.com/n8n-io/n8n/commit/814e2a89241bdc6a26defb6bfd3d87abdc477ae0))
* **editor:** Make connector buttons background opaque when dark mode is enabled system-wide ([#13180](https://github.com/n8n-io/n8n/issues/13180)) ([77be25d](https://github.com/n8n-io/n8n/commit/77be25d337e32f2bb32e191ee579f30d0442b537))
* **Gmail Trigger Node:** Prevent error for empty emails, improve type safety ([#13171](https://github.com/n8n-io/n8n/issues/13171)) ([115a367](https://github.com/n8n-io/n8n/commit/115a367caeb9cbec8597d328cd969fff5ab6d941))
* **Google Sheets Node:** Do not delete row_number key from input item ([#13158](https://github.com/n8n-io/n8n/issues/13158)) ([da5e4be](https://github.com/n8n-io/n8n/commit/da5e4be0fd645df24892f81c553bc1808e3fec93))
* **Google Sheets Node:** RMC should correctly map columns if data location set in options ([#13116](https://github.com/n8n-io/n8n/issues/13116)) ([5d05f7f](https://github.com/n8n-io/n8n/commit/5d05f7f436a32b98d35a7b87968990e845ec56bb))
* **Google Sheets Trigger Node:** Do not return header row in rowAdded mode ([#13119](https://github.com/n8n-io/n8n/issues/13119)) ([cd8b300](https://github.com/n8n-io/n8n/commit/cd8b300d5c9c2a2911b50c737c88ba799a2f0799))
* **Microsoft OneDrive Node:** Try to download file using downloadUrl ([#13200](https://github.com/n8n-io/n8n/issues/13200)) ([67cd05c](https://github.com/n8n-io/n8n/commit/67cd05c6dc9407b09ed89a9dbb041f2f6d0ac500))
* **OpenAI Node:** Limit chat history to context window when using memory ([#13137](https://github.com/n8n-io/n8n/issues/13137)) ([f057cfb](https://github.com/n8n-io/n8n/commit/f057cfb46af198566935d811ba294e596c9ab5ec))
* **Summarize Node:** Not dealing with null values properly ([#13044](https://github.com/n8n-io/n8n/issues/13044)) ([9324e4f](https://github.com/n8n-io/n8n/commit/9324e4ffe66a8268e3d7d0eb2c127e35caee7a4c))


### Features

* Add ConvertAPI cred only node ([#12663](https://github.com/n8n-io/n8n/issues/12663)) ([731a9a7](https://github.com/n8n-io/n8n/commit/731a9a79456066d72f5d7ba6c343eca420407979))
* **core:** Add an option to allow community nodes as tools ([#13075](https://github.com/n8n-io/n8n/issues/13075)) ([2b133aa](https://github.com/n8n-io/n8n/commit/2b133aa201325e27baddaa2bfd5995dca2093728))
* **core:** Add migration to create model for folders feature ([#13060](https://github.com/n8n-io/n8n/issues/13060)) ([03f4ed8](https://github.com/n8n-io/n8n/commit/03f4ed8445bb1e1f0ef5c82b0164e50db3e2c45c))
* **editor:** Add ‘execute workflow’ buttons below triggers on the canvas ([#12769](https://github.com/n8n-io/n8n/issues/12769)) ([b17cbec](https://github.com/n8n-io/n8n/commit/b17cbec3af446e67db57a0927011d51a9317dff2))
* **editor:** Add docs link in $fromAI hover info tooltip ([#13097](https://github.com/n8n-io/n8n/issues/13097)) ([ff8b1c1](https://github.com/n8n-io/n8n/commit/ff8b1c11082f4e8caf2a474e57be3b3b328a1be3))
* **editor:** Expose `View Execution` links for erroneous sub-executions ([#13185](https://github.com/n8n-io/n8n/issues/13185)) ([11cf1cd](https://github.com/n8n-io/n8n/commit/11cf1cd23a181714e445ef58e97fdd7dca870dd7))
* **Microsoft Teams Node:** New operation sendAndWait ([#12964](https://github.com/n8n-io/n8n/issues/12964)) ([e925562](https://github.com/n8n-io/n8n/commit/e92556260f2b95022a852825f8475be369f0440a))
* **OpenAI Chat Model Node:** Add reasoning effort option to control the amount of reasoning tokens to use ([#13103](https://github.com/n8n-io/n8n/issues/13103)) ([76e0c99](https://github.com/n8n-io/n8n/commit/76e0c9961344d4baac60a50f1ec1e849e40586e6))


### Performance Improvements

* **core:** Batch workflow activation to speed up startup ([#13191](https://github.com/n8n-io/n8n/issues/13191)) ([17acf70](https://github.com/n8n-io/n8n/commit/17acf70591422bfea84b13f24c35d628bff4d35e))



# [1.78.0](https://github.com/n8n-io/n8n/compare/n8n@1.77.0...n8n@1.78.0) (2025-02-06)


### Bug Fixes

* **AI Agent Node:** Ignore SSL errors option for SQLAgent ([#13052](https://github.com/n8n-io/n8n/issues/13052)) ([a90529f](https://github.com/n8n-io/n8n/commit/a90529fd51ca88bc9640d24490dbeb2023c98e30))
* **Code Node:** Do not validate code within comments ([#12938](https://github.com/n8n-io/n8n/issues/12938)) ([cdfa225](https://github.com/n8n-io/n8n/commit/cdfa22593b69cf647c2a798d6571a9bbbd11c1b2))
* **core:** "Respond to Webhook" should work with workflows with waiting nodes ([#12806](https://github.com/n8n-io/n8n/issues/12806)) ([e8635f2](https://github.com/n8n-io/n8n/commit/e8635f257433748f4d7d2c4b0ae794de6bff5b28))
* **core:** Do not emit `workflow-post-execute` event for waiting executions ([#13065](https://github.com/n8n-io/n8n/issues/13065)) ([1593b6c](https://github.com/n8n-io/n8n/commit/1593b6cb4112ab2a85ca93c4eaec7d5f088895b1))
* **core:** Do not enable strict type validation by default for resource mapper ([#13037](https://github.com/n8n-io/n8n/issues/13037)) ([fdcff90](https://github.com/n8n-io/n8n/commit/fdcff9082b97314f8b04579ab6fa81c724916320))
* **core:** Fix empty node execution stack ([#12945](https://github.com/n8n-io/n8n/issues/12945)) ([7031569](https://github.com/n8n-io/n8n/commit/7031569a028bcc85558fcb614f8143d68a7f81f0))
* **core:** Only use new resource mapper type validation when it is enabled ([#13099](https://github.com/n8n-io/n8n/issues/13099)) ([a37c8e8](https://github.com/n8n-io/n8n/commit/a37c8e8fb86aaa3244ac13500ffa0e7c0d809a6f))
* **editor:** Actually enforce the version and don't break for old values in local storage ([#13025](https://github.com/n8n-io/n8n/issues/13025)) ([884a7e2](https://github.com/n8n-io/n8n/commit/884a7e23f84258756d8dcdd2dfe933bdedf61adc))
* **editor:** Add telemetry to source control feature ([#13016](https://github.com/n8n-io/n8n/issues/13016)) ([18eaa54](https://github.com/n8n-io/n8n/commit/18eaa5423dfc9348374c2cff4ae0e6f152268fbb))
* **editor:** Allow switch to `Fixed` for boolean and number parameters with invalid expressions ([#12948](https://github.com/n8n-io/n8n/issues/12948)) ([118be24](https://github.com/n8n-io/n8n/commit/118be24d25f001525ced03d9426a6129fa5a2053))
* **editor:** Allow to re-open sub-connection node creator if already active ([#13041](https://github.com/n8n-io/n8n/issues/13041)) ([16d59e9](https://github.com/n8n-io/n8n/commit/16d59e98edc427bf68edbce4cd2174a44d6dcfb1))
* **editor:** Code node overwrites code when switching nodes after edits ([#13078](https://github.com/n8n-io/n8n/issues/13078)) ([00e3ebc](https://github.com/n8n-io/n8n/commit/00e3ebc9e2e0b8cc2d88b678c3a2a21602dac010))
* **editor:** Fix execution running status listener for chat messages ([#12951](https://github.com/n8n-io/n8n/issues/12951)) ([4d55a29](https://github.com/n8n-io/n8n/commit/4d55a294600dc2c86f6f7019da923b66a4b9de7e))
* **editor:** Fix position of connector buttons when the line is straight ([#13034](https://github.com/n8n-io/n8n/issues/13034)) ([3a908ac](https://github.com/n8n-io/n8n/commit/3a908aca17f0bc1cf5fb5eb8813cc94f27f0bcdf))
* **editor:** Fix showing and hiding canvas edge toolbar when hovering ([#13009](https://github.com/n8n-io/n8n/issues/13009)) ([ac7bc4f](https://github.com/n8n-io/n8n/commit/ac7bc4f1911f913233eeeae5d229432fdff332c4))
* **editor:** Make AI transform node read only in executions view ([#12970](https://github.com/n8n-io/n8n/issues/12970)) ([ce1deb8](https://github.com/n8n-io/n8n/commit/ce1deb8aea528eef996fc774d0fff1dc61df5843))
* **editor:** Prevent infinite loop in expressions crashing the browser ([#12732](https://github.com/n8n-io/n8n/issues/12732)) ([8c2dbcf](https://github.com/n8n-io/n8n/commit/8c2dbcfeced70a0a84137773269cc6db2928d174))
* **editor:** Refine push modal layout ([#12886](https://github.com/n8n-io/n8n/issues/12886)) ([212a5bf](https://github.com/n8n-io/n8n/commit/212a5bf23eb11cc3296e7a8d002a4b7727d5193c))
* **editor:** SchemaView renders duplicate structures properly ([#12943](https://github.com/n8n-io/n8n/issues/12943)) ([0d8a544](https://github.com/n8n-io/n8n/commit/0d8a544975f72724db931778d7e3ace8a12b6cfc))
* **editor:** Update node issues when opening execution ([#12972](https://github.com/n8n-io/n8n/issues/12972)) ([1a91523](https://github.com/n8n-io/n8n/commit/1a915239c6571d7744023c6df6242dabe97c912e))
* **editor:** Use correct connection index when connecting adjancent nodes after deleting a node ([#12973](https://github.com/n8n-io/n8n/issues/12973)) ([c7a15d5](https://github.com/n8n-io/n8n/commit/c7a15d5980d181a865f8e2ec6a5f70d0681dcf56))
* **GitHub Node:** Don't truncate filenames retrieved from GitHub ([#12923](https://github.com/n8n-io/n8n/issues/12923)) ([7e18447](https://github.com/n8n-io/n8n/commit/7e1844757fe0d544e8881d229d16af95ed53fb21))
* **Google Cloud Firestore Node:** Fix potential prototype pollution vulnerability ([#13035](https://github.com/n8n-io/n8n/issues/13035)) ([f150f79](https://github.com/n8n-io/n8n/commit/f150f79ad6c7d43e036688b1de8d6c2c8140aca9))
* Increment runIndex in WorkflowToolV2 tool executions to avoid reusing out of date inputs ([#13008](https://github.com/n8n-io/n8n/issues/13008)) ([cc907fb](https://github.com/n8n-io/n8n/commit/cc907fbca9aa00fe07dd54a2fcac8983f2321ad1))
* Sync partial execution version of FE and BE, also allow enforcing a specific version ([#12840](https://github.com/n8n-io/n8n/issues/12840)) ([a155043](https://github.com/n8n-io/n8n/commit/a15504329bac582225185705566297d9cc27bf73))
* **Wise Node:** Use ISO formatting for timestamps ([#10288](https://github.com/n8n-io/n8n/issues/10288)) ([1a2d39a](https://github.com/n8n-io/n8n/commit/1a2d39a158c9a61bdaf11124b09ae70de65ebbf1))


### Features

* Add reusable frontend `composables` package ([#13077](https://github.com/n8n-io/n8n/issues/13077)) ([ef87da4](https://github.com/n8n-io/n8n/commit/ef87da4c193a08e089e48044906a4f5ce9959a22))
* Add support for client credentials with Azure Log monitor ([#13038](https://github.com/n8n-io/n8n/issues/13038)) ([2c2d631](https://github.com/n8n-io/n8n/commit/2c2d63157b7866f1a68cc45c5823e29570ccff77))
* Allow multi API creation via the UI ([#12845](https://github.com/n8n-io/n8n/issues/12845)) ([ad3250c](https://github.com/n8n-io/n8n/commit/ad3250ceb0df84379917e684d54d4100e3bf44f5))
* Allow setting API keys expiration ([#12954](https://github.com/n8n-io/n8n/issues/12954)) ([9bcbc2c](https://github.com/n8n-io/n8n/commit/9bcbc2c2ccbb88537e9b7554c92b631118d870f1))
* **core:** Add sorting to GET `/workflows` endpoint ([#13029](https://github.com/n8n-io/n8n/issues/13029)) ([b60011a](https://github.com/n8n-io/n8n/commit/b60011a1808d47f32ab84e685dba0e915e82df8f))
* **core:** Enable usage as a tool for more nodes ([#12930](https://github.com/n8n-io/n8n/issues/12930)) ([9deb759](https://github.com/n8n-io/n8n/commit/9deb75916e4eb63b899ba79b40cbd24b69a752db))
* **core:** Handle Declarative nodes more like regular nodes ([#13007](https://github.com/n8n-io/n8n/issues/13007)) ([a65a9e6](https://github.com/n8n-io/n8n/commit/a65a9e631b13bbe70ad64727fb1109ae7cd014eb))
* **Discord Node:** New sendAndWait operation ([#12894](https://github.com/n8n-io/n8n/issues/12894)) ([d47bfdd](https://github.com/n8n-io/n8n/commit/d47bfddd656367454b51da39cf87dbfb2bd59eb2))
* **editor:** Display schema preview for unexecuted nodes ([#12901](https://github.com/n8n-io/n8n/issues/12901)) ([0063bbb](https://github.com/n8n-io/n8n/commit/0063bbb30b45b3af92aff4c0f76b905d50a71a2d))
* **editor:** Easy $fromAI Button for AI Tools ([#12587](https://github.com/n8n-io/n8n/issues/12587)) ([2177376](https://github.com/n8n-io/n8n/commit/21773764d37c37a6464a3885d3fa548a5feb4fd8))
* **editor:** Show fixed collection parameter issues in UI ([#12899](https://github.com/n8n-io/n8n/issues/12899)) ([12d686c](https://github.com/n8n-io/n8n/commit/12d686ce52694f4c0b88f92a744451c1b0c66dec))
* **Facebook Graph API Node:** Update node to support API v22.0 ([#13024](https://github.com/n8n-io/n8n/issues/13024)) ([0bc0fc6](https://github.com/n8n-io/n8n/commit/0bc0fc6c1226688c29bf5f8f0ba7e8f244e16fbc))
* **HTTP Request Tool Node:** Relax binary data detection ([#13048](https://github.com/n8n-io/n8n/issues/13048)) ([b67a003](https://github.com/n8n-io/n8n/commit/b67a003e0b154d4e8c04392bec1c7b28171b5908))
* Human in the loop section ([#12883](https://github.com/n8n-io/n8n/issues/12883)) ([9590e5d](https://github.com/n8n-io/n8n/commit/9590e5d58b8964de9ce901bf07b537926d18b6b7))
* **n8n Form Node:** Add Hidden Fields ([#12803](https://github.com/n8n-io/n8n/issues/12803)) ([0da1114](https://github.com/n8n-io/n8n/commit/0da1114981978e371b216bdabc0c3bbdceeefa09))
* **n8n Form Node:** Respond with Text ([#12979](https://github.com/n8n-io/n8n/issues/12979)) ([182fc15](https://github.com/n8n-io/n8n/commit/182fc150bec62e9a5e2801d6c403e4a6bd35f728))
* **OpenAI Chat Model Node, OpenAI Node:** Include o3 models in model selection ([#13005](https://github.com/n8n-io/n8n/issues/13005)) ([37d152c](https://github.com/n8n-io/n8n/commit/37d152c148cafbe493c22e07f5d55ff24fcb0ca4))
* **Summarize Node:** Preserves original field data type ([#13069](https://github.com/n8n-io/n8n/issues/13069)) ([be5e49d](https://github.com/n8n-io/n8n/commit/be5e49d56c09d65c9768e948471626cfd3606c0c))



# [1.77.0](https://github.com/n8n-io/n8n/compare/n8n@1.76.0...n8n@1.77.0) (2025-01-29)


### Bug Fixes

* **core:** Account for pre-execution failure in scaling mode ([#12815](https://github.com/n8n-io/n8n/issues/12815)) ([b4d27c4](https://github.com/n8n-io/n8n/commit/b4d27c49e32bfacbd2690bf1c07194562f6a4a61))
* **core:** Display the last activated plan name when multiple are activated ([#12835](https://github.com/n8n-io/n8n/issues/12835)) ([03365f0](https://github.com/n8n-io/n8n/commit/03365f096d3d5c8e3a6537f37cda412959705346))
* **core:** Fix possible corruption of OAuth2 credential ([#12880](https://github.com/n8n-io/n8n/issues/12880)) ([ac84ea1](https://github.com/n8n-io/n8n/commit/ac84ea14452cbcec95f14073e8e70427169e6a7f))
* **core:** Fix usage of external libs in task runner ([#12788](https://github.com/n8n-io/n8n/issues/12788)) ([3d9d5bf](https://github.com/n8n-io/n8n/commit/3d9d5bf9d58f3c49830d42a140d6c8c6b59952dc))
* **core:** Handle max stalled count error better ([#12824](https://github.com/n8n-io/n8n/issues/12824)) ([eabf160](https://github.com/n8n-io/n8n/commit/eabf1609577cd94a6bad5020c34378d840a13bc0))
* **core:** Improve error handling in credential decryption and parsing ([#12868](https://github.com/n8n-io/n8n/issues/12868)) ([0c86bf2](https://github.com/n8n-io/n8n/commit/0c86bf2b3761bb93fd3cedba7a483ae5d97bd332))
* **core:** Renew license on startup for instances with detached floating entitlements ([#12884](https://github.com/n8n-io/n8n/issues/12884)) ([f32eef8](https://github.com/n8n-io/n8n/commit/f32eef85bd066ee9b54d110355c6b80124d67437))
* **core:** Update execution entity and execution data in transaction ([#12756](https://github.com/n8n-io/n8n/issues/12756)) ([1f43181](https://github.com/n8n-io/n8n/commit/1f4318136011bffaad04527790a9eba79effce35))
* **core:** Validate credential data before encryption ([#12885](https://github.com/n8n-io/n8n/issues/12885)) ([3d27a14](https://github.com/n8n-io/n8n/commit/3d27a1498702206b738cf978d037191306cec42b))
* **editor:** Add notice when user hits the limit for execution metadata item length ([#12676](https://github.com/n8n-io/n8n/issues/12676)) ([02df25c](https://github.com/n8n-io/n8n/commit/02df25c450a0a384a32d0815d8a2faec7562a8ae))
* **editor:** Don't send run data for full manual executions ([#12687](https://github.com/n8n-io/n8n/issues/12687)) ([9139dc3](https://github.com/n8n-io/n8n/commit/9139dc3c2916186648fb5bf63d14fcb90773eb1c))
* **editor:** Fix sub-execution links in empty output tables ([#12781](https://github.com/n8n-io/n8n/issues/12781)) ([114ed88](https://github.com/n8n-io/n8n/commit/114ed88368d137443b9c6605d4fe11b02053549d))
* **editor:** Fix workflow move project select filtering ([#12764](https://github.com/n8n-io/n8n/issues/12764)) ([358d284](https://github.com/n8n-io/n8n/commit/358d2843e5e468071d6764419169811e93138c35))
* **editor:** Focus executions iframe when n8n is ready to delegate keyboard events ([#12741](https://github.com/n8n-io/n8n/issues/12741)) ([d506218](https://github.com/n8n-io/n8n/commit/d5062189dbca02dfdf485fc220cc2a7b05e3e6cc))
* **editor:** Handle large payloads in the AI Assistant requests better ([#12747](https://github.com/n8n-io/n8n/issues/12747)) ([eb4dea1](https://github.com/n8n-io/n8n/commit/eb4dea1ca891bb7ac07c8bbbae8803de080c4623))
* **editor:** Hide Set up Template button for empty workflows ([#12808](https://github.com/n8n-io/n8n/issues/12808)) ([36e615b](https://github.com/n8n-io/n8n/commit/36e615b28f395623457bbb9bf4ab6fd69102b6ea))
* **editor:** Load appropriate credentials in canvas V2 for new workflow ([#12722](https://github.com/n8n-io/n8n/issues/12722)) ([2020dc5](https://github.com/n8n-io/n8n/commit/2020dc502feae6cae827dfbcc40ffed89bcc334a))
* **editor:** Properly set active project in new canvas ([#12810](https://github.com/n8n-io/n8n/issues/12810)) ([648c6f9](https://github.com/n8n-io/n8n/commit/648c6f9315b16b885e04716e7e0035a73b358fb0))
* **editor:** Render inline SVGs correctly on the external secrets settings page ([#12802](https://github.com/n8n-io/n8n/issues/12802)) ([5820ade](https://github.com/n8n-io/n8n/commit/5820ade1e4b9d638c9b6369aef369d6dc9320da6))
* **editor:** Show input selector when node has error ([#12813](https://github.com/n8n-io/n8n/issues/12813)) ([5b760e7](https://github.com/n8n-io/n8n/commit/5b760e7f7fc612b10307b4871e24b549f5d9d420))
* **editor:** Show mappings by default in sub-node NDVs when the root node isn't executed ([#12642](https://github.com/n8n-io/n8n/issues/12642)) ([fb662dd](https://github.com/n8n-io/n8n/commit/fb662dd95cae3bc51d05d05e32e772d05adafa1e))
* **Postgres PGVector Store Node:** Release postgres connections back to the pool ([#12723](https://github.com/n8n-io/n8n/issues/12723)) ([663dfb4](https://github.com/n8n-io/n8n/commit/663dfb48defd944f88f0ecc4f3347ea4f8a7c831))


### Features

* Add DeepSeek Chat Model node ([#12873](https://github.com/n8n-io/n8n/issues/12873)) ([9918afa](https://github.com/n8n-io/n8n/commit/9918afa51b16116abb73692a66df84e48128f406))
* Add OpenRouter node ([#12882](https://github.com/n8n-io/n8n/issues/12882)) ([dc85b02](https://github.com/n8n-io/n8n/commit/dc85b022d111d1e8b038ca1a9f6a1041f19cf2b0))
* Add timeout options to sendAndWait operations ([#12753](https://github.com/n8n-io/n8n/issues/12753)) ([3e9f24d](https://github.com/n8n-io/n8n/commit/3e9f24ddf462349145d89fe183313c95512c699b))
* **API:** Add route for schema static files ([#12770](https://github.com/n8n-io/n8n/issues/12770)) ([d981b56](https://github.com/n8n-io/n8n/commit/d981b5659a26f92b11e5d0cd5570504fd683626c))
* **core:** Explicitly report external hook failures ([#12830](https://github.com/n8n-io/n8n/issues/12830)) ([a24e442](https://github.com/n8n-io/n8n/commit/a24e4420bb9023f808acd756d125dffaea325968))
* **core:** Rename two task runner env vars ([#12763](https://github.com/n8n-io/n8n/issues/12763)) ([60187ca](https://github.com/n8n-io/n8n/commit/60187cab9bc9d21aa6ba710d772c068324e429f1))
* **editor:** Add evaluation workflow and enhance workflow selector with pinned data support ([#12773](https://github.com/n8n-io/n8n/issues/12773)) ([be967eb](https://github.com/n8n-io/n8n/commit/be967ebec07fab223513f93f50bcc389b9a4c548))
* **editor:** Always keep at least one executing node indicator in the workflow ([#12829](https://github.com/n8n-io/n8n/issues/12829)) ([c25c613](https://github.com/n8n-io/n8n/commit/c25c613a04a6773fa4014d9a0d290e443bcabbe0))
* **Google Chat Node:** Updates ([#12827](https://github.com/n8n-io/n8n/issues/12827)) ([e146ad0](https://github.com/n8n-io/n8n/commit/e146ad021a0be22cf51bafa3c015d03550e03d97))
* **Microsoft Outlook Node:** New operation sendAndWait ([#12795](https://github.com/n8n-io/n8n/issues/12795)) ([f4bf55f](https://github.com/n8n-io/n8n/commit/f4bf55f0d8278ff954344cf6397c10d8261b39a4))
* **n8n Form Node:** Add read-only/custom HTML form elements ([#12760](https://github.com/n8n-io/n8n/issues/12760)) ([ba8aa39](https://github.com/n8n-io/n8n/commit/ba8aa3921613c590caaac627fbb9837ccaf87783))
* **Send Email Node:** New operation sendAndWait ([#12775](https://github.com/n8n-io/n8n/issues/12775)) ([a197fbb](https://github.com/n8n-io/n8n/commit/a197fbb21b5642843d8bc3e657049aca99e0729d))
* **Summarize Node:** Turns error when field not found in items into warning ([#11889](https://github.com/n8n-io/n8n/issues/11889)) ([d7dda3f](https://github.com/n8n-io/n8n/commit/d7dda3f5de52925e554455f9f10e51bd173ea856))
* **Telegram Node:** New operation sendAndWait ([#12771](https://github.com/n8n-io/n8n/issues/12771)) ([2c58d47](https://github.com/n8n-io/n8n/commit/2c58d47f8eee1f865ecc1eeb89aa20c69c28abae))



# [1.76.0](https://github.com/n8n-io/n8n/compare/n8n@1.75.0...n8n@1.76.0) (2025-01-22)


### Bug Fixes

* **core:** Align saving behavior in `workflowExecuteAfter` hooks ([#12731](https://github.com/n8n-io/n8n/issues/12731)) ([9d76210](https://github.com/n8n-io/n8n/commit/9d76210a570e025d01d1f6596667abf40fbd8d12))
* **core:** AugmentObject should handle the constructor property correctly ([#12744](https://github.com/n8n-io/n8n/issues/12744)) ([36bc164](https://github.com/n8n-io/n8n/commit/36bc164da486f2e2d05091b457b8eea6521ca22e))
* **core:** Fix keyboard shortcuts for non-ansi layouts ([#12672](https://github.com/n8n-io/n8n/issues/12672)) ([4c8193f](https://github.com/n8n-io/n8n/commit/4c8193fedc2e3967c9a06c0652483128df509653))
* **core:** Fix license CLI commands showing incorrect renewal setting ([#12759](https://github.com/n8n-io/n8n/issues/12759)) ([024ada8](https://github.com/n8n-io/n8n/commit/024ada822c1bc40958e594bb08707cf77d3397ec))
* **core:** Fix license initialization failure on startup ([#12737](https://github.com/n8n-io/n8n/issues/12737)) ([ac2f647](https://github.com/n8n-io/n8n/commit/ac2f6476c114f51fafb9b7b66e41e0c87f4a1bf6))
* **core:** Recover successful data-less executions ([#12720](https://github.com/n8n-io/n8n/issues/12720)) ([a39b8bd](https://github.com/n8n-io/n8n/commit/a39b8bd32be50c8323e415f820b25b4bcb81d960))
* **core:** Remove run data of utility nodes for partial executions v2 ([#12673](https://github.com/n8n-io/n8n/issues/12673)) ([b66a9dc](https://github.com/n8n-io/n8n/commit/b66a9dc8fb6f7b19122cacbb7e2f86b4c921c3fb))
* **core:** Sync `hookFunctionsSave` and `hookFunctionsSaveWorker` ([#12740](https://github.com/n8n-io/n8n/issues/12740)) ([d410b8f](https://github.com/n8n-io/n8n/commit/d410b8f5a7e99658e1e8dcb2e02901bd01ce9c59))
* **core:** Update isDocker check to return true on kubernetes/containerd ([#12603](https://github.com/n8n-io/n8n/issues/12603)) ([c55dac6](https://github.com/n8n-io/n8n/commit/c55dac66ed97a2317d4c696c3b505790ec5d72fe))
* **editor:** Add unicode code points to expression language for emoji ([#12633](https://github.com/n8n-io/n8n/issues/12633)) ([819ebd0](https://github.com/n8n-io/n8n/commit/819ebd058d1d60b3663d92b4a652728da7134a3b))
* **editor:** Correct missing whitespace in JSON output ([#12677](https://github.com/n8n-io/n8n/issues/12677)) ([b098b19](https://github.com/n8n-io/n8n/commit/b098b19c7f0e3a9848c3fcfa012999050f2d3c7a))
* **editor:** Defer crypto.randomUUID call in CodeNodeEditor ([#12630](https://github.com/n8n-io/n8n/issues/12630)) ([58f6532](https://github.com/n8n-io/n8n/commit/58f6532630bacd288d3c0a79b40150f465898419))
* **editor:** Fix Code node bug erasing and overwriting code when switching between nodes ([#12637](https://github.com/n8n-io/n8n/issues/12637)) ([02d953d](https://github.com/n8n-io/n8n/commit/02d953db34ec4e44977a8ca908628b62cca82fde))
* **editor:** Fix execution list hover & selection colour in dark mode ([#12628](https://github.com/n8n-io/n8n/issues/12628)) ([95c40c0](https://github.com/n8n-io/n8n/commit/95c40c02cb8fef77cf633cf5aec08e98746cff36))
* **editor:** Fix JsonEditor with expressions ([#12739](https://github.com/n8n-io/n8n/issues/12739)) ([56c93ca](https://github.com/n8n-io/n8n/commit/56c93caae026738c1c0bebb4187b238e34a330f6))
* **editor:** Fix navbar height flickering during load ([#12738](https://github.com/n8n-io/n8n/issues/12738)) ([a96b3f0](https://github.com/n8n-io/n8n/commit/a96b3f0091798a52bb33107b919b5d8287ba7506))
* **editor:** Open chat when executing agent node in canvas v2  ([#12617](https://github.com/n8n-io/n8n/issues/12617)) ([457edd9](https://github.com/n8n-io/n8n/commit/457edd99bb853d8ccf3014605d5823933f3c0bc6))
* **editor:** Partial execution of a workflow with manual chat trigger ([#12662](https://github.com/n8n-io/n8n/issues/12662)) ([2f81b29](https://github.com/n8n-io/n8n/commit/2f81b29d341535b512df0aa01b25a91d109f113f))
* **editor:** Show connector label above the line when it's straight ([#12622](https://github.com/n8n-io/n8n/issues/12622)) ([c97bd48](https://github.com/n8n-io/n8n/commit/c97bd48a77643b9c2a5d7218e21b957af15cee0b))
* **editor:** Show run workflow button when chat trigger has pinned data ([#12616](https://github.com/n8n-io/n8n/issues/12616)) ([da8aafc](https://github.com/n8n-io/n8n/commit/da8aafc0e3a1b5d862f0723d0d53d2c38bcaebc3))
* **editor:** Update workflow re-initialization to use query parameter ([#12650](https://github.com/n8n-io/n8n/issues/12650)) ([982131a](https://github.com/n8n-io/n8n/commit/982131a75a32f741c120156826c303989aac189c))
* **Execute Workflow Node:** Pass binary data to sub-workflow ([#12635](https://github.com/n8n-io/n8n/issues/12635)) ([e9c152e](https://github.com/n8n-io/n8n/commit/e9c152e369a4c2762bd8e6ad17eaa704bb3771bb))
* **Google Gemini Chat Model Node:** Add base URL support for Google Gemini Chat API ([#12643](https://github.com/n8n-io/n8n/issues/12643)) ([14f4bc7](https://github.com/n8n-io/n8n/commit/14f4bc769027789513808b4000444edf99dc5d1c))
* **GraphQL Node:** Change default request format to json instead of graphql ([#11346](https://github.com/n8n-io/n8n/issues/11346)) ([c7c122f](https://github.com/n8n-io/n8n/commit/c7c122f9173df824cc1b5ab864333bffd0d31f82))
* **Jira Software Node:** Get custom fields(RLC) in update operation for server deployment type ([#12719](https://github.com/n8n-io/n8n/issues/12719)) ([353df79](https://github.com/n8n-io/n8n/commit/353df7941117e20547cd4f3fc514979a54619720))
* **n8n Form Node:** Remove the ability to change the formatting of dates ([#12666](https://github.com/n8n-io/n8n/issues/12666)) ([14904ff](https://github.com/n8n-io/n8n/commit/14904ff77951fef23eb789a43947492a4cd3fa20))
* **OpenAI Chat Model Node:** Fix loading of custom models when using custom credential URL ([#12634](https://github.com/n8n-io/n8n/issues/12634)) ([7cc553e](https://github.com/n8n-io/n8n/commit/7cc553e3b277a16682bfca1ea08cb98178e38580))
* **OpenAI Chat Model Node:** Restore default model value ([#12745](https://github.com/n8n-io/n8n/issues/12745)) ([d1b6692](https://github.com/n8n-io/n8n/commit/d1b6692736182fa2eab768ba3ad0adb8504ebbbd))
* **Postgres Chat Memory Node:** Do not terminate the connection pool ([#12674](https://github.com/n8n-io/n8n/issues/12674)) ([e7f00bc](https://github.com/n8n-io/n8n/commit/e7f00bcb7f2dce66ca07a9322d50f96356c1a43d))
* **Postgres Node:** Allow using composite key in upsert queries ([#12639](https://github.com/n8n-io/n8n/issues/12639)) ([83ce3a9](https://github.com/n8n-io/n8n/commit/83ce3a90963ba76601234f4314363a8ccc310f0f))
* **Wait Node:** Fix for hasNextPage in waiting forms ([#12636](https://github.com/n8n-io/n8n/issues/12636)) ([652b8d1](https://github.com/n8n-io/n8n/commit/652b8d170b9624d47b5f2d8d679c165cc14ea548))


### Features

* Add credential only node for Microsoft Azure Monitor ([#12645](https://github.com/n8n-io/n8n/issues/12645)) ([6ef8882](https://github.com/n8n-io/n8n/commit/6ef8882a108c672ab097c9dd1c590d4e9e7f3bcc))
* Add Miro credential only node ([#12746](https://github.com/n8n-io/n8n/issues/12746)) ([5b29086](https://github.com/n8n-io/n8n/commit/5b29086e2f9b7f638fac4440711f673438e57492))
* Add SSM endpoint to AWS credentials ([#12212](https://github.com/n8n-io/n8n/issues/12212)) ([565c7b8](https://github.com/n8n-io/n8n/commit/565c7b8b9cfd3e10f6a2c60add96fea4c4d95d33))
* **core:** Enable task runner by default ([#12726](https://github.com/n8n-io/n8n/issues/12726)) ([9e2a01a](https://github.com/n8n-io/n8n/commit/9e2a01aeaf36766a1cf7a1d9a4d6e02f45739bd3))
* **editor:** Force final canvas v2 migration and remove switcher from UI ([#12717](https://github.com/n8n-io/n8n/issues/12717)) ([29335b9](https://github.com/n8n-io/n8n/commit/29335b9b6acf97c817bea70688e8a2786fbd8889))
* **editor:** VariablesView Reskin - Add Filters for missing values ([#12611](https://github.com/n8n-io/n8n/issues/12611)) ([1eeb788](https://github.com/n8n-io/n8n/commit/1eeb788d327287d21eab7ad6f2156453ab7642c7))
* **Jira Software Node:** Personal Access Token credential type ([#11038](https://github.com/n8n-io/n8n/issues/11038)) ([1c7a38f](https://github.com/n8n-io/n8n/commit/1c7a38f6bab108daa47401cd98c185590bf299a8))
* **n8n Form Trigger Node:** Form Improvements ([#12590](https://github.com/n8n-io/n8n/issues/12590)) ([f167578](https://github.com/n8n-io/n8n/commit/f167578b3251e553a4d000e731e1bb60348916ad))
* Synchronize deletions when pulling from source control ([#12170](https://github.com/n8n-io/n8n/issues/12170)) ([967ee4b](https://github.com/n8n-io/n8n/commit/967ee4b89b94b92fc3955c56bf4c9cca0bd64eac))



# [1.75.0](https://github.com/n8n-io/n8n/compare/n8n@1.74.0...n8n@1.75.0) (2025-01-15)


### Bug Fixes

* **core:** AugmentObject should check for own propeties correctly ([#12534](https://github.com/n8n-io/n8n/issues/12534)) ([0cdf393](https://github.com/n8n-io/n8n/commit/0cdf39374305e6bbcedb047db7d3756168e6e89e))
* **core:** Disallow code generation in task runner ([#12522](https://github.com/n8n-io/n8n/issues/12522)) ([35b6180](https://github.com/n8n-io/n8n/commit/35b618098b7d23e272bf77b55c172dbe531c821f))
* **core:** Fix node exclusion on the frontend types ([#12544](https://github.com/n8n-io/n8n/issues/12544)) ([b2cbed9](https://github.com/n8n-io/n8n/commit/b2cbed9865888f6f3bc528984d4091d86a88f0d6))
* **core:** Fix orchestration flow with expired license ([#12444](https://github.com/n8n-io/n8n/issues/12444)) ([ecff3b7](https://github.com/n8n-io/n8n/commit/ecff3b732a028d7225bfbed4ffc65dc20c4ed608))
* **core:** Fix Sentry error reporting on task runners ([#12495](https://github.com/n8n-io/n8n/issues/12495)) ([88c0838](https://github.com/n8n-io/n8n/commit/88c0838dd72f11646bdb3586223d6c16631cccab))
* **core:** Improve cyclic dependency check in the DI container ([#12600](https://github.com/n8n-io/n8n/issues/12600)) ([c3c4a20](https://github.com/n8n-io/n8n/commit/c3c4a200024fb08afb9380357d1490c6707c5ec3))
* **core:** Only show personal credentials in the personal space ([#12433](https://github.com/n8n-io/n8n/issues/12433)) ([8a42d55](https://github.com/n8n-io/n8n/commit/8a42d55d91f4a37fff5669d52d52428b3a4ddd44))
* **core:** Prefix package name in `supportedNodes` on generated types as well ([#12514](https://github.com/n8n-io/n8n/issues/12514)) ([4a1a999](https://github.com/n8n-io/n8n/commit/4a1a9993624c92dd81f5418f9268cb93878069ab))
* **core:** Prevent prototype pollution in task runner ([#12588](https://github.com/n8n-io/n8n/issues/12588)) ([bdf266c](https://github.com/n8n-io/n8n/commit/bdf266cf55032d05641b20dce8804412dc93b6d5))
* **core:** Prevent prototype pollution of internal classes in task runner ([#12610](https://github.com/n8n-io/n8n/issues/12610)) ([eceee7f](https://github.com/n8n-io/n8n/commit/eceee7f3f8899d200b1c5720087cc494eec22e6a))
* **core:** Use timing safe function to compare runner auth tokens ([#12485](https://github.com/n8n-io/n8n/issues/12485)) ([8fab98f](https://github.com/n8n-io/n8n/commit/8fab98f3f1f767d05825d24cbf155d56375fdb3e))
* **core:** Validate values which are intentionally 0 ([#12382](https://github.com/n8n-io/n8n/issues/12382)) ([562506e](https://github.com/n8n-io/n8n/commit/562506e92aeb26423145801bff80037e5ce2ac46))
* Don't break oauth credentials when updating them and allow fixing broken oauth credentials by repeating the authorization flow ([#12563](https://github.com/n8n-io/n8n/issues/12563)) ([73897c7](https://github.com/n8n-io/n8n/commit/73897c7662a432834eb6f9d0f9ace8d986c1acb5))
* **editor:** Don't show toolsUnused notice if run had errors ([#12529](https://github.com/n8n-io/n8n/issues/12529)) ([3ec5b28](https://github.com/n8n-io/n8n/commit/3ec5b2850c47057032e61c2acdbdfc1dcdd931f7))
* **editor:** Ensure proper "AI Template" URL construction in node creator ([#12566](https://github.com/n8n-io/n8n/issues/12566)) ([13bf69f](https://github.com/n8n-io/n8n/commit/13bf69f75c67bc37a37013e776525768676a4b88))
* **editor:** Fix NDV resize handle and scrollbar overlapping ([#12509](https://github.com/n8n-io/n8n/issues/12509)) ([c28f302](https://github.com/n8n-io/n8n/commit/c28f302c2f863bd7aa73ad52e5d040f927e33220))
* **editor:** Fix parameter input validation ([#12532](https://github.com/n8n-io/n8n/issues/12532)) ([6711cbc](https://github.com/n8n-io/n8n/commit/6711cbcc641a2fc70f5c15a7e2dcc640a3f98b66))
* **editor:** Fix selection rectangle context menu on new canvas ([#12584](https://github.com/n8n-io/n8n/issues/12584)) ([c8e3c53](https://github.com/n8n-io/n8n/commit/c8e3c5399efde93486c1dd5c373cb2c5ff8a0691))
* **editor:** Fix the `openselectivenodecreator` custom action on new canvas ([#12580](https://github.com/n8n-io/n8n/issues/12580)) ([2110e9a](https://github.com/n8n-io/n8n/commit/2110e9a0513b8c36beb85302e0d38a2658ea5d6e))
* **editor:** Fix workflow initilisation for test definition routes & add unit tests ([#12507](https://github.com/n8n-io/n8n/issues/12507)) ([2775f61](https://github.com/n8n-io/n8n/commit/2775f617ae5c267c0a1ce7a54d05d4077cdbc0f7))
* **editor:** Make clicking item in RLC work the first time on small screens ([#12585](https://github.com/n8n-io/n8n/issues/12585)) ([479933f](https://github.com/n8n-io/n8n/commit/479933fbd5c88e783827960e018abb979de8a039))
* **editor:** Make sure code editors work correctly in fullscreen ([#12597](https://github.com/n8n-io/n8n/issues/12597)) ([aa1f3a7](https://github.com/n8n-io/n8n/commit/aa1f3a7d989883d55df3777775b8d7d336f6e3b7))
* **editor:** Override selected nodes on single click without Meta/Ctrl key ([#12549](https://github.com/n8n-io/n8n/issues/12549)) ([02c2d5e](https://github.com/n8n-io/n8n/commit/02c2d5e71d15b9292fddd585f47bd8334da468c5))
* **editor:** Show NDV errors when opening existing nodes with errors ([#12567](https://github.com/n8n-io/n8n/issues/12567)) ([bee7267](https://github.com/n8n-io/n8n/commit/bee7267fe38ab12a79fa4ec0e775f45d98d48aa5))
* **editor:** Swap Activate/Deactivate texts in FloatingToolbar ([#12526](https://github.com/n8n-io/n8n/issues/12526)) ([44679b4](https://github.com/n8n-io/n8n/commit/44679b42aa1e14bc7069bee47d0a91ca84b1dba4))
* **editor:** Update filter and feedback for source control ([#12504](https://github.com/n8n-io/n8n/issues/12504)) ([865fc21](https://github.com/n8n-io/n8n/commit/865fc21276727e8d88ccee0355147904b81c4421))
* **editor:** Update selected node when navigating via flowing nodes ([#12581](https://github.com/n8n-io/n8n/issues/12581)) ([88659d8](https://github.com/n8n-io/n8n/commit/88659d8a2901786c894902e19466f395bcdaab8e))
* **Google Calendar Node:** Updates and fixes ([#10715](https://github.com/n8n-io/n8n/issues/10715)) ([7227a29](https://github.com/n8n-io/n8n/commit/7227a29845fd178ced4d281597c62e7a03245456))
* **Spotify Node:** Fix issue with null values breaking the response ([#12080](https://github.com/n8n-io/n8n/issues/12080)) ([a56a462](https://github.com/n8n-io/n8n/commit/a56a46259d257003c813103578260d625b3f17dd))


### Features

* **editor:** Make node credential select searchable ([#12497](https://github.com/n8n-io/n8n/issues/12497)) ([91277c4](https://github.com/n8n-io/n8n/commit/91277c44f1cf3f334b3b50d47d7dcc79b11c7c63))
* **editor:** Persist sidebar collapsed status preference ([#12505](https://github.com/n8n-io/n8n/issues/12505)) ([dba7d46](https://github.com/n8n-io/n8n/commit/dba7d46f3ec91d26a597a50dede7b6ca292c728f))



# [1.74.0](https://github.com/n8n-io/n8n/compare/n8n@1.73.0...n8n@1.74.0) (2025-01-08)


### Bug Fixes

* **core:** Align concurrency and timeout defaults between instance and runner ([#12503](https://github.com/n8n-io/n8n/issues/12503)) ([9953477](https://github.com/n8n-io/n8n/commit/9953477450c28ec2d211e55aadb825dbae2ee4d6))
* **core:** Allow `index` as top-level item key for Code node ([#12469](https://github.com/n8n-io/n8n/issues/12469)) ([1b91000](https://github.com/n8n-io/n8n/commit/1b9100032fc9f8c33e263c8299e04054105da384))
* **core:** Don't fail task runner task if logging fails ([#12401](https://github.com/n8n-io/n8n/issues/12401)) ([0860fbe](https://github.com/n8n-io/n8n/commit/0860fbe97108edc21bc01dec3b6ef13e60e728d4))
* **core:** Ensure tasks timeout even if they don't receive settings ([#12431](https://github.com/n8n-io/n8n/issues/12431)) ([b194026](https://github.com/n8n-io/n8n/commit/b1940268e6110ed3d8949318a5252ac6563d624f))
* **core:** Fix execution cancellation issues in scaling mode ([#12343](https://github.com/n8n-io/n8n/issues/12343)) ([e26b406](https://github.com/n8n-io/n8n/commit/e26b406665e20761279c4e315d04501350427de5))
* **core:** Fix manually running a pinned trigger with offloading enabled ([#12491](https://github.com/n8n-io/n8n/issues/12491)) ([be2dcff](https://github.com/n8n-io/n8n/commit/be2dcffc9487973d3e287dd4f6956dbba03757e3))
* **core:** Fix task runner sending too many offers ([#12415](https://github.com/n8n-io/n8n/issues/12415)) ([4498e35](https://github.com/n8n-io/n8n/commit/4498e3519276020d3eb01752b5ce0d8ecfbf5fa4))
* **core:** Increase default concurrency and timeout in task runners ([#12496](https://github.com/n8n-io/n8n/issues/12496)) ([4182095](https://github.com/n8n-io/n8n/commit/4182095af1c02832af2523f31e9cb85d9a345e60))
* **core:** Prevent `__default__` jobs in scaling mode ([#12402](https://github.com/n8n-io/n8n/issues/12402)) ([072664b](https://github.com/n8n-io/n8n/commit/072664b40e06943e0b8ff44287730f2ca569646f))
* **core:** Register workflows as active only after all of the triggers and pollers setup successfully ([#12244](https://github.com/n8n-io/n8n/issues/12244)) ([f924f2a](https://github.com/n8n-io/n8n/commit/f924f2a6d736e33ab5fc12cbac6cba27340839db))
* **core:** Return unredacted credentials from `GET credentials/:id` ([#12447](https://github.com/n8n-io/n8n/issues/12447)) ([ecabe34](https://github.com/n8n-io/n8n/commit/ecabe34705bbbba07613ba14760449ef38e1b31f))
* **core:** Use rate limiter for task runner endpoints ([#12486](https://github.com/n8n-io/n8n/issues/12486)) ([491cb60](https://github.com/n8n-io/n8n/commit/491cb605e3c93d7a261bb0cef0d38f2ddc3affe8))
* **editor:** Allow zooming when panning keycode is pressed on new canvas ([#12327](https://github.com/n8n-io/n8n/issues/12327)) ([983e87a](https://github.com/n8n-io/n8n/commit/983e87a9b0c83d35354ce4df34096f47173d0ea7))
* **editor:** Consistent protected environment styling and messaging ([#12374](https://github.com/n8n-io/n8n/issues/12374)) ([6891cef](https://github.com/n8n-io/n8n/commit/6891cefa6d0359f85a596829b6055a13529fb1fb))
* **editor:** First project button tweaks border and copy ([#12376](https://github.com/n8n-io/n8n/issues/12376)) ([e234756](https://github.com/n8n-io/n8n/commit/e234756457d3c3526531ced4471bf9e69a79fa55))
* **editor:** Fix Multi option parameter expression when the value is an array ([#12430](https://github.com/n8n-io/n8n/issues/12430)) ([452a7bf](https://github.com/n8n-io/n8n/commit/452a7bfe2c1e786c46a3ed99de007b0cf3f28d15))
* **editor:** Improve configurable nodes design on new canvas ([#12317](https://github.com/n8n-io/n8n/issues/12317)) ([0ecce10](https://github.com/n8n-io/n8n/commit/0ecce10faf60ae44d11007d45e87766b678d3a84))
* **editor:** Minor styling improvements in project settings page ([#12405](https://github.com/n8n-io/n8n/issues/12405)) ([09ddce0](https://github.com/n8n-io/n8n/commit/09ddce05800f426d33489ae28c416bb6aab2fd91))
* **editor:** Never show Pinned Data Callout for Input Panel ([#12446](https://github.com/n8n-io/n8n/issues/12446)) ([1d5c9bd](https://github.com/n8n-io/n8n/commit/1d5c9bd466becf8aa245a1e8d0b799616d18914a))
* **editor:** Nodes' icon color in dark mode ([#12279](https://github.com/n8n-io/n8n/issues/12279)) ([01b781a](https://github.com/n8n-io/n8n/commit/01b781a10828ca2c4cf32762373ad40904c02d2c))
* **editor:** Only ignore managed credentials in the HTTP node ([#12417](https://github.com/n8n-io/n8n/issues/12417)) ([6b46657](https://github.com/n8n-io/n8n/commit/6b46657412a1efff35be5083f0ff4c00f9b3e7f9))
* **editor:** Remove primary highlight color from edge being executed on new canvas ([#12307](https://github.com/n8n-io/n8n/issues/12307)) ([50913de](https://github.com/n8n-io/n8n/commit/50913de2651450e18307a833ada57656d8959493))
* **editor:** Render empty string instead of [empty] ([#12448](https://github.com/n8n-io/n8n/issues/12448)) ([2c72047](https://github.com/n8n-io/n8n/commit/2c72047d0b260db5a4b1fd0d7448ab19378e908f))
* **editor:** Show all workflows in the error workflow dropdown in the workflow settings ([#12413](https://github.com/n8n-io/n8n/issues/12413)) ([ccda7f9](https://github.com/n8n-io/n8n/commit/ccda7f9c62e2ba04dbd8a86cfeb5016b56f19c7a))
* **editor:** Unify disabled parameters background color ([#12306](https://github.com/n8n-io/n8n/issues/12306)) ([8c63599](https://github.com/n8n-io/n8n/commit/8c635993bd65c84707938d9564d54c1ae17f1c1f))
* **HTTP Request Node:** Fix typo in hint ([#12439](https://github.com/n8n-io/n8n/issues/12439)) ([b6230b6](https://github.com/n8n-io/n8n/commit/b6230b63f2ed8c7531b53c896f8b033c599e156e))
* **OpenAI Node:** Add quotes to default base URL ([#12312](https://github.com/n8n-io/n8n/issues/12312)) ([2e90eba](https://github.com/n8n-io/n8n/commit/2e90eba47eff81f8b17a305cbc1656f929d622f8))
* **OpenAI Node:** Update node to account for URL in credentials ([#12356](https://github.com/n8n-io/n8n/issues/12356)) ([f78cceb](https://github.com/n8n-io/n8n/commit/f78ccebe514819dca03f5c220274b94fd6d1c73b))
* **Postgres Node:** Account for JSON expressions ([#12012](https://github.com/n8n-io/n8n/issues/12012)) ([06b86af](https://github.com/n8n-io/n8n/commit/06b86af7356b3be0af146c49f9720b24157b9e61))
* **Postgres Node:** Allow passing in arrays to JSON columns for insert ([#12452](https://github.com/n8n-io/n8n/issues/12452)) ([9dd0686](https://github.com/n8n-io/n8n/commit/9dd068632b1542126831baa83cf638ce369b0947))
* **Postgres Node:** Re-use connection pool across executions ([#12346](https://github.com/n8n-io/n8n/issues/12346)) ([2ca37f5](https://github.com/n8n-io/n8n/commit/2ca37f5f7f7f80c50dbc8c87146b8bff510f01c8))
* Run workflow if active and single webhook service has pin data ([#12425](https://github.com/n8n-io/n8n/issues/12425)) ([8053a4a](https://github.com/n8n-io/n8n/commit/8053a4a1763d143da80b9e4e00dcef9b716ce6b2))
* Set correct default for added Resource Mapper boolean fields ([#12344](https://github.com/n8n-io/n8n/issues/12344)) ([b4c77f2](https://github.com/n8n-io/n8n/commit/b4c77f27b66275ddb58138e8d2fe1509265e9652))
* **Supabase Node:** Allow for filtering on the same field multiple times ([#12429](https://github.com/n8n-io/n8n/issues/12429)) ([d7cc789](https://github.com/n8n-io/n8n/commit/d7cc789d79477aff40ff4eca0175c7578aef338a))
* **Zep Vector Store Node:** Cloud vector store integration ([#12353](https://github.com/n8n-io/n8n/issues/12353)) ([2433d6b](https://github.com/n8n-io/n8n/commit/2433d6b7d3dede2595dd5b637ca8bbc1103272b3))


### Features

* (Execute Workflow Node): Inputs for Sub-workflows ([#11830](https://github.com/n8n-io/n8n/issues/11830)) ([#11837](https://github.com/n8n-io/n8n/issues/11837)) ([d411663](https://github.com/n8n-io/n8n/commit/d4116630a638195c7d87e01e2b5c151941636056))
* Add load options to new tool mode for vector stores ([#12462](https://github.com/n8n-io/n8n/issues/12462)) ([3109de6](https://github.com/n8n-io/n8n/commit/3109de6073b237ee3dcc93afb69345586f3b836d))
* Add migration to add `managed` column to credentials table ([#12275](https://github.com/n8n-io/n8n/issues/12275)) ([3cb7081](https://github.com/n8n-io/n8n/commit/3cb70814465e8fa504e909ef36b21b79d4b70b28))
* Allow using Vector Stores directly as Tools ([#12311](https://github.com/n8n-io/n8n/issues/12311)) ([76dded4](https://github.com/n8n-io/n8n/commit/76dded4bea9d26ad84fdbde74d577d244eb4e223))
* **core:** Add endpoint to create free AI credits ([#12362](https://github.com/n8n-io/n8n/issues/12362)) ([ac4e042](https://github.com/n8n-io/n8n/commit/ac4e0422316a4dcd19151dd7d504e2b3cccbc038))
* **core:** Add includeData parameter to `GET /credentials` ([#12220](https://github.com/n8n-io/n8n/issues/12220)) ([f56ad8c](https://github.com/n8n-io/n8n/commit/f56ad8cf49f7cf0665035d2e43bb7ff5b8fd75f3))
* **core:** Comply with `NO_COLOR` in logs ([#12347](https://github.com/n8n-io/n8n/issues/12347)) ([1e60bbc](https://github.com/n8n-io/n8n/commit/1e60bbcf169e8624a97ddde543cdd1d406e5c7ca))
* **core:** Offload manual executions to workers ([#11284](https://github.com/n8n-io/n8n/issues/11284)) ([9432aa0](https://github.com/n8n-io/n8n/commit/9432aa0b00e74faf4651ac673f18e16b7e56e145))
* **editor:** Add free AI credits CTA ([#12365](https://github.com/n8n-io/n8n/issues/12365)) ([f873196](https://github.com/n8n-io/n8n/commit/f8731963f6754386f15c8417c0cc32dba87c481a))
* **editor:** Add support for project icons ([#12349](https://github.com/n8n-io/n8n/issues/12349)) ([9117718](https://github.com/n8n-io/n8n/commit/9117718cc960e2bad5a5db07b10e9e7b561ec5e4))
* **editor:** Easy AI workflow improvements ([#12400](https://github.com/n8n-io/n8n/issues/12400)) ([8dc691d](https://github.com/n8n-io/n8n/commit/8dc691dc62692f8af143c84032391397adeb790d))
* **editor:** Make workflows, credentials, executions and new canvas usable on mobile and touch devices ([#12372](https://github.com/n8n-io/n8n/issues/12372)) ([06c9473](https://github.com/n8n-io/n8n/commit/06c94732103687705d71c5a1c5bfa993e3df3427))
* **editor:** New Code editor based on the TypeScript language service ([#12285](https://github.com/n8n-io/n8n/issues/12285)) ([52ae02a](https://github.com/n8n-io/n8n/commit/52ae02abaa92e5bbfda58843c8eccc845506fa4b))
* **editor:** Update Sub-Workflow Debugging Copy ([#12483](https://github.com/n8n-io/n8n/issues/12483)) ([04e2928](https://github.com/n8n-io/n8n/commit/04e2928d345f83c202c762e4673cf878b4762f33))
* **Google Vertex Chat Model Node:** Add an option to specify GCP region ([#12300](https://github.com/n8n-io/n8n/issues/12300)) ([30f9c03](https://github.com/n8n-io/n8n/commit/30f9c033db28112e1f97bb55d41b5bfce265cb51))
* **HighLevel Node:** Add support for calendar items ([#10820](https://github.com/n8n-io/n8n/issues/10820)) ([6e189fd](https://github.com/n8n-io/n8n/commit/6e189fda776051e09e90b3d86ecd0d1e80dcc0c6))
* **Microsoft Entra ID Node:** New node ([#11779](https://github.com/n8n-io/n8n/issues/11779)) ([3006ccf](https://github.com/n8n-io/n8n/commit/3006ccf41bb911ba72f087a1479889fbf308c17d))



# [1.73.0](https://github.com/n8n-io/n8n/compare/n8n@1.72.0...n8n@1.73.0) (2024-12-19)


### Bug Fixes

* **core:** Ensure runners do not throw on unsupported console methods ([#12167](https://github.com/n8n-io/n8n/issues/12167)) ([57c6a61](https://github.com/n8n-io/n8n/commit/57c6a6167dd2b30f0082a416daefce994ecad33a))
* **core:** Fix `$getWorkflowStaticData` on task runners ([#12153](https://github.com/n8n-io/n8n/issues/12153)) ([b479f14](https://github.com/n8n-io/n8n/commit/b479f14ef5012551b823bea5d2ffbddedfd50a77))
* **core:** Fix binary data helpers (like `prepareBinaryData`) with task runner ([#12259](https://github.com/n8n-io/n8n/issues/12259)) ([0f1461f](https://github.com/n8n-io/n8n/commit/0f1461f2d5d7ec34236ed7fcec3e2f9ee7eb73c4))
* **core:** Fix race condition in AI tool invocation with multiple items from the parent ([#12169](https://github.com/n8n-io/n8n/issues/12169)) ([dce0c58](https://github.com/n8n-io/n8n/commit/dce0c58f8605c33fc50ec8aa422f0fb5eee07637))
* **core:** Fix serialization of circular json with task runner ([#12288](https://github.com/n8n-io/n8n/issues/12288)) ([a99d726](https://github.com/n8n-io/n8n/commit/a99d726f42d027b64f94eda0d385b597c5d5be2e))
* **core:** Upgrade nanoid to address CVE-2024-55565 ([#12171](https://github.com/n8n-io/n8n/issues/12171)) ([8c0bd02](https://github.com/n8n-io/n8n/commit/8c0bd0200c386b122f495c453ccc97a001e4729c))
* **editor:** Add new create first project CTA ([#12189](https://github.com/n8n-io/n8n/issues/12189)) ([878b419](https://github.com/n8n-io/n8n/commit/878b41904d76eda3ee230f850127b4d56993de24))
* **editor:** Fix canvas ready opacity transition on new canvas ([#12264](https://github.com/n8n-io/n8n/issues/12264)) ([5d33a6b](https://github.com/n8n-io/n8n/commit/5d33a6ba8a2bccea097402fd04c0e2b00e423e76))
* **editor:** Fix rendering of code-blocks in sticky notes ([#12227](https://github.com/n8n-io/n8n/issues/12227)) ([9b59035](https://github.com/n8n-io/n8n/commit/9b5903524b95bd21d5915908780942790cf88d27))
* **editor:** Fix sticky color picker getting covered by nodes on new canvas ([#12263](https://github.com/n8n-io/n8n/issues/12263)) ([27bd3c8](https://github.com/n8n-io/n8n/commit/27bd3c85b3a4ddcf763a543b232069bb108130cf))
* **editor:** Improve commit modal user facing messaging ([#12161](https://github.com/n8n-io/n8n/issues/12161)) ([ad39243](https://github.com/n8n-io/n8n/commit/ad392439826b17bd0b84f981e0958d88f09e7fe9))
* **editor:** Prevent connection line from showing when clicking the plus button of a node ([#12265](https://github.com/n8n-io/n8n/issues/12265)) ([9180b46](https://github.com/n8n-io/n8n/commit/9180b46b52302b203eecf3bb81c3f2132527a1e6))
* **editor:** Prevent stickies from being edited in preview mode in the new canvas ([#12222](https://github.com/n8n-io/n8n/issues/12222)) ([6706dcd](https://github.com/n8n-io/n8n/commit/6706dcdf72d54f33c1cf4956602c3a64a1578826))
* **editor:** Reduce cases for Auto-Add of ChatTrigger for AI Agents ([#12154](https://github.com/n8n-io/n8n/issues/12154)) ([365e82d](https://github.com/n8n-io/n8n/commit/365e82d2008dff2f9c91664ee04d7a78363a8b30))
* **editor:** Remove invalid connections after node handles change ([#12247](https://github.com/n8n-io/n8n/issues/12247)) ([6330bec](https://github.com/n8n-io/n8n/commit/6330bec4db0175b558f2747837323fdbb25b634a))
* **editor:** Set dangerouslyUseHTMLString in composable ([#12280](https://github.com/n8n-io/n8n/issues/12280)) ([6ba91b5](https://github.com/n8n-io/n8n/commit/6ba91b5e1ed197c67146347a6f6e663ecdf3de48))
* **editor:** Set RunData outputIndex based on incoming data ([#12182](https://github.com/n8n-io/n8n/issues/12182)) ([dc4261a](https://github.com/n8n-io/n8n/commit/dc4261ae7eca6cf277404cd514c90fad42f14ae0))
* **editor:** Update the universal create button interaction ([#12105](https://github.com/n8n-io/n8n/issues/12105)) ([5300e0a](https://github.com/n8n-io/n8n/commit/5300e0ac45bf832b3d2957198a49a1c687f3fe1f))
* **Elasticsearch Node:** Fix issue stopping search queries being sent ([#11464](https://github.com/n8n-io/n8n/issues/11464)) ([388a83d](https://github.com/n8n-io/n8n/commit/388a83dfbdc6ac301e4df704666df9f09fb7d0b3))
* **Extract from File Node:** Detect file encoding  ([#12081](https://github.com/n8n-io/n8n/issues/12081)) ([92af245](https://github.com/n8n-io/n8n/commit/92af245d1aab5bfad8618fda69b2405f5206875d))
* **Github Node:** Fix fetch of file names with ? character ([#12206](https://github.com/n8n-io/n8n/issues/12206)) ([39462ab](https://github.com/n8n-io/n8n/commit/39462abe1fde7e82b5e5b8f3ceebfcadbfd7c925))
* **Invoice Ninja Node:** Fix actions for bank transactions ([#11511](https://github.com/n8n-io/n8n/issues/11511)) ([80eea49](https://github.com/n8n-io/n8n/commit/80eea49cf0bf9db438eb85af7cd22aeb11fbfed2))
* **Linear Node:** Fix issue with error handling ([#12191](https://github.com/n8n-io/n8n/issues/12191)) ([b8eae5f](https://github.com/n8n-io/n8n/commit/b8eae5f28a7d523195f4715cd8da77b3a884ae4c))
* **MongoDB Node:** Fix checks on projection feature call ([#10563](https://github.com/n8n-io/n8n/issues/10563)) ([58bab46](https://github.com/n8n-io/n8n/commit/58bab461c4c5026b2ca5ea143cbcf98bf3a4ced8))
* **Postgres Node:** Allow users to wrap strings with $$  ([#12034](https://github.com/n8n-io/n8n/issues/12034)) ([0c15e30](https://github.com/n8n-io/n8n/commit/0c15e30778cc5cb10ed368df144d6fbb2504ec70))
* **Redis Node:** Add support for username auth ([#12274](https://github.com/n8n-io/n8n/issues/12274)) ([64c0414](https://github.com/n8n-io/n8n/commit/64c0414ef28acf0f7ec42b4b0bb21cbf2921ebe7))


### Features

* Add solarwinds ipam credentials ([#12005](https://github.com/n8n-io/n8n/issues/12005)) ([882484e](https://github.com/n8n-io/n8n/commit/882484e8ee7d1841d5d600414ca48e9915abcfa8))
* Add SolarWinds Observability node credentials ([#11805](https://github.com/n8n-io/n8n/issues/11805)) ([e8a5db5](https://github.com/n8n-io/n8n/commit/e8a5db5beb572edbb61dd9100b70827ccc4cca58))
* **AI Agent Node:** Update descriptions and titles for Chat Trigger options in AI Agents and Memory ([#12155](https://github.com/n8n-io/n8n/issues/12155)) ([07a6ae1](https://github.com/n8n-io/n8n/commit/07a6ae11b3291c1805553d55ba089fe8dd919fd8))
* **API:** Exclude pinned data from workflows ([#12261](https://github.com/n8n-io/n8n/issues/12261)) ([e0dc385](https://github.com/n8n-io/n8n/commit/e0dc385f8bc8ee13fbc5bbf35e07654e52b193e9))
* **editor:** Params pane collection improvements ([#11607](https://github.com/n8n-io/n8n/issues/11607)) ([6e44c71](https://github.com/n8n-io/n8n/commit/6e44c71c9ca82cce20eb55bb9003930bbf66a16c))
* **editor:** Support adding nodes via drag and drop from node creator on new canvas ([#12197](https://github.com/n8n-io/n8n/issues/12197)) ([1bfd9c0](https://github.com/n8n-io/n8n/commit/1bfd9c0e913f3eefc4593f6c344db1ae1f6e4df4))
* **Facebook Graph API Node:** Update node to support API v21.0 ([#12116](https://github.com/n8n-io/n8n/issues/12116)) ([14c33f6](https://github.com/n8n-io/n8n/commit/14c33f666fe92f7173e4f471fb478e629e775c62))
* **Linear Trigger Node:** Add support for admin scope ([#12211](https://github.com/n8n-io/n8n/issues/12211)) ([410ea9a](https://github.com/n8n-io/n8n/commit/410ea9a2ef2e14b5e8e4493e5db66cfc2290d8f6))
* **MailerLite Node:** Update node to support new api ([#11933](https://github.com/n8n-io/n8n/issues/11933)) ([d6b8e65](https://github.com/n8n-io/n8n/commit/d6b8e65abeb411f86538c1630dcce832ee0846a9))
* Send and wait operation - freeText and customForm response types ([#12106](https://github.com/n8n-io/n8n/issues/12106)) ([e98c7f1](https://github.com/n8n-io/n8n/commit/e98c7f160b018243dc88490d46fb1047a4d7fcdc))


### Performance Improvements

* **editor:** SchemaView performance improvement by ≈90% 🚀  ([#12180](https://github.com/n8n-io/n8n/issues/12180)) ([6a58309](https://github.com/n8n-io/n8n/commit/6a5830959f5fb493a4119869b8298d8ed702c84a))



# [1.72.0](https://github.com/n8n-io/n8n/compare/n8n@1.71.0...n8n@1.72.0) (2024-12-11)


### Bug Fixes

* Allow disabling MFA with recovery codes ([#12014](https://github.com/n8n-io/n8n/issues/12014)) ([95d56fe](https://github.com/n8n-io/n8n/commit/95d56fee8d0168b75fca6dcf41702d2f10c930a8))
* Chat triggers don't work with the new partial execution flow ([#11952](https://github.com/n8n-io/n8n/issues/11952)) ([2b6a72f](https://github.com/n8n-io/n8n/commit/2b6a72f1289c01145edf2b88e5027d2b9b2ed624))
* **core:** Execute nodes after loops correctly with the new partial execution flow ([#11978](https://github.com/n8n-io/n8n/issues/11978)) ([891dd7f](https://github.com/n8n-io/n8n/commit/891dd7f995c78a2355a049b7ced981a5f6b1c40c))
* **core:** Fix support for multiple invocation of AI tools ([#12141](https://github.com/n8n-io/n8n/issues/12141)) ([c572c06](https://github.com/n8n-io/n8n/commit/c572c0648ca5b644b222157b3cabac9c05704a84))
* **core:** Make sure task runner exits ([#12123](https://github.com/n8n-io/n8n/issues/12123)) ([c5effca](https://github.com/n8n-io/n8n/commit/c5effca7d47a713f157eea21d7892002e9ab7283))
* **core:** Remove run data of nodes unrelated to the current partial execution ([#12099](https://github.com/n8n-io/n8n/issues/12099)) ([c4e4d37](https://github.com/n8n-io/n8n/commit/c4e4d37a8785d1a4bcd376cb1c49b82a80aa4391))
* **core:** Return homeProject when filtering workflows by project id ([#12077](https://github.com/n8n-io/n8n/issues/12077)) ([efafeed](https://github.com/n8n-io/n8n/commit/efafeed33482100a23fa0163a53b9ce93cd6b2c3))
* **editor:** Don't reset all Parameter Inputs when switched to read-only  ([#12063](https://github.com/n8n-io/n8n/issues/12063)) ([706702d](https://github.com/n8n-io/n8n/commit/706702dff8da3c2e949e2c98dd5b34b299a1f17c))
* **editor:** Fix canvas panning using `Control` + `Left Mouse Button` on Windows ([#12104](https://github.com/n8n-io/n8n/issues/12104)) ([43009b6](https://github.com/n8n-io/n8n/commit/43009b6aa820f24b9e6f519e7a45592aa21db03e))
* **editor:** Fix Nodeview.v2 reinitialise based on route changes ([#12062](https://github.com/n8n-io/n8n/issues/12062)) ([b1f8663](https://github.com/n8n-io/n8n/commit/b1f866326574974eb2936e6b02771346e83e7137))
* **editor:** Fix svg background pattern rendering on safari ([#12079](https://github.com/n8n-io/n8n/issues/12079)) ([596f221](https://github.com/n8n-io/n8n/commit/596f22103c01e14063ebb2388c4dabf4714d37c6))
* **editor:** Fix switching from v2 to v1 ([#12050](https://github.com/n8n-io/n8n/issues/12050)) ([5c76de3](https://github.com/n8n-io/n8n/commit/5c76de324c2e25b0d8b74cdab79f04aa616d8c4f))
* **editor:** Improvements to the commit modal ([#12031](https://github.com/n8n-io/n8n/issues/12031)) ([4fe1952](https://github.com/n8n-io/n8n/commit/4fe1952e2fb3379d95da42a7bb531851af6d0094))
* **editor:** Load node types in demo and preview modes ([#12048](https://github.com/n8n-io/n8n/issues/12048)) ([4ac5f95](https://github.com/n8n-io/n8n/commit/4ac5f9527bbec382a65ed3f1d9c41d6948c154e3))
* **editor:** Polyfill crypto.randomUUID ([#12052](https://github.com/n8n-io/n8n/issues/12052)) ([0537524](https://github.com/n8n-io/n8n/commit/0537524c3e45d7633415c7a9175a3857ad52cd58))
* **editor:** Redirect Settings to the proper sub page depending on the instance type (cloud or not) ([#12053](https://github.com/n8n-io/n8n/issues/12053)) ([a16d006](https://github.com/n8n-io/n8n/commit/a16d006f893cac927d674fa447b08c1205b67c54))
* **editor:** Render sanitized HTML content in toast messages ([#12139](https://github.com/n8n-io/n8n/issues/12139)) ([0468945](https://github.com/n8n-io/n8n/commit/0468945c99f083577c4cc71f671b4b950f6aeb86))
* **editor:** Universal button snags ([#11974](https://github.com/n8n-io/n8n/issues/11974)) ([956b11a](https://github.com/n8n-io/n8n/commit/956b11a560528336a74be40f722fa05bf3cca94d))
* **editor:** Update concurrency UI considering different types of instances ([#12068](https://github.com/n8n-io/n8n/issues/12068)) ([fa572bb](https://github.com/n8n-io/n8n/commit/fa572bbca4397b1cc42668530497444630ed17eb))
* **FTP Node:** Fix issue with creating folders on rename ([#9340](https://github.com/n8n-io/n8n/issues/9340)) ([eb7d593](https://github.com/n8n-io/n8n/commit/eb7d5934ef8bc6e999d6de4c0b8025ce175df5dd))
* **n8n Form Node:** Completion page display if EXECUTIONS_DATA_SAVE_ON_SUCCESS=none ([#11869](https://github.com/n8n-io/n8n/issues/11869)) ([f4c2523](https://github.com/n8n-io/n8n/commit/f4c252341985fe03927a2fd5d60ba846ec3dfc77))
* **OpenAI Node:** Allow updating assistant files ([#12042](https://github.com/n8n-io/n8n/issues/12042)) ([7b20f8a](https://github.com/n8n-io/n8n/commit/7b20f8aaa8befd19dbad0af3bf1b881342c1fca5))


### Features

* **AI Transform Node:** Reduce payload size ([#11965](https://github.com/n8n-io/n8n/issues/11965)) ([d8ca8de](https://github.com/n8n-io/n8n/commit/d8ca8de13a4cbb856696873bdb56c66b12a5b027))
* **core:** Add option to filter for empty variables ([#12112](https://github.com/n8n-io/n8n/issues/12112)) ([a63f0e8](https://github.com/n8n-io/n8n/commit/a63f0e878e21da9924451e2679939209b34b6583))
* **core:** Cancel runner task on timeout in external mode ([#12101](https://github.com/n8n-io/n8n/issues/12101)) ([addb4fa](https://github.com/n8n-io/n8n/commit/addb4fa352c88d856e463bb2b7001173c4fd6a7d))
* **core:** Parent workflows should wait for sub-workflows to finish ([#11985](https://github.com/n8n-io/n8n/issues/11985)) ([60b3dcc](https://github.com/n8n-io/n8n/commit/60b3dccf9317da6f3013be35a78ce21d0416ad80))
* **editor:** Implementing the `Easy AI Workflow` experiment ([#12043](https://github.com/n8n-io/n8n/issues/12043)) ([67ed1d2](https://github.com/n8n-io/n8n/commit/67ed1d2c3c2e69d5a96daf7de2795c02f5d8f15b))
* **Redis Node:** Add support for continue on fail / error output branch ([#11714](https://github.com/n8n-io/n8n/issues/11714)) ([ed35958](https://github.com/n8n-io/n8n/commit/ed359586c88a7662f4d94d58c5a87cf91d027ab9))



# [1.71.0](https://github.com/n8n-io/n8n/compare/n8n@1.70.0...n8n@1.71.0) (2024-12-04)


### Bug Fixes

* **core:** Fix push for waiting executions ([#11984](https://github.com/n8n-io/n8n/issues/11984)) ([8d71307](https://github.com/n8n-io/n8n/commit/8d71307da0398e7e39bf53e8e1cfa21ac1ceaf69))
* **core:** Improve header parameter parsing on http client responses ([#11953](https://github.com/n8n-io/n8n/issues/11953)) ([41e9e39](https://github.com/n8n-io/n8n/commit/41e9e39b5b53ecd9d8d1b385df65a26ecb9bccd8))
* **core:** Opt-out from optimizations if `$item` is used ([#12036](https://github.com/n8n-io/n8n/issues/12036)) ([872535a](https://github.com/n8n-io/n8n/commit/872535a40c85dcfad3a4b27c57c026ae003f562f))
* **core:** Use the configured timezone in task runner ([#12032](https://github.com/n8n-io/n8n/issues/12032)) ([2e6845a](https://github.com/n8n-io/n8n/commit/2e6845afcbc30dff73c3f3f15f21278cab397387))
* **core:** Validate node name when creating `NodeOperationErrror` ([#11999](https://github.com/n8n-io/n8n/issues/11999)) ([e68c9da](https://github.com/n8n-io/n8n/commit/e68c9da30c31cd5f994cb01ce759192562bfbd40))
* **editor:** Add execution concurrency info and paywall ([#11847](https://github.com/n8n-io/n8n/issues/11847)) ([57d3269](https://github.com/n8n-io/n8n/commit/57d3269e400ee4e7e3636614870ebdfdb0aa8c1d))
* **editor:** Fix bug causing connection lines to disappear when hovering stickies  ([#11950](https://github.com/n8n-io/n8n/issues/11950)) ([439a1cc](https://github.com/n8n-io/n8n/commit/439a1cc4f39243e91715b21a84b8e7266ce872cd))
* **editor:** Fix canvas keybindings using splitter keys such as zooming using `+` key ([#12022](https://github.com/n8n-io/n8n/issues/12022)) ([6af9c82](https://github.com/n8n-io/n8n/commit/6af9c82af6020e99d61e442ee9c2d40761baf027))
* **editor:** Fix community check ([#11979](https://github.com/n8n-io/n8n/issues/11979)) ([af0398a](https://github.com/n8n-io/n8n/commit/af0398a5e3a8987c01c7112e6f689b35e1ef92fe))
* **editor:** Fix copy/paste keyboard events in canvas chat ([#12004](https://github.com/n8n-io/n8n/issues/12004)) ([967340a](https://github.com/n8n-io/n8n/commit/967340a2938a79c89319121bf57a8d654f88e06c))
* **editor:** Fix node showing as successful if errors exists on subsequent runs ([#12019](https://github.com/n8n-io/n8n/issues/12019)) ([8616b17](https://github.com/n8n-io/n8n/commit/8616b17cc6c305da69bbb54fd56ab7cb34213f7c))
* **editor:** Fix pin data showing up in production executions on new canvas ([#11951](https://github.com/n8n-io/n8n/issues/11951)) ([5f6f8a1](https://github.com/n8n-io/n8n/commit/5f6f8a1bddfd76b586c08da821e8b59070f449fc))
* **editor:** Handle source control initialization to prevent UI form crashing ([#11776](https://github.com/n8n-io/n8n/issues/11776)) ([6be8e86](https://github.com/n8n-io/n8n/commit/6be8e86c45bd64d000bc95d2ef2d68220e930c02))
* **editor:** Implement dirty nodes  for partial executions ([#11739](https://github.com/n8n-io/n8n/issues/11739)) ([b8da4ff](https://github.com/n8n-io/n8n/commit/b8da4ff9edb0fbb0093c4c41fe11f8e67b696ca3))
* **editor:** Resolve going back from Settings ([#11958](https://github.com/n8n-io/n8n/issues/11958)) ([d74423c](https://github.com/n8n-io/n8n/commit/d74423c75198d38d0d99a1879051b5e964ecae74))
* **editor:** Unify executions card label color ([#11949](https://github.com/n8n-io/n8n/issues/11949)) ([fc79718](https://github.com/n8n-io/n8n/commit/fc797188d63e87df34b3a153eb4a0d0b7361b3f5))
* **editor:** Use optional chaining for all members in execution data when using the debug feature ([#12024](https://github.com/n8n-io/n8n/issues/12024)) ([67aa0c9](https://github.com/n8n-io/n8n/commit/67aa0c9107bda16b1cb6d273e17c3cde77035f51))
* **GraphQL Node:** Throw error if GraphQL variables are not objects or strings ([#11904](https://github.com/n8n-io/n8n/issues/11904)) ([85f30b2](https://github.com/n8n-io/n8n/commit/85f30b27ae282da58a25186d13ff17196dcd7d9c))
* **HTTP Request Node:** Use iconv-lite to decode http responses, to support more encoding types ([#11930](https://github.com/n8n-io/n8n/issues/11930)) ([461b39c](https://github.com/n8n-io/n8n/commit/461b39c5df5dd446cb8ceef469b204c7c5111229))
* Load workflows with unconnected Switch outputs ([#12020](https://github.com/n8n-io/n8n/issues/12020)) ([abc851c](https://github.com/n8n-io/n8n/commit/abc851c0cff298607a0dc2f2882aa17136898f45))
* **n8n Form Node:** Use https to load google fonts ([#11948](https://github.com/n8n-io/n8n/issues/11948)) ([eccd924](https://github.com/n8n-io/n8n/commit/eccd924f5e8dbe59e37099d1a6fbe8866fef55bf))
* **Telegram Trigger Node:** Fix header secret check ([#12018](https://github.com/n8n-io/n8n/issues/12018)) ([f16de4d](https://github.com/n8n-io/n8n/commit/f16de4db01c0496205635a3203a44098e7908453))
* **Webflow Node:** Fix issue with pagination in v2 node ([#11934](https://github.com/n8n-io/n8n/issues/11934)) ([1eb94bc](https://github.com/n8n-io/n8n/commit/1eb94bcaf54d9e581856ce0b87253e1c28fa68e2))
* **Webflow Node:** Fix issue with publishing items ([#11982](https://github.com/n8n-io/n8n/issues/11982)) ([0a8a57e](https://github.com/n8n-io/n8n/commit/0a8a57e4ec8081ab1a53f36d686b3d5dcaae2476))


### Features

* **AI Transform Node:** Node Prompt improvements ([#11611](https://github.com/n8n-io/n8n/issues/11611)) ([40a7445](https://github.com/n8n-io/n8n/commit/40a7445f0873af2cdbd10b12bd691c07a43e27cc))
* **Code Node:** Warning if pairedItem absent or could not be auto mapped ([#11737](https://github.com/n8n-io/n8n/issues/11737)) ([3a5bd12](https://github.com/n8n-io/n8n/commit/3a5bd129459272cbac960ae2754db3028943f87e))
* **editor:** Canvas chat UI & UX improvements ([#11924](https://github.com/n8n-io/n8n/issues/11924)) ([1e25774](https://github.com/n8n-io/n8n/commit/1e25774541461c86da5c4af8efec792e2814eeb1))
* **editor:** Persist user's preferred display modes on localStorage ([#11929](https://github.com/n8n-io/n8n/issues/11929)) ([bd69316](https://github.com/n8n-io/n8n/commit/bd693162b86a21c90880bab2c2e67aab733095ff))


### Performance Improvements

* **editor:** Virtualize SchemaView ([#11694](https://github.com/n8n-io/n8n/issues/11694)) ([9c6def9](https://github.com/n8n-io/n8n/commit/9c6def91975764522fa52cdf21e9cb5bdb4d721d))



# [1.70.0](https://github.com/n8n-io/n8n/compare/n8n@1.69.0...n8n@1.70.0) (2024-11-27)


### Bug Fixes

* **AI Agent Node:** Add binary message before scratchpad to prevent tool calling loops ([#11845](https://github.com/n8n-io/n8n/issues/11845)) ([5c80cb5](https://github.com/n8n-io/n8n/commit/5c80cb57cf709a1097a38e0394aad6fce5330eba))
* CodeNodeEditor walk  cannot read properties of null ([#11129](https://github.com/n8n-io/n8n/issues/11129)) ([d99e0a7](https://github.com/n8n-io/n8n/commit/d99e0a7c979a1ee96b2eea1b9011d5bce375289a))
* **core:** Bring back execution data on the `executionFinished` push message ([#11821](https://github.com/n8n-io/n8n/issues/11821)) ([0313570](https://github.com/n8n-io/n8n/commit/03135702f18e750ba44840dccfec042270629a2b))
* **core:** Correct invalid WS status code on removing connection ([#11901](https://github.com/n8n-io/n8n/issues/11901)) ([1d80225](https://github.com/n8n-io/n8n/commit/1d80225d26ba01f78934a455acdcca7b83be7205))
* **core:** Don't use unbound context methods in code sandboxes ([#11914](https://github.com/n8n-io/n8n/issues/11914)) ([f6c0d04](https://github.com/n8n-io/n8n/commit/f6c0d045e9683cd04ee849f37b96697097c5b41d))
* **core:** Fix broken execution query when using projectId ([#11852](https://github.com/n8n-io/n8n/issues/11852)) ([a061dbc](https://github.com/n8n-io/n8n/commit/a061dbca07ad686c563e85c56081bc1a7830259b))
* **core:** Fix validation of items returned in the task runner ([#11897](https://github.com/n8n-io/n8n/issues/11897)) ([a535e88](https://github.com/n8n-io/n8n/commit/a535e88f1aec8fbbf2eb9397d38748f49773de2d))
* **editor:** Add missing trigger waiting tooltip on new canvas ([#11918](https://github.com/n8n-io/n8n/issues/11918)) ([a8df221](https://github.com/n8n-io/n8n/commit/a8df221bfbb5428d93d03f539bcfdaf29ee20c21))
* **editor:** Don't re-render input panel after node finishes executing ([#11813](https://github.com/n8n-io/n8n/issues/11813)) ([b3a99a2](https://github.com/n8n-io/n8n/commit/b3a99a2351079c37ed6d83f43920ba80f3832234))
* **editor:** Fix AI assistant loading message layout ([#11819](https://github.com/n8n-io/n8n/issues/11819)) ([89b4807](https://github.com/n8n-io/n8n/commit/89b48072432753137b498c338af7777036fdde7a))
* **editor:** Fix new canvas discovery tooltip position after adding github stars button ([#11898](https://github.com/n8n-io/n8n/issues/11898)) ([f4ab5c7](https://github.com/n8n-io/n8n/commit/f4ab5c7b9244b8fdde427c12c1a152fbaaba0c34))
* **editor:** Fix node position not getting set when dragging selection on new canvas ([#11871](https://github.com/n8n-io/n8n/issues/11871)) ([595de81](https://github.com/n8n-io/n8n/commit/595de81c03b3e488ab41fb8d1d316c3db6a8372a))
* **editor:** Restore workers view ([#11876](https://github.com/n8n-io/n8n/issues/11876)) ([3aa72f6](https://github.com/n8n-io/n8n/commit/3aa72f613f64c16d7dff67ffe66037894e45aa7c))
* **editor:** Turn NPS survey into a modal and make sure it shows above the Ask AI button ([#11814](https://github.com/n8n-io/n8n/issues/11814)) ([ca169f3](https://github.com/n8n-io/n8n/commit/ca169f3f3455fa39ce9120b30d7b409bade6561e))
* **editor:** Use `crypto.randomUUID()` to initialize node id if missing on new canvas ([#11873](https://github.com/n8n-io/n8n/issues/11873)) ([bc4857a](https://github.com/n8n-io/n8n/commit/bc4857a1b3d6ea389f11fb8246a1cee33b8a008e))
* **n8n Form Node:** Duplicate popup in manual mode ([#11925](https://github.com/n8n-io/n8n/issues/11925)) ([2c34bf4](https://github.com/n8n-io/n8n/commit/2c34bf4ea6137fb0fb321969684ffa621da20fa3))
* **n8n Form Node:** Redirect if completion page to trigger ([#11822](https://github.com/n8n-io/n8n/issues/11822)) ([1a8fb7b](https://github.com/n8n-io/n8n/commit/1a8fb7bdc428c6a23c8708e2dcf924f1f10b47a9))
* **OpenAI Node:** Remove preview chatInput parameter for `Assistant:Messsage` operation ([#11825](https://github.com/n8n-io/n8n/issues/11825)) ([4dde287](https://github.com/n8n-io/n8n/commit/4dde287cde3af7c9c0e57248e96b8f1270da9332))
* Retain execution data between partial executions (new flow) ([#11828](https://github.com/n8n-io/n8n/issues/11828)) ([3320436](https://github.com/n8n-io/n8n/commit/3320436a6fdf8472b3843b9fe8d4de7af7f5ef5c))


### Features

* Add SharePoint credentials ([#11570](https://github.com/n8n-io/n8n/issues/11570)) ([05c6109](https://github.com/n8n-io/n8n/commit/05c61091db9bdd62fdcca910ead50d0bd512966a))
* Add Zabbix credential only node ([#11489](https://github.com/n8n-io/n8n/issues/11489)) ([fbd1ecf](https://github.com/n8n-io/n8n/commit/fbd1ecfb29461fee393914bc200ec72c654d8944))
* **AI Transform Node:** Support for drag and drop ([#11276](https://github.com/n8n-io/n8n/issues/11276)) ([2c252b0](https://github.com/n8n-io/n8n/commit/2c252b0b2d5282f4a87bce76f93c4c02dd8ff5e3))
* **editor:** Drop `response` wrapper requirement from Subworkflow Tool output ([#11785](https://github.com/n8n-io/n8n/issues/11785)) ([cd3598a](https://github.com/n8n-io/n8n/commit/cd3598aaab6cefe58a4cb9df7d93fb501415e9d3))
* **editor:** Improve node and edge bring-to-front mechanism on new canvas ([#11793](https://github.com/n8n-io/n8n/issues/11793)) ([b89ca9d](https://github.com/n8n-io/n8n/commit/b89ca9d482faa5cb542898f3973fb6e7c9a8437a))
* **editor:** Make new canvas connections go underneath node when looping backwards ([#11833](https://github.com/n8n-io/n8n/issues/11833)) ([91d1bd8](https://github.com/n8n-io/n8n/commit/91d1bd8d333454f3971605df73c3703102d2a9e9))
* **editor:** Make the left sidebar in Expressions editor draggable ([#11838](https://github.com/n8n-io/n8n/issues/11838)) ([a713b3e](https://github.com/n8n-io/n8n/commit/a713b3ed25feb1790412fc320cf41a0967635263))
* **editor:** Migrate existing users to new canvas and set new canvas as default ([#11896](https://github.com/n8n-io/n8n/issues/11896)) ([caa7447](https://github.com/n8n-io/n8n/commit/caa744785a2cc5063a5fb9d269c0ea53ea432298))
* **Slack Node:** Update wait for approval to use markdown ([#11754](https://github.com/n8n-io/n8n/issues/11754)) ([40dd02f](https://github.com/n8n-io/n8n/commit/40dd02f360d0d8752fe89c4304c18cac9858c530))



# [1.69.0](https://github.com/n8n-io/n8n/compare/n8n@1.68.0...n8n@1.69.0) (2024-11-20)


### Bug Fixes

* Add supported versions warning to Zep memory node ([#11803](https://github.com/n8n-io/n8n/issues/11803)) ([9cc5bc1](https://github.com/n8n-io/n8n/commit/9cc5bc1aef974fe6c2511c1597b90c8b54ba6b9c))
* **AI Agent Node:** Escape curly brackets in tools description for non Tool agents ([#11772](https://github.com/n8n-io/n8n/issues/11772)) ([83abdfa](https://github.com/n8n-io/n8n/commit/83abdfaf027a0533824a3ac3e4bab3cad971821a))
* **Anthropic Chat Model Node:** Update credentials test endpoint ([#11756](https://github.com/n8n-io/n8n/issues/11756)) ([6cf0aba](https://github.com/n8n-io/n8n/commit/6cf0abab5bcddb407571271b9f174e66bb209790))
* **core:** Add missing env vars to task runner config ([#11810](https://github.com/n8n-io/n8n/issues/11810)) ([870c576](https://github.com/n8n-io/n8n/commit/870c576ed9d7ce4ef005db9c8bedd78e91084c9c))
* **core:** Allow Azure's SAML metadata XML containing WS-Federation nodes to pass validation ([#11724](https://github.com/n8n-io/n8n/issues/11724)) ([3b62bd5](https://github.com/n8n-io/n8n/commit/3b62bd58c264be0225a74ae0eb35c4761c419b79))
* **core:** Delete binary data parent folder when pruning executions ([#11790](https://github.com/n8n-io/n8n/issues/11790)) ([17ef2c6](https://github.com/n8n-io/n8n/commit/17ef2c63f69b811bdd28006df3b6edd446837971))
* **core:** Fix `diagnostics.enabled` default value ([#11809](https://github.com/n8n-io/n8n/issues/11809)) ([5fa72b0](https://github.com/n8n-io/n8n/commit/5fa72b0512b00bdc6a1065b7b604c9640f469454))
* **core:** Improve the security on OAuth callback endpoints  ([#11593](https://github.com/n8n-io/n8n/issues/11593)) ([274fcf4](https://github.com/n8n-io/n8n/commit/274fcf45d393d8db1d2fb5ae1e774a4c9198a178))
* **core:** Restore old names for pruning config keys ([#11782](https://github.com/n8n-io/n8n/issues/11782)) ([d15b8d0](https://github.com/n8n-io/n8n/commit/d15b8d05092d2ed9dd45fcfa34b4177f60469ebd))
* **core:** Unload any existing version of a community nodes package before upgrading it ([#11727](https://github.com/n8n-io/n8n/issues/11727)) ([1d8fd13](https://github.com/n8n-io/n8n/commit/1d8fd13d841b73466ba5f8044d17d7199da7e856))
* **editor:** Add documentation link to insufficient quota message ([#11777](https://github.com/n8n-io/n8n/issues/11777)) ([1987363](https://github.com/n8n-io/n8n/commit/1987363f7941285c51fda849a4ac92832368b25a))
* **editor:** Add project header subtitle ([#11797](https://github.com/n8n-io/n8n/issues/11797)) ([ff4261c](https://github.com/n8n-io/n8n/commit/ff4261c16845c7de1790fdf0eaa9f57b37822289))
* **editor:** Change Home label to Overview ([#11736](https://github.com/n8n-io/n8n/issues/11736)) ([1a78360](https://github.com/n8n-io/n8n/commit/1a783606b4ef22d85e173a2a780d5c49ff208932))
* **editor:** Fix executions sorting ([#11808](https://github.com/n8n-io/n8n/issues/11808)) ([cd5ad65](https://github.com/n8n-io/n8n/commit/cd5ad65e90a3be4d67b51521772e0fceb7f4abc7))
* **editor:** Fix partial executions not working due to broken push message queue and race conditions ([#11798](https://github.com/n8n-io/n8n/issues/11798)) ([b05d435](https://github.com/n8n-io/n8n/commit/b05d43519994abdd34a65462d14184c779d0b667))
* **editor:** Fix reordered switch connections when copying nodes on new canvas ([#11788](https://github.com/n8n-io/n8n/issues/11788)) ([6c2dad7](https://github.com/n8n-io/n8n/commit/6c2dad79143f5b0c255ab8c97c3255314834c458))
* **editor:** Fix the issue with RMC Values to Send collection disappears  ([#11710](https://github.com/n8n-io/n8n/issues/11710)) ([7bb9002](https://github.com/n8n-io/n8n/commit/7bb9002cbc10cf58550f53a30c6fd7151f8e7355))
* **editor:** Improve formatting of expired trial error message ([#11708](https://github.com/n8n-io/n8n/issues/11708)) ([8a0ad0f](https://github.com/n8n-io/n8n/commit/8a0ad0f910feeada6d0c63e81c3e97a1a6e44de7))
* **editor:** Optimize application layout ([#11769](https://github.com/n8n-io/n8n/issues/11769)) ([91f9390](https://github.com/n8n-io/n8n/commit/91f9390b90a68d064ea00d10505bf3767ddec1d4))
* **Google Sheets Trigger Node:** Fix issue with regex showing correct sheet as invalid ([#11770](https://github.com/n8n-io/n8n/issues/11770)) ([d5ba1a0](https://github.com/n8n-io/n8n/commit/d5ba1a059b7a67154f17f8ad3fcfe66c5c031059))
* **HTTP Request Node:** Continue using error ([#11733](https://github.com/n8n-io/n8n/issues/11733)) ([d1bae1a](https://github.com/n8n-io/n8n/commit/d1bae1ace062dd5b64087e0313e78599b5994355))
* **n8n Form Node:** Support expressions in completion page ([#11781](https://github.com/n8n-io/n8n/issues/11781)) ([1099167](https://github.com/n8n-io/n8n/commit/10991675fe2e6913e8f03d565b670257941f18e5))
* Prevent workflow to run if active and single webhook service ([#11752](https://github.com/n8n-io/n8n/issues/11752)) ([bcb9a20](https://github.com/n8n-io/n8n/commit/bcb9a2078186ff80e03ca3b8532d3585c307d86b))
* **Read/Write Files from Disk Node:** Escape parenthesis when reading file ([#11753](https://github.com/n8n-io/n8n/issues/11753)) ([285534e](https://github.com/n8n-io/n8n/commit/285534e6d0ceb60290bd0a928054e494252148fe))
* **YouTube Node:** Issue in published before and after dates filters ([#11741](https://github.com/n8n-io/n8n/issues/11741)) ([7381c28](https://github.com/n8n-io/n8n/commit/7381c28af00148b329690021b921267a48a6eaa3))


### Features

* **core:** Improve debugging of sub-workflows ([#11602](https://github.com/n8n-io/n8n/issues/11602)) ([fd3254d](https://github.com/n8n-io/n8n/commit/fd3254d5874a03b57421246b77a519787536a93e))
* **core:** Improve handling of manual executions with wait nodes ([#11750](https://github.com/n8n-io/n8n/issues/11750)) ([61696c3](https://github.com/n8n-io/n8n/commit/61696c3db313cdc97925af728ff5c68415f9b6b2))
* **editor:** Add Info Note to NDV Output Panel if no existing Tools were used during Execution ([#11672](https://github.com/n8n-io/n8n/issues/11672)) ([de0e861](https://github.com/n8n-io/n8n/commit/de0e86150f4d0615481e5ec3869465cfd1ce822f))
* **editor:** Add option to create sub workflow from workflows list in `Execute Workflow` node ([#11706](https://github.com/n8n-io/n8n/issues/11706)) ([c265d44](https://github.com/n8n-io/n8n/commit/c265d44841eb147115563ce24c56666b1e321433))
* **editor:** Add selection navigation using the keyboard on new canvas ([#11679](https://github.com/n8n-io/n8n/issues/11679)) ([6cd9b99](https://github.com/n8n-io/n8n/commit/6cd9b996af0406caf65941503276524de9e2add4))
* **editor:** Add universal Create Resource Menu ([#11564](https://github.com/n8n-io/n8n/issues/11564)) ([b38ce14](https://github.com/n8n-io/n8n/commit/b38ce14ec94d74aa1c9780a0572804ff6266588d))
* **Embeddings Azure OpenAI Node, Azure OpenAI Chat Model Node:** Add support for basePath url in Azure Open AI nodes ([#11784](https://github.com/n8n-io/n8n/issues/11784)) ([e298ebe](https://github.com/n8n-io/n8n/commit/e298ebe90d69f466ee897855472eaa7be1d96aba))
* **Embeddings OpenAI Node, Embeddings Azure OpenAI Node:** Add dimensions option ([#11773](https://github.com/n8n-io/n8n/issues/11773)) ([de01a8a](https://github.com/n8n-io/n8n/commit/de01a8a01d37f33ab8bcbc65588cafebda969922))
* GitHub stars dismiss button ([#11794](https://github.com/n8n-io/n8n/issues/11794)) ([8fbad74](https://github.com/n8n-io/n8n/commit/8fbad74ab685c2ba0395c30cee0ddf9498fb8984))



# [1.68.0](https://github.com/n8n-io/n8n/compare/n8n@1.67.0...n8n@1.68.0) (2024-11-13)


### Bug Fixes

* **AI Agent Node:** Throw better errors for non-tool agents when using structured tools ([#11582](https://github.com/n8n-io/n8n/issues/11582)) ([9b6123d](https://github.com/n8n-io/n8n/commit/9b6123dfb2648f880c7829211fa07666611ad0ea))
* **Auto-fixing Output Parser Node:** Only run retry chain on parsing errors ([#11569](https://github.com/n8n-io/n8n/issues/11569)) ([21b31e4](https://github.com/n8n-io/n8n/commit/21b31e488ff6ab0bcf3c79edcd17b9e37d4c64a4))
* **core:** Continue with error output reverse items in success branch ([#11684](https://github.com/n8n-io/n8n/issues/11684)) ([6d5ee83](https://github.com/n8n-io/n8n/commit/6d5ee832966fab96043b0d65697c059ced61d334))
* **core:** Ensure task runner server closes websocket connection correctly ([#11633](https://github.com/n8n-io/n8n/issues/11633)) ([b496bf3](https://github.com/n8n-io/n8n/commit/b496bf3147d2cd873d24371be02cb7ea5dbd8621))
* **core:** Handle websocket connection error more gracefully in task runners ([#11635](https://github.com/n8n-io/n8n/issues/11635)) ([af7d6e6](https://github.com/n8n-io/n8n/commit/af7d6e68d0436ff8a3d4e8410dc8ee4f3a035c44))
* **core:** Improve model sub-nodes error handling ([#11418](https://github.com/n8n-io/n8n/issues/11418)) ([57467d0](https://github.com/n8n-io/n8n/commit/57467d0285d67509322630c4c01130022f274a41))
* **core:** Make push work for waiting webhooks ([#11678](https://github.com/n8n-io/n8n/issues/11678)) ([600479b](https://github.com/n8n-io/n8n/commit/600479bf36ba8870d4aecacad19a2dc5f2d97959))
* **core:** Revert all the context helpers changes ([#11616](https://github.com/n8n-io/n8n/issues/11616)) ([20fd38f](https://github.com/n8n-io/n8n/commit/20fd38f3517f7ef35604ba16abb4d951270b4d50))
* **core:** Set the authentication methad to `email` during startup if the SAML configuration in the database has been corrupted ([#11600](https://github.com/n8n-io/n8n/issues/11600)) ([6439291](https://github.com/n8n-io/n8n/commit/6439291738dec16261979d6d835acbc63743d51a))
* **core:** Use cached value in retrieval of personal project owner ([#11533](https://github.com/n8n-io/n8n/issues/11533)) ([04029d8](https://github.com/n8n-io/n8n/commit/04029d82a11b52990890380ba7094055b18e7c1f))
* Credentials save button is hidden unless you make changes to the ([#11492](https://github.com/n8n-io/n8n/issues/11492)) ([835fbfe](https://github.com/n8n-io/n8n/commit/835fbfe337dd8dc0d0b0318c7227e174484e1328))
* **editor:** Add stickies to node insert position conflict check allowlist ([#11624](https://github.com/n8n-io/n8n/issues/11624)) ([fc39e3c](https://github.com/n8n-io/n8n/commit/fc39e3ca16231c176957e2504d55df6b416874fe))
* **editor:** Adjust Scrollbar Width of RunData Header Row ([#11561](https://github.com/n8n-io/n8n/issues/11561)) ([d17d76a](https://github.com/n8n-io/n8n/commit/d17d76a85d5425bc091d29fc84605ffbccbca984))
* **editor:** Cap NDV Output View Tab Index to prevent rare edge case ([#11614](https://github.com/n8n-io/n8n/issues/11614)) ([a6c8ee4](https://github.com/n8n-io/n8n/commit/a6c8ee4a82e6055766dc1307f79c774c17bb5f4d))
* **editor:** Do not show hover tooltip when autocomplete is active ([#11653](https://github.com/n8n-io/n8n/issues/11653)) ([23caf43](https://github.com/n8n-io/n8n/commit/23caf43e30342a21d45c825f438aa1e6193601d1))
* **editor:** Enable pinning main output with error and always allow unpinning ([#11452](https://github.com/n8n-io/n8n/issues/11452)) ([40c8882](https://github.com/n8n-io/n8n/commit/40c88822acdcda6401bd92b9cf89d013c44b8453))
* **editor:** Fix collapsing nested items in expression modal schema view ([#11645](https://github.com/n8n-io/n8n/issues/11645)) ([41dea52](https://github.com/n8n-io/n8n/commit/41dea522fbfb1c9acee51f47f384973914454b5f))
* **editor:** Fix default workflow settings ([#11632](https://github.com/n8n-io/n8n/issues/11632)) ([658568e](https://github.com/n8n-io/n8n/commit/658568e2700bfd5b61da53f3052403d0098c2d90))
* **editor:** Fix duplicate chat trigger ([#11693](https://github.com/n8n-io/n8n/issues/11693)) ([a025848](https://github.com/n8n-io/n8n/commit/a025848ec4be96f74d4de2ab104256b6d89bb837))
* **editor:** Fix hiding SQL query output when trying to select ([#11649](https://github.com/n8n-io/n8n/issues/11649)) ([4dbf2f4](https://github.com/n8n-io/n8n/commit/4dbf2f4256111985b367030020f1494b8a8b95af))
* **editor:** Fix scrolling in code edit modal ([#11647](https://github.com/n8n-io/n8n/issues/11647)) ([8f695f3](https://github.com/n8n-io/n8n/commit/8f695f3417820e7b9bb04b78972f6abbd61abbe8))
* **editor:** Prevent error being thrown in RLC while loading ([#11676](https://github.com/n8n-io/n8n/issues/11676)) ([ca8cb45](https://github.com/n8n-io/n8n/commit/ca8cb455ba59831295c238afb11aeab6ad18428e))
* **editor:** Prevent NodeCreator from swallowing AskAssistant enter event ([#11532](https://github.com/n8n-io/n8n/issues/11532)) ([db94f16](https://github.com/n8n-io/n8n/commit/db94f169fcd03983fc78a3b4c5e11543610825bf))
* **editor:** Show node executing status shortly before switching to success on new canvas ([#11675](https://github.com/n8n-io/n8n/issues/11675)) ([b0ba24c](https://github.com/n8n-io/n8n/commit/b0ba24cbbc55cebc26e9f62ead7396c4c8fbd062))
* **editor:** Show only error title and 'Open errored node' button; hide 'Ask Assistant' in root for sub-node errors ([#11573](https://github.com/n8n-io/n8n/issues/11573)) ([8cba100](https://github.com/n8n-io/n8n/commit/8cba1004888f60ca653ee069501c13b3cadcc561))
* **Facebook Lead Ads Trigger Node:** Fix issue with optional fields ([#11692](https://github.com/n8n-io/n8n/issues/11692)) ([70d315b](https://github.com/n8n-io/n8n/commit/70d315b3d5b8f5f3e0f39527bba11e254a52028e))
* **Google BigQuery Node:** Add item index to insert error ([#11702](https://github.com/n8n-io/n8n/issues/11702)) ([145d092](https://github.com/n8n-io/n8n/commit/145d0921b217bbd4b625beaacfa14429560bf51b))
* **Google Drive Node:** Fix file upload for streams ([#11698](https://github.com/n8n-io/n8n/issues/11698)) ([770230f](https://github.com/n8n-io/n8n/commit/770230fbfe0b9e86527254e201c4602fbced94ff))
* **In-Memory Vector Store Node:** Fix displaying execution data of connected embedding nodes ([#11701](https://github.com/n8n-io/n8n/issues/11701)) ([40ade15](https://github.com/n8n-io/n8n/commit/40ade151724f4af28a6ed959fd9363450ea711fd))
* **Item List Output Parser Node:** Fix number of items parameter issue ([#11696](https://github.com/n8n-io/n8n/issues/11696)) ([01ebe9d](https://github.com/n8n-io/n8n/commit/01ebe9dd38629afbab954fb489f3ef2bb7ab5b34))
* **n8n Form Node:** Find completion page ([#11674](https://github.com/n8n-io/n8n/issues/11674)) ([ed3ad6d](https://github.com/n8n-io/n8n/commit/ed3ad6d684597f7c4b7419dfa81d476e66f10eba))
* **n8n Form Node:** Open form page if form trigger has pin data ([#11673](https://github.com/n8n-io/n8n/issues/11673)) ([f0492bd](https://github.com/n8n-io/n8n/commit/f0492bd3bb0d94802a2707fb1cf861313b6ea808))
* **n8n Form Node:** Trigger page stack in waiting if error in workflow ([#11671](https://github.com/n8n-io/n8n/issues/11671)) ([94b5873](https://github.com/n8n-io/n8n/commit/94b5873248212a5500f02cf3c0d74df6f9d8fb26))
* **n8n Form Trigger Node:** Checkboxes different sizes ([#11677](https://github.com/n8n-io/n8n/issues/11677)) ([c08d23c](https://github.com/n8n-io/n8n/commit/c08d23c00f01bb6fcb3b75f02e0338af375f9b32))
* NDV search bugs ([#11613](https://github.com/n8n-io/n8n/issues/11613)) ([c32cf64](https://github.com/n8n-io/n8n/commit/c32cf644a6b8c21558e802449329877845de70b1))
* **Notion Node:** Extract page url ([#11643](https://github.com/n8n-io/n8n/issues/11643)) ([cbdd535](https://github.com/n8n-io/n8n/commit/cbdd535fe0cb4e032ea82f008dcf35cc5f2264c2))
* **Redis Chat Memory Node:** Respect the SSL flag from the credential ([#11689](https://github.com/n8n-io/n8n/issues/11689)) ([b5cbf75](https://github.com/n8n-io/n8n/commit/b5cbf7566d351d8a8e9972f13ff5867ff1c8d7d0))
* **Supabase Node:** Reset query parameters in get many operation ([#11630](https://github.com/n8n-io/n8n/issues/11630)) ([7458229](https://github.com/n8n-io/n8n/commit/74582290c04d2dd32300b1a6c7715862ae837d34))
* **Switch Node:** Maintain output connections ([#11162](https://github.com/n8n-io/n8n/issues/11162)) ([9bd79fc](https://github.com/n8n-io/n8n/commit/9bd79fceebc4453d0fe40ae5f628d5e31ff2b326))


### Features

* **AI Transform Node:** Show warning for binary data ([#11560](https://github.com/n8n-io/n8n/issues/11560)) ([ddbb263](https://github.com/n8n-io/n8n/commit/ddbb263dce0fc458abc95d850217251bb49d2b83))
* **core:** Make all http requests made with `httpRequestWithAuthentication` abortable ([#11704](https://github.com/n8n-io/n8n/issues/11704)) ([0d8aada](https://github.com/n8n-io/n8n/commit/0d8aada49005d6a6078e8460003a0de61a8f423c))
* **editor:** Improve how we show default Agent prompt and Memory session parameters ([#11491](https://github.com/n8n-io/n8n/issues/11491)) ([565f8cd](https://github.com/n8n-io/n8n/commit/565f8cd8c78b534a50e272997d659d162fa86625))
* **editor:** Improve workflow loading performance on new canvas ([#11629](https://github.com/n8n-io/n8n/issues/11629)) ([f1e2df7](https://github.com/n8n-io/n8n/commit/f1e2df7d0753aa0f33cf299100a063bf89cc8b35))
* **editor:** Redesign Canvas Chat ([#11634](https://github.com/n8n-io/n8n/issues/11634)) ([a412ab7](https://github.com/n8n-io/n8n/commit/a412ab7ebfcd6aa9051a8ca36e34f1067102c998))
* **editor:** Restrict when a ChatTrigger Node is added automatically ([#11523](https://github.com/n8n-io/n8n/issues/11523)) ([93a6f85](https://github.com/n8n-io/n8n/commit/93a6f858fa3eb53f8b48b2a3d6b7377279dd6ed1))
* Github star button in-app ([#11695](https://github.com/n8n-io/n8n/issues/11695)) ([0fd684d](https://github.com/n8n-io/n8n/commit/0fd684d90c830f8b0aab12b7f78a1fa5619c62c9))
* **Oura Node:** Update node for v2 api ([#11604](https://github.com/n8n-io/n8n/issues/11604)) ([3348fbb](https://github.com/n8n-io/n8n/commit/3348fbb1547c430ff8707b298640e3461d3f6536))


### Performance Improvements

* **editor:** Add lint rules for optimization-friendly syntax ([#11681](https://github.com/n8n-io/n8n/issues/11681)) ([88295c7](https://github.com/n8n-io/n8n/commit/88295c70495ae3d017674d5745972a346fcbaf12))



# [1.67.0](https://github.com/n8n-io/n8n/compare/n8n@1.66.0...n8n@1.67.0) (2024-11-06)


### Bug Fixes

* Bring back nodes panel telemetry events ([#11456](https://github.com/n8n-io/n8n/issues/11456)) ([130c942](https://github.com/n8n-io/n8n/commit/130c942f633788d1b2f937d6fea342d4450c6e3d))
* **core:** Account for double quotes in instance base URL ([#11495](https://github.com/n8n-io/n8n/issues/11495)) ([c5191e6](https://github.com/n8n-io/n8n/commit/c5191e697a9a9ebfa2b67587cd01b5835ebf6ea8))
* **core:** Do not delete waiting executions when saving of successful executions is disabled ([#11458](https://github.com/n8n-io/n8n/issues/11458)) ([e8757e5](https://github.com/n8n-io/n8n/commit/e8757e58f69e091ac3d2a2f8e8c8e33ac57c1e47))
* **core:** Don't send a `executionFinished` event to the browser with no run data if the execution has already been cleaned up ([#11502](https://github.com/n8n-io/n8n/issues/11502)) ([d1153f5](https://github.com/n8n-io/n8n/commit/d1153f51e80911cbc8f34ba5f038f349b75295c3))
* **core:** Include `projectId` in range query middleware ([#11590](https://github.com/n8n-io/n8n/issues/11590)) ([a6070af](https://github.com/n8n-io/n8n/commit/a6070afdda29631fd36e5213f52bf815268bcda4))
* **core:** Save exeution progress for waiting executions, even when progress saving is disabled ([#11535](https://github.com/n8n-io/n8n/issues/11535)) ([6b9353c](https://github.com/n8n-io/n8n/commit/6b9353c80f61ab36945fff434d98242dc1cab7b3))
* **core:** Use the correct docs URL for regular nodes when used as tools ([#11529](https://github.com/n8n-io/n8n/issues/11529)) ([a092b8e](https://github.com/n8n-io/n8n/commit/a092b8e972e1253d92df416f19096a045858e7c1))
* **Edit Image Node:** Fix Text operation by setting Arial as default font ([#11125](https://github.com/n8n-io/n8n/issues/11125)) ([60c1ace](https://github.com/n8n-io/n8n/commit/60c1ace64be29d651ce7b777fbb576598e38b9d7))
* **editor:** Auto focus first fields on SignIn, SignUp and ForgotMyPassword views ([#11445](https://github.com/n8n-io/n8n/issues/11445)) ([5b5bd72](https://github.com/n8n-io/n8n/commit/5b5bd7291dde17880b7699f7e6832938599ffd8f))
* **editor:** Do not overwrite the webhookId in the new canvas ([#11562](https://github.com/n8n-io/n8n/issues/11562)) ([dfd785b](https://github.com/n8n-io/n8n/commit/dfd785bc0894257eb6e62b0dd8f71248c27aae53))
* **editor:** Ensure Enter key on Cancel button correctly cancels node rename ([#11563](https://github.com/n8n-io/n8n/issues/11563)) ([be05ae3](https://github.com/n8n-io/n8n/commit/be05ae36e7790156cb48b317fc254ae46a3b2d8c))
* **editor:** Fix emitting `n8nReady` notification via `postmessage` on new canvas ([#11558](https://github.com/n8n-io/n8n/issues/11558)) ([463d101](https://github.com/n8n-io/n8n/commit/463d101f3592e6df4afd66c4d0fde0cb4aec34cc))
* **editor:** Fix run index input for RunData view in sub-nodes ([#11538](https://github.com/n8n-io/n8n/issues/11538)) ([434d31c](https://github.com/n8n-io/n8n/commit/434d31ce928342d52b6ab8b78639afd7829216d4))
* **editor:** Fix selected credential being overwritten in NDV ([#11496](https://github.com/n8n-io/n8n/issues/11496)) ([a26c0e2](https://github.com/n8n-io/n8n/commit/a26c0e2c3c7da87bfaba9737a967aa0070810d85))
* **editor:** Keep workflow pristine after load on new canvas ([#11579](https://github.com/n8n-io/n8n/issues/11579)) ([7254359](https://github.com/n8n-io/n8n/commit/7254359855b89769613cd5cc24dbb4f45a7cc76f))
* Show Pinned data in demo mode ([#11490](https://github.com/n8n-io/n8n/issues/11490)) ([ca2a583](https://github.com/n8n-io/n8n/commit/ca2a583b5cbb0cba3ecb694261806de16547aa91))
* Toast not aligned to the bottom when AI assistant disable ([#11549](https://github.com/n8n-io/n8n/issues/11549)) ([e80f7e0](https://github.com/n8n-io/n8n/commit/e80f7e0a02a972379f73af6a44de11768081086e))


### Features

* Add Rapid7 InsightVm credentials ([#11462](https://github.com/n8n-io/n8n/issues/11462)) ([46eceab](https://github.com/n8n-io/n8n/commit/46eceabc27ac219b11b85c16c533a2cff848c5dd))
* **AI Transform Node:** UX improvements ([#11280](https://github.com/n8n-io/n8n/issues/11280)) ([8a48407](https://github.com/n8n-io/n8n/commit/8a484077af3d3e1fe2d1b90b1ea9edf4ba41fcb6))
* **Anthropic Chat Model Node:** Add support for Haiku 3.5 ([#11551](https://github.com/n8n-io/n8n/issues/11551)) ([8b39825](https://github.com/n8n-io/n8n/commit/8b398256a81594a52f20f8eb8adf8ff205209bc1))
* **Convert to File Node:** Add delimiter convert to csv ([#11556](https://github.com/n8n-io/n8n/issues/11556)) ([63d454b](https://github.com/n8n-io/n8n/commit/63d454b776c092ff8c6c521a7e083774adb8f649))
* **editor:** Update panning and selection keybindings on new canvas ([#11534](https://github.com/n8n-io/n8n/issues/11534)) ([5e2e205](https://github.com/n8n-io/n8n/commit/5e2e205394adf76faf02aee2d4f21df71848e1d4))
* **Gmail Trigger Node:** Add filter option to include drafts ([#11441](https://github.com/n8n-io/n8n/issues/11441)) ([7a2be77](https://github.com/n8n-io/n8n/commit/7a2be77f384a32ede3acad8fe24fb89227c058bf))
* **Intercom Node:** Update credential to new style ([#11485](https://github.com/n8n-io/n8n/issues/11485)) ([b137e13](https://github.com/n8n-io/n8n/commit/b137e13845f0714ebf7421c837f5ab104b66709b))



# [1.66.0](https://github.com/n8n-io/n8n/compare/n8n@1.65.0...n8n@1.66.0) (2024-10-31)


### Bug Fixes

* **Asana Node:** Fix issue with pagination ([#11415](https://github.com/n8n-io/n8n/issues/11415)) ([04c075a](https://github.com/n8n-io/n8n/commit/04c075a46bcc7b1964397f0244b0fde99476212d))
* **core:** Add 'user_id' to `license-community-plus-registered` telemetry event ([#11430](https://github.com/n8n-io/n8n/issues/11430)) ([7a8dafe](https://github.com/n8n-io/n8n/commit/7a8dafe9902fbc0d5001c50579c34959b95211ab))
* **core:** Add safeguard for command publishing ([#11337](https://github.com/n8n-io/n8n/issues/11337)) ([656439e](https://github.com/n8n-io/n8n/commit/656439e87138f9f96dea5a683cfdac3f661ffefb))
* **core:** Ensure `LoggerProxy` is not scoped ([#11379](https://github.com/n8n-io/n8n/issues/11379)) ([f4ea943](https://github.com/n8n-io/n8n/commit/f4ea943c9cb2321e41705de6c5c27535a0f5eae0))
* **core:** Ensure `remove-triggers-and-pollers` command is not debounced ([#11486](https://github.com/n8n-io/n8n/issues/11486)) ([529d4fc](https://github.com/n8n-io/n8n/commit/529d4fc3ef5206bd1b02d27634342cc50b45997e))
* **core:** Ensure job processor does not reprocess amended executions ([#11438](https://github.com/n8n-io/n8n/issues/11438)) ([c152a3a](https://github.com/n8n-io/n8n/commit/c152a3ac56f140a39eea4771a94f5a3082118df7))
* **core:** Fix Message Event Bus Metrics not counting up for labeled metrics ([#11396](https://github.com/n8n-io/n8n/issues/11396)) ([7fc3b25](https://github.com/n8n-io/n8n/commit/7fc3b25d21c6c4f1802f34b1ae065a65cac3001b))
* **core:** Fix resolving of $fromAI expression via `evaluateExpression` ([#11397](https://github.com/n8n-io/n8n/issues/11397)) ([2e64464](https://github.com/n8n-io/n8n/commit/2e6446454defbd3e5a47b66e6fd46d4f1b9fbd0f))
* **core:** Make execution and its data creation atomic ([#11392](https://github.com/n8n-io/n8n/issues/11392)) ([ed30d43](https://github.com/n8n-io/n8n/commit/ed30d43236bf3c6b657022636a02a41be01aa152))
* **core:** On unhandled rejections, extract the original exception correctly ([#11389](https://github.com/n8n-io/n8n/issues/11389)) ([8608bae](https://github.com/n8n-io/n8n/commit/8608baeb7ec302daddc8adca6e39778dcf7b2eda))
* **editor:**  Fix TypeError: Cannot read properties of undefined (reading '0') ([#11399](https://github.com/n8n-io/n8n/issues/11399)) ([ae37c52](https://github.com/n8n-io/n8n/commit/ae37c520a91c75e353e818944b36a3619c0d8b4a))
* **editor:** Add Retry button for AI Assistant errors ([#11345](https://github.com/n8n-io/n8n/issues/11345)) ([7699240](https://github.com/n8n-io/n8n/commit/7699240073122cdef31cf109fd37fa66961f588a))
* **editor:** Change tooltip for workflow with execute workflow trigger ([#11374](https://github.com/n8n-io/n8n/issues/11374)) ([dcd6038](https://github.com/n8n-io/n8n/commit/dcd6038c3085135803cdaa546a239359a6d449eb))
* **editor:** Ensure toasts show above modal overlays ([#11410](https://github.com/n8n-io/n8n/issues/11410)) ([351134f](https://github.com/n8n-io/n8n/commit/351134f786af933f5f310bf8d9897269387635a0))
* **editor:** Fit view consistently after nodes are initialized on new canvas ([#11457](https://github.com/n8n-io/n8n/issues/11457)) ([497d637](https://github.com/n8n-io/n8n/commit/497d637fc5308b9c4a06bc764152fde1f1a9c130))
* **editor:** Fix adding connections when initializing workspace in templates view on new canvas ([#11451](https://github.com/n8n-io/n8n/issues/11451)) ([ea47b02](https://github.com/n8n-io/n8n/commit/ea47b025fb16c967d4fc73dcacc6e260d2aecd61))
* **editor:** Fix rendering of AI logs ([#11450](https://github.com/n8n-io/n8n/issues/11450)) ([73b0a80](https://github.com/n8n-io/n8n/commit/73b0a80ac92b4f4b5a300d0ec1c833b4395a222a))
* **editor:** Hide data mapping tooltip in credential edit modal ([#11356](https://github.com/n8n-io/n8n/issues/11356)) ([ff14dcb](https://github.com/n8n-io/n8n/commit/ff14dcb3a1ddaea4eca7c1ecd2e92c0abb0c413c))
* **editor:** Prevent running workflow that has issues if listening to webhook ([#11402](https://github.com/n8n-io/n8n/issues/11402)) ([8b0a48f](https://github.com/n8n-io/n8n/commit/8b0a48f53010378e497e4cc362fda75a958cf363))
* **editor:** Run external hooks after settings have been initialized ([#11423](https://github.com/n8n-io/n8n/issues/11423)) ([0ab24c8](https://github.com/n8n-io/n8n/commit/0ab24c814abd1787268750ba808993ab2735ac52))
* **editor:** Support middle click to scroll when using a mouse on new canvas ([#11384](https://github.com/n8n-io/n8n/issues/11384)) ([46f3b4a](https://github.com/n8n-io/n8n/commit/46f3b4a258f89f02e0d2bd1eef25a22e3a721167))
* **HTTP Request Tool Node:** Fix HTML response optimization issue ([#11439](https://github.com/n8n-io/n8n/issues/11439)) ([cf37e94](https://github.com/n8n-io/n8n/commit/cf37e94dd875e9f6ab1f189146fb34e7296af93c))
* **n8n Form Node:** Form Trigger does not wait in multi-form mode ([#11404](https://github.com/n8n-io/n8n/issues/11404)) ([151f4dd](https://github.com/n8n-io/n8n/commit/151f4dd7b8f800af424f8ae64cb8238975fb3cb8))
* Update required node js version in CONTRIBUTING.md ([#11437](https://github.com/n8n-io/n8n/issues/11437)) ([4f511aa](https://github.com/n8n-io/n8n/commit/4f511aab68651caa8fe47f70cd7cdb88bb06a3e2))


### Features

* **Anthropic Chat Model Node:** Add model claude-3-5-sonnet-20241022 ([#11465](https://github.com/n8n-io/n8n/issues/11465)) ([f6c8890](https://github.com/n8n-io/n8n/commit/f6c8890a8069de221b9b96e735418ecc9624cf7b))
* **core:** Handle nodes with multiple inputs and connections during partial executions ([#11376](https://github.com/n8n-io/n8n/issues/11376)) ([cb7c4d2](https://github.com/n8n-io/n8n/commit/cb7c4d29a6f042b590822e5b9c67fff0a8f0863d))
* **editor:** Add descriptive header to projects /workflow ([#11203](https://github.com/n8n-io/n8n/issues/11203)) ([5d19e8f](https://github.com/n8n-io/n8n/commit/5d19e8f2b45dc1abc5a8253f9e3a0fdacb1ebd91))
* **editor:** Improve placeholder for vector store tool ([#11483](https://github.com/n8n-io/n8n/issues/11483)) ([629e092](https://github.com/n8n-io/n8n/commit/629e09240785bc648ff6575f97910fbb4e77cdab))
* **editor:** Remove edge execution animation on new canvas ([#11446](https://github.com/n8n-io/n8n/issues/11446)) ([a701d87](https://github.com/n8n-io/n8n/commit/a701d87f5ba94ffc811e424b60e188b26ac6c1c5))
* **editor:** Update ownership pills ([#11155](https://github.com/n8n-io/n8n/issues/11155)) ([8147038](https://github.com/n8n-io/n8n/commit/8147038cf87dca657602e617e49698065bf1a63f))



# [1.65.0](https://github.com/n8n-io/n8n/compare/n8n@1.64.0...n8n@1.65.0) (2024-10-24)


### Bug Fixes

* **AI Agent Node:** Preserve `intermediateSteps` when using output parser with non-tool agent ([#11363](https://github.com/n8n-io/n8n/issues/11363)) ([e61a853](https://github.com/n8n-io/n8n/commit/e61a8535aa39653b9a87575ea911a65318282167))
* **API:** `PUT /credentials/:id` should move the specified credential, not the first one in the database ([#11365](https://github.com/n8n-io/n8n/issues/11365)) ([e6b2f8e](https://github.com/n8n-io/n8n/commit/e6b2f8e7e6ebbb6e3776a976297d519e99ac6c64))
* **API:** Correct credential schema for response in `POST /credentials` ([#11340](https://github.com/n8n-io/n8n/issues/11340)) ([f495875](https://github.com/n8n-io/n8n/commit/f4958756b4976e0b608b9155dab84564f7e8804e))
* **core:** Account for waiting jobs during shutdown ([#11338](https://github.com/n8n-io/n8n/issues/11338)) ([c863abd](https://github.com/n8n-io/n8n/commit/c863abd08300b53ea898fc4d06aae97dec7afa9b))
* **core:** Add missing primary key to execution annotation tags table ([#11168](https://github.com/n8n-io/n8n/issues/11168)) ([b4b543d](https://github.com/n8n-io/n8n/commit/b4b543d41daa07753eca24ab93bf7445f672361d))
* **core:** Change dedupe value column type from varchar(255) to text ([#11357](https://github.com/n8n-io/n8n/issues/11357)) ([7a71cff](https://github.com/n8n-io/n8n/commit/7a71cff4d75fe4e7282a398b4843428e0161ba8c))
* **core:** Do not debounce webhooks, triggers and pollers activation ([#11306](https://github.com/n8n-io/n8n/issues/11306)) ([64bddf8](https://github.com/n8n-io/n8n/commit/64bddf86536ddd688638a643d24f80c947a12f31))
* **core:** Enforce nodejs version consistently ([#11323](https://github.com/n8n-io/n8n/issues/11323)) ([0fa2e8c](https://github.com/n8n-io/n8n/commit/0fa2e8ca85005362d9043d82469f3c3525f4c4ef))
* **core:** Fix memory issue with empty model response ([#11300](https://github.com/n8n-io/n8n/issues/11300)) ([216b119](https://github.com/n8n-io/n8n/commit/216b119350949de70f15cf2d61f474770803ad7a))
* **core:** Fix race condition when resolving post-execute promise ([#11360](https://github.com/n8n-io/n8n/issues/11360)) ([4f1816e](https://github.com/n8n-io/n8n/commit/4f1816e03db00219bc2e723e3048848aef7f8fe1))
* **core:** Sanitise IdP provided information in SAML test pages ([#11171](https://github.com/n8n-io/n8n/issues/11171)) ([74fc388](https://github.com/n8n-io/n8n/commit/74fc3889b946e8f224e65ef8d3d44125404aa4fc))
* Don't show pin button in input panel when there's binary data ([#11267](https://github.com/n8n-io/n8n/issues/11267)) ([c0b5b92](https://github.com/n8n-io/n8n/commit/c0b5b92f62a2d7ba60492eb27daced268b654fe9))
* **editor:** Add Personal project to main navigation ([#11161](https://github.com/n8n-io/n8n/issues/11161)) ([1f441f9](https://github.com/n8n-io/n8n/commit/1f441f97528f58e905eaf8930577bbcd08debf06))
* **editor:** Fix Cannot read properties of undefined (reading 'finished') ([#11367](https://github.com/n8n-io/n8n/issues/11367)) ([475d72e](https://github.com/n8n-io/n8n/commit/475d72e0bc9e13c6dc56129902f6f89c67547f78))
* **editor:** Fix delete all existing executions ([#11352](https://github.com/n8n-io/n8n/issues/11352)) ([3ec103f](https://github.com/n8n-io/n8n/commit/3ec103f8baaa89e579844947d945f00bec9e498e))
* **editor:** Fix pin data button disappearing after reload ([#11198](https://github.com/n8n-io/n8n/issues/11198)) ([3b2f63e](https://github.com/n8n-io/n8n/commit/3b2f63e248cd0cba04087e2f40e13d670073707d))
* **editor:** Fix RunData non-binary pagination when binary data is present ([#11309](https://github.com/n8n-io/n8n/issues/11309)) ([901888d](https://github.com/n8n-io/n8n/commit/901888d5b1027098653540c72f787f176941f35a))
* **editor:** Fix sorting problem in older browsers that don't support `toSorted` ([#11204](https://github.com/n8n-io/n8n/issues/11204)) ([c728a2f](https://github.com/n8n-io/n8n/commit/c728a2ffe01f510a237979a54897c4680a407800))
* **editor:** Follow-up fixes to projects side menu ([#11327](https://github.com/n8n-io/n8n/issues/11327)) ([4dde772](https://github.com/n8n-io/n8n/commit/4dde772814c55e66efcc9b369ae443328af21b14))
* **editor:** Keep always focus on the first item on the node's search panel ([#11193](https://github.com/n8n-io/n8n/issues/11193)) ([c57cac9](https://github.com/n8n-io/n8n/commit/c57cac9e4d447c3a4240a565f9f2de8aa3b7c513))
* **editor:** Open Community+ enrollment modal only for the instance owner ([#11292](https://github.com/n8n-io/n8n/issues/11292)) ([76724c3](https://github.com/n8n-io/n8n/commit/76724c3be6e001792433045c2b2aac0ef16d4b8a))
* **editor:** Record sessionStarted telemetry event in Setting Store ([#11334](https://github.com/n8n-io/n8n/issues/11334)) ([1b734dd](https://github.com/n8n-io/n8n/commit/1b734dd9f42885594ce02400cfb395a4f5e7e088))
* Ensure NDV params don't get cut off early and scrolled to the top ([#11252](https://github.com/n8n-io/n8n/issues/11252)) ([054fe97](https://github.com/n8n-io/n8n/commit/054fe9745ff6864f9088aa4cd66ed9e7869520d5))
* **HTTP Request Tool Node:** Fix the undefined response issue when authentication is enabled ([#11343](https://github.com/n8n-io/n8n/issues/11343)) ([094ec68](https://github.com/n8n-io/n8n/commit/094ec68d4c00848013aa4eec4ac5efbd2c92afc5))
* Include error in the message in JS task runner sandbox ([#11359](https://github.com/n8n-io/n8n/issues/11359)) ([0708b3a](https://github.com/n8n-io/n8n/commit/0708b3a1f8097af829c92fe106ea6ba375d6c500))
* **Microsoft SQL Node:** Fix execute query to allow for non select query to run ([#11335](https://github.com/n8n-io/n8n/issues/11335)) ([ba158b4](https://github.com/n8n-io/n8n/commit/ba158b4f8533bd3430db8766d4921f75db5c1a11))
* **OpenAI Chat Model Node, Ollama Chat Model Node:** Change default model to a more up-to-date option ([#11293](https://github.com/n8n-io/n8n/issues/11293)) ([0be04c6](https://github.com/n8n-io/n8n/commit/0be04c6348d8c059a96c3d37a6d6cd587bfb97f3))
* **Pinecone Vector Store Node:** Prevent populating of vectors after manually stopping the execution ([#11288](https://github.com/n8n-io/n8n/issues/11288)) ([fbae17d](https://github.com/n8n-io/n8n/commit/fbae17d8fb35a5197fa183e3639bb36762dc73d2))
* **Postgres Node:** Special datetime values cause errors ([#11225](https://github.com/n8n-io/n8n/issues/11225)) ([3c57f46](https://github.com/n8n-io/n8n/commit/3c57f46aaeb968d2974f2dc9790317a6a6fab624))
* Resend invite operation on users list ([#11351](https://github.com/n8n-io/n8n/issues/11351)) ([e4218de](https://github.com/n8n-io/n8n/commit/e4218debd18812fa3aa508339afd3de03c4d69dc))
* **SSH Node:** Cleanup temporary binary files as soon as possible ([#11305](https://github.com/n8n-io/n8n/issues/11305)) ([08a7b5b](https://github.com/n8n-io/n8n/commit/08a7b5b7425663ec6593114921c2e22ab37d039e))


### Features

* Add report bug buttons ([#11304](https://github.com/n8n-io/n8n/issues/11304)) ([296f68f](https://github.com/n8n-io/n8n/commit/296f68f041b93fd32ac7be2b53c2b41d58c2998a))
* **AI Agent Node:** Make tools optional when using OpenAI model with Tools agent ([#11212](https://github.com/n8n-io/n8n/issues/11212)) ([fed7c3e](https://github.com/n8n-io/n8n/commit/fed7c3ec1fb0553adaa9a933f91aabfd54fe83a3))
* **core:**  introduce JWT API keys for the public API ([#11005](https://github.com/n8n-io/n8n/issues/11005)) ([679fa4a](https://github.com/n8n-io/n8n/commit/679fa4a10a85fc96e12ca66fe12cdb32368bc12b))
* **core:** Enforce config file permissions on startup ([#11328](https://github.com/n8n-io/n8n/issues/11328)) ([c078a51](https://github.com/n8n-io/n8n/commit/c078a516bec857831cc904ef807d0791b889f3a2))
* **core:** Handle cycles in workflows when partially executing them ([#11187](https://github.com/n8n-io/n8n/issues/11187)) ([321d6de](https://github.com/n8n-io/n8n/commit/321d6deef18806d88d97afef2f2c6f29e739ccb4))
* **editor:** Separate node output execution tooltip from status icon ([#11196](https://github.com/n8n-io/n8n/issues/11196)) ([cd15e95](https://github.com/n8n-io/n8n/commit/cd15e959c7af82a7d8c682e94add2b2640624a70))
* **GitHub Node:** Add workflow resource operations ([#10744](https://github.com/n8n-io/n8n/issues/10744)) ([d309112](https://github.com/n8n-io/n8n/commit/d3091126472faa2c8f270650e54027d19dc56bb6))
* **n8n Form Page Node:** New node ([#10390](https://github.com/n8n-io/n8n/issues/10390)) ([643d66c](https://github.com/n8n-io/n8n/commit/643d66c0ae084a0d93dac652703adc0a32cab8de))
* **n8n Google My Business Node:** New node ([#10504](https://github.com/n8n-io/n8n/issues/10504)) ([bf28fbe](https://github.com/n8n-io/n8n/commit/bf28fbefe5e8ba648cba1555a2d396b75ee32bbb))
* Run `mfa.beforeSetup` hook before enabling MFA ([#11116](https://github.com/n8n-io/n8n/issues/11116)) ([25c1c32](https://github.com/n8n-io/n8n/commit/25c1c3218cf1075ca3abd961236f3b2fbd9d6ba9))
* **Structured Output Parser Node:** Refactor Output Parsers and Improve Error Handling ([#11148](https://github.com/n8n-io/n8n/issues/11148)) ([45274f2](https://github.com/n8n-io/n8n/commit/45274f2e7f081e194e330e1c9e6a5c26fca0b141))



# [1.64.0](https://github.com/n8n-io/n8n/compare/n8n@1.63.0...n8n@1.64.0) (2024-10-16)


### Bug Fixes

* Adjust arrow button colors in dark mode ([#11248](https://github.com/n8n-io/n8n/issues/11248)) ([439132c](https://github.com/n8n-io/n8n/commit/439132c291a812d57702c94eaa12878394ac4c69))
* **core:** Ensure error reporter does not promote `info` to `error` messages ([#11245](https://github.com/n8n-io/n8n/issues/11245)) ([a7fc7fc](https://github.com/n8n-io/n8n/commit/a7fc7fc22997acec86dc94386c95349fd018f4ae))
* **core:** Override executions mode if `regular` during worker startup ([#11250](https://github.com/n8n-io/n8n/issues/11250)) ([c0aa28c](https://github.com/n8n-io/n8n/commit/c0aa28c6cf3f77b04e04663217c9df8e3803ed3f))
* **core:** Wrap nodes for tool use at a suitable time ([#11238](https://github.com/n8n-io/n8n/issues/11238)) ([c2fb881](https://github.com/n8n-io/n8n/commit/c2fb881d61291209802438d95892d052f5c82d43))
* Don't show pinned data tooltip for pinned nodes ([#11249](https://github.com/n8n-io/n8n/issues/11249)) ([c2ad156](https://github.com/n8n-io/n8n/commit/c2ad15646d326a8f71e314d54efe202a5bcdd296))
* **editor:** Bring back the "Forgot password" link on SigninView ([#11216](https://github.com/n8n-io/n8n/issues/11216)) ([4e78c46](https://github.com/n8n-io/n8n/commit/4e78c46a7450c7fc0694369944d4fb446cef2348))
* **editor:** Fix chat crashing when rendering output-parsed content ([#11210](https://github.com/n8n-io/n8n/issues/11210)) ([4aaebfd](https://github.com/n8n-io/n8n/commit/4aaebfd4358f590e98c453ad4e65cc2c9d0f76f8))
* **editor:** Make submit in ChangePasswordView work again ([#11227](https://github.com/n8n-io/n8n/issues/11227)) ([4f27b39](https://github.com/n8n-io/n8n/commit/4f27b39b45b58779d363980241e6e5e11b58f5da))
* Expressions display actual result of evaluating expression inside string ([#11257](https://github.com/n8n-io/n8n/issues/11257)) ([7f5f0a9](https://github.com/n8n-io/n8n/commit/7f5f0a9df3b3fae6e2f9787443ac1cf9415d5932))
* **Google Ads Node:** Update to use v17 api ([#11243](https://github.com/n8n-io/n8n/issues/11243)) ([3d97f02](https://github.com/n8n-io/n8n/commit/3d97f02a8d2b6e5bc7c97c5271bed97417ecacd2))
* **Google Calendar Node:** Fix issue with conference data types not loading ([#11185](https://github.com/n8n-io/n8n/issues/11185)) ([4012758](https://github.com/n8n-io/n8n/commit/401275884e5db0287e4eeffb3c7497dd5e024880))
* **Google Calendar Node:** Mode to add or replace attendees in event update ([#11132](https://github.com/n8n-io/n8n/issues/11132)) ([6c6a8ef](https://github.com/n8n-io/n8n/commit/6c6a8efdea83cf7194304ce089d7b72d8f6c1a9d))
* **HTTP Request Tool Node:** Respond with an error when receive binary response ([#11219](https://github.com/n8n-io/n8n/issues/11219)) ([0d23a7f](https://github.com/n8n-io/n8n/commit/0d23a7fb5ba41545f70c4848d30b90af91b1e7e6))
* **MySQL Node:** Fix "Maximum call stack size exceeded" error when handling a large number of rows ([#11242](https://github.com/n8n-io/n8n/issues/11242)) ([b7ee0c4](https://github.com/n8n-io/n8n/commit/b7ee0c4087eae346bc7e5360130d6c812dbe99db))
* **n8n Trigger Node:** Merge with Workflow Trigger node ([#11174](https://github.com/n8n-io/n8n/issues/11174)) ([6ec6b51](https://github.com/n8n-io/n8n/commit/6ec6b5197ae97eb86496effd458fcc0b9b223ef3))
* **OpenAI Node:** Fix tool parameter parsing issue ([#11201](https://github.com/n8n-io/n8n/issues/11201)) ([5a1d81a](https://github.com/n8n-io/n8n/commit/5a1d81ad917fde5cd6a387fe2d4ec6aab6b71349))
* **Set Node:** Fix issue with UI properties not being hidden ([#11263](https://github.com/n8n-io/n8n/issues/11263)) ([1affc27](https://github.com/n8n-io/n8n/commit/1affc27b6bf9a559061a06f92bebe8167d938665))
* **Strava Trigger Node:** Fix issue with webhook not being deleted ([#11226](https://github.com/n8n-io/n8n/issues/11226)) ([566529c](https://github.com/n8n-io/n8n/commit/566529ca1149988a54a58b3c34bbe4d9f1add6db))


### Features

* Add tracking for node errors and update node graph ([#11060](https://github.com/n8n-io/n8n/issues/11060)) ([d3b05f1](https://github.com/n8n-io/n8n/commit/d3b05f1c54e62440666297d8e484ccd22168da48))
* **core:** Dedupe ([#10101](https://github.com/n8n-io/n8n/issues/10101)) ([52dd2c7](https://github.com/n8n-io/n8n/commit/52dd2c76196c6895b47145c2b85a6895ce2874d4))
* **editor:** Send workflow context to assistant store ([#11135](https://github.com/n8n-io/n8n/issues/11135)) ([fade9e4](https://github.com/n8n-io/n8n/commit/fade9e43c84a0ae1fbc80f3ee546a418970e2380))
* **Gong Node:** New node ([#10777](https://github.com/n8n-io/n8n/issues/10777)) ([785b47f](https://github.com/n8n-io/n8n/commit/785b47feb3b83cf36aaed57123f8baca2bbab307))


### Performance Improvements

* **Google Sheets Node:** Don't load whole spreadsheet dataset to determine columns when appending data ([#11235](https://github.com/n8n-io/n8n/issues/11235)) ([26ad091](https://github.com/n8n-io/n8n/commit/26ad091f473bca4e5d3bdc257e0818be02e52db5))



# [1.63.0](https://github.com/n8n-io/n8n/compare/n8n@1.62.1...n8n@1.63.0) (2024-10-09)


### Bug Fixes

* **Convert to File Node:** Convert to ICS start date defaults to now ([#11114](https://github.com/n8n-io/n8n/issues/11114)) ([1146c4e](https://github.com/n8n-io/n8n/commit/1146c4e98d8c85c15ac67fa1c3bfb731234531e3))
* **core:** Allow loading nodes from multiple custom directories ([#11130](https://github.com/n8n-io/n8n/issues/11130)) ([1b84b0e](https://github.com/n8n-io/n8n/commit/1b84b0e5e7485d9f99d61a8ae3df49efadca0745))
* **core:** Always set `startedAt` when executions start running ([#11098](https://github.com/n8n-io/n8n/issues/11098)) ([722f4a8](https://github.com/n8n-io/n8n/commit/722f4a8b771058800b992a482ad5f644b650960d))
* **core:** Fix AI nodes not working with new partial execution flow ([#11055](https://github.com/n8n-io/n8n/issues/11055)) ([0eee5df](https://github.com/n8n-io/n8n/commit/0eee5dfd597817819dbe0463a63f671fde53432f))
* **core:** Print errors that happen before the execution starts on the worker instead of just on the main instance ([#11099](https://github.com/n8n-io/n8n/issues/11099)) ([1d14557](https://github.com/n8n-io/n8n/commit/1d145574611661ecd9ab1a39d815c0ea915b9a1c))
* **core:** Separate error handlers for main and worker ([#11091](https://github.com/n8n-io/n8n/issues/11091)) ([bb59cc7](https://github.com/n8n-io/n8n/commit/bb59cc71acc9e494e54abc8402d58db39e5a664e))
* **editor:**  Shorten overflowing Node Label in InputLabels on hover and focus ([#11110](https://github.com/n8n-io/n8n/issues/11110)) ([87a0b68](https://github.com/n8n-io/n8n/commit/87a0b68f9009c1c776d937c6ca62096e88c95ed6))
* **editor:** Add safety to prevent undefined errors ([#11104](https://github.com/n8n-io/n8n/issues/11104)) ([565b117](https://github.com/n8n-io/n8n/commit/565b117a52f8eac9202a1a62c43daf78b293dcf8))
* **editor:** Fix design system form element sizing ([#11040](https://github.com/n8n-io/n8n/issues/11040)) ([67c3453](https://github.com/n8n-io/n8n/commit/67c3453885bc619fedc8338a6dd0d8d66dead931))
* **editor:** Fix getInitials when Intl.Segmenter is not supported ([#11103](https://github.com/n8n-io/n8n/issues/11103)) ([7e8955b](https://github.com/n8n-io/n8n/commit/7e8955b322b1d2c84c0f479a5977484d8d5e3135))
* **editor:** Fix schema view in AI tools ([#11089](https://github.com/n8n-io/n8n/issues/11089)) ([09cfdbd](https://github.com/n8n-io/n8n/commit/09cfdbd1817eba46c935308880fe9f95ded252b0))
* **editor:** Respect tag querystring filter when listing workflows ([#11029](https://github.com/n8n-io/n8n/issues/11029)) ([59c5ff6](https://github.com/n8n-io/n8n/commit/59c5ff61354302562ba5a2340c66811afdd1523b))
* **editor:** Show previous nodes autocomplete in AI tool nodes ([#11111](https://github.com/n8n-io/n8n/issues/11111)) ([8566b3a](https://github.com/n8n-io/n8n/commit/8566b3a99939f45ac263830eee30d0d4ade9305c))
* **editor:** Update Usage page for Community+ edition ([#11074](https://github.com/n8n-io/n8n/issues/11074)) ([3974981](https://github.com/n8n-io/n8n/commit/3974981ea5c67f6f2bbb90a96b405d9d0cfa21af))
* Fix transaction handling for 'revert' command ([#11145](https://github.com/n8n-io/n8n/issues/11145)) ([a782336](https://github.com/n8n-io/n8n/commit/a7823367f13c3dba0c339eaafaad0199bd524b13))
* Forbid access to files outside source control work directory ([#11152](https://github.com/n8n-io/n8n/issues/11152)) ([606eedb](https://github.com/n8n-io/n8n/commit/606eedbf1b302e153bd13b7cef80847711e3a9ee))
* **Gitlab Node:** Author name and email not being set ([#11077](https://github.com/n8n-io/n8n/issues/11077)) ([fce1233](https://github.com/n8n-io/n8n/commit/fce1233b58624d502c9c68f4b32a4bb7d76f1814))
* Incorrect error message on calling wrong webhook method ([#11093](https://github.com/n8n-io/n8n/issues/11093)) ([d974b01](https://github.com/n8n-io/n8n/commit/d974b015d030c608158ff0c3fa3b7f4cbb8eadd3))
* **n8n Form Trigger Node:** When clicking on a multiple choice label, the wrong one is selected ([#11059](https://github.com/n8n-io/n8n/issues/11059)) ([948edd1](https://github.com/n8n-io/n8n/commit/948edd1a047cf3dbddb3b0e9ec5de4bac3e97b9f))
* **NASA Node:** Astronomy-Picture-Of-The-Day fails when it's YouTube video ([#11046](https://github.com/n8n-io/n8n/issues/11046)) ([c70969d](https://github.com/n8n-io/n8n/commit/c70969da2bcabeb33394073a69ccef208311461b))
* **Postgres PGVector Store Node:** Fix filtering in retriever mode ([#11075](https://github.com/n8n-io/n8n/issues/11075)) ([dbd2ae1](https://github.com/n8n-io/n8n/commit/dbd2ae199506a24c2df4c983111a56f2adf63eee))
* Show result of waiting execution on canvas after execution complete ([#10815](https://github.com/n8n-io/n8n/issues/10815)) ([90b4bfc](https://github.com/n8n-io/n8n/commit/90b4bfc472ef132d2280b175ae7410dfb8e549b2))
* **Slack Node:** User id not sent correctly to API when updating user profile ([#11153](https://github.com/n8n-io/n8n/issues/11153)) ([ed9e61c](https://github.com/n8n-io/n8n/commit/ed9e61c46055d8e636a70c9c175d7d4ba596dd48))


### Features

* **core:** Introduce scoped logging ([#11127](https://github.com/n8n-io/n8n/issues/11127)) ([c68782c](https://github.com/n8n-io/n8n/commit/c68782c633b7ef6253ea705c5a222d4536491fd5))
* **editor:**  Add navigation dropdown component ([#11047](https://github.com/n8n-io/n8n/issues/11047)) ([e081fd1](https://github.com/n8n-io/n8n/commit/e081fd1f0b5a0700017a8dc92f013f0abdbad319))
* **editor:** Add route for create / edit / share credentials ([#11134](https://github.com/n8n-io/n8n/issues/11134)) ([5697de4](https://github.com/n8n-io/n8n/commit/5697de4429c5d94f25ce1bd14c84fb4266ea47a7))
* **editor:** Community+ enrollment ([#10776](https://github.com/n8n-io/n8n/issues/10776)) ([92cf860](https://github.com/n8n-io/n8n/commit/92cf860f9f2994442facfddc758bc60f5cbec520))
* Human in the loop ([#10675](https://github.com/n8n-io/n8n/issues/10675)) ([41228b4](https://github.com/n8n-io/n8n/commit/41228b472de11affc8cd0821284427c2c9e8b421))
* **OpenAI Node:** Allow to specify thread ID for Assistant -> Message operation ([#11080](https://github.com/n8n-io/n8n/issues/11080)) ([6a2f9e7](https://github.com/n8n-io/n8n/commit/6a2f9e72959fb0e89006b69c31fbcee1ead1cde9))
* Opt in to additional features on community for existing users ([#11166](https://github.com/n8n-io/n8n/issues/11166)) ([c2adfc8](https://github.com/n8n-io/n8n/commit/c2adfc85451c5103eaad068f882066fd36c4aebe))


### Performance Improvements

* **core:** Optimize worker healthchecks ([#11092](https://github.com/n8n-io/n8n/issues/11092)) ([19fb728](https://github.com/n8n-io/n8n/commit/19fb728da0839c57603e55da4e407715e6c5b081))



## [1.62.1](https://github.com/n8n-io/n8n/compare/n8n@1.61.0...n8n@1.62.1) (2024-10-02)


### Bug Fixes

* **AI Agent Node:** Fix output parsing and empty tool input handling in AI Agent node ([#10970](https://github.com/n8n-io/n8n/issues/10970)) ([3a65bdc](https://github.com/n8n-io/n8n/commit/3a65bdc1f522932d463b4da0e67d29076887d06c))
* **API:** Fix workflow project transfer ([#10651](https://github.com/n8n-io/n8n/issues/10651)) ([5f89e3a](https://github.com/n8n-io/n8n/commit/5f89e3a01c1bbb3589ff0464fd5bc991426f55dc))
* **AwsS3 Node:** Fix search only using first input parameters ([#10998](https://github.com/n8n-io/n8n/issues/10998)) ([846cfde](https://github.com/n8n-io/n8n/commit/846cfde8dcaf7bf80f0a4ca7d65fc2a7b61d0e23))
* **Chat Trigger Node:** Fix Allowed Origins paramter ([#11011](https://github.com/n8n-io/n8n/issues/11011)) ([b5f4afe](https://github.com/n8n-io/n8n/commit/b5f4afe12ec77f527080a4b7f812e12f9f73f8df))
* **core:** Fix ownerless project case in statistics service ([#11051](https://github.com/n8n-io/n8n/issues/11051)) ([bdaadf1](https://github.com/n8n-io/n8n/commit/bdaadf10e058e2c0b1141289189d6526c030a2ca))
* **core:** Handle Redis disconnects gracefully ([#11007](https://github.com/n8n-io/n8n/issues/11007)) ([cd91648](https://github.com/n8n-io/n8n/commit/cd916480c2d2b55f2215c72309dc432340fc3f30))
* **core:** Prevent backend from loading duplicate copies of nodes packages ([#10979](https://github.com/n8n-io/n8n/issues/10979)) ([4584f22](https://github.com/n8n-io/n8n/commit/4584f22a9b16883779d8555cda309fd8bd113f6c))
* **core:** Upgrade @n8n/typeorm to address a rare mutex release issue ([#10993](https://github.com/n8n-io/n8n/issues/10993)) ([2af0fbf](https://github.com/n8n-io/n8n/commit/2af0fbf52f0b404697f5148f81ad0035c9ffb6b9))
* **editor:** Allow resources to move between personal and team projects ([#10683](https://github.com/n8n-io/n8n/issues/10683)) ([136d491](https://github.com/n8n-io/n8n/commit/136d49132567558b7d27069c857c0e0bfee70ce2))
* **editor:** Color scheme for a markdown code blocks in dark mode ([#11008](https://github.com/n8n-io/n8n/issues/11008)) ([b20d2eb](https://github.com/n8n-io/n8n/commit/b20d2eb403f71fe1dc21c92df118adcebef51ffe))
* **editor:** Fix filter execution by "Queued" ([#10987](https://github.com/n8n-io/n8n/issues/10987)) ([819d20f](https://github.com/n8n-io/n8n/commit/819d20fa2eee314b88a7ce1c4db632afac514704))
* **editor:** Fix performance issue in credentials list ([#10988](https://github.com/n8n-io/n8n/issues/10988)) ([7073ec6](https://github.com/n8n-io/n8n/commit/7073ec6fe5384cc8c50dcb242212999a1fbc9041))
* **editor:** Fix schema view pill highlighting ([#10936](https://github.com/n8n-io/n8n/issues/10936)) ([1b973dc](https://github.com/n8n-io/n8n/commit/1b973dcd8dbce598e6ada490fd48fad52f7b4f3a))
* **editor:** Fix workflow executions list page redirection ([#10981](https://github.com/n8n-io/n8n/issues/10981)) ([fe7d060](https://github.com/n8n-io/n8n/commit/fe7d0605681dc963f5e5d1607f9d40c5173e0f9f))
* **editor:** Format action names properly when action is not defined ([#11030](https://github.com/n8n-io/n8n/issues/11030)) ([9c43fb3](https://github.com/n8n-io/n8n/commit/9c43fb301d1ccb82e42f46833e19587289803cd3))
* **Elasticsearch Node:** Fix issue with self signed certificates not working ([#10954](https://github.com/n8n-io/n8n/issues/10954)) ([79622b5](https://github.com/n8n-io/n8n/commit/79622b5f267f2a4a53f3eb48e228939d6e3a9caa))
* **Facebook Lead Ads Trigger Node:** Pagination fix in RLC ([#10956](https://github.com/n8n-io/n8n/issues/10956)) ([6322372](https://github.com/n8n-io/n8n/commit/632237261087ada0177b67922f9f48ca02ef1d9e))
* **Github Document Loader Node:** Pass through apiUrl from credentials & fix log output ([#11049](https://github.com/n8n-io/n8n/issues/11049)) ([a7af981](https://github.com/n8n-io/n8n/commit/a7af98183c47a5e215869c8269729b0fb2f318b5))
* **Google Sheets Node:** Updating on row_number using automatic matching  ([#10940](https://github.com/n8n-io/n8n/issues/10940)) ([ed91495](https://github.com/n8n-io/n8n/commit/ed91495ebc1e09b89533ffef4b775eaa0139f365))
* **HTTP Request Tool Node:** Remove default user agent header ([#10971](https://github.com/n8n-io/n8n/issues/10971)) ([5a99e93](https://github.com/n8n-io/n8n/commit/5a99e93f8d2c66d7dbcef382478badd63bc4a0b5))
* **Postgres Node:** Falsy query parameters ignored ([#10960](https://github.com/n8n-io/n8n/issues/10960)) ([4a63cff](https://github.com/n8n-io/n8n/commit/4a63cff5ec722c810e3ff2bd7b0bb1e32f7f403b))
* **Respond to Webhook Node:** Node does not work with Wait node ([#10992](https://github.com/n8n-io/n8n/issues/10992)) ([2df5a5b](https://github.com/n8n-io/n8n/commit/2df5a5b649f8ba3b747782d6d5045820aa74955d))
* **RSS Feed Trigger Node:** Fix regression on missing timestamps ([#10991](https://github.com/n8n-io/n8n/issues/10991)) ([d2bc076](https://github.com/n8n-io/n8n/commit/d2bc0760e2b5c977fcc683f0a0281f099a9c538d))
* **Supabase Node:** Fix issue with delete not always working ([#10952](https://github.com/n8n-io/n8n/issues/10952)) ([1944b46](https://github.com/n8n-io/n8n/commit/1944b46fd472bb59552b5fbf7783168a622a2bd2))
* **Text Classifier Node:** Default system prompt template ([#11018](https://github.com/n8n-io/n8n/issues/11018)) ([77fec19](https://github.com/n8n-io/n8n/commit/77fec195d92e0fe23c60552a72e8c030cf7e5e5c))
* **Todoist Node:** Fix listSearch filter bug in Todoist Node ([#10989](https://github.com/n8n-io/n8n/issues/10989)) ([c4b3272](https://github.com/n8n-io/n8n/commit/c4b327248d7aa1352e8d6acec5627ff406aea3d4))
* **Todoist Node:** Make Section Name optional in Move Task operation ([#10732](https://github.com/n8n-io/n8n/issues/10732)) ([799006a](https://github.com/n8n-io/n8n/commit/799006a3cce6abe210469c839ae392d0c1aec486))


### Features

* Add more context to support chat ([#11014](https://github.com/n8n-io/n8n/issues/11014)) ([8a30f92](https://github.com/n8n-io/n8n/commit/8a30f92156d6a4fe73113bd3cdfb751b8c9ce4b4))
* Add Sysdig API credentials for SecOps ([#7033](https://github.com/n8n-io/n8n/issues/7033)) ([a8d1a1e](https://github.com/n8n-io/n8n/commit/a8d1a1ea854fb2c69643b0a5738440b389121ca3))
* **core:** Filter executions by project ID in internal API ([#10976](https://github.com/n8n-io/n8n/issues/10976)) ([06d749f](https://github.com/n8n-io/n8n/commit/06d749ffa7ced503141d8b07e22c47d971eb1623))
* **core:** Implement Dynamic Parameters within regular nodes used as AI Tools ([#10862](https://github.com/n8n-io/n8n/issues/10862)) ([ef5b7cf](https://github.com/n8n-io/n8n/commit/ef5b7cf9b77b653111eb5b1d9de8116c9f6b9f92))
* **editor:** Do not show error for remote options when credentials aren't specified ([#10944](https://github.com/n8n-io/n8n/issues/10944)) ([9fc3699](https://github.com/n8n-io/n8n/commit/9fc3699beb0c150909889ed17740a5cd9e0461c3))
* **editor:** Enable drag and drop in code editors (Code/SQL/HTML) ([#10888](https://github.com/n8n-io/n8n/issues/10888)) ([af9e227](https://github.com/n8n-io/n8n/commit/af9e227ad4848995b9d82c72f814dbf9d1de506f))
* **editor:** Overhaul document title management ([#10999](https://github.com/n8n-io/n8n/issues/10999)) ([bb28956](https://github.com/n8n-io/n8n/commit/bb2895689fb006897bc244271aca6f0bfa1839b9))
* **editor:** Remove execution annotation feature flag ([#11020](https://github.com/n8n-io/n8n/issues/11020)) ([e7199db](https://github.com/n8n-io/n8n/commit/e7199dbfccdbdf1c4273f916e3006ca610c230e9))
* **editor:** Support node-creator actions for vector store nodes ([#11032](https://github.com/n8n-io/n8n/issues/11032)) ([72b70d9](https://github.com/n8n-io/n8n/commit/72b70d9d98daeba654baf6785ff1ae234c73c977))
* **Google BigQuery Node:** Return numeric values as integers ([#10943](https://github.com/n8n-io/n8n/issues/10943)) ([d7c1d24](https://github.com/n8n-io/n8n/commit/d7c1d24f74648740b2f425640909037ba06c5030))
* **Invoice Ninja Node:** Add more query params to getAll requests ([#9238](https://github.com/n8n-io/n8n/issues/9238)) ([50b7238](https://github.com/n8n-io/n8n/commit/50b723836e70bbe405594f690b73057f9c33fbe4))
* **Iterable Node:** Add support for EDC and USDC selection ([#10908](https://github.com/n8n-io/n8n/issues/10908)) ([0ca9c07](https://github.com/n8n-io/n8n/commit/0ca9c076ca51d313392e45c3b013f2e83aaea843))
* **Question and Answer Chain Node:** Customize question and answer system prompt ([#10385](https://github.com/n8n-io/n8n/issues/10385)) ([08a27b3](https://github.com/n8n-io/n8n/commit/08a27b3148aac2282f64339ddc33ac7c90835d84))



# [1.61.0](https://github.com/n8n-io/n8n/compare/n8n@1.60.0...n8n@1.61.0) (2024-09-25)


### Bug Fixes

* **core:** Add executionData to expressions in pagination code ([#10926](https://github.com/n8n-io/n8n/issues/10926)) ([eac103e](https://github.com/n8n-io/n8n/commit/eac103e367d59a532b9ba12db78a0dd10aee62fb))
* **core:** Fix webhook binary data max size configuration ([#10897](https://github.com/n8n-io/n8n/issues/10897)) ([693fb7e](https://github.com/n8n-io/n8n/commit/693fb7e580b7e030c86977bff6d319bbee4fcd62))
* **core:** Remove subworkflow license check ([#10893](https://github.com/n8n-io/n8n/issues/10893)) ([0290e38](https://github.com/n8n-io/n8n/commit/0290e38f990275074eb7e7ccd0b41f1ae0215dd2))
* **editor:** Credentials scopes and n8n scopes mix up ([#10930](https://github.com/n8n-io/n8n/issues/10930)) ([e069608](https://github.com/n8n-io/n8n/commit/e0696080227aee7ccb50d51a82873e8a1ba4667d))
* **editor:** Fix design system form component sizing ([#10961](https://github.com/n8n-io/n8n/issues/10961)) ([cf153ea](https://github.com/n8n-io/n8n/commit/cf153ea085165115ee523fbb1bd32080dde47eda))
* **editor:** Fix modal overflow when AI is enabled in code node ([#10887](https://github.com/n8n-io/n8n/issues/10887)) ([f9f303f](https://github.com/n8n-io/n8n/commit/f9f303f562084db8c8956da267680b1f935aa2df))
* **editor:** Fix source control push modal checkboxes ([#10910](https://github.com/n8n-io/n8n/issues/10910)) ([8db8817](https://github.com/n8n-io/n8n/commit/8db88178511749b19a5878816ef062092fd9f2be))
* **editor:** Fix styling and typography in AI Assistant chat ([#10895](https://github.com/n8n-io/n8n/issues/10895)) ([57ff3cc](https://github.com/n8n-io/n8n/commit/57ff3cc27b9470bfbe2486c3c1831c57f5a4075f))
* **editor:** Prevent clipboard xss injection ([#10894](https://github.com/n8n-io/n8n/issues/10894)) ([e20ab59](https://github.com/n8n-io/n8n/commit/e20ab59c1dcf9da19a30268ce19930bfa7e38992))
* **editor:** Prevent node name input in NDV to expand unnecessarily ([#10922](https://github.com/n8n-io/n8n/issues/10922)) ([a2237d1](https://github.com/n8n-io/n8n/commit/a2237d128ff6a4d65cd30325b6b9d9b765ca7be6))
* **editor:** Update gird size when opening credentials support chat ([#10882](https://github.com/n8n-io/n8n/issues/10882)) ([b86fd80](https://github.com/n8n-io/n8n/commit/b86fd80fc9fe06011367ca04a75e4b52533db1fe))
* **editor:** Use `:focus-visible` instead for `:focus` for buttons ([#10921](https://github.com/n8n-io/n8n/issues/10921)) ([bf28d09](https://github.com/n8n-io/n8n/commit/bf28d0965c46620a106c87037bafd2cf936f1050))
* **editor:** Use correct output for connected nodes in schema view ([#10928](https://github.com/n8n-io/n8n/issues/10928)) ([ad60d49](https://github.com/n8n-io/n8n/commit/ad60d49b4251138a7c69cb5e9f00c3ef875486e0))
* Enable Assistant on other credential views ([#10931](https://github.com/n8n-io/n8n/issues/10931)) ([557db9c](https://github.com/n8n-io/n8n/commit/557db9c170a89447ec9cc14aa1af51e5fd11dd92))
* Ensure user id for early track events ([#10885](https://github.com/n8n-io/n8n/issues/10885)) ([23c09ea](https://github.com/n8n-io/n8n/commit/23c09eae4223545c717270a5cd305d2e57e1ad5b))
* **Google Sheets Node:** Insert data if sheet is empty instead of error ([#10942](https://github.com/n8n-io/n8n/issues/10942)) ([c75990e](https://github.com/n8n-io/n8n/commit/c75990e0632c581384542610a886ef89621a9403))
* Hide assistant button when showing Click to connect ([#10932](https://github.com/n8n-io/n8n/issues/10932)) ([d74cff2](https://github.com/n8n-io/n8n/commit/d74cff20301f285588f93207f29660d25fdbc8da))
* **HTTP Request Node:** Do not modify request object when sanitizing message for UI ([#10923](https://github.com/n8n-io/n8n/issues/10923)) ([8cc10cc](https://github.com/n8n-io/n8n/commit/8cc10cc2c1869b9abcafd157e41be65ce2b6f499))
* **MQTT Node:** Close connection if connection attempt fails ([#10873](https://github.com/n8n-io/n8n/issues/10873)) ([ee7147c](https://github.com/n8n-io/n8n/commit/ee7147c6b3b053ac8fc317319ab257204e599f16))
* **MySQL Node:** Fix "Maximum call stack size exceeded" error when handling a large number of rows ([#10965](https://github.com/n8n-io/n8n/issues/10965)) ([62159bd](https://github.com/n8n-io/n8n/commit/62159bd71c9a0303b597a68113e0ac50473ee8d4))
* **Notion Node:** Allow UUID v8 in notion id checks ([#10938](https://github.com/n8n-io/n8n/issues/10938)) ([46beda0](https://github.com/n8n-io/n8n/commit/46beda05f6771c31bcf0b6a781976d8261079a66))


### Features

* **Brandfetch Node:** Update to use new API ([#10877](https://github.com/n8n-io/n8n/issues/10877)) ([08ba9a3](https://github.com/n8n-io/n8n/commit/08ba9a36a43b6c84f69bb04fa4d6419a7a4adddf))
* **editor:** Setup Sentry integration ([#10945](https://github.com/n8n-io/n8n/issues/10945)) ([6de4dff](https://github.com/n8n-io/n8n/commit/6de4dfff87e4da888567081a9928d9682bdea11d))
* **editor:** Show a notice before deleting annotated executions ([#10934](https://github.com/n8n-io/n8n/issues/10934)) ([dcc1c72](https://github.com/n8n-io/n8n/commit/dcc1c72fc4b56c3252183541b22da801804d4f79))
* Page size 1 option ([#10957](https://github.com/n8n-io/n8n/issues/10957)) ([bdc0622](https://github.com/n8n-io/n8n/commit/bdc0622f59e98c9e6c542f5cb59a2dbd9008ba96))
* **Slack Node:** Add option to hide workflow link on message update ([#10927](https://github.com/n8n-io/n8n/issues/10927)) ([422c946](https://github.com/n8n-io/n8n/commit/422c9463c8d931a728615a1fe5a10f05a96ecaa2))


### Performance Improvements

* **editor:** Use virtual scrolling in `RunDataJson.vue` ([#10838](https://github.com/n8n-io/n8n/issues/10838)) ([f5474ff](https://github.com/n8n-io/n8n/commit/f5474ff79198a2f5a145d0a9df1bb651ea677ec5))



# [1.60.0](https://github.com/n8n-io/n8n/compare/n8n@1.59.0...n8n@1.60.0) (2024-09-18)


### Bug Fixes

* **Azure OpenAI Chat Model Node:** Add response format option ([#10851](https://github.com/n8n-io/n8n/issues/10851)) ([0b5299a](https://github.com/n8n-io/n8n/commit/0b5299a248fdd451ceabb98ff6a2b38e818d02f8))
* **Contentful Node:** Add missing additional fields to entry > get ([#10830](https://github.com/n8n-io/n8n/issues/10830)) ([c43aef1](https://github.com/n8n-io/n8n/commit/c43aef1a266cc6ccf8f778c290f8cb8ba2ee28cf))
* **core:** Prevent shutdown error in regular mode ([#10844](https://github.com/n8n-io/n8n/issues/10844)) ([acb4194](https://github.com/n8n-io/n8n/commit/acb4194fa1a1d0497dd1f48045f069e1db28c432))
* **core:** Restore queue listeners for `webhook` process ([#10781](https://github.com/n8n-io/n8n/issues/10781)) ([86f4877](https://github.com/n8n-io/n8n/commit/86f4877bab978a1ec2f53df23b6c515507cd8f72))
* **editor:** Add missing node parameter values to AI Assistant request ([#10788](https://github.com/n8n-io/n8n/issues/10788)) ([d65ade4](https://github.com/n8n-io/n8n/commit/d65ade4e92eed3cfc47854d493fac6885a1a852b))
* **editor:** Address edge toolbar rendering glitches ([#10839](https://github.com/n8n-io/n8n/issues/10839)) ([e0c0dde](https://github.com/n8n-io/n8n/commit/e0c0ddee59e889f50dd5033d0a933bad60fb7e3a))
* **editor:** Allow custom git repo urls in source control settings ([#10849](https://github.com/n8n-io/n8n/issues/10849)) ([a63a9b5](https://github.com/n8n-io/n8n/commit/a63a9b53f06d3a00e8e76c0ab9f2571604c01922))
* **editor:** Fix completion on $input.item. in Code node ([#10800](https://github.com/n8n-io/n8n/issues/10800)) ([45dccf3](https://github.com/n8n-io/n8n/commit/45dccf3d0c8282987833962a8e3f3a77d256ea37))
* **editor:** Make expression edit modal read-only in executions view ([#10806](https://github.com/n8n-io/n8n/issues/10806)) ([394ef88](https://github.com/n8n-io/n8n/commit/394ef888433b1d48593531ab9eea93a3c3ae6040))
* **editor:** Make schema view search copy more clear ([#10807](https://github.com/n8n-io/n8n/issues/10807)) ([7f1c131](https://github.com/n8n-io/n8n/commit/7f1c131b72ad1b98b4a8c976b8a0ef5d963d5f1f))
* **editor:** Minimap Show nodes outside viewport ([#10843](https://github.com/n8n-io/n8n/issues/10843)) ([9c95db8](https://github.com/n8n-io/n8n/commit/9c95db8282c9f3cef5568aa9793ca977d4d8a347))
* **editor:** Prevent clipboard XSS injection ([#10805](https://github.com/n8n-io/n8n/issues/10805)) ([db846d3](https://github.com/n8n-io/n8n/commit/db846d3235a360b4b729312b6ffe0d75be08fd45))
* **editor:** Render image binary-data using img tags ([#10829](https://github.com/n8n-io/n8n/issues/10829)) ([7c23101](https://github.com/n8n-io/n8n/commit/7c23101ab8c12b735a17deb35637f3f12c00aeb0))
* **editor:** Replace v-html with custom directive to sanitize html ([#10804](https://github.com/n8n-io/n8n/issues/10804)) ([44e5fb9](https://github.com/n8n-io/n8n/commit/44e5fb9b06c794033204ef1744b54b3b87160082))
* **editor:** Restore V1 keybinding, Space Key to toggle panning ([#10841](https://github.com/n8n-io/n8n/issues/10841)) ([5a1db6d](https://github.com/n8n-io/n8n/commit/5a1db6db1adad43887e839181719818474bc66b0))
* Fix telemetry causing console error ([#10828](https://github.com/n8n-io/n8n/issues/10828)) ([3be31e2](https://github.com/n8n-io/n8n/commit/3be31e27edc6e71400bde23f992ba98b2365bcff))
* **Google Vertex Chat Model Node:** Clean service account private key ([#10770](https://github.com/n8n-io/n8n/issues/10770)) ([e6d84db](https://github.com/n8n-io/n8n/commit/e6d84db89930afc16f4a08fae87d8af4a059e6d7))
* **HTTP Request Tool Node:** Fix subsequent tool calls reusung the same options ([#10808](https://github.com/n8n-io/n8n/issues/10808)) ([d647ef4](https://github.com/n8n-io/n8n/commit/d647ef41acf672177ea5e8ce0e99d78c565e34b2))
* **OpenAI Node, Basic LLM Chain Node, Tool Agent Node:** Better OpenAI API rate limit errors ([#10797](https://github.com/n8n-io/n8n/issues/10797)) ([ab83c4b](https://github.com/n8n-io/n8n/commit/ab83c4b4166d5ad5f4ca46a636f83c8802fe3ec0))
* Prevent copying workflow when copying outside of canvas ([#10813](https://github.com/n8n-io/n8n/issues/10813)) ([22c1890](https://github.com/n8n-io/n8n/commit/22c1890139c89e74df67b9673a1d0c85d647eb9d))
* **RSS Feed Trigger Node:** Handle empty items gracefully ([#10855](https://github.com/n8n-io/n8n/issues/10855)) ([c55df63](https://github.com/n8n-io/n8n/commit/c55df63abc234ace6ac8e54ed094d10797671264))


### Features

* **core:** Allow customizing max file size in form-data payloads for webhooks ([#10857](https://github.com/n8n-io/n8n/issues/10857)) ([a3335e0](https://github.com/n8n-io/n8n/commit/a3335e0ecd3796c874985d3c6fbbaabc35dc3490))
* **core:** Introduce worker metrics ([#10850](https://github.com/n8n-io/n8n/issues/10850)) ([08ebe1e](https://github.com/n8n-io/n8n/commit/08ebe1e4807b3d7b4a4840887cbb30f547a5c89a))
* **editor:** Add truncate directive ([#10842](https://github.com/n8n-io/n8n/issues/10842)) ([57836cc](https://github.com/n8n-io/n8n/commit/57836cc17a57c790d2ffb2463abb16a03321eb59))
* **editor:** Show Collaboration pane only when there are multiple active users ([#10772](https://github.com/n8n-io/n8n/issues/10772)) ([a0af1d9](https://github.com/n8n-io/n8n/commit/a0af1d9a06c78d29f215dc010332ea7c8f28717d))
* **Invoice Ninja Node:** Add actions for bank transactions ([#10389](https://github.com/n8n-io/n8n/issues/10389)) ([5a2c7e0](https://github.com/n8n-io/n8n/commit/5a2c7e00a0ca1a151a7fec56da5f99b086c25b1f))
* **OpenAI Node:** Include O1 models in the models select ([#10801](https://github.com/n8n-io/n8n/issues/10801)) ([b2b1abc](https://github.com/n8n-io/n8n/commit/b2b1abc5319bdbf2bc855649ea27359b22aba009))



# [1.59.0](https://github.com/n8n-io/n8n/compare/n8n@1.58.0...n8n@1.59.0) (2024-09-11)


### Bug Fixes

* **Chat Trigger Node:** Fix auth in "Embedded Chat" mode ([#10734](https://github.com/n8n-io/n8n/issues/10734)) ([96db501](https://github.com/n8n-io/n8n/commit/96db501a615ff7ec91bb66ea49532a2c6ca2a172))
* **core:** Allow license:clear command to be used for licenses that failed renewal ([#10665](https://github.com/n8n-io/n8n/issues/10665)) ([a422c5a](https://github.com/n8n-io/n8n/commit/a422c5ac7b8f609eeab891230d9660f71bf225c5))
* **core:** Update subworkflow execution status correctly ([#10764](https://github.com/n8n-io/n8n/issues/10764)) ([4f94319](https://github.com/n8n-io/n8n/commit/4f94319cd93885ebe830fa1f0e6b757de80f7356))
* **editor:** Add arrow end to connection line ([#10704](https://github.com/n8n-io/n8n/issues/10704)) ([43713dc](https://github.com/n8n-io/n8n/commit/43713dcd89fcb98ea7e24d27127861fc4b0d7872))
* **editor:** Add sticky note readonly state in new canvas ([#10678](https://github.com/n8n-io/n8n/issues/10678)) ([c5bc8e6](https://github.com/n8n-io/n8n/commit/c5bc8e6eb9eadadf44f763e5e5aac4b35d03cc31))
* **editor:** Auto-focus expression input when switching from "fixed" mode ([#10686](https://github.com/n8n-io/n8n/issues/10686)) ([54ab2b1](https://github.com/n8n-io/n8n/commit/54ab2b14e41fe84a455c7e7d5c73d7347844d2fb))
* **editor:** Don't render pinned icon for disabled nodes ([#10712](https://github.com/n8n-io/n8n/issues/10712)) ([879b837](https://github.com/n8n-io/n8n/commit/879b8375812106b3f6909b7de27858175ba5575d))
* **editor:** Fix error rendering and indexing of LLM sub-node outputs ([#10688](https://github.com/n8n-io/n8n/issues/10688)) ([50459ba](https://github.com/n8n-io/n8n/commit/50459bacab517bacb97d2884fda69f8412c9960c))
* **editor:** Fix xss issues in toast usages ([#10733](https://github.com/n8n-io/n8n/issues/10733)) ([6df6f5f](https://github.com/n8n-io/n8n/commit/6df6f5f8df9a8fc0899524a1b69859815eeb341f))
* **editor:** Follow up fixes and improvements to viewer role ([#10684](https://github.com/n8n-io/n8n/issues/10684)) ([63548e6](https://github.com/n8n-io/n8n/commit/63548e6ead5c122732628b5feb1515f492d5e033))
* **editor:** Increase connector snap radius ([#10757](https://github.com/n8n-io/n8n/issues/10757)) ([297b668](https://github.com/n8n-io/n8n/commit/297b668f32f9ecfc82c1205ea4e915408cab482e))
* **editor:** Plus node button should not be visible on readonly mode ([#10692](https://github.com/n8n-io/n8n/issues/10692)) ([62cb189](https://github.com/n8n-io/n8n/commit/62cb189985035c447ad31c275337b3fb24089265))
* **editor:** Prevent action's panel flickering while dragging a node  ([#10739](https://github.com/n8n-io/n8n/issues/10739)) ([efa5573](https://github.com/n8n-io/n8n/commit/efa5573278a60d55d5b509aac48cc112c79334d2))
* **editor:** Restrict when the collision avoidance algorithm is used ([#10755](https://github.com/n8n-io/n8n/issues/10755)) ([bf43d67](https://github.com/n8n-io/n8n/commit/bf43d673571b2fc18fe5d660171f0da165909dfc))
* **editor:** Show docs link in credential modal when docs sidebar is hidden ([#10750](https://github.com/n8n-io/n8n/issues/10750)) ([87333cb](https://github.com/n8n-io/n8n/commit/87333cbefebe652256fa1d60ba7a4b946fdfe17d))
* **Email Trigger (IMAP) Node:** Ensure connection close does not block deactivation ([#10689](https://github.com/n8n-io/n8n/issues/10689)) ([156eb72](https://github.com/n8n-io/n8n/commit/156eb72ebefa1d963ff46eff6652e2c947ef031b))
* Fix the issue in Trigger Nodes where poll time was not loaded ([#10695](https://github.com/n8n-io/n8n/issues/10695)) ([1dea8f4](https://github.com/n8n-io/n8n/commit/1dea8f4c7da2a04434c274faf8e0a9a7a693f5a4))
* **Gmail Trigger Node:** Change Gmail Trigger dedupe logic ([#10717](https://github.com/n8n-io/n8n/issues/10717)) ([9f3e03d](https://github.com/n8n-io/n8n/commit/9f3e03d728d8acda5ae4166c5837b00cb1311e96))
* Google Contacts node warm up request, Google Calendar node events>getAll fields option ([#10700](https://github.com/n8n-io/n8n/issues/10700)) ([22c70d5](https://github.com/n8n-io/n8n/commit/22c70d50697023cf448a379d7778695abb718ce9))
* **If Node:** Update copy for type conversion parameter ([#10769](https://github.com/n8n-io/n8n/issues/10769)) ([ee5fbc5](https://github.com/n8n-io/n8n/commit/ee5fbc543ce1d33a56cf118dbd048d6693a15875))
* **n8n Form Trigger Node:** Do not rerun trigger when it has run data ([#10687](https://github.com/n8n-io/n8n/issues/10687)) ([3adbcab](https://github.com/n8n-io/n8n/commit/3adbcab27de34ea5a2c7a88b2ad0d80e3f6d4a0b))
* **OpenAI Chat Model Node:** Prevent filtering of fine-tuned models in model selector ([#10662](https://github.com/n8n-io/n8n/issues/10662)) ([4e89912](https://github.com/n8n-io/n8n/commit/4e899125884bdd97c97446d90e89668688fe7573))
* Prevent AI assistant session reset when workflow is saved ([#10707](https://github.com/n8n-io/n8n/issues/10707)) ([91d9be2](https://github.com/n8n-io/n8n/commit/91d9be20667c20599f64a24fa99386c78476d425))
* Show a more user friendly error message if initial Db connection times out ([#10682](https://github.com/n8n-io/n8n/issues/10682)) ([4efcbc5](https://github.com/n8n-io/n8n/commit/4efcbc593685286837022e5600d81e67f3e0131c))
* **Webflow Node:** Update scopes to include forms ([#10554](https://github.com/n8n-io/n8n/issues/10554)) ([d3861b3](https://github.com/n8n-io/n8n/commit/d3861b31ceef16f566c525c7651453a1b84ed2a4))
* **YouTube Node:** Fix Date filters ([#10725](https://github.com/n8n-io/n8n/issues/10725)) ([21936c8](https://github.com/n8n-io/n8n/commit/21936c88a84b8c03a8d02391cb7112b0e4d9f1f9))


### Features

* **Code Tool Node:** Option to specify input schema ([#10693](https://github.com/n8n-io/n8n/issues/10693)) ([421aa71](https://github.com/n8n-io/n8n/commit/421aa712515d9beeae7c0201b173cb7324473f69))
* **editor:** Add lint for $('Node').item in runOnceForAllItems mode ([#10743](https://github.com/n8n-io/n8n/issues/10743)) ([1b04be1](https://github.com/n8n-io/n8n/commit/1b04be1240ec29151e79162680907710c71c6488))
* **editor:** Logs markdown block improvements ([#10681](https://github.com/n8n-io/n8n/issues/10681)) ([db6e832](https://github.com/n8n-io/n8n/commit/db6e8326c7119d90fa6a51f82099026f50587202))
* Filter parameter: Improve loose type validation for booleans ([#10702](https://github.com/n8n-io/n8n/issues/10702)) ([e9b8d99](https://github.com/n8n-io/n8n/commit/e9b8d99084f0ea2063a1d691928025e534980b4e))
* **Lemlist Node:** Add V2 to support more API operations ([#10615](https://github.com/n8n-io/n8n/issues/10615)) ([20b1cf2](https://github.com/n8n-io/n8n/commit/20b1cf2b7597c78e28f522945b8cbad2ee535cd7))
* **OpenAI Node:** Add Max Tools Iteration parameter and prevent tool calling after execution is aborted ([#10735](https://github.com/n8n-io/n8n/issues/10735)) ([5c47a5f](https://github.com/n8n-io/n8n/commit/5c47a5f691d42dae84a9df8a32a5ea600d83f6dd))


### Performance Improvements

* **editor:** Fix WorkflowDetails excessive re-rendering ([#10767](https://github.com/n8n-io/n8n/issues/10767)) ([00013a2](https://github.com/n8n-io/n8n/commit/00013a2069fff5e5d9398c5921c90d34dc384299))



# [1.58.0](https://github.com/n8n-io/n8n/compare/n8n@1.57.0...n8n@1.58.0) (2024-09-05)


### Bug Fixes

* **AI Agent Node:** Fix tools agent when using memory and Anthropic models ([#10513](https://github.com/n8n-io/n8n/issues/10513)) ([746e7b8](https://github.com/n8n-io/n8n/commit/746e7b89f7e9b99126fb69110773548dfe91b74f))
* **API:** Update express-openapi-validator to resolve AIKIDO-2024-10229 ([#10612](https://github.com/n8n-io/n8n/issues/10612)) ([1dcb814](https://github.com/n8n-io/n8n/commit/1dcb814ced7cfbc80eddbb4bc03108341a9f27f5))
* **core:** Declutter webhook insertion errors ([#10650](https://github.com/n8n-io/n8n/issues/10650)) ([36177b0](https://github.com/n8n-io/n8n/commit/36177b0943cf72bae3b0075453498dd1e41684d0))
* **core:** Flush responses for ai streaming endpoints ([#10633](https://github.com/n8n-io/n8n/issues/10633)) ([6bb6a5c](https://github.com/n8n-io/n8n/commit/6bb6a5c6cd1da3503a1a2b35bcf4c685cd3f964f))
* **core:** Tighten check for company size survey answer ([#10646](https://github.com/n8n-io/n8n/issues/10646)) ([e5aba60](https://github.com/n8n-io/n8n/commit/e5aba60afff93364d91f17c00ea18d38d9dbc970))
* **editor:** Add confirmation toast when changing user role ([#10592](https://github.com/n8n-io/n8n/issues/10592)) ([95da4d4](https://github.com/n8n-io/n8n/commit/95da4d4797e800c04b2b17c23c941c785dd62393))
* **editor:** Add pinned data only to manual executions in execution view ([#10605](https://github.com/n8n-io/n8n/issues/10605)) ([a12e9ed](https://github.com/n8n-io/n8n/commit/a12e9edac042957939c63f0a5c35572930632352))
* **editor:** Add tooltips to workflow history button ([#10570](https://github.com/n8n-io/n8n/issues/10570)) ([4a125f5](https://github.com/n8n-io/n8n/commit/4a125f511c5537977652900b7712a2ad908140e7))
* **editor:** Allow disabling SSO when config request fails ([#10635](https://github.com/n8n-io/n8n/issues/10635)) ([ce39933](https://github.com/n8n-io/n8n/commit/ce39933766fa18107f4082de0cba0b6702cbbbfa))
* **editor:** Fix notification rendering HTML as text ([#10642](https://github.com/n8n-io/n8n/issues/10642)) ([5eba534](https://github.com/n8n-io/n8n/commit/5eba5343191665cd4639632ba303464176c279c4))
* **editor:** Fix opening executions tab from a new, unsaved workflow ([#10652](https://github.com/n8n-io/n8n/issues/10652)) ([cd0891e](https://github.com/n8n-io/n8n/commit/cd0891e4f1cfdc90b2090958a39564ba99534627))
* **Gmail Trigger Node:** Don't return date instances, but date strings instead ([#10582](https://github.com/n8n-io/n8n/issues/10582)) ([9e1dac0](https://github.com/n8n-io/n8n/commit/9e1dac04655a20c5c7b99552742312fd9237604b))
* **HTTP Request Node:** Sanitize authorization headers ([#10607](https://github.com/n8n-io/n8n/issues/10607)) ([405c55a](https://github.com/n8n-io/n8n/commit/405c55a1f7cf34e7b6e46a86031ef9a41956ca78))
* **Wait Node:** Append n8n attribution option ([#10585](https://github.com/n8n-io/n8n/issues/10585)) ([81f4322](https://github.com/n8n-io/n8n/commit/81f4322d456773281aec4b47447465bdffd311fe))


### Features

* **core:** Execution curation ([#10342](https://github.com/n8n-io/n8n/issues/10342)) ([022ddcb](https://github.com/n8n-io/n8n/commit/022ddcbef9f1ac1b89bcfd5f7759d67325b07392))
* **core:** Implement wrapping of regular nodes as AI Tools ([#10641](https://github.com/n8n-io/n8n/issues/10641)) ([da44fe4](https://github.com/n8n-io/n8n/commit/da44fe4b8967055b7b1f849750e1fafa0ba67218))
* **core:** Introduce DB health check ([#10661](https://github.com/n8n-io/n8n/issues/10661)) ([a8e80d0](https://github.com/n8n-io/n8n/commit/a8e80d0c4b7531fe32be1d4057656885359f42fc))
* **core:** Make Postgres connection timeout configurable ([#10670](https://github.com/n8n-io/n8n/issues/10670)) ([8154031](https://github.com/n8n-io/n8n/commit/81540318b4c55f3a09c9776e23d2211abdbd36f7))
* **core:** Switch to MJML for email templates ([#10518](https://github.com/n8n-io/n8n/issues/10518)) ([dbc10fe](https://github.com/n8n-io/n8n/commit/dbc10fe9f522f31eb06add6f3f6863ce24510547))
* **editor:** Add A/B testing feature flag for credential docs modal ([#10664](https://github.com/n8n-io/n8n/issues/10664)) ([899b0a1](https://github.com/n8n-io/n8n/commit/899b0a19efc49c1c087f78bbb1a59d726a510965))
* **editor:** Add AI Assistant support chat ([#10656](https://github.com/n8n-io/n8n/issues/10656)) ([3a80780](https://github.com/n8n-io/n8n/commit/3a8078068e5c0b01dfd34ff838fe1b30d604abc6))
* **editor:** Implement new app layout ([#10548](https://github.com/n8n-io/n8n/issues/10548)) ([95a9cd2](https://github.com/n8n-io/n8n/commit/95a9cd2c739cf4f817eb8df6509a9112ac24a3b1))
* **editor:** Make highlighted data pane floating ([#10638](https://github.com/n8n-io/n8n/issues/10638)) ([8b5c333](https://github.com/n8n-io/n8n/commit/8b5c333d3dca03ba51a5873b75451fbfafc5ae15))
* More hints to nodes  ([#10565](https://github.com/n8n-io/n8n/issues/10565)) ([66ddb4a](https://github.com/n8n-io/n8n/commit/66ddb4a6f367602c9aaad1bfb0cc6fac3facd15e))
* **Postgres PGVector Store Node:** Add PGVector vector store node ([#10517](https://github.com/n8n-io/n8n/issues/10517)) ([650389d](https://github.com/n8n-io/n8n/commit/650389d90763a45c037e74a1a1193c3cbe103a16))
* Reintroduce collaboration feature ([#10602](https://github.com/n8n-io/n8n/issues/10602)) ([2ea2bfe](https://github.com/n8n-io/n8n/commit/2ea2bfe762c02047e522f28dd97f197735b3fb46))
* **Text Classifier Node:** Add output fixing parser ([#10667](https://github.com/n8n-io/n8n/issues/10667)) ([aa37c32](https://github.com/n8n-io/n8n/commit/aa37c32f266ffff93cd903888b1c15caa0468830))



# [1.57.0](https://github.com/n8n-io/n8n/compare/n8n@1.56.0...n8n@1.57.0) (2024-08-28)


### Bug Fixes

* **AI Agent Node:** Allow AWS Bedrock Chat to be used with conversational agent ([#10489](https://github.com/n8n-io/n8n/issues/10489)) ([bdcc657](https://github.com/n8n-io/n8n/commit/bdcc657965af5f604aac1eaff7d937f69a08ce1c))
* **core:** Make boolean config value parsing backward-compatible ([#10560](https://github.com/n8n-io/n8n/issues/10560)) ([70b410f](https://github.com/n8n-io/n8n/commit/70b410f4b00dd599fcd4249aa105098aa262da66))
* **core:** Restore Redis cache key ([#10520](https://github.com/n8n-io/n8n/issues/10520)) ([873056a](https://github.com/n8n-io/n8n/commit/873056a92e52cc629d2873c960656d5f06d4728e))
* **core:** Scheduler tasks should not trigger on follower instances ([#10507](https://github.com/n8n-io/n8n/issues/10507)) ([3428f28](https://github.com/n8n-io/n8n/commit/3428f28a732f79e067b3cb515cc59d835de246a6))
* **core:** Stop explicit redis client disconnect on shutdown ([#10551](https://github.com/n8n-io/n8n/issues/10551)) ([f712812](https://github.com/n8n-io/n8n/commit/f71281221efb79d65d8d7610c292bc90cef13d7a))
* **editor:** Ensure `Datatable` component renders `All` option ([#10525](https://github.com/n8n-io/n8n/issues/10525)) ([bc27beb](https://github.com/n8n-io/n8n/commit/bc27beb6629883003a8991d7e840ffaa066d41ac))
* **editor:** Prevent Safari users from accessing the frontend over insecure contexts ([#10510](https://github.com/n8n-io/n8n/issues/10510)) ([a73b9a3](https://github.com/n8n-io/n8n/commit/a73b9a38d6c48e2f78593328e7d9933f2493dbb6))
* **editor:** Scale output item selector input width with value ([#10555](https://github.com/n8n-io/n8n/issues/10555)) ([52c574d](https://github.com/n8n-io/n8n/commit/52c574d83f344f03b0e39984bbc3ac0402e50791))
* **Google Sheets Trigger Node:** Show sheet name is too long error ([#10542](https://github.com/n8n-io/n8n/issues/10542)) ([4e15007](https://github.com/n8n-io/n8n/commit/4e1500757700ec984cdad8b9cfcd76ee00ae127e))
* **Wait Node:** Prevent waiting until invalid date ([#10523](https://github.com/n8n-io/n8n/issues/10523)) ([c0e7620](https://github.com/n8n-io/n8n/commit/c0e7620036738f8d0b382d0d0610b981dcbc29e0))


### Features

* Add new credentials for the HTTP Request node ([#9833](https://github.com/n8n-io/n8n/issues/9833)) ([26f1af3](https://github.com/n8n-io/n8n/commit/26f1af397b2b25e3394fc2dae91a5c281bf33d66))
* **AI Agent Node:** Add tutorial link to agent node ([#10493](https://github.com/n8n-io/n8n/issues/10493)) ([5c7cc36](https://github.com/n8n-io/n8n/commit/5c7cc36c23e58a47a1e71911e7303a1bd54f167e))
* **core:** Expose queue metrics for Prometheus ([#10559](https://github.com/n8n-io/n8n/issues/10559)) ([008c510](https://github.com/n8n-io/n8n/commit/008c510b7623fefb8c60730c7eac54dd9bb2e3fc))
* **editor:** Implement workflowSelector parameter type ([#10482](https://github.com/n8n-io/n8n/issues/10482)) ([84e54be](https://github.com/n8n-io/n8n/commit/84e54beac763f25399c9687f695f1e658e3ce434))


### Performance Improvements

* **core:** Make execution queries faster ([#9817](https://github.com/n8n-io/n8n/issues/9817)) ([dc7dc99](https://github.com/n8n-io/n8n/commit/dc7dc995d5e2ea8fbd0dcb54cfa8aa93ecb437c9))

### Other
* **Add user journey link to [n8n.io](https://n8n.io)** ([#10331](https://github.com/n8n-io/n8n/pull/10331))


# [1.56.0](https://github.com/n8n-io/n8n/compare/n8n@1.55.0...n8n@1.56.0) (2024-08-21)


### Bug Fixes

* Better errors in Switch, If and Filter nodes ([#10457](https://github.com/n8n-io/n8n/issues/10457)) ([aea82cb](https://github.com/n8n-io/n8n/commit/aea82cb74421d516919742127daf669808b57604))
* **Calendly Trigger Node:** Fix issue with webhook url matching ([#10378](https://github.com/n8n-io/n8n/issues/10378)) ([09c3a8b](https://github.com/n8n-io/n8n/commit/09c3a8b36733a9634ef5948922d6aa7a19bbb592))
* **core:** Fix payload property in `workflow-post-execute` event ([#10413](https://github.com/n8n-io/n8n/issues/10413)) ([d98e29e](https://github.com/n8n-io/n8n/commit/d98e29e3d53de87aec276260615fa60473a2692f))
* **core:** Fix XSS validation and separate URL validation ([#10424](https://github.com/n8n-io/n8n/issues/10424)) ([91467ab](https://github.com/n8n-io/n8n/commit/91467ab325e4c71c20c522f3143246d270101626))
* **core:** Replace `sanitize-html` with `xss` in XSS validator constraint ([#10479](https://github.com/n8n-io/n8n/issues/10479)) ([5dea51a](https://github.com/n8n-io/n8n/commit/5dea51aad7d9e7ffc676d16f4bbbdecce5876f0b))
* **core:** Use class-validator with XSS check for survey answers ([#10490](https://github.com/n8n-io/n8n/issues/10490)) ([547a606](https://github.com/n8n-io/n8n/commit/547a60642ce9e54819d4e600c822d87dabd59b2e))
* **core:** Use explicit types in configs to ensure valid decorator metadata ([#10433](https://github.com/n8n-io/n8n/issues/10433)) ([2043daa](https://github.com/n8n-io/n8n/commit/2043daa2570bc04b0b8d41f277901a8cc8a7b98f))
* **editor:** Add workflow scopes when initializing workflow  ([#10455](https://github.com/n8n-io/n8n/issues/10455)) ([b857c2c](https://github.com/n8n-io/n8n/commit/b857c2cda0a9e4386a540d5e1e741570d9453588))
* **editor:** Buffer json chunks in stream response ([#10439](https://github.com/n8n-io/n8n/issues/10439)) ([37797f3](https://github.com/n8n-io/n8n/commit/37797f38d81b12d030ba85034baeb49192ea575c))
* **editor:** Fix flaky mapping tests ([#10453](https://github.com/n8n-io/n8n/issues/10453)) ([fc6d413](https://github.com/n8n-io/n8n/commit/fc6d4138d58282f676b32f1a6011b1b6d0184bf2))
* **editor:** Fix overflow in AI Assistant chat messages ([#10491](https://github.com/n8n-io/n8n/issues/10491)) ([4a6ca63](https://github.com/n8n-io/n8n/commit/4a6ca632100731f85875c639f2164bf1ef415009))
* **editor:** Highlight matching type in filter component ([#10425](https://github.com/n8n-io/n8n/issues/10425)) ([6bca879](https://github.com/n8n-io/n8n/commit/6bca879d4ae30c7f9a35e8d6672de42cf93be727))
* **editor:** Show item count in output panel schema view ([#10426](https://github.com/n8n-io/n8n/issues/10426)) ([4dee7cc](https://github.com/n8n-io/n8n/commit/4dee7cc36e5f7768d0b71095b194bf357c92e941))
* **editor:** Truncate long data pill labels in schema view ([#10427](https://github.com/n8n-io/n8n/issues/10427)) ([1bf2f4f](https://github.com/n8n-io/n8n/commit/1bf2f4f6171d666391bb3a3a312468bc083446e3))
* Filter component - improve errors ([#10456](https://github.com/n8n-io/n8n/issues/10456)) ([61ac0c7](https://github.com/n8n-io/n8n/commit/61ac0c77755210f570b887951fe6bbec1a323811))
* **Google Sheets Node:** Better error when column to match on is empty ([#10442](https://github.com/n8n-io/n8n/issues/10442)) ([ce46bf5](https://github.com/n8n-io/n8n/commit/ce46bf516a86d9779f37dd75b0c680d26d88e15d))
* **Google Sheets Node:** Update name and hint for useAppend option ([#10443](https://github.com/n8n-io/n8n/issues/10443)) ([c5a0c04](https://github.com/n8n-io/n8n/commit/c5a0c049eaf44419c690d151de42fb0c10bd406e))
* **Google Sheets Node:** Update to returnAllMatches option ([#10440](https://github.com/n8n-io/n8n/issues/10440)) ([f7fb02e](https://github.com/n8n-io/n8n/commit/f7fb02e92a756781f8e35bbbfc25d71c12cb70af))
* **Invoice Ninja Node:** Fix payment types ([#10462](https://github.com/n8n-io/n8n/issues/10462)) ([129245d](https://github.com/n8n-io/n8n/commit/129245da10be1d645f61e929e40b128bd7813f17))
* **n8n Form Trigger Node:** Show basic authentication modal on wrong credentials ([#10423](https://github.com/n8n-io/n8n/issues/10423)) ([0dc3e99](https://github.com/n8n-io/n8n/commit/0dc3e99b26bec45e747d83f383cfe5169d89e6b7))
* **OpenAI Node:** Throw node operations error in case of openAi client error ([#10448](https://github.com/n8n-io/n8n/issues/10448)) ([0d3ed46](https://github.com/n8n-io/n8n/commit/0d3ed461996bbad06015c455f133baab6506437f))
* Project Viewer always seeing a connection error when testing credentials ([#10417](https://github.com/n8n-io/n8n/issues/10417)) ([613cdd2](https://github.com/n8n-io/n8n/commit/613cdd2ba2c0f224c4857a5fc3eea36dbd683049))
* Remove unimplemented Postgres credentials options ([#10461](https://github.com/n8n-io/n8n/issues/10461)) ([17ac784](https://github.com/n8n-io/n8n/commit/17ac7844f29d819b91dfaf90b9fe386d98060c42))
* Rename Assistant back ([#10481](https://github.com/n8n-io/n8n/issues/10481)) ([c410aed](https://github.com/n8n-io/n8n/commit/c410aed4c22182943dc80ede63acda00b7898e10))
* Require mfa code to change email ([#10354](https://github.com/n8n-io/n8n/issues/10354)) ([39c8e50](https://github.com/n8n-io/n8n/commit/39c8e50ad0513649f5a8cef911b7d6cdd61c2372))
* **Respond to Webhook Node:** Fix issue preventing the chat trigger from working ([#9886](https://github.com/n8n-io/n8n/issues/9886)) ([9d6ad88](https://github.com/n8n-io/n8n/commit/9d6ad88c14a88fd0dfcb4f9981e38d19cf5f3067))
* Show input names when node has multiple inputs ([#10434](https://github.com/n8n-io/n8n/issues/10434)) ([973956c](https://github.com/n8n-io/n8n/commit/973956cc26c78c329ff6eb6934d4f0a24060c87c))
* **Toggl Trigger Node:** Update API version ([#10207](https://github.com/n8n-io/n8n/issues/10207)) ([9bdb1d6](https://github.com/n8n-io/n8n/commit/9bdb1d6dca43fe491c5eb96f093b7eec4509eaff))


### Features

* **core:** Support bidirectional communication between specific mains and specific workers ([#10377](https://github.com/n8n-io/n8n/issues/10377)) ([d0fc9de](https://github.com/n8n-io/n8n/commit/d0fc9dee0e17211c1ed130b19286e9573c9ebfbd))
* **Facebook Graph API Node:** Update node to support API v18 - v20 ([#10419](https://github.com/n8n-io/n8n/issues/10419)) ([e7ee10f](https://github.com/n8n-io/n8n/commit/e7ee10f243663d899d32e61bc6264b4df444e2af))



# [1.55.0](https://github.com/n8n-io/n8n/compare/n8n@1.54.0...n8n@1.55.0) (2024-08-14)


### Bug Fixes

* Add better error handling for chat errors ([#10408](https://github.com/n8n-io/n8n/issues/10408)) ([f82b6e4](https://github.com/n8n-io/n8n/commit/f82b6e4ba9bf527b3a4c17872162d9ae124ead0d))
* **AI Agent Node:** Fix issues with some tools not populating ([#10406](https://github.com/n8n-io/n8n/issues/10406)) ([51a1edd](https://github.com/n8n-io/n8n/commit/51a1eddbf00393f3881c340cf37cfcca59566c99))
* **core:** Account for cancelling an execution with no workers available ([#10343](https://github.com/n8n-io/n8n/issues/10343)) ([b044e78](https://github.com/n8n-io/n8n/commit/b044e783e73a499dbd7532a5d489a782d3d021da))
* **core:** Account for owner when filtering by project ID in `GET /workflows` in Public API ([#10379](https://github.com/n8n-io/n8n/issues/10379)) ([5ac65b3](https://github.com/n8n-io/n8n/commit/5ac65b36bcb1351c6233b951f064f60862f790a5))
* **core:** Enforce shutdown timer and sequence on `SIGINT` for main ([#10346](https://github.com/n8n-io/n8n/issues/10346)) ([5255793](https://github.com/n8n-io/n8n/commit/5255793afee5653d8356b8e4d2e1009d5cf36164))
* **core:** Filter out prototype and constructor lookups in expressions ([#10382](https://github.com/n8n-io/n8n/issues/10382)) ([8e7d29a](https://github.com/n8n-io/n8n/commit/8e7d29ad3c4872b1cc147dfcfe9a864ba916692f))
* **core:** Fix duplicate Redis publisher ([#10392](https://github.com/n8n-io/n8n/issues/10392)) ([45813de](https://github.com/n8n-io/n8n/commit/45813debc963096f63cc0aabe82d9d9f853a39d7))
* **core:** Fix worker shutdown errors when active executions ([#10353](https://github.com/n8n-io/n8n/issues/10353)) ([e071b73](https://github.com/n8n-io/n8n/commit/e071b73bab34edd4b3e6aef6497514acc504cdc6))
* **core:** Prevent XSS in user update endpoints ([#10338](https://github.com/n8n-io/n8n/issues/10338)) ([7898498](https://github.com/n8n-io/n8n/commit/78984986a6b4add89df9743b94c113046f1d5ee8))
* **core:** Prevent XSS via static cache dir ([#10339](https://github.com/n8n-io/n8n/issues/10339)) ([4f392b5](https://github.com/n8n-io/n8n/commit/4f392b5e3e0ee166e85a2e060b3ec7fcf145229b))
* **core:** Rate limit MFA activation and verification endpoints ([#10330](https://github.com/n8n-io/n8n/issues/10330)) ([b6c47c0](https://github.com/n8n-io/n8n/commit/b6c47c0e3214878d42980d5c9535df52b3984b3c))
* **editor:** Connect up new project viewer role to the FE ([#9913](https://github.com/n8n-io/n8n/issues/9913)) ([117e2d9](https://github.com/n8n-io/n8n/commit/117e2d968fcc535f32c583ac8f2dc8a84e8cd6bd))
* **editor:** Enable credential sharing between all types of projects ([#10233](https://github.com/n8n-io/n8n/issues/10233)) ([1cf48cc](https://github.com/n8n-io/n8n/commit/1cf48cc3019c1cf27e2f3c9affd18426237e9064))
* **editor:** Fix rendering of SVG icons in public chat on iOS ([#10381](https://github.com/n8n-io/n8n/issues/10381)) ([7ab3811](https://github.com/n8n-io/n8n/commit/7ab38114dbf3881afba39287a061446ec4bf0431))
* **editor:** Fixing XSS vulnerability in toast messages ([#10329](https://github.com/n8n-io/n8n/issues/10329)) ([38bdd9f](https://github.com/n8n-io/n8n/commit/38bdd9f5d0d9ca06fab1a7e1a3e7a4a648a6a89a))
* **editor:** Revert change that hid swagger docs in the ui ([#10350](https://github.com/n8n-io/n8n/issues/10350)) ([bae49d3](https://github.com/n8n-io/n8n/commit/bae49d3198d4bcc27e7996cd4f7be3132becc98e))
* **n8n Form Trigger Node:** Fix issue preventing v1 node from working ([#10364](https://github.com/n8n-io/n8n/issues/10364)) ([9b647a9](https://github.com/n8n-io/n8n/commit/9b647a9837434e8b75e3ad754ff5136bb5ac760d))
* Require mfa code for password change if its enabled ([#10341](https://github.com/n8n-io/n8n/issues/10341)) ([9d7caac](https://github.com/n8n-io/n8n/commit/9d7caacc699f10962783393925a980ec6f1ca975))
* Require mfa code to disable mfa ([#10345](https://github.com/n8n-io/n8n/issues/10345)) ([3384f52](https://github.com/n8n-io/n8n/commit/3384f52a35b835ba1d8633dc94bab0ad6e7023b3))


### Features

* Add Ask assistant behind feature flag ([#9995](https://github.com/n8n-io/n8n/issues/9995)) ([5ed2a77](https://github.com/n8n-io/n8n/commit/5ed2a77740db1f02b27c571f4dfdfa206ebdb19c))
* **AI Transform Node:** New node ([#10405](https://github.com/n8n-io/n8n/issues/10405)) ([4d222ac](https://github.com/n8n-io/n8n/commit/4d222ac19d943b69fd9f87abe5e5c5f5141eed8d))
* **AI Transform Node:** New node ([#9990](https://github.com/n8n-io/n8n/issues/9990)) ([0de9d56](https://github.com/n8n-io/n8n/commit/0de9d56619ed1c055407353046b8a9ebe78da527))
* **core:** Allow overriding npm registry for community packages ([#10325](https://github.com/n8n-io/n8n/issues/10325)) ([33a2703](https://github.com/n8n-io/n8n/commit/33a2703429d9eaa41f72d2e7d2da5be60b6c620f))
* **editor:** Add schema view to expression modal ([#9976](https://github.com/n8n-io/n8n/issues/9976)) ([71b6c67](https://github.com/n8n-io/n8n/commit/71b6c671797024d7b516352fa9b7ecda101ce3b2))
* **MySQL Node:** Return decimal types as numbers ([#10313](https://github.com/n8n-io/n8n/issues/10313)) ([f744d7c](https://github.com/n8n-io/n8n/commit/f744d7c100be68669d9a3efd0033dd371a3cfaf7))
* **Okta Node:** Add Okta Node ([#10278](https://github.com/n8n-io/n8n/issues/10278)) ([5cac0f3](https://github.com/n8n-io/n8n/commit/5cac0f339d649cfe5857d33738210cbc1599370b))



# [1.54.0](https://github.com/n8n-io/n8n/compare/n8n@1.53.0...n8n@1.54.0) (2024-08-07)


### Bug Fixes

* **core:** Ensure OAuth token data is not stubbed in source control ([#10302](https://github.com/n8n-io/n8n/issues/10302)) ([98115e9](https://github.com/n8n-io/n8n/commit/98115e95df8289a8ec400a570a7f256382f8e286))
* **core:** Fix expressions in webhook nodes(Form, Webhook) to access previous node's data ([#10247](https://github.com/n8n-io/n8n/issues/10247)) ([88a1701](https://github.com/n8n-io/n8n/commit/88a170176a3447e7f847e9cf145aeb867b1c5fcf))
* **core:** Fix user telemetry bugs ([#10293](https://github.com/n8n-io/n8n/issues/10293)) ([42a0b59](https://github.com/n8n-io/n8n/commit/42a0b594d6ea2527c55a2aa9976c904cf70ecf92))
* **core:** Make execution and its data creation atomic ([#10276](https://github.com/n8n-io/n8n/issues/10276)) ([ae50bb9](https://github.com/n8n-io/n8n/commit/ae50bb95a8e5bf1cdbf9483da54b84094b82e260))
* **core:** Make OAuth1/OAuth2 callback not require auth ([#10263](https://github.com/n8n-io/n8n/issues/10263)) ([a8e2774](https://github.com/n8n-io/n8n/commit/a8e2774f5382e202556b5506c7788265786aa973))
* **core:** Revert transactions until we remove the legacy sqlite driver  ([#10299](https://github.com/n8n-io/n8n/issues/10299)) ([1eba7c3](https://github.com/n8n-io/n8n/commit/1eba7c3c763ac5b6b28c1c6fc43fc8c215249292))
* **core:** Surface enterprise trial error message ([#10267](https://github.com/n8n-io/n8n/issues/10267)) ([432ac1d](https://github.com/n8n-io/n8n/commit/432ac1da59e173ce4c0f2abbc416743d9953ba70))
* **core:** Upgrade tournament to address some XSS vulnerabilities ([#10277](https://github.com/n8n-io/n8n/issues/10277)) ([43ae159](https://github.com/n8n-io/n8n/commit/43ae159ea40c574f8e41bdfd221ab2bf3268eee7))
* **core:** VM2 sandbox should not throw on `new Promise` ([#10298](https://github.com/n8n-io/n8n/issues/10298)) ([7e95f9e](https://github.com/n8n-io/n8n/commit/7e95f9e2e40a99871f1b6abcdacb39ac5f857332))
* **core:** Webhook and form baseUrl missing ([#10290](https://github.com/n8n-io/n8n/issues/10290)) ([8131d66](https://github.com/n8n-io/n8n/commit/8131d66f8ca1b1da00597a12859ee4372148a0c9))
* **editor:** Enable moving resources only if team projects are available by the license ([#10271](https://github.com/n8n-io/n8n/issues/10271)) ([42ba884](https://github.com/n8n-io/n8n/commit/42ba8841c401126c77158a53dc8fcbb45dfce8fd))
* **editor:** Fix execution retry button ([#10275](https://github.com/n8n-io/n8n/issues/10275)) ([55f2ffe](https://github.com/n8n-io/n8n/commit/55f2ffe256c91a028cee95c3bbb37a093a1c0f81))
* **editor:** Update design system Avatar component to show initials also when only firstName or lastName is given ([#10308](https://github.com/n8n-io/n8n/issues/10308)) ([46bbf09](https://github.com/n8n-io/n8n/commit/46bbf09beacad12472d91786b91d845fe2afb26d))
* **editor:** Update tags filter/editor to not show non existing tag as a selectable option ([#10297](https://github.com/n8n-io/n8n/issues/10297)) ([557a76e](https://github.com/n8n-io/n8n/commit/557a76ec2326de72fb7a8b46fc4353f8fd9b591d))
* **Invoice Ninja Node:** Fix payment types ([#10196](https://github.com/n8n-io/n8n/issues/10196)) ([c5acbb7](https://github.com/n8n-io/n8n/commit/c5acbb7ec0d24ec9b30c221fa3b2fb615fb9ec7f))
* Loop node no input data shown ([#10224](https://github.com/n8n-io/n8n/issues/10224)) ([c8ee852](https://github.com/n8n-io/n8n/commit/c8ee852159207be0cfe2c3e0ee8e7b29d838aa35))


### Features

* **core:** Allow filtering executions and users by project in Public API  ([#10250](https://github.com/n8n-io/n8n/issues/10250)) ([7056e50](https://github.com/n8n-io/n8n/commit/7056e50b006bda665f64ce6234c5c1967891c415))
* **core:** Allow transferring credentials in Public API ([#10259](https://github.com/n8n-io/n8n/issues/10259)) ([07d7b24](https://github.com/n8n-io/n8n/commit/07d7b247f02a9d7185beca7817deb779a3d665dd))
* **core:** Show sub-node error on the logs pane. Open logs pane on sub-node error ([#10248](https://github.com/n8n-io/n8n/issues/10248)) ([57d1c9a](https://github.com/n8n-io/n8n/commit/57d1c9a99e97308f2f1b8ae05ac3861a835e8e5a))
* **core:** Support community packages in scaling-mode  ([#10228](https://github.com/n8n-io/n8n/issues/10228)) ([88086a4](https://github.com/n8n-io/n8n/commit/88086a41ff5b804b35aa9d9503dc2d48836fe4ec))
* **core:** Support create, delete, edit role for users in Public API ([#10279](https://github.com/n8n-io/n8n/issues/10279)) ([84efbd9](https://github.com/n8n-io/n8n/commit/84efbd9b9c51f536b21a4f969ab607d277bef692))
* **core:** Support create, read, update, delete projects in Public API ([#10269](https://github.com/n8n-io/n8n/issues/10269)) ([489ce10](https://github.com/n8n-io/n8n/commit/489ce100634c3af678fb300e9a39d273042542e6))
* **editor:** Auto-add LLM chain for new LLM nodes on empty canvas ([#10245](https://github.com/n8n-io/n8n/issues/10245)) ([06419d9](https://github.com/n8n-io/n8n/commit/06419d9483ae916e79aace6d8c17e265b419b15d))
* **Elasticsearch Node:** Add bulk operations for Elasticsearch ([#9940](https://github.com/n8n-io/n8n/issues/9940)) ([bf8f848](https://github.com/n8n-io/n8n/commit/bf8f848645dfd31527713a55bd1fc93865327017))
* **Lemlist Trigger Node:** Update Trigger events ([#10311](https://github.com/n8n-io/n8n/issues/10311)) ([15f10ec](https://github.com/n8n-io/n8n/commit/15f10ec325cb5eda0f952bed3a5f171dd91bc639))
* **MongoDB Node:** Add projection to query options on Find ([#9972](https://github.com/n8n-io/n8n/issues/9972)) ([0a84e0d](https://github.com/n8n-io/n8n/commit/0a84e0d8b047669f5cf023c21383d01c929c5b4f))
* **Postgres Chat Memory, Redis Chat Memory, Xata:** Add support for context window length ([#10203](https://github.com/n8n-io/n8n/issues/10203)) ([e3edeaa](https://github.com/n8n-io/n8n/commit/e3edeaa03526f041d15d1099ea91869e38a0decc))
* **Stripe Trigger Node:** Add Stripe webhook descriptions based on the workflow ID and name ([#9956](https://github.com/n8n-io/n8n/issues/9956)) ([3433465](https://github.com/n8n-io/n8n/commit/34334651e0e6874736a437a894176bed4590e5a7))
* **Webflow Node:** Update to use the v2 API ([#9996](https://github.com/n8n-io/n8n/issues/9996)) ([6d8323f](https://github.com/n8n-io/n8n/commit/6d8323fadea8af04483eb1a873df0cf3ccc2a891))



# [1.53.0](https://github.com/n8n-io/n8n/compare/n8n@1.52.0...n8n@1.53.0) (2024-07-31)


### Bug Fixes

* Better error message when calling data transformation functions on a null value ([#10210](https://github.com/n8n-io/n8n/issues/10210)) ([1718125](https://github.com/n8n-io/n8n/commit/1718125c6d8589cf24dc8d34f6808dd6f1802691))
* **core:** Fix missing successful items on continueErrorOutput with multiple outputs ([#10218](https://github.com/n8n-io/n8n/issues/10218)) ([1a7713e](https://github.com/n8n-io/n8n/commit/1a7713ef263680da43f08b6c8a15aee7a0341493))
* **core:** Flush instance stopped event immediately ([#10238](https://github.com/n8n-io/n8n/issues/10238)) ([d6770b5](https://github.com/n8n-io/n8n/commit/d6770b5fcaec6438d677b918aaeb1669ad7424c2))
* **core:** Restore log event `n8n.workflow.failed` ([#10253](https://github.com/n8n-io/n8n/issues/10253)) ([3e96b29](https://github.com/n8n-io/n8n/commit/3e96b293329525c9d4b2fcef87b3803e458c8e7f))
* **core:** Upgrade @n8n/vm2 to address CVE‑2023‑37466 ([#10265](https://github.com/n8n-io/n8n/issues/10265)) ([2a09a03](https://github.com/n8n-io/n8n/commit/2a09a036d2e916acff7ee50904f1d011a93758e1))
* **editor:** Defer `User saved credentials` telemetry event for OAuth credentials ([#10215](https://github.com/n8n-io/n8n/issues/10215)) ([40a5226](https://github.com/n8n-io/n8n/commit/40a5226e24448a4428143e69d80ebc78238365a1))
* **editor:** Fix custom API call notice ([#10227](https://github.com/n8n-io/n8n/issues/10227)) ([5b47c8b](https://github.com/n8n-io/n8n/commit/5b47c8b57b25528cd2d6f97bc6d98707d47f35bc))
* **editor:** Fix issue with existing credential not opening in HTTP agent tool ([#10167](https://github.com/n8n-io/n8n/issues/10167)) ([906b4c3](https://github.com/n8n-io/n8n/commit/906b4c3c7b2919111cf23eaa12b3c4d507969179))
* **editor:** Fix parameter input glitch when there was an error loading remote options ([#10209](https://github.com/n8n-io/n8n/issues/10209)) ([c0e3743](https://github.com/n8n-io/n8n/commit/c0e37439a87105a0e66c8ebced42c06dab30dc5e))
* **editor:** Fix workflow execution list scrolling after filter change ([#10226](https://github.com/n8n-io/n8n/issues/10226)) ([7e64358](https://github.com/n8n-io/n8n/commit/7e643589c67adc0218216ec4b89a95f0edfedbee))
* **Google BigQuery Node:** Send timeoutMs in query, pagination support ([#10205](https://github.com/n8n-io/n8n/issues/10205)) ([f5722e8](https://github.com/n8n-io/n8n/commit/f5722e8823ccd2bc2b5f43ba3c849797d5690a93))
* **Google Sheets Node:** Add column names row if sheet is empty ([#10200](https://github.com/n8n-io/n8n/issues/10200)) ([82eba9f](https://github.com/n8n-io/n8n/commit/82eba9fc5ff49b8e2a9db93c10b253fb67a8c644))
* **Google Sheets Node:** Do not insert row_number as a new column, do not checkForSchemaChanges in update operation ([#10201](https://github.com/n8n-io/n8n/issues/10201)) ([5136d10](https://github.com/n8n-io/n8n/commit/5136d10ca3492f92af67d4a1d4abc774419580cc))
* **Google Sheets Node:** Fix Google Sheet URL regex ([#10195](https://github.com/n8n-io/n8n/issues/10195)) ([e6fd996](https://github.com/n8n-io/n8n/commit/e6fd996973d4f40facf0ebf1eea3cc26acd0603d))
* **HTTP Request Node:** Resolve max pages expression ([#10192](https://github.com/n8n-io/n8n/issues/10192)) ([bfc8e1b](https://github.com/n8n-io/n8n/commit/bfc8e1b56f7714e1f52aae747d58d686b86e60f0))
* **LinkedIn Node:** Fix issue with some characters cutting off posts early ([#10185](https://github.com/n8n-io/n8n/issues/10185)) ([361b5e7](https://github.com/n8n-io/n8n/commit/361b5e7c37ba49b68dcf5b8122621aad4d8d96e0))
* **Postgres Node:** Expressions in query parameters for Postgres executeQuery operation ([#10217](https://github.com/n8n-io/n8n/issues/10217)) ([519fc4d](https://github.com/n8n-io/n8n/commit/519fc4d75325a80b84cc4dcacf52d6f4c02e3a44))
* **Postgres Node:** Option to treat query parameters enclosed in single quotas as text ([#10214](https://github.com/n8n-io/n8n/issues/10214)) ([00ec253](https://github.com/n8n-io/n8n/commit/00ec2533374d3def465efee718592fc4001d5602))
* **Read/Write Files from Disk Node:** Notice update in file selector, replace backslashes with forward slashes if windows path ([#10186](https://github.com/n8n-io/n8n/issues/10186)) ([3eac673](https://github.com/n8n-io/n8n/commit/3eac673b17986c5c74bd2adb5ad589ba0ca55319))
* **Text Classifier Node:** Use proper documentation URL and respect continueOnFail ([#10216](https://github.com/n8n-io/n8n/issues/10216)) ([452f52c](https://github.com/n8n-io/n8n/commit/452f52c124017e002e86c547ba42b1633b14beed))
* **Trello Node:** Use body for POST requests ([#10189](https://github.com/n8n-io/n8n/issues/10189)) ([7775d50](https://github.com/n8n-io/n8n/commit/7775d5059b7f69d9af22e7ad7d12c6cf9092a4e5))
* **Wait Node:** Authentication fix ([#10236](https://github.com/n8n-io/n8n/issues/10236)) ([f87854f](https://github.com/n8n-io/n8n/commit/f87854f8db360b7b870583753fcfb4af95adab8c))


### Features

* **Calendly Trigger Node:** Add OAuth Credentials Support ([#10251](https://github.com/n8n-io/n8n/issues/10251)) ([326c983](https://github.com/n8n-io/n8n/commit/326c983915a2c382e32398358e7dcadd022c0b77))
* **core:** Allow filtering workflows by project and transferring workflows in Public API ([#10231](https://github.com/n8n-io/n8n/issues/10231)) ([d719899](https://github.com/n8n-io/n8n/commit/d719899223907b20a17883a35e4ef637a3453532))
* **editor:** Show new executions as `Queued` in the UI, until they actually start ([#10204](https://github.com/n8n-io/n8n/issues/10204)) ([44728d7](https://github.com/n8n-io/n8n/commit/44728d72423f5549dda09589f4a618ebd80899cb))
* **HTTP Request Node:** Add option to disable lowercase headers ([#10154](https://github.com/n8n-io/n8n/issues/10154)) ([5aba69b](https://github.com/n8n-io/n8n/commit/5aba69bcf4d232d9860f3cd9fe57cb8839a2f96f))
* **Information Extractor Node:** Add new simplified AI-node for information extraction ([#10149](https://github.com/n8n-io/n8n/issues/10149)) ([3d235b0](https://github.com/n8n-io/n8n/commit/3d235b0b2df756df35ac60e3dcd87ad183a07167))
* Introduce Google Cloud Platform as external secrets provider  ([#10146](https://github.com/n8n-io/n8n/issues/10146)) ([3ccb9df](https://github.com/n8n-io/n8n/commit/3ccb9df2f902e46f8cbb9c46c0727f29d752a773))
* **n8n Form Trigger Node:** Improvements ([#10092](https://github.com/n8n-io/n8n/issues/10092)) ([711b667](https://github.com/n8n-io/n8n/commit/711b667ebefe55740e5eb39f1f0f24ceee10e7b0))
* Recovery option for jsonParse helper ([#10182](https://github.com/n8n-io/n8n/issues/10182)) ([d165b33](https://github.com/n8n-io/n8n/commit/d165b33ceac4d24d0fc290bffe63b5f551204e38))
* **Sentiment Analysis Node:** Implement Sentiment Analysis node ([#10184](https://github.com/n8n-io/n8n/issues/10184)) ([8ef0a0c](https://github.com/n8n-io/n8n/commit/8ef0a0c58ac2a84aad649ccbe72aa907d005cc44))
* **Shopify Node:** Update Shopify API version ([#10155](https://github.com/n8n-io/n8n/issues/10155)) ([e2ee915](https://github.com/n8n-io/n8n/commit/e2ee91569a382bfbf787cf45204c72c821a860a0))
* Support create, read, delete variables in Public API ([#10241](https://github.com/n8n-io/n8n/issues/10241)) ([af695eb](https://github.com/n8n-io/n8n/commit/af695ebf934526d926ea87fe87df61aa73d70979))



# [1.52.0](https://github.com/n8n-io/n8n/compare/n8n@1.51.0...n8n@1.52.0) (2024-07-24)


### Bug Fixes

* **core:** Fix handling of common events for relays ([#10135](https://github.com/n8n-io/n8n/issues/10135)) ([d2a3a4a](https://github.com/n8n-io/n8n/commit/d2a3a4a080cdcc04f50fa33fd81d361efce3f709))
* **core:** Fix SSH Tunnels when using private key ([#10148](https://github.com/n8n-io/n8n/issues/10148)) ([a96db34](https://github.com/n8n-io/n8n/commit/a96db344e54658787426d967dfa299c7a6dd14e7))
* **core:** Metadata inserts using existing IDs and failing with postgres ([#10108](https://github.com/n8n-io/n8n/issues/10108)) ([4547a49](https://github.com/n8n-io/n8n/commit/4547a49db15a20f5f147e859b6c2c01f60f9565c))
* **core:** Respect prefix for all Prometheus metrics ([#10130](https://github.com/n8n-io/n8n/issues/10130)) ([b1816db](https://github.com/n8n-io/n8n/commit/b1816db449ed451443f353b69166b7ca700ba51e))
* **core:** Support branches containing slashes in source control ([#10109](https://github.com/n8n-io/n8n/issues/10109)) ([03a833d](https://github.com/n8n-io/n8n/commit/03a833db51a25dda6cf0d8494f06c6704f6f3c7f))
* **core:** Support execution recovery when saving execution progress ([#10104](https://github.com/n8n-io/n8n/issues/10104)) ([d887c82](https://github.com/n8n-io/n8n/commit/d887c82d808a79babc726fc789cc014194ae2ac6))
* **editor:** Allow `$secrets` to resolve on credentials ([#10093](https://github.com/n8n-io/n8n/issues/10093)) ([bf57f38](https://github.com/n8n-io/n8n/commit/bf57f38d1c417ba8b20144934c8e97a75c1f51cc))
* **editor:** Fix saving and connecting on LDAP setup form ([#10163](https://github.com/n8n-io/n8n/issues/10163)) ([30784fb](https://github.com/n8n-io/n8n/commit/30784fb76cec790a782fae40973a956a8d81c0b2))
* **editor:** Fix updating/uninstalling community nodes ([#10138](https://github.com/n8n-io/n8n/issues/10138)) ([de015ff](https://github.com/n8n-io/n8n/commit/de015ff2978a5ee3345449626025c6d0793b6f5a))
* **editor:** Remove "move" action from workflow and credential on community plan ([#10057](https://github.com/n8n-io/n8n/issues/10057)) ([5a9a271](https://github.com/n8n-io/n8n/commit/5a9a2713b499cc7dcddb500a54e24bbf7145b504))
* **editor:** UX Improvements to RBAC feature set ([#9683](https://github.com/n8n-io/n8n/issues/9683)) ([028a8a2](https://github.com/n8n-io/n8n/commit/028a8a2c754e4f6d6a5f0918a656eb4554eb869f))
* **HelpScout Node:** Fix issue with thread types not working correctly ([#10084](https://github.com/n8n-io/n8n/issues/10084)) ([68d3beb](https://github.com/n8n-io/n8n/commit/68d3bebfeebea9054bbbaebac31c2e3fa34336bb))
* **MQTT Node:** Node hangs forever on failed connection ([#10048](https://github.com/n8n-io/n8n/issues/10048)) ([76c2906](https://github.com/n8n-io/n8n/commit/76c290655de7d4e626725a05fd991a0858cca0d7))
* **n8n Form Trigger Node:** Execution from canvas ([#10132](https://github.com/n8n-io/n8n/issues/10132)) ([b07c5e2](https://github.com/n8n-io/n8n/commit/b07c5e201165165c4e91ddd19b6fa79703ba2a9c))
* **Notion Node:** Fix issue preventing some database page urls from working ([#10070](https://github.com/n8n-io/n8n/issues/10070)) ([7848c19](https://github.com/n8n-io/n8n/commit/7848c19f543d5f5f62b89cc5644639c6afdb8fa6))
* **RabbitMQ Node:** Fix issue with arguments not being sent ([#9397](https://github.com/n8n-io/n8n/issues/9397)) ([1c666e6](https://github.com/n8n-io/n8n/commit/1c666e6e7c2be2e2d0dcc528870fddfa8b02318b))


### Features

* **editor:** Split Tools and Models into sub-sections ([#10159](https://github.com/n8n-io/n8n/issues/10159)) ([3846eb9](https://github.com/n8n-io/n8n/commit/3846eb967afd77dba6f037e8185ed94494454d5a))
* Introduce Azure Key Vault as external secrets provider ([#10054](https://github.com/n8n-io/n8n/issues/10054)) ([1b6c2d3](https://github.com/n8n-io/n8n/commit/1b6c2d3a37a78ed07ada93be2a57e4b7f7149e58))
* **Pinecone Vector Store Node, Supabase Vector Store Node:** Add update operation to vector store nodes ([#10060](https://github.com/n8n-io/n8n/issues/10060)) ([7e1eeb4](https://github.com/n8n-io/n8n/commit/7e1eeb4c31d3f25ec31baa7390b11a7e3280ce01))
* **Send Email Node:** Smtp credential improvements ([#10147](https://github.com/n8n-io/n8n/issues/10147)) ([dc13ceb](https://github.com/n8n-io/n8n/commit/dc13ceb41649eab42ef073247f3b52c040826e98))



# [1.51.0](https://github.com/n8n-io/n8n/compare/n8n@1.50.0...n8n@1.51.0) (2024-07-17)


### Bug Fixes

* **AMQP Sender Node:** Node hangs forever on disconnect ([#10026](https://github.com/n8n-io/n8n/issues/10026)) ([27410ab](https://github.com/n8n-io/n8n/commit/27410ab2af87573045f38e14e7e20bedd3b0365d))
* **AMQP Trigger Node:** Manual execution updated error reduced wait time ([#10035](https://github.com/n8n-io/n8n/issues/10035)) ([f78f4ea](https://github.com/n8n-io/n8n/commit/f78f4ea3492560bc7056023fd0276990f3ac9b00))
* **AWS Comprehend Node:** Add paired item support ([#10015](https://github.com/n8n-io/n8n/issues/10015)) ([470d496](https://github.com/n8n-io/n8n/commit/470d4966c67a3e4155d59e6fadab467b73134ec4))
* **core:** Ensure executions cannot resume if already running ([#10014](https://github.com/n8n-io/n8n/issues/10014)) ([d651be4](https://github.com/n8n-io/n8n/commit/d651be4e01a869a6f7d70e691e0f5e244f59490e))
* **core:** Redact `csrfSecret` when returning oauth credentials to the frontend ([#10075](https://github.com/n8n-io/n8n/issues/10075)) ([48f047e](https://github.com/n8n-io/n8n/commit/48f047ee2ecbfbd364151816df5fc21e09ca72a6))
* **core:** Stopping an execution should reject any response promises ([#9992](https://github.com/n8n-io/n8n/issues/9992)) ([36b314d](https://github.com/n8n-io/n8n/commit/36b314d0311ef84f275efbc20997c6a77db81b31))
* **editor:** Ensure all static assets are accessible from the server ([#10062](https://github.com/n8n-io/n8n/issues/10062)) ([3bde845](https://github.com/n8n-io/n8n/commit/3bde8453efa9a4d14404c63bdc061c87843d49d2))
* **editor:** Handle disabled nodes in schema view ([#10052](https://github.com/n8n-io/n8n/issues/10052)) ([ab5688c](https://github.com/n8n-io/n8n/commit/ab5688c582c05afd7d3e0967eda0f5dc73d6d3ed))
* **editor:** Make schema view use the correct output ([#10016](https://github.com/n8n-io/n8n/issues/10016)) ([c29664d](https://github.com/n8n-io/n8n/commit/c29664d68851ec33e4d810fa24aba72bb6cecc86))
* **editor:** Provide autocomplete for nodes, even when intermediate node has not run ([#10036](https://github.com/n8n-io/n8n/issues/10036)) ([46d6edc](https://github.com/n8n-io/n8n/commit/46d6edc2a4edd49ae58c0c60977809554e07f4ee))
* **editor:** Remove push event listeners when migrating away from the canvas ([#10063](https://github.com/n8n-io/n8n/issues/10063)) ([0d12f0a](https://github.com/n8n-io/n8n/commit/0d12f0a6b36aaaae5e1f9fab8ad73feeba9ec5ed))
* **editor:** Use selected input item for autocomplete ([#10019](https://github.com/n8n-io/n8n/issues/10019)) ([1d2b403](https://github.com/n8n-io/n8n/commit/1d2b403644278fa6158272edc4295d4565554e37))
* **Email Trigger (IMAP) Node:** Reconnect not working correctly ([#10064](https://github.com/n8n-io/n8n/issues/10064)) ([68d5d7e](https://github.com/n8n-io/n8n/commit/68d5d7e2e90ede5d021a12304dd665247dde5243))
* Filter component - array contains comparison not correct when ignore case option set to true ([#10012](https://github.com/n8n-io/n8n/issues/10012)) ([4a3b97c](https://github.com/n8n-io/n8n/commit/4a3b97cede531adbf81274c1ec2ce4ee400cb48e))
* **GitHub Node:** File Create operation prevent duplicated base64 encoding ([#10040](https://github.com/n8n-io/n8n/issues/10040)) ([9bcc926](https://github.com/n8n-io/n8n/commit/9bcc926a91d7afab0c2ef6eb57e818ef79e3a8f7))
* **HTTP Request Node:** Respect the original encoding of the incoming response  ([#9869](https://github.com/n8n-io/n8n/issues/9869)) ([2d19aef](https://github.com/n8n-io/n8n/commit/2d19aef54083d97e94e50a1ee58e8525bbf28548))
* HTTP Request tool - allow hyphens in placeholders ([#10037](https://github.com/n8n-io/n8n/issues/10037)) ([8cd9370](https://github.com/n8n-io/n8n/commit/8cd93704bee116eceb0e3bd5fa849c4b314454ec))
* HTTP Request tool - do not error on missing headers  ([#10044](https://github.com/n8n-io/n8n/issues/10044)) ([04b62e0](https://github.com/n8n-io/n8n/commit/04b62e0398eafd923d5f27a3e1c71b925ddb8817))
* **HubSpot Node:** Migrate from v2 owners api ([#10013](https://github.com/n8n-io/n8n/issues/10013)) ([56dd491](https://github.com/n8n-io/n8n/commit/56dd491bcaeab1d11d7874f190eaf20d2e315ca1))
* Number input defaults to 0 not allowing to have arbitrary precision ([#10021](https://github.com/n8n-io/n8n/issues/10021)) ([e4e66ab](https://github.com/n8n-io/n8n/commit/e4e66ab7da5651fede8b3065419ffb393a2fd16d))
* **OpenAI Chat Model Node:** Respect baseURL override for /models ([#10076](https://github.com/n8n-io/n8n/issues/10076)) ([e5dda57](https://github.com/n8n-io/n8n/commit/e5dda5731dfbb50f5aaf2b152f9c5bc89b1d80a6))
* **Telegram Trigger Node:** Fix issue with videos not being downloaded ([#10007](https://github.com/n8n-io/n8n/issues/10007)) ([e84ab35](https://github.com/n8n-io/n8n/commit/e84ab35c4ab0ec47bdbd4343e58c62bbb70f3ec9))
* **Webhook Node:** Binary property option name and description update ([#10043](https://github.com/n8n-io/n8n/issues/10043)) ([9302e33](https://github.com/n8n-io/n8n/commit/9302e33d558564bb5ba172eaeb8c300693b87286))


### Features

* **Asana Node:** Add support for project privacy settings ([#10027](https://github.com/n8n-io/n8n/issues/10027)) ([429481c](https://github.com/n8n-io/n8n/commit/429481c5c4b7f448739a561596873038185ba467))
* Better error when calling expression function on input that is undefined or null ([#10009](https://github.com/n8n-io/n8n/issues/10009)) ([519e57b](https://github.com/n8n-io/n8n/commit/519e57bda5115149357fb2b1c2270e481ea09e38))
* **editor:** Make expression autocomplete search case-insensitive ([#10017](https://github.com/n8n-io/n8n/issues/10017)) ([cde6fe9](https://github.com/n8n-io/n8n/commit/cde6fe90e5c8a9c5983e27f0d82599425fba915b))
* **editor:** Tweak node creator search logic for AI sub-nodes ([#10025](https://github.com/n8n-io/n8n/issues/10025)) ([7db1656](https://github.com/n8n-io/n8n/commit/7db16561dc890849e2d5742bb73f9d5b8e79e37d))
* **Google Vertex Chat Model Node:** Add support for Google Vertex AI Chat models ([#9970](https://github.com/n8n-io/n8n/issues/9970)) ([071130a](https://github.com/n8n-io/n8n/commit/071130a2dc0b450eb6ce6d39fe28cfeefd05633c))
* **Postgres Chat Memory Node:** Implement Postgres Chat Memory node ([#10071](https://github.com/n8n-io/n8n/issues/10071)) ([9cbbb63](https://github.com/n8n-io/n8n/commit/9cbbb6335df0d36f66f22c18041d12f14dc59b32))
* **Text Classifier Node:** Add Text Classifier Node ([#9997](https://github.com/n8n-io/n8n/issues/9997)) ([28ca7d6](https://github.com/n8n-io/n8n/commit/28ca7d6a2dd818c8795acda6ddf7329b8621d9de))



# [1.50.0](https://github.com/n8n-io/n8n/compare/n8n@1.49.0...n8n@1.50.0) (2024-07-10)


### Bug Fixes

* **core:** Aborting manual trigger tests should call `closeFunction` ([#9980](https://github.com/n8n-io/n8n/issues/9980)) ([6107798](https://github.com/n8n-io/n8n/commit/61077985163037ed3c6a8e9e7476cd6c525ff5f2))
* **core:** Allow owner and admin to edit nodes with credentials that haven't been shared with them explicitly ([#9922](https://github.com/n8n-io/n8n/issues/9922)) ([0f49598](https://github.com/n8n-io/n8n/commit/0f495986f89b60ec9bb86801f9779ee9aa87ccfb))
* **core:** Clear active execution on cancellation in scaling mode ([#9979](https://github.com/n8n-io/n8n/issues/9979)) ([7e972c7](https://github.com/n8n-io/n8n/commit/7e972c78afaf950effec17d8eee16cbf86101d03))
* **core:** Disconnect Redis after pausing queue during worker shutdown ([#9928](https://github.com/n8n-io/n8n/issues/9928)) ([c82579b](https://github.com/n8n-io/n8n/commit/c82579bf760cc4b5a2670b14e4e48fc37e2e2263))
* **core:** Don't execute 'workflowExecuteBefore' hook on execution continuations ([#9905](https://github.com/n8n-io/n8n/issues/9905)) ([adb8315](https://github.com/n8n-io/n8n/commit/adb83155ca9478a548e6fe926735d5872de10fea))
* **core:** Prevent multiple values in the execution metadata for the same key and executionId ([#9953](https://github.com/n8n-io/n8n/issues/9953)) ([2e6b03b](https://github.com/n8n-io/n8n/commit/2e6b03b2cb471aefa8104b7b80cf12e64f16e4fb))
* **Google Sheets Node:** Append fails if cells have some default values added by data validation rules ([#9950](https://github.com/n8n-io/n8n/issues/9950)) ([d1821eb](https://github.com/n8n-io/n8n/commit/d1821eba9221eb243b62ad561193102b24dd05a5))
* **Invoice Ninja Node:** Fix assigning an invoice to a payment ([#9590](https://github.com/n8n-io/n8n/issues/9590)) ([7a3c127](https://github.com/n8n-io/n8n/commit/7a3c127b2cbea01f9a21c8d517d1dc919bc8121f))
* **Invoice Ninja Node:** Fix emailing and marking invoice as paid / sent ([#9589](https://github.com/n8n-io/n8n/issues/9589)) ([908ddd8](https://github.com/n8n-io/n8n/commit/908ddd8a24e8a858d9c1eddf2f727234e66a62f7))


### Features

* **Chat Trigger Node:** Add support for file uploads & harmonize public and development chat  ([#9802](https://github.com/n8n-io/n8n/issues/9802)) ([df78315](https://github.com/n8n-io/n8n/commit/df783151b86e2db3e325d3b9d85f4abb71d3d246))
* **Google Cloud Firestore Node:** Add support for service account and document creation with id ([#9713](https://github.com/n8n-io/n8n/issues/9713)) ([cb1bbf5](https://github.com/n8n-io/n8n/commit/cb1bbf5fd395ec4855ac21d851b180c8526b698a))
* **Orbit Node:** Deprecate Orbit nicely ([#9962](https://github.com/n8n-io/n8n/issues/9962)) ([9577d9c](https://github.com/n8n-io/n8n/commit/9577d9c847b56d9907d2bbe9ec85127bb8f67cfa))
* Qdrant Vector Store search filter ([#9900](https://github.com/n8n-io/n8n/issues/9900)) ([fbe4bca](https://github.com/n8n-io/n8n/commit/fbe4bca634e8e03c9455843e1a1f89706d1557d2))
* **Splunk Node:** Overhaul ([#9813](https://github.com/n8n-io/n8n/issues/9813)) ([e5c3247](https://github.com/n8n-io/n8n/commit/e5c324753fb41752f9722d61c5d336d6e5c67cca))
* **Telegram Node:** Add support to Keyboard Button Mini Apps ([#9511](https://github.com/n8n-io/n8n/issues/9511)) ([3a17943](https://github.com/n8n-io/n8n/commit/3a179439c7586189b8264131fd16da9d14f074b6))



# [1.49.0](https://github.com/n8n-io/n8n/compare/n8n@1.48.0...n8n@1.49.0) (2024-07-03)


### Bug Fixes

* **core:** Add a WebCrypto Polyfill for older versions of Node.js 18 ([#9894](https://github.com/n8n-io/n8n/issues/9894)) ([59c8bf1](https://github.com/n8n-io/n8n/commit/59c8bf1c44057b3f798645a22ad16362401ebeed))
* **core:** Don't allow using credentials that are not part of the same project ([#9916](https://github.com/n8n-io/n8n/issues/9916)) ([ab2a548](https://github.com/n8n-io/n8n/commit/ab2a5488560a814fc72c0c5cd71e5f62f05cd235))
* **core:** Filter out certain executions from crash recovery ([#9904](https://github.com/n8n-io/n8n/issues/9904)) ([7044d1c](https://github.com/n8n-io/n8n/commit/7044d1ca2841b6d87ae929072bb94dda82909795))
* **core:** Fix AddActivatedAtUserSetting migration on MariaDB ([#9910](https://github.com/n8n-io/n8n/issues/9910)) ([db29e84](https://github.com/n8n-io/n8n/commit/db29e84666b814fd4710dc3ade6e53304216fad5))
* **core:** Fix execution cancellation in scaling mode ([#9841](https://github.com/n8n-io/n8n/issues/9841)) ([e613de2](https://github.com/n8n-io/n8n/commit/e613de28ca2db23746b586e0a0b33f1c1ee1abe5))
* **core:** Fix worker logs relay ([#9919](https://github.com/n8n-io/n8n/issues/9919)) ([7c53433](https://github.com/n8n-io/n8n/commit/7c5343319144ce3524b14018eef77eace221b608))
* **core:** Throw on adding execution without execution data ([#9903](https://github.com/n8n-io/n8n/issues/9903)) ([abb7458](https://github.com/n8n-io/n8n/commit/abb74587db88a56453b269826885df0d01766290))
* **editor:** Don't try to load credentials on the demo route ([#9926](https://github.com/n8n-io/n8n/issues/9926)) ([b80df2a](https://github.com/n8n-io/n8n/commit/b80df2a47ebe4450862e200c9cf47f6e94012c91))
* **editor:** Enable expression preview in SQL node when looking at executions ([#9733](https://github.com/n8n-io/n8n/issues/9733)) ([d9747d5](https://github.com/n8n-io/n8n/commit/d9747d5e9b42d7f379f6f4219b960893b7b153b3))
* **editor:** Fix frontend project roles ([#9901](https://github.com/n8n-io/n8n/issues/9901)) ([f229577](https://github.com/n8n-io/n8n/commit/f2295772094ff936e210f52ebcbc938915d1c129))
* **editor:** Fix new node credential creation via Resource Locator Component ([#9896](https://github.com/n8n-io/n8n/issues/9896)) ([55cbc90](https://github.com/n8n-io/n8n/commit/55cbc900a48c579b712dddfa74e133e1d9c11799))
* **editor:** Fix performance issues related to expressions and pinned data ([#9882](https://github.com/n8n-io/n8n/issues/9882)) ([13d83f2](https://github.com/n8n-io/n8n/commit/13d83f2037d659fccc8889dd994ddd984467d987))
* **editor:** Improve text wrapping in schema view ([#9888](https://github.com/n8n-io/n8n/issues/9888)) ([dc1c5fc](https://github.com/n8n-io/n8n/commit/dc1c5fce8af732c438d2f1698ee08f18d2358a6c))
* **Execute Workflow Node:** Continue on fail behaviour not correctly implemented ([#9890](https://github.com/n8n-io/n8n/issues/9890)) ([16b1a09](https://github.com/n8n-io/n8n/commit/16b1a094b19e5f803a460b99c6062a1175bec153))
* **LinkedIn Node:** Fix issue with legacy credential no longer working ([#9912](https://github.com/n8n-io/n8n/issues/9912)) ([873b7e5](https://github.com/n8n-io/n8n/commit/873b7e59dcea276c9f792570805a6de8ad4607a3))


### Features

* Add Zep Cloud Memory component ([#9657](https://github.com/n8n-io/n8n/issues/9657)) ([41c47a2](https://github.com/n8n-io/n8n/commit/41c47a28a9d4502287ca1bbbb4704f2763288a11))
* **Copper Node:** Update credential to support HTTP Request node ([#9837](https://github.com/n8n-io/n8n/issues/9837)) ([e6ad5a7](https://github.com/n8n-io/n8n/commit/e6ad5a71935a5f82168bf300246ccb3535648b0b))
* **editor:** Add docs sidebar to credential modal ([#9914](https://github.com/n8n-io/n8n/issues/9914)) ([b2f8ea7](https://github.com/n8n-io/n8n/commit/b2f8ea7918d7e10e91db0e04ef5b7ad40a5bdbb5))
* **editor:** Remove Segment ([#9878](https://github.com/n8n-io/n8n/issues/9878)) ([10f7d4b](https://github.com/n8n-io/n8n/commit/10f7d4b5b92013407c9a4eb9edd619d385efe10f))
* **Embeddings Cohere Node:** Add v3 Cohere models ([#9887](https://github.com/n8n-io/n8n/issues/9887)) ([403e19b](https://github.com/n8n-io/n8n/commit/403e19b3e316db81b62eb456b38e7325bf13529c))
* **GitHub Node:** Add support for state reasons when editing an issue ([#9848](https://github.com/n8n-io/n8n/issues/9848)) ([61c20d1](https://github.com/n8n-io/n8n/commit/61c20d1ae3c65b04c767c5b704c4fc4efd356ccf))
* Introduce debug info button ([#9895](https://github.com/n8n-io/n8n/issues/9895)) ([be9a247](https://github.com/n8n-io/n8n/commit/be9a247577ffc28559a23fea2db9b2c598dca036))
* **Merge Node:** Overhaul, v3 ([#9528](https://github.com/n8n-io/n8n/issues/9528)) ([af69c80](https://github.com/n8n-io/n8n/commit/af69c80bf5a22f80979405041210dc77d2682c51))
* **Vector Store Tool Node:** Add Vector Store Tool ([#9865](https://github.com/n8n-io/n8n/issues/9865)) ([df2bc84](https://github.com/n8n-io/n8n/commit/df2bc84d2b3830d31319c108f1b01256de95e774))
* **Zammad Node:** Add reply_to and sender fields to article on ticket creation ([#9911](https://github.com/n8n-io/n8n/issues/9911)) ([957b2d6](https://github.com/n8n-io/n8n/commit/957b2d6108dccd9495291c4764816cc27e112e87))



# [1.48.0](https://github.com/n8n-io/n8n/compare/n8n@1.47.0...n8n@1.48.0) (2024-06-27)


### Bug Fixes

* **core:** Fix init for `AuditEventRelay` ([#9839](https://github.com/n8n-io/n8n/issues/9839)) ([16d3083](https://github.com/n8n-io/n8n/commit/16d3083af7465d0788f25d843e497b4c7d69de92))
* **core:** Fix telemetry for concurrency control ([#9845](https://github.com/n8n-io/n8n/issues/9845)) ([e25682d](https://github.com/n8n-io/n8n/commit/e25682ddad6ee961a1afe5365d7bbad871a20a4c))
* **editor:** Fix initialize authenticated features ([#9867](https://github.com/n8n-io/n8n/issues/9867)) ([4de58dc](https://github.com/n8n-io/n8n/commit/4de58dcbf5f29bf5414414aa4703356f69a29356))
* **editor:** Load credentials for workflow before determining credentials errors ([#9876](https://github.com/n8n-io/n8n/issues/9876)) ([4008c14](https://github.com/n8n-io/n8n/commit/4008c147d76daa6ff6d43f30c9a18bf1cef7e5d5))
* **editor:** Optimizing main sidebar to have more space for Projects ([#9686](https://github.com/n8n-io/n8n/issues/9686)) ([5cdcb61](https://github.com/n8n-io/n8n/commit/5cdcb61f668a6e00829bee25f40cc869376a9cd7))
* **editor:** Properly update workflow info in main header ([#9789](https://github.com/n8n-io/n8n/issues/9789)) ([1ba656e](https://github.com/n8n-io/n8n/commit/1ba656ef4aae97c78162114ad8de533b275db280))
* **editor:** Show error state correctly in options parameter with remote options ([#9836](https://github.com/n8n-io/n8n/issues/9836)) ([5bc58ef](https://github.com/n8n-io/n8n/commit/5bc58efde9c127eef8082b23cf5d8dcd91162cf4))
* **editor:** Use pinned data to resolve expressions in unexecuted nodes ([#9693](https://github.com/n8n-io/n8n/issues/9693)) ([6cb3072](https://github.com/n8n-io/n8n/commit/6cb3072a5db366404f3d16323498371d28582c06))
* Fix missing node logos ([#9844](https://github.com/n8n-io/n8n/issues/9844)) ([1eeaf32](https://github.com/n8n-io/n8n/commit/1eeaf32523c30f000a1bb8f362c478a086ca7928))
* **Zulip Node:** Fix a typo preventing some messages from updating ([#7078](https://github.com/n8n-io/n8n/issues/7078)) ([553b135](https://github.com/n8n-io/n8n/commit/553b135b0b73fa29062d2b6ef28f98c47bcd186b))


### Features

* Add RS client to hooks service ([#9834](https://github.com/n8n-io/n8n/issues/9834)) ([b807e67](https://github.com/n8n-io/n8n/commit/b807e6726f6ac86df9078c25275b6360a4fcee42))
* **Anthropic Chat Model Node:** Add support for Claude 3.5 Sonnet ([#9832](https://github.com/n8n-io/n8n/issues/9832)) ([2ce97be](https://github.com/n8n-io/n8n/commit/2ce97be33e8aa4f3023d486441ccc4860a0e07ca))
* **editor:** Show multiple nodes in input pane schema view ([#9816](https://github.com/n8n-io/n8n/issues/9816)) ([e51de9d](https://github.com/n8n-io/n8n/commit/e51de9d3916e3fcaa05e92dfb8b9b5c722bff33c))



# [1.47.0](https://github.com/n8n-io/n8n/compare/n8n@1.46.0...n8n@1.47.0) (2024-06-20)


### Bug Fixes

* **AI Agent Node:** Exclude tools agent from unsupported node versions ([#9728](https://github.com/n8n-io/n8n/issues/9728)) ([28d1a5d](https://github.com/n8n-io/n8n/commit/28d1a5d00d9f8a3bb2f812bb11d9d31c1cbadb24))
* **Airtable Node:** Make multipleRecordLinks editable in fields ([#9608](https://github.com/n8n-io/n8n/issues/9608)) ([fdde995](https://github.com/n8n-io/n8n/commit/fdde9957c80613a27762eeb54272cc492f499dbf))
* **AWS SES Node:** Fix issue with email aliases not working for sending from or sending to ([#9811](https://github.com/n8n-io/n8n/issues/9811)) ([e1e8a75](https://github.com/n8n-io/n8n/commit/e1e8a7576308cbc0833cdae35d51810f63b98382))
* Changes to workflow staticData erroneously updating updatedAt ([#9790](https://github.com/n8n-io/n8n/issues/9790)) ([adbd0d1](https://github.com/n8n-io/n8n/commit/adbd0d17abcf8d46bdef44ff45cecbc3bb6c8755))
* **core:** Ensure execution recovery skips successful executions ([#9793](https://github.com/n8n-io/n8n/issues/9793)) ([4131408](https://github.com/n8n-io/n8n/commit/4131408e5e28e4f40287c4880a4b5347e3cdc169))
* **core:** Ensure followers do not recover executions from logs ([#9785](https://github.com/n8n-io/n8n/issues/9785)) ([7c358e5](https://github.com/n8n-io/n8n/commit/7c358e5baafa295f826f891266457cc6c61cd6de))
* **core:** Update transactional email links for RBAC ([#9727](https://github.com/n8n-io/n8n/issues/9727)) ([ceb7f07](https://github.com/n8n-io/n8n/commit/ceb7f074eb1b22ebc698fc168f73a0da6a3d9769))
* **core:** Upgrade `ws` to address CVE-2024-37890 ([#9801](https://github.com/n8n-io/n8n/issues/9801)) ([f98c4b8](https://github.com/n8n-io/n8n/commit/f98c4b8ac033133e4897b5d42326b0d21e2e96be))
* **editor:** Active toggle incorrectly displayed as inactive in execution view ([#9778](https://github.com/n8n-io/n8n/issues/9778)) ([551fb6d](https://github.com/n8n-io/n8n/commit/551fb6d7a2e59fe1b93183745962d9eff4741d44))
* **editor:** Add telemetry to resource moving ([#9720](https://github.com/n8n-io/n8n/issues/9720)) ([e84d253](https://github.com/n8n-io/n8n/commit/e84d2538b6f59e424d92b1f622edb7d6cff756e8))
* **editor:** Error dropdown in resource locator disappears when search filter is required ([#9681](https://github.com/n8n-io/n8n/issues/9681)) ([1a3f72b](https://github.com/n8n-io/n8n/commit/1a3f72b751bf82b1f537882d692ccd6cff7c3f94))
* **editor:** Fix node icon in node creator header ([#9782](https://github.com/n8n-io/n8n/issues/9782)) ([b7d356f](https://github.com/n8n-io/n8n/commit/b7d356f49cdd5d9e63e1aeffecb25da0fc906d6a))
* **editor:** Improve touch device detection ([#9675](https://github.com/n8n-io/n8n/issues/9675)) ([3b86f52](https://github.com/n8n-io/n8n/commit/3b86f52b0290c98ce371be90b2aea699efedbc73))
* **editor:** Revert header toggle fix ([#9800](https://github.com/n8n-io/n8n/issues/9800)) ([11fe48b](https://github.com/n8n-io/n8n/commit/11fe48b3dc91375140a53b73093733536e48d4cb))
* **editor:** Use BroadcastChannel instead of window.opener for OAuth callback window ([#9779](https://github.com/n8n-io/n8n/issues/9779)) ([87cb199](https://github.com/n8n-io/n8n/commit/87cb199745ae4ae9d73f3dfdf5c2bd95acfb9c9e))
* **editor:** Use segments/graphemes when creating the compact sidebar entries ([#9776](https://github.com/n8n-io/n8n/issues/9776)) ([be7249f](https://github.com/n8n-io/n8n/commit/be7249f568d922238c1a95c9d182a01b25ac0ddb))
* **Elasticsearch Node:** Fix issue with self signed certificates ([#9805](https://github.com/n8n-io/n8n/issues/9805)) ([77bf166](https://github.com/n8n-io/n8n/commit/77bf16667b4c9a70ce23e88106b6b9da3d9f0e27))
* Fix sending pin data twice causing payload too large errors ([#9710](https://github.com/n8n-io/n8n/issues/9710)) ([6c1a4c8](https://github.com/n8n-io/n8n/commit/6c1a4c8ebfd60c769bba9441ef732b726ab8d9db))
* **Google Sheets Node:** Check for column names changes before upsert, append, update ([#9649](https://github.com/n8n-io/n8n/issues/9649)) ([223488f](https://github.com/n8n-io/n8n/commit/223488f190223596d9ec634dd0ecb3cce1ea442b))
* **Slack Node:** Do not try to parse block if it's already object ([#9643](https://github.com/n8n-io/n8n/issues/9643)) ([8f94dcc](https://github.com/n8n-io/n8n/commit/8f94dcc0e9dee141d3ea922328abd81c0c6d1707))
* When editing nodes only show the credentials in the dropdown that the user is allowed to use in that workflow ([#9718](https://github.com/n8n-io/n8n/issues/9718)) ([2cf4364](https://github.com/n8n-io/n8n/commit/2cf4364ee0d4343e952e9571574a17ef6122b482))


### Features

* Add custom data to public API execution endpoints ([#9705](https://github.com/n8n-io/n8n/issues/9705)) ([a104660](https://github.com/n8n-io/n8n/commit/a1046607bf6b136c9e1047350007901e695cb52f))
* **core:** Expand crash recovery to cover queue mode ([#9676](https://github.com/n8n-io/n8n/issues/9676)) ([c58621a](https://github.com/n8n-io/n8n/commit/c58621ab79181c0b76d4102af6c76adc4ebdc69c))
* **core:** Use WebCrypto to generate all random numbers and strings ([#9786](https://github.com/n8n-io/n8n/issues/9786)) ([65c5609](https://github.com/n8n-io/n8n/commit/65c5609ab51881c223dcbf5ee567dbc83e6dd4e5))
* HTTP request tool ([#9228](https://github.com/n8n-io/n8n/issues/9228)) ([be2635e](https://github.com/n8n-io/n8n/commit/be2635e50e922be6a3f9984d641ac57b78c86874))
* **JWT Node:** Add an option to allow a "kid" (key ID) header claim ([#9797](https://github.com/n8n-io/n8n/issues/9797)) ([15d631c](https://github.com/n8n-io/n8n/commit/15d631c412b3c13c8d996d409a524d1061286cf4))
* **Pipedrive Node:** Add sort field for get all persons ([#8138](https://github.com/n8n-io/n8n/issues/8138)) ([4e89343](https://github.com/n8n-io/n8n/commit/4e893436fb2347859616a583eab2a412b193e392))
* **Set Node:** Preserve binary data by default ([#9668](https://github.com/n8n-io/n8n/issues/9668)) ([d116353](https://github.com/n8n-io/n8n/commit/d1163533a6a262074526a6514789e3d011e3b864))


### Performance Improvements

* **core:** Introduce concurrency control for main mode ([#9453](https://github.com/n8n-io/n8n/issues/9453)) ([7973423](https://github.com/n8n-io/n8n/commit/797342343f5ef560e8333e2ad67b4395bc0aad0a))



# [1.46.0](https://github.com/n8n-io/n8n/compare/n8n@1.45.0...n8n@1.46.0) (2024-06-12)


### Bug Fixes

* **Chat Trigger Node:** Fix public chat container dimensions ([#9664](https://github.com/n8n-io/n8n/issues/9664)) ([3b10c0f](https://github.com/n8n-io/n8n/commit/3b10c0f6aa87969965ed8a4ec339b295d6fe6199))
* **core:** Allow graceful shutdown for main with active executions ([#9661](https://github.com/n8n-io/n8n/issues/9661)) ([4b345be](https://github.com/n8n-io/n8n/commit/4b345bec0326f0fb874afb0f62ec246cca70344f))
* **core:** Fix optional chaining in continue on fail check ([#9667](https://github.com/n8n-io/n8n/issues/9667)) ([6ae6a5e](https://github.com/n8n-io/n8n/commit/6ae6a5ebdf9e8d23ffd2bb4a230665088a2c269b))
* **editor:** Color node connections correctly in execution preview for nodes that have pinned data ([#9669](https://github.com/n8n-io/n8n/issues/9669)) ([ebba7c8](https://github.com/n8n-io/n8n/commit/ebba7c87cdc96b08f8a2075d6f4907f7671dea4b))
* **editor:** Fix node connection showing incorrect item count during … ([#9684](https://github.com/n8n-io/n8n/issues/9684)) ([99b54bb](https://github.com/n8n-io/n8n/commit/99b54bb0296a855f6bbaf1183b8a554dcf072bb7))
* **editor:** Improve dragndrop of input pills with spaces ([#9656](https://github.com/n8n-io/n8n/issues/9656)) ([291d46a](https://github.com/n8n-io/n8n/commit/291d46af155cd5c512f5e7d4597e31d7ea02bc54))
* **editor:** Improve large data warning in input/output panel ([#9671](https://github.com/n8n-io/n8n/issues/9671)) ([4918ac8](https://github.com/n8n-io/n8n/commit/4918ac81dee2ad950ea0088c99b687a5e7e447b4))
* **editor:** Indent on tabs in expression fields ([#9659](https://github.com/n8n-io/n8n/issues/9659)) ([bb7227d](https://github.com/n8n-io/n8n/commit/bb7227d18d574af35871c2d2f2a2d1310932e0ff))
* **editor:** Node background for executing nodes in dark mode ([#9682](https://github.com/n8n-io/n8n/issues/9682)) ([ae00b44](https://github.com/n8n-io/n8n/commit/ae00b446a79e86cf570287c904fd6dde41ddf71a))
* **editor:** Persist tag filter when clicking tag directly in workflows page ([#9709](https://github.com/n8n-io/n8n/issues/9709)) ([0502738](https://github.com/n8n-io/n8n/commit/0502738c0d63d2da5cca4d9e857ce3b4bec2f8c8))
* **editor:** Prevent running workflows using keyboard shortcuts if execution is disabled ([#9644](https://github.com/n8n-io/n8n/issues/9644)) ([e9e3b25](https://github.com/n8n-io/n8n/commit/e9e3b254fe10e6b9b1783e931caadf792866d3fc))
* **editor:** Prevent saving already saved workflows ([#9670](https://github.com/n8n-io/n8n/issues/9670)) ([b652405](https://github.com/n8n-io/n8n/commit/b652405a0614e45d051268bb05051b454da21d0a))
* **editor:** Remove transparency from dark mode callouts ([#9650](https://github.com/n8n-io/n8n/issues/9650)) ([566b52c](https://github.com/n8n-io/n8n/commit/566b52c4e1b438f10aa6290aa6486ddd095708c9))
* **editor:** Render credentials editable when opening them from the node view ([#9678](https://github.com/n8n-io/n8n/issues/9678)) ([dc17cf3](https://github.com/n8n-io/n8n/commit/dc17cf3a490ea0dc0a3612f41a7d35e2723c15f9))
* **Gotify Node:** Fix issue with self signed certificates not working ([#9647](https://github.com/n8n-io/n8n/issues/9647)) ([68e856d](https://github.com/n8n-io/n8n/commit/68e856d1556d487bc1d5cd3c85dd09d7445b2bc9))
* Introduce `HooksService` ([#8962](https://github.com/n8n-io/n8n/issues/8962)) ([dda7901](https://github.com/n8n-io/n8n/commit/dda7901398cd7dc81297884f186b9f98f41278b4))
* **Jira Software Node:** Fix the order by feature ([#9639](https://github.com/n8n-io/n8n/issues/9639)) ([7aea824](https://github.com/n8n-io/n8n/commit/7aea8243fe32876158c9db6807f654554bf9555e))
* **n8n Form Trigger Node:** Error if Respond to Webhook and respond node not in workflow ([#9641](https://github.com/n8n-io/n8n/issues/9641)) ([b45f3dc](https://github.com/n8n-io/n8n/commit/b45f3dc9fbfbf190cec4f283b05dac66db5fe8f9))
* **Remove Duplicates Node:** Tolerate null fields ([#9642](https://github.com/n8n-io/n8n/issues/9642)) ([a684681](https://github.com/n8n-io/n8n/commit/a684681ea12329a821bdba9a665d79a365dacd9d))
* Reset pagination when output size changes ([#9652](https://github.com/n8n-io/n8n/issues/9652)) ([e520f8a](https://github.com/n8n-io/n8n/commit/e520f8a98f186ecefca8555afdbc08cbc19ef4b0))
* **X (Formerly Twitter) Node:** Change how tweet id is retrieved from quote URL ([#9635](https://github.com/n8n-io/n8n/issues/9635)) ([9853ecc](https://github.com/n8n-io/n8n/commit/9853ecc5bc84a64dc334668fb1c5dd632ebbb56d))


### Features

* Add support for dark mode node icons and colors ([#9412](https://github.com/n8n-io/n8n/issues/9412)) ([600013a](https://github.com/n8n-io/n8n/commit/600013a1ab770c0ff508aae930802f3f8f48ffb4))
* **core:** Add batching and other options to declarative nodes ([#8885](https://github.com/n8n-io/n8n/issues/8885)) ([4e56863](https://github.com/n8n-io/n8n/commit/4e568631bebb8db41a8ec9b4651abb0e8903eeed))
* **core:** Implement `project:viewer` role ([#9611](https://github.com/n8n-io/n8n/issues/9611)) ([6187cc5](https://github.com/n8n-io/n8n/commit/6187cc5762fe2156504041f41020d0fdad063f49))
* **editor:** Add isEmpty on DateTime, add is empty to all types in filter component ([#9645](https://github.com/n8n-io/n8n/issues/9645)) ([eccc637](https://github.com/n8n-io/n8n/commit/eccc637b63cbc2581f29feb27f148ba437bcf5d4))
* **editor:** Add move resources option to workflows and credentials on ([#9654](https://github.com/n8n-io/n8n/issues/9654)) ([bc35e8c](https://github.com/n8n-io/n8n/commit/bc35e8c33d470399466514b4d4874c965d7edc08))
* **editor:** Harmonize rendering of new-lines in RunData ([#9614](https://github.com/n8n-io/n8n/issues/9614)) ([bc3dcf7](https://github.com/n8n-io/n8n/commit/bc3dcf706f578837e8d6fe6473d414d9dd58e3c4))
* **OpenAI Node:** Allow to select Image analyze model & improve types ([#9660](https://github.com/n8n-io/n8n/issues/9660)) ([1fdd657](https://github.com/n8n-io/n8n/commit/1fdd657a0ce0b9722ee697d05bbada7ecf4cdf05))
* Update NPS Value Survey ([#9638](https://github.com/n8n-io/n8n/issues/9638)) ([50bd5b9](https://github.com/n8n-io/n8n/commit/50bd5b9080213d4286c37b93f598753dbee32eb4))



# [1.45.0](https://github.com/n8n-io/n8n/compare/n8n@1.44.0...n8n@1.45.0) (2024-06-05)


### Bug Fixes

* **AI Agent Node:** Improve Tools agent empty tool input message ([#9622](https://github.com/n8n-io/n8n/issues/9622)) ([e7f6162](https://github.com/n8n-io/n8n/commit/e7f616290f20c37121f554303f775a102569bdc7))
* **core:** Ensure graceful shutdown for workers ([#9547](https://github.com/n8n-io/n8n/issues/9547)) ([7fc00d8](https://github.com/n8n-io/n8n/commit/7fc00d8d104c2ceebf56f897c8d54fc292003811))
* **core:** Ensure ID is a positive integer when fetching execution ([#9629](https://github.com/n8n-io/n8n/issues/9629)) ([411ffbd](https://github.com/n8n-io/n8n/commit/411ffbda7f6a82e2ee249daa39e614c184df8643))
* **core:** Start WaitTracker only in the main container ([#9600](https://github.com/n8n-io/n8n/issues/9600)) ([08d9c9a](https://github.com/n8n-io/n8n/commit/08d9c9a7876bd0fd0d087cdc9175d94a33de0cc9))
* **core:** Upgrade mysql2 to address CVE-2024-21512 ([#9565](https://github.com/n8n-io/n8n/issues/9565)) ([4b6e5f0](https://github.com/n8n-io/n8n/commit/4b6e5f09e6770938de5e590a7e0d4565e3dc865c))
* **editor:** Commit theme change from Save button ([#9619](https://github.com/n8n-io/n8n/issues/9619)) ([744c94d](https://github.com/n8n-io/n8n/commit/744c94d94b3576f2a1d4227e49185be77b8c6954))
* **editor:** Filter credentials by project ID also for new workflow ([#9615](https://github.com/n8n-io/n8n/issues/9615)) ([c92765d](https://github.com/n8n-io/n8n/commit/c92765dcdb48789aa111ace29165a4b811fea710))
* **editor:** Improve error messages around pinned data ([#9632](https://github.com/n8n-io/n8n/issues/9632)) ([a8bb53f](https://github.com/n8n-io/n8n/commit/a8bb53f4e3dd5aee8f3b707cb0ee92ccc98e960e))
* **editor:** Render checkboxes in markdown ([#9549](https://github.com/n8n-io/n8n/issues/9549)) ([47d7741](https://github.com/n8n-io/n8n/commit/47d774100bd7a120de50d679e0052d6a1ae5e88a))
* **editor:** Replace more variants of BASE_PATH in static assets ([#9564](https://github.com/n8n-io/n8n/issues/9564)) ([d361b42](https://github.com/n8n-io/n8n/commit/d361b42c7035a3edbdd999a322c9327a8f565f77))
* **editor:** Show correct schema for output with falsy keys ([#9556](https://github.com/n8n-io/n8n/issues/9556)) ([020bd36](https://github.com/n8n-io/n8n/commit/020bd3635444d83f1aef310714470140dcac7c6e))
* **editor:** Show owner email in the owner badge if the resource owner is a pending user ([#9560](https://github.com/n8n-io/n8n/issues/9560)) ([2e9bd67](https://github.com/n8n-io/n8n/commit/2e9bd6739b5a510b6726bbe55dfe09267107e70f))
* **editor:** Show workflow data in header when execution page is hard reloaded ([#9529](https://github.com/n8n-io/n8n/issues/9529)) ([e68a3fd](https://github.com/n8n-io/n8n/commit/e68a3fd6ce7c710c398171b3deb8d8eb565e23ba))
* **editor:** Skip disabled nodes when detecting workflow issues ([#9610](https://github.com/n8n-io/n8n/issues/9610)) ([245c63f](https://github.com/n8n-io/n8n/commit/245c63f216c1074f8857f123e1dfae9b2b2b29bc))
* **HTTP Request Node:** Sanitize secrets of predefined credentials ([#9612](https://github.com/n8n-io/n8n/issues/9612)) ([84f091d](https://github.com/n8n-io/n8n/commit/84f091d3e5f9c661e373acd0c058ee158965b6e8))
* **Jira Software Node:** Fix comments limit and add sorting ([#9634](https://github.com/n8n-io/n8n/issues/9634)) ([a946ead](https://github.com/n8n-io/n8n/commit/a946ead46efecf6864505d465b0369ed67a1f2c7))
* Make AWS credential work with global AWS services ([#9631](https://github.com/n8n-io/n8n/issues/9631)) ([9dbea73](https://github.com/n8n-io/n8n/commit/9dbea7393a9e55edeb5cf9646f5068891e14f84c))


### Features

* **core:** Allow customizing rate limits on a per-route basis, and add rate limiting to more endpoints ([#9522](https://github.com/n8n-io/n8n/issues/9522)) ([7be616e](https://github.com/n8n-io/n8n/commit/7be616e5831678b42deb7de98c974369f7bf8967))
* **core:** Allow transferring credentials from any project to any team project ([#9563](https://github.com/n8n-io/n8n/issues/9563)) ([202c91e](https://github.com/n8n-io/n8n/commit/202c91e7edc2a99eec56436f94f0e552ac4816b5))
* **core:** Allow transferring workflows from any project to any team project ([#9534](https://github.com/n8n-io/n8n/issues/9534)) ([d6db8cb](https://github.com/n8n-io/n8n/commit/d6db8cbf23b46fa2f93c7460bf1df9047b2cfab2))
* **editor:** Add remove node and connections functionality to canvas v2 ([#9602](https://github.com/n8n-io/n8n/issues/9602)) ([f6a466c](https://github.com/n8n-io/n8n/commit/f6a466cd8750930eb7ea717e5113c5a4a477af26))
* **editor:** Chat Trigger tweaks ([#9618](https://github.com/n8n-io/n8n/issues/9618)) ([5322802](https://github.com/n8n-io/n8n/commit/5322802992032e4e5f7c528a1b0668dcbed49db2))
* **editor:** Node Creator AI nodes improvements  ([#9484](https://github.com/n8n-io/n8n/issues/9484)) ([be4f54d](https://github.com/n8n-io/n8n/commit/be4f54de157dde60e7ae6b0611fa599a059cd17f))
* **editor:** Overhaul input selector in NDV ([#9520](https://github.com/n8n-io/n8n/issues/9520)) ([c0ec990](https://github.com/n8n-io/n8n/commit/c0ec990f4cc78909e963b82f1492dafafab23b5a))
* **editor:** Update sticky content when checkbox state changes ([#9596](https://github.com/n8n-io/n8n/issues/9596)) ([5361e9f](https://github.com/n8n-io/n8n/commit/5361e9f69ae2211beda2f760ee215cd89c1d77e9))
* **HighLevel Node:** Api v2 support, new node version ([#9554](https://github.com/n8n-io/n8n/issues/9554)) ([19e5c03](https://github.com/n8n-io/n8n/commit/19e5c0397ad75b47c6068db194a3f938722095c8))
* Run once for each item tooltip ([#9486](https://github.com/n8n-io/n8n/issues/9486)) ([b91e50f](https://github.com/n8n-io/n8n/commit/b91e50fc92e3e41f2b4529caa054557309d891d0))



# [1.44.0](https://github.com/n8n-io/n8n/compare/n8n@1.43.0...n8n@1.44.0) (2024-05-30)


### Bug Fixes

* **core:** Block Public API related REST calls when Public API is not enabled ([#9521](https://github.com/n8n-io/n8n/issues/9521)) ([ac4e0fb](https://github.com/n8n-io/n8n/commit/ac4e0fbb47b818973958e37e6b80201ad2ffed6f))
* **core:** Prevent re-parsing of dynamically loaded options ([#9503](https://github.com/n8n-io/n8n/issues/9503)) ([a58be17](https://github.com/n8n-io/n8n/commit/a58be175cc8a65975b7aac15fc3143c38cf3682b))
* **core:** Set source control repository to track remote if ready ([#9532](https://github.com/n8n-io/n8n/issues/9532)) ([dbaac82](https://github.com/n8n-io/n8n/commit/dbaac82f79fd73d5dc11b29faa0e2cee4c55cc3f))
* **core:** Try setting postgres search_path on the database ([#9530](https://github.com/n8n-io/n8n/issues/9530)) ([e55bf03](https://github.com/n8n-io/n8n/commit/e55bf0393ae625ff34d41f1e861008cf7916dbdf))
* **core:** Upgrade sheetjs to address CVE-2024-22363 ([#9498](https://github.com/n8n-io/n8n/issues/9498)) ([8737c09](https://github.com/n8n-io/n8n/commit/8737c0965e3dd2d6eec0f05737cc96c0f12c43c5))
* Don't throw errors for NaN in number operators in the filter component  ([#9506](https://github.com/n8n-io/n8n/issues/9506)) ([936bbb2](https://github.com/n8n-io/n8n/commit/936bbb20684ac6f0d376f5a4ee3760e9587223f7))
* **editor:** Executions view popup in dark mode ([#9517](https://github.com/n8n-io/n8n/issues/9517)) ([1abb26e](https://github.com/n8n-io/n8n/commit/1abb26e2dacc2891417ea66f6a5f3dccc4b784cd))
* **editor:** Fix empty node name handling ([#9548](https://github.com/n8n-io/n8n/issues/9548)) ([da41d31](https://github.com/n8n-io/n8n/commit/da41d31bc0e19667a7fef7fac4008c7cb1c6c470))
* **editor:** Make sure auto loading and auto scrolling works in executions tab ([#9505](https://github.com/n8n-io/n8n/issues/9505)) ([3a2e545](https://github.com/n8n-io/n8n/commit/3a2e5455a98dae35ba1a52ec98f67a1fb27fac96))
* **editor:** Prevent expression editor focus being lost when user is selecting ([#9525](https://github.com/n8n-io/n8n/issues/9525)) ([6698179](https://github.com/n8n-io/n8n/commit/6698179a69511d8f009100c66c062218a26cfaad))
* **editor:** Prevent updating node parameter value if it hasn't changed ([#9535](https://github.com/n8n-io/n8n/issues/9535)) ([63990f1](https://github.com/n8n-io/n8n/commit/63990f14e3991770c1b9fbfd56edd6d0f3abd54b))
* **editor:** Prevent XSS in node-issues tooltip ([#9490](https://github.com/n8n-io/n8n/issues/9490)) ([301e846](https://github.com/n8n-io/n8n/commit/301e846cf64a7fce8191696e828eaf1c3fc82e88))
* **editor:** Redirect to workflows list after deleting a workflow ([#9546](https://github.com/n8n-io/n8n/issues/9546)) ([cadb59f](https://github.com/n8n-io/n8n/commit/cadb59fecbf1adeb1c226f9decd92a334656a895))
* **editor:** Send only execution id in postMessage when previewing an execution ([#9514](https://github.com/n8n-io/n8n/issues/9514)) ([49b5bd7](https://github.com/n8n-io/n8n/commit/49b5bd70f0d1c0dce46ea85d23deb75dbea6c51c))
* **editor:** Show execution error toast also if there is no error stack just message ([#9526](https://github.com/n8n-io/n8n/issues/9526)) ([f914c97](https://github.com/n8n-io/n8n/commit/f914c97d11d471aff1dbf66f9334ec98df613d6e))
* **editor:** Show input panel with not connected message ([#9495](https://github.com/n8n-io/n8n/issues/9495)) ([8566301](https://github.com/n8n-io/n8n/commit/85663017313a707c95b63c734942a29ef4473740))
* **editor:** Update webhook paths when duplicating workflow ([#9516](https://github.com/n8n-io/n8n/issues/9516)) ([3be7bb8](https://github.com/n8n-io/n8n/commit/3be7bb898bc2ecc0c2553df2a3e48bd125867ced))


### Features

* **core:** Print the name of the migration that cannot be reverted when using `n8n db:revert` ([#9473](https://github.com/n8n-io/n8n/issues/9473)) ([3b93aae](https://github.com/n8n-io/n8n/commit/3b93aae6dce7827dfb36279447327dfd89fddff5))
* **core:** Upgrade all langchain related dependencies ([#9504](https://github.com/n8n-io/n8n/issues/9504)) ([a77e8dd](https://github.com/n8n-io/n8n/commit/a77e8dd79ec7cbeb357ad03747fe2e4270d91a63))
* **editor:** Show expression infobox on hover and cursor position ([#9507](https://github.com/n8n-io/n8n/issues/9507)) ([ec0373f](https://github.com/n8n-io/n8n/commit/ec0373f666ed7d5c416fdef44afd8dd748755c9f))
* HighLevel oauth2 api credentials ([#9542](https://github.com/n8n-io/n8n/issues/9542)) ([be58905](https://github.com/n8n-io/n8n/commit/be5890536f9b99916de20ae3c771776149132026))


### Performance Improvements

* **core:** Optimize executions filtering by metadata ([#9477](https://github.com/n8n-io/n8n/issues/9477)) ([9bdc83a](https://github.com/n8n-io/n8n/commit/9bdc83a399592a2ca0761070f0e7074a6a3ffa7d))



# [1.43.0](https://github.com/n8n-io/n8n/compare/n8n@1.42.0...n8n@1.43.0) (2024-05-22)


### Bug Fixes

* **core:** Account for retry of execution aborted by pre-execute hook ([#9474](https://github.com/n8n-io/n8n/issues/9474)) ([a217866](https://github.com/n8n-io/n8n/commit/a217866cef6caaef9244f3d16d90f7027adc0c12))
* **core:** Add an option to disable STARTTLS for SMTP connections ([#9415](https://github.com/n8n-io/n8n/issues/9415)) ([0d73588](https://github.com/n8n-io/n8n/commit/0d7358807b4244be574060726388bd49fc90dc64))
* **core:** Do not allow admins to delete the instance owner ([#9489](https://github.com/n8n-io/n8n/issues/9489)) ([fc83005](https://github.com/n8n-io/n8n/commit/fc83005ba0876ebea70f93de700adbd6e3095c96))
* **core:** Do not allow admins to generate password-reset links for instance owner ([#9488](https://github.com/n8n-io/n8n/issues/9488)) ([88b9a40](https://github.com/n8n-io/n8n/commit/88b9a4070b7df943c3ba22047c0656a5d0a2111c))
* **core:** Fix 431 for large dynamic node parameters ([#9384](https://github.com/n8n-io/n8n/issues/9384)) ([d21ad15](https://github.com/n8n-io/n8n/commit/d21ad15c1f12739af6a28983a6469347c26f1e08))
* **core:** Handle credential in body for oauth2 refresh token ([#9179](https://github.com/n8n-io/n8n/issues/9179)) ([c9855e3](https://github.com/n8n-io/n8n/commit/c9855e3dce42f8830636914458d1061668a466a8))
* **core:** Remove excess args from routing error ([#9377](https://github.com/n8n-io/n8n/issues/9377)) ([b1f977e](https://github.com/n8n-io/n8n/commit/b1f977ebd084ab3a8fb1d13109063de7d2a15296))
* **core:** Retry before continue on fail ([#9395](https://github.com/n8n-io/n8n/issues/9395)) ([9b2ce81](https://github.com/n8n-io/n8n/commit/9b2ce819d42c4a541ae94956aaab608a989ec588))
* **editor:** Emit change events from filter component on update ([#9479](https://github.com/n8n-io/n8n/issues/9479)) ([62df433](https://github.com/n8n-io/n8n/commit/62df4331d448dfdabd51db33560a87dd5d805a13))
* **editor:** Fix blank Public API page ([#9409](https://github.com/n8n-io/n8n/issues/9409)) ([14fe9f2](https://github.com/n8n-io/n8n/commit/14fe9f268feeb0ca106ddaaa94c69cb356011524))
* **editor:** Fix i18n translation addition ([#9451](https://github.com/n8n-io/n8n/issues/9451)) ([04dd476](https://github.com/n8n-io/n8n/commit/04dd4760e173bfc8a938413a5915d63291da8afe))
* **editor:** Fix node execution errors showing undefined ([#9487](https://github.com/n8n-io/n8n/issues/9487)) ([62ee796](https://github.com/n8n-io/n8n/commit/62ee79689569b5d2c9823afac238e66e4c645d9b))
* **editor:** Fix outdated roles in variables labels ([#9411](https://github.com/n8n-io/n8n/issues/9411)) ([38b498e](https://github.com/n8n-io/n8n/commit/38b498e73a71a9ca8b10a89e498aa8330acf2626))
* **editor:** Fix project settings layout ([#9475](https://github.com/n8n-io/n8n/issues/9475)) ([96cf41f](https://github.com/n8n-io/n8n/commit/96cf41f8516881f0ba15b0b01dda7712f1edc845))
* **editor:** Fix type errors in `components/executions/workflow` ([#9448](https://github.com/n8n-io/n8n/issues/9448)) ([9c768a0](https://github.com/n8n-io/n8n/commit/9c768a0443520f0c031d4d807d955d7778a00997))
* **editor:** Fix type errors in i18n plugin ([#9441](https://github.com/n8n-io/n8n/issues/9441)) ([a7d3e59](https://github.com/n8n-io/n8n/commit/a7d3e59aef36dd65429ad0b2ea4696b107620eeb))
* **editor:** Fix workflow history TS errors ([#9433](https://github.com/n8n-io/n8n/issues/9433)) ([bc05faf](https://github.com/n8n-io/n8n/commit/bc05faf0a6a0913013e4d46eefb1e45abc390883))
* **editor:** Secondary button in dark mode ([#9401](https://github.com/n8n-io/n8n/issues/9401)) ([aad43d8](https://github.com/n8n-io/n8n/commit/aad43d8cdcc9621fbd864fbe0235c9ff4ddbfe3e))
* **Email Trigger (IMAP) Node:** Handle attachments correctly ([#9410](https://github.com/n8n-io/n8n/issues/9410)) ([68a6c81](https://github.com/n8n-io/n8n/commit/68a6c8172973091e8474a9f173fa4a5e97284f18))
* Fix color picker type errors ([#9436](https://github.com/n8n-io/n8n/issues/9436)) ([2967df2](https://github.com/n8n-io/n8n/commit/2967df2fe098278dd20126dc033b03cbb4b903ce))
* Fix type errors in community nodes components ([#9445](https://github.com/n8n-io/n8n/issues/9445)) ([aac19d3](https://github.com/n8n-io/n8n/commit/aac19d328564bfecda53b338e2c56e5e30e5c0c1))
* **Gmail Trigger Node:** Fetching duplicate emails ([#9424](https://github.com/n8n-io/n8n/issues/9424)) ([3761537](https://github.com/n8n-io/n8n/commit/3761537880f53d9e54b0200a63b067dc3d154787))
* **HTML Node:** Fix typo preventing row attributes from being set in tables ([#9440](https://github.com/n8n-io/n8n/issues/9440)) ([28e3e21](https://github.com/n8n-io/n8n/commit/28e3e211771fd73a88e34b81858188156fca5fbb))
* **HubSpot Trigger Node:** Fix issue with ticketId not being set ([#9403](https://github.com/n8n-io/n8n/issues/9403)) ([b5c7c06](https://github.com/n8n-io/n8n/commit/b5c7c061b7e854a06bd725f7905a7f3ac8dfedc2))
* **Mattermost Node:** Change loadOptions to fetch all items ([#9413](https://github.com/n8n-io/n8n/issues/9413)) ([1377e21](https://github.com/n8n-io/n8n/commit/1377e212c709bc9ca6586c030ec083e89a3d8c37))
* **Microsoft OneDrive Trigger Node:** Fix issue with test run failing ([#9386](https://github.com/n8n-io/n8n/issues/9386)) ([92a1d65](https://github.com/n8n-io/n8n/commit/92a1d65c4b00683cc334c70f183e5f8c99bfae65))
* **RSS Feed Trigger Node:** Use newest date instead of first item for new items ([#9182](https://github.com/n8n-io/n8n/issues/9182)) ([7236a55](https://github.com/n8n-io/n8n/commit/7236a558b945c69fa5680e42c538af7c5276cc31))
* Update operations to run per item ([#8967](https://github.com/n8n-io/n8n/issues/8967)) ([ef9d4ab](https://github.com/n8n-io/n8n/commit/ef9d4aba90c92f9b72a17de242a4ffeb7c034802))


### Features

* Add Slack trigger node ([#9190](https://github.com/n8n-io/n8n/issues/9190)) ([bf54930](https://github.com/n8n-io/n8n/commit/bf549301df541c43931fe4493b4bad7905fb0c8a))
* **Custom n8n Workflow Tool Node:** Add support for tool input schema ([#9470](https://github.com/n8n-io/n8n/issues/9470)) ([2fa46b6](https://github.com/n8n-io/n8n/commit/2fa46b6faac5618a10403066c3dddf4ea9def12c))
* **editor:** Add examples for Luxon DateTime expression methods ([#9361](https://github.com/n8n-io/n8n/issues/9361)) ([40bce7f](https://github.com/n8n-io/n8n/commit/40bce7f44332042bf8dba0442044acd76cc9bf21))
* **editor:** Add examples for root expression methods ([#9373](https://github.com/n8n-io/n8n/issues/9373)) ([a591f63](https://github.com/n8n-io/n8n/commit/a591f63e3ff51c19fe48185144725e881c418b23))
* **editor:** Expand supported Unicode range for expressions ([#9420](https://github.com/n8n-io/n8n/issues/9420)) ([2118236](https://github.com/n8n-io/n8n/commit/211823650ba298aac899ff944819290f0bd4654a))
* **editor:** Update Node Details View header tabs structure ([#9425](https://github.com/n8n-io/n8n/issues/9425)) ([2782534](https://github.com/n8n-io/n8n/commit/2782534d78e9613bda41675b4574c8016b10b0a4))
* **Extract from File Node:** Add option to set encoding for CSV files ([#9392](https://github.com/n8n-io/n8n/issues/9392)) ([f13dbc9](https://github.com/n8n-io/n8n/commit/f13dbc9cc31fba20b4cb0bedf11e56e16079f946))
* **Linear Node:** Add identifier to outputs ([#9469](https://github.com/n8n-io/n8n/issues/9469)) ([ffe034c](https://github.com/n8n-io/n8n/commit/ffe034c72e07346cdbea4dda96c7e2c38ea73c45))
* **OpenAI Node:** Use v2 assistants API and add support for memory ([#9406](https://github.com/n8n-io/n8n/issues/9406)) ([ce3eb12](https://github.com/n8n-io/n8n/commit/ce3eb12a6ba325d3785d54d90ff5a32152afd4c0))
* RBAC ([#8922](https://github.com/n8n-io/n8n/issues/8922)) ([596c472](https://github.com/n8n-io/n8n/commit/596c472ecc756bf934c51e7efae0075fb23313b4))
* **Strava Node:** Update to use sport type ([#9462](https://github.com/n8n-io/n8n/issues/9462)) ([9da9368](https://github.com/n8n-io/n8n/commit/9da93680c28f9191eac7edc452e5123749e5c148))
* **Telegram Node:** Add support for local bot api server ([#8437](https://github.com/n8n-io/n8n/issues/8437)) ([87f965e](https://github.com/n8n-io/n8n/commit/87f965e9055904486f5fd815c060abb4376296a0))



# [1.42.0](https://github.com/n8n-io/n8n/compare/n8n@1.41.0...n8n@1.42.0) (2024-05-15)


### Bug Fixes

* **Code Node:** Bind helper methods to the correct context ([#9380](https://github.com/n8n-io/n8n/issues/9380)) ([82c8801](https://github.com/n8n-io/n8n/commit/82c8801f25446085bc8da5055d9932eed4321f47))
* **Cortex Node:** Fix issue with analyzer response not working for file observables ([#9374](https://github.com/n8n-io/n8n/issues/9374)) ([ed22dcd](https://github.com/n8n-io/n8n/commit/ed22dcd88ac7f8433b9ed5dc2139d8779b0e1d4c))
* **editor:** Render backticks as code segments in error view ([#9352](https://github.com/n8n-io/n8n/issues/9352)) ([4ed5850](https://github.com/n8n-io/n8n/commit/4ed585040b20c50919e2ec2252216639c85194cb))
* **Mattermost Node:** Fix issue when fetching reactions ([#9375](https://github.com/n8n-io/n8n/issues/9375)) ([78e7c7a](https://github.com/n8n-io/n8n/commit/78e7c7a9da96a293262cea5304509261ad10020c))


### Features

* **AI Agent Node:** Implement Tool calling agent ([#9339](https://github.com/n8n-io/n8n/issues/9339)) ([677f534](https://github.com/n8n-io/n8n/commit/677f534661634c74340f50723e55e241570d5a56))
* **core:** Allow using a custom certificates in docker containers ([#8705](https://github.com/n8n-io/n8n/issues/8705)) ([6059722](https://github.com/n8n-io/n8n/commit/6059722fbfeeca31addfc31ed287f79f40aaad18))
* **core:** Node hints(warnings) system ([#8954](https://github.com/n8n-io/n8n/issues/8954)) ([da6088d](https://github.com/n8n-io/n8n/commit/da6088d0bbb952fcdf595a650e1e01b7b02a2b7e))
* **core:** Node version available in expression ([#9350](https://github.com/n8n-io/n8n/issues/9350)) ([a00467c](https://github.com/n8n-io/n8n/commit/a00467c9fa57d740de9eccfcd136267bc9e9559d))
* **editor:** Add examples for number & boolean, add new methods ([#9358](https://github.com/n8n-io/n8n/issues/9358)) ([7b45dc3](https://github.com/n8n-io/n8n/commit/7b45dc313f42317f894469c6aa8abecc55704e3a))
* **editor:** Add examples for object and array expression methods ([#9360](https://github.com/n8n-io/n8n/issues/9360)) ([5293663](https://github.com/n8n-io/n8n/commit/52936633af9c71dff1957ee43a5eda48f7fc1bf1))
* **editor:** Add item selector to expression output ([#9281](https://github.com/n8n-io/n8n/issues/9281)) ([dc5994b](https://github.com/n8n-io/n8n/commit/dc5994b18580b9326574c5208d9beaf01c746f33))
* **editor:** Autocomplete info box: improve structure and add examples ([#9019](https://github.com/n8n-io/n8n/issues/9019)) ([c92c870](https://github.com/n8n-io/n8n/commit/c92c870c7335f4e2af63fa1c6bcfd086b2957ef8))
* **editor:** Remove AI Error Debugging ([#9337](https://github.com/n8n-io/n8n/issues/9337)) ([cda062b](https://github.com/n8n-io/n8n/commit/cda062bde63bcbfdd599d0662ddbe89c27a71686))
* **Slack Node:** Add block support for message updates ([#8925](https://github.com/n8n-io/n8n/issues/8925)) ([1081429](https://github.com/n8n-io/n8n/commit/1081429a4d0f7e2d1fc1841303448035b46e44d1))


### Performance Improvements

* Add tailwind to editor and design system ([#9032](https://github.com/n8n-io/n8n/issues/9032)) ([1c1e444](https://github.com/n8n-io/n8n/commit/1c1e4443f41dd39da8d5fa3951c8dffb0fbfce10))



# [1.41.0](https://github.com/n8n-io/n8n/compare/n8n@1.40.0...n8n@1.41.0) (2024-05-08)


### Bug Fixes

* Cast boolean values in filter parameter ([#9260](https://github.com/n8n-io/n8n/issues/9260)) ([30c8efc](https://github.com/n8n-io/n8n/commit/30c8efc4cc9b25fabc8d9c56e8c29e7e77c04325))
* **core:** Prevent occassional 429s on license init in multi-main setup ([#9284](https://github.com/n8n-io/n8n/issues/9284)) ([22b6f90](https://github.com/n8n-io/n8n/commit/22b6f909505d7c3d9c0583a90599e6e9c244e21e))
* **core:** Report missing SAML attributes early with an actionable error message ([#9316](https://github.com/n8n-io/n8n/issues/9316)) ([225fdbb](https://github.com/n8n-io/n8n/commit/225fdbb379f6dd0005bd4ccb3791c96de35b1653))
* **core:** Webhooks responding with binary data should not prematurely end the response stream ([#9063](https://github.com/n8n-io/n8n/issues/9063)) ([23b676d](https://github.com/n8n-io/n8n/commit/23b676d7cb9708d7a99fc031cfeec22b854be1d9))
* **editor:** Fix multi-select parameters with load options getting cleared ([#9324](https://github.com/n8n-io/n8n/issues/9324)) ([0ee4b6c](https://github.com/n8n-io/n8n/commit/0ee4b6c86000ab164211c1ebed90306cd144af1b))
* **editor:** Fix shortcut issue on save buttons ([#9309](https://github.com/n8n-io/n8n/issues/9309)) ([e74c14f](https://github.com/n8n-io/n8n/commit/e74c14ffbe088ac74dc6358068cd54af9a850cad))
* **editor:** Resolve `$vars` and `$secrets` in expressions in credentials fields ([#9289](https://github.com/n8n-io/n8n/issues/9289)) ([d92f994](https://github.com/n8n-io/n8n/commit/d92f994913befd31aec409ef8e40b290ac4185ba))
* **editor:** Show MFA section to instance owner, even when external auth is enabled ([#9301](https://github.com/n8n-io/n8n/issues/9301)) ([b65e0e2](https://github.com/n8n-io/n8n/commit/b65e0e28114f576f89e271ab8ffdb8550e1be60f))
* **Gmail Node:** Remove duplicate options when creating drafts ([#9299](https://github.com/n8n-io/n8n/issues/9299)) ([bfb0eb7](https://github.com/n8n-io/n8n/commit/bfb0eb7a06f219424486a55256ecca46c14a85ba))
* **Linear Node:** Fix issue with data not always being returned ([#9273](https://github.com/n8n-io/n8n/issues/9273)) ([435272b](https://github.com/n8n-io/n8n/commit/435272b568826edf899dbaba9d10077fbe134ea6))
* **n8n Form Trigger Node:** Fix missing options when using respond to webhook ([#9282](https://github.com/n8n-io/n8n/issues/9282)) ([6ab3781](https://github.com/n8n-io/n8n/commit/6ab378157041abfc918ae1d9408821f8fd5cfb34))
* **Pipedrive Node:** Improve type-safety in custom-property handling ([#9319](https://github.com/n8n-io/n8n/issues/9319)) ([c8895c5](https://github.com/n8n-io/n8n/commit/c8895c540e5c8edfb576960a5ba4ec9ac4426d5b))
* **Read PDF Node:** Disable JS evaluation from PDFs ([#9336](https://github.com/n8n-io/n8n/issues/9336)) ([c4bf5b2](https://github.com/n8n-io/n8n/commit/c4bf5b2b9285402ae09960eb64a5d6f20356eeaf))


### Features

* **editor:** Implement AI Assistant chat UI ([#9300](https://github.com/n8n-io/n8n/issues/9300)) ([491c6ec](https://github.com/n8n-io/n8n/commit/491c6ec546c4ec8ab4eb88d020c13820071bf6dc))
* **editor:** Temporarily disable AI error helper ([#9329](https://github.com/n8n-io/n8n/issues/9329)) ([35b983b](https://github.com/n8n-io/n8n/commit/35b983b6dfbb6ab02367801a15581e80a2d87340))
* **LinkedIn Node:** Upgrade LinkedIn API version ([#9307](https://github.com/n8n-io/n8n/issues/9307)) ([3860077](https://github.com/n8n-io/n8n/commit/3860077f8100fb790acf1d930839e86719a454fd))
* **Redis Node:** Add support for TLS ([#9266](https://github.com/n8n-io/n8n/issues/9266)) ([0a2de09](https://github.com/n8n-io/n8n/commit/0a2de093c01689b8f179b3f4413a4ce29ccf279a))
* **Send Email Node:** Add an option to customize client host-name on SMTP connections ([#9322](https://github.com/n8n-io/n8n/issues/9322)) ([d0d52de](https://github.com/n8n-io/n8n/commit/d0d52def8fb4113a7a4866d30f2e9c7bfe11075e))
* **Slack Node:** Update to use the new API method for file uploads ([#9323](https://github.com/n8n-io/n8n/issues/9323)) ([695e762](https://github.com/n8n-io/n8n/commit/695e762663fde79b9555be8cf075ee4144f380f1))



# [1.40.0](https://github.com/n8n-io/n8n/compare/n8n@1.39.0...n8n@1.40.0) (2024-05-02)


### Bug Fixes

* **Airtable Node:** Do not allow to use deprecated api keys in v1 ([#9171](https://github.com/n8n-io/n8n/issues/9171)) ([017ae6e](https://github.com/n8n-io/n8n/commit/017ae6e1025fb4ae28b46b9c411e4b5c70e280e9))
* **core:** Add `view engine` to webhook server to support forms ([#9224](https://github.com/n8n-io/n8n/issues/9224)) ([24c3150](https://github.com/n8n-io/n8n/commit/24c3150056401ddcf49f7266897b6c73ccc06253))
* **core:** Fix browser session refreshes not working ([#9212](https://github.com/n8n-io/n8n/issues/9212)) ([1efeecc](https://github.com/n8n-io/n8n/commit/1efeeccc5bae306a798a66a8cf3e669ad3689262))
* **core:** Prevent node param resolution from failing telemetry graph generation ([#9257](https://github.com/n8n-io/n8n/issues/9257)) ([f6c9493](https://github.com/n8n-io/n8n/commit/f6c9493355726ddf516fb54a37adf49a2ce0efd0))
* **core:** Stop relying on filesystem for SSH keys ([#9217](https://github.com/n8n-io/n8n/issues/9217)) ([093dcef](https://github.com/n8n-io/n8n/commit/093dcefafc5a09f7622391d8b01b9aecfa9c8f2f))
* **Discord Node:** When using OAuth2 authentication, check if user is a guild member when sending direct message ([#9183](https://github.com/n8n-io/n8n/issues/9183)) ([00dfad3](https://github.com/n8n-io/n8n/commit/00dfad3279bd2a45a8331e734b331f4ab3fce75c))
* **editor:** Fix read-only mode in inline expression editor ([#9232](https://github.com/n8n-io/n8n/issues/9232)) ([99f384e](https://github.com/n8n-io/n8n/commit/99f384e2cf6b16d08a8bdc150a2833463b35f14b))
* **editor:** Prevent excess runs in manual execution with run data ([#9259](https://github.com/n8n-io/n8n/issues/9259)) ([426a12a](https://github.com/n8n-io/n8n/commit/426a12ac0ec1d637063828db008a2fb9c32ddfff))
* **editor:** Throw expression error on attempting to set variables at runtime ([#9229](https://github.com/n8n-io/n8n/issues/9229)) ([fec04d5](https://github.com/n8n-io/n8n/commit/fec04d5f796c677b6127addcb700d6442c2c3a26))
* Elaborate scope of Sustainable Use License ([#9233](https://github.com/n8n-io/n8n/issues/9233)) ([442aaba](https://github.com/n8n-io/n8n/commit/442aaba116cf0cfe7c1e7b8d570e321cc6a14143))
* **Google BigQuery Node:** Better error messages, transform timestamps ([#9255](https://github.com/n8n-io/n8n/issues/9255)) ([7ff24f1](https://github.com/n8n-io/n8n/commit/7ff24f134b706d0b5b7d7c13d3e69bd1a0f4c5b8))
* **Google Drive Node:** Create from text operation ([#9185](https://github.com/n8n-io/n8n/issues/9185)) ([d9e7494](https://github.com/n8n-io/n8n/commit/d9e74949c4db7282c3ab42bd6825aa5acc042400))
* **Jira Trigger Node:** Update credentials UI ([#9198](https://github.com/n8n-io/n8n/issues/9198)) ([ed98ca2](https://github.com/n8n-io/n8n/commit/ed98ca2fb77fc81362e6480ee6a12a64915418f9))
* **LangChain Code Node:** Fix execution of custom n8n tools called via LC code node ([#9265](https://github.com/n8n-io/n8n/issues/9265)) ([741e829](https://github.com/n8n-io/n8n/commit/741e8299d64cd774cc35ea312433f50d865f1318))
* **LangChain Code Node:** Fix resolution of scoped langchain modules ([#9258](https://github.com/n8n-io/n8n/issues/9258)) ([445c05d](https://github.com/n8n-io/n8n/commit/445c05dca46225e195ab122cf77d6d1088460e20))
* **MySQL Node:** Query to statements splitting fix ([#9207](https://github.com/n8n-io/n8n/issues/9207)) ([dc84452](https://github.com/n8n-io/n8n/commit/dc844528f4554ae41037e2c25542237a74d86f3f))


### Features

* Add Ask AI to HTTP Request Node ([#8917](https://github.com/n8n-io/n8n/issues/8917)) ([cd9bc44](https://github.com/n8n-io/n8n/commit/cd9bc44bddf7fc78acec9ee7c96a40077a07615f))
* **Gmail Node:** Add support for creating drafts using an alias ([#8728](https://github.com/n8n-io/n8n/issues/8728)) ([3986356](https://github.com/n8n-io/n8n/commit/3986356c8995998cb6ab392ae07f41efcb46d4bd))
* **Gmail Node:** Add thread option for draft emails ([#8729](https://github.com/n8n-io/n8n/issues/8729)) ([2dd0b32](https://github.com/n8n-io/n8n/commit/2dd0b329ca243de87eb1b59bf831593f70c42784))
* **Groq Chat Model Node:** Add support for Groq chat models  ([#9250](https://github.com/n8n-io/n8n/issues/9250)) ([96f02bd](https://github.com/n8n-io/n8n/commit/96f02bd6552cf9ea75fcb8ba29c3afac9553aa25))
* **HTTP Request Node:** Option to provide SSL Certificates in Http Request Node ([#9125](https://github.com/n8n-io/n8n/issues/9125)) ([306b68d](https://github.com/n8n-io/n8n/commit/306b68da6bb37dbce67dcf5c4791c2986750579c))
* **Jira Software Node:** Add Wiki Markup support for Jira Cloud comments ([#8857](https://github.com/n8n-io/n8n/issues/8857)) ([756012b](https://github.com/n8n-io/n8n/commit/756012b0524e09601fada80213dd4da3057d329a))
* **Microsoft To Do Node:** Add an option to set a reminder when updating a task ([#6918](https://github.com/n8n-io/n8n/issues/6918)) ([22b2afd](https://github.com/n8n-io/n8n/commit/22b2afdd23bef2a301cd9d3743400e0d69463b1b))
* **MISP Node:** Rest search operations ([#9196](https://github.com/n8n-io/n8n/issues/9196)) ([b694e77](https://github.com/n8n-io/n8n/commit/b694e7743e17507b901706c5023a9aac83b903dd))
* **Ollama Chat Model Node:** Add aditional Ollama config parameters & fix vision ([#9215](https://github.com/n8n-io/n8n/issues/9215)) ([e17e767](https://github.com/n8n-io/n8n/commit/e17e767e700a74b187706552fc879c00fd551611))
* **Pipedrive Node:** Add busy and description options to activities ([#9208](https://github.com/n8n-io/n8n/issues/9208)) ([9b3ac16](https://github.com/n8n-io/n8n/commit/9b3ac1648f1888d79079fd50998140fd27efae97))
* **Postgres Node:** Add option IS NOT NULL and hide value input fields ([#9241](https://github.com/n8n-io/n8n/issues/9241)) ([e896889](https://github.com/n8n-io/n8n/commit/e89688939438b2d5414155f053530bd9eb34b300))
* **S3 Node:** Add support for self signed SSL certificates ([#9269](https://github.com/n8n-io/n8n/issues/9269)) ([ddff804](https://github.com/n8n-io/n8n/commit/ddff80416df87166627fdefc755e3f79102c5664))
* **Telegram Node:** Disable page preview by default ([#9267](https://github.com/n8n-io/n8n/issues/9267)) ([41ce178](https://github.com/n8n-io/n8n/commit/41ce178491135b5f972974ebecec0f5f223a71ce))
* Upgrade typeorm for separate sqlite read & write connections ([#9230](https://github.com/n8n-io/n8n/issues/9230)) ([0b52320](https://github.com/n8n-io/n8n/commit/0b523206358886d5b81d7009ce95cb9d3ba9fa40))
* **Wise Node:** Add XML as supported format in getStatement operation ([#9193](https://github.com/n8n-io/n8n/issues/9193)) ([a424b59](https://github.com/n8n-io/n8n/commit/a424b59e4949e96c0e56319cea91fcf084a5208e))
* **Wise Trigger Node:** Add support for balance updates ([#9189](https://github.com/n8n-io/n8n/issues/9189)) ([42a9891](https://github.com/n8n-io/n8n/commit/42a9891081e7f1a19364c406b056eee036180c24))



# [1.39.0](https://github.com/n8n-io/n8n/compare/n8n@1.38.0...n8n@1.39.0) (2024-04-24)


### Bug Fixes

* **core:** Exclude oAuth callback urls from browser-id checks ([#9158](https://github.com/n8n-io/n8n/issues/9158)) ([46e432b](https://github.com/n8n-io/n8n/commit/46e432b177b4f1ae437f598674f188fb11ee1f20))
* **core:** Improve browserId checks, and add logging ([#9161](https://github.com/n8n-io/n8n/issues/9161)) ([ff9ae54](https://github.com/n8n-io/n8n/commit/ff9ae549fdc6962e9990987c54804d2570da6a12))
* **core:** Upgrade mysql2 to address CVE-2024-21511 ([#9206](https://github.com/n8n-io/n8n/issues/9206)) ([3996d28](https://github.com/n8n-io/n8n/commit/3996d2852a2e2a056af008a8f1a1c6cec9ba6084))
* **editor:** Fix expression preview when previous node is selected ([#9140](https://github.com/n8n-io/n8n/issues/9140)) ([85780ea](https://github.com/n8n-io/n8n/commit/85780eade57f30e6870c314fa465d523e3646005))
* **editor:** Fix parameter reset on credential change in Discord node ([#9137](https://github.com/n8n-io/n8n/issues/9137)) ([135ef75](https://github.com/n8n-io/n8n/commit/135ef75add8a42ce5163cce934ac5b2757ca4fe3))
* **editor:** Fix sessionId for manual chat trigger execution ([#9187](https://github.com/n8n-io/n8n/issues/9187)) ([f5ccb5f](https://github.com/n8n-io/n8n/commit/f5ccb5fe33392654a292de34b9ed8319901d303b))
* **editor:** Make sticky node content parameter non require to support empty stickies ([#9192](https://github.com/n8n-io/n8n/issues/9192)) ([f6142ff](https://github.com/n8n-io/n8n/commit/f6142ff275abb443940e9d8a4694c7f54c77a183))
* **editor:** Prevent duplicate values in preview for SQL editor ([#9129](https://github.com/n8n-io/n8n/issues/9129)) ([5acbfb4](https://github.com/n8n-io/n8n/commit/5acbfb423436b94e58af0e532e567bdc3783a622))
* **Google Sheets Node:** Fix "Append or Update" on an empty sheet ([#9175](https://github.com/n8n-io/n8n/issues/9175)) ([29ee4fa](https://github.com/n8n-io/n8n/commit/29ee4fab61c2f364b249b91c7561b176e78f37ac))
* **Notion Node:** Add itemIndex to API and operation errors ([#9150](https://github.com/n8n-io/n8n/issues/9150)) ([946f09f](https://github.com/n8n-io/n8n/commit/946f09f62842c963e94d97555d1b5bf7789a1b99))
* **Postgres Node:** Convert js arrays to postgres type, if column type is ARRAY ([#9160](https://github.com/n8n-io/n8n/issues/9160)) ([08e3502](https://github.com/n8n-io/n8n/commit/08e35027f1d4f483670dce44e8026c77aa4e6c3f))
* **Respond to Webhook Node:** Fix issue stopping form trigger response ([#9157](https://github.com/n8n-io/n8n/issues/9157)) ([6c63cd9](https://github.com/n8n-io/n8n/commit/6c63cd971162d3f018b210d221ffc2a56535550a))
* **Schedule Trigger Node:** Default to 0 minute if falsy on hourly run ([#9146](https://github.com/n8n-io/n8n/issues/9146)) ([d756609](https://github.com/n8n-io/n8n/commit/d75660982636389516cd97305e3c19912b77ea9c))
* **Splunk Node:** Retry attempts if no response from API call, better error with suggestion to use Retry On Fail  ([#9176](https://github.com/n8n-io/n8n/issues/9176)) ([05a569c](https://github.com/n8n-io/n8n/commit/05a569c1cd1f2ecf40987c5f677dad61fd6324e5))


### Features

* Add WhatsApp Business Trigger Node ([#8840](https://github.com/n8n-io/n8n/issues/8840)) ([23a2dd0](https://github.com/n8n-io/n8n/commit/23a2dd08b6e5391b61b73bdd4496cdb2f6fa9205))
* **core:** Setup helmet.js for setting security headers ([#9027](https://github.com/n8n-io/n8n/issues/9027)) ([0ed4671](https://github.com/n8n-io/n8n/commit/0ed46711f426f7edf5fa7833673b6b07348a3bd7))
* **core:** Upgrade mysql2 to address CVE-2024-21507, CVE-2024-21508, and CVE-2024-21509 ([#9154](https://github.com/n8n-io/n8n/issues/9154)) ([9bd8e10](https://github.com/n8n-io/n8n/commit/9bd8e10b356ab965bfee5d13bf339f057bcfdb14))
* **n8n Form Trigger Node:** Option to remove attribution ([#9162](https://github.com/n8n-io/n8n/issues/9162)) ([699fd70](https://github.com/n8n-io/n8n/commit/699fd70c2427397455939391f95a5cd65521afb3))
* **Webhook Node:** Setting to enable multiple outputs/methods ([#9086](https://github.com/n8n-io/n8n/issues/9086)) ([2bf0a39](https://github.com/n8n-io/n8n/commit/2bf0a3933e0d7da46be73b8671e72e69d7d472df))
* **Zammad Node:** Add more options to the Organizations endpoint  ([#9180](https://github.com/n8n-io/n8n/issues/9180)) ([15c88d6](https://github.com/n8n-io/n8n/commit/15c88d6839fb0b59fe5112b846ba61a29e9e3e45))



# [1.38.0](https://github.com/n8n-io/n8n/compare/n8n@1.37.0...n8n@1.38.0) (2024-04-17)


### Bug Fixes

* **core:** Don't create multiple owners when importing credentials or workflows ([#9112](https://github.com/n8n-io/n8n/issues/9112)) ([3eb5be5](https://github.com/n8n-io/n8n/commit/3eb5be5f5a1a62d7cf39381a67c8d747c397a969))
* **core:** Don't revert irreversibble migrations ([#9105](https://github.com/n8n-io/n8n/issues/9105)) ([3bb821f](https://github.com/n8n-io/n8n/commit/3bb821f10e2d865040fd1d89bec9836c7f98b8ef))
* **core:** Support MySQL in `MoveSshKeysToDatabase` migration ([#9120](https://github.com/n8n-io/n8n/issues/9120)) ([cf435c3](https://github.com/n8n-io/n8n/commit/cf435c33110d620295587e61b355ead6e4819958))
* **editor:** Do not show overlapping trash icon in the node's settings ([#9119](https://github.com/n8n-io/n8n/issues/9119)) ([c00150b](https://github.com/n8n-io/n8n/commit/c00150bb8ff88f8905536e5b4612c4c8cdd755a7))
* **editor:** Open links from embedded chat in new tab ([#9121](https://github.com/n8n-io/n8n/issues/9121)) ([284de5d](https://github.com/n8n-io/n8n/commit/284de5d6c7af901ee11ecda4c80b3998fd6b5657))
* **editor:** Render dates correctly in parameter hint ([#9089](https://github.com/n8n-io/n8n/issues/9089)) ([064e8f4](https://github.com/n8n-io/n8n/commit/064e8f4a1dc5afaa7ab21b770e3fbb9165805add))
* **Execute Workflow Node:** Assign fallback pairedItem only if not present in output item and different length of input output  ([#9145](https://github.com/n8n-io/n8n/issues/9145)) ([a95e401](https://github.com/n8n-io/n8n/commit/a95e4016967b2ef443ad0ea07338ab830d5c0100))
* Fix issue with Crowdstrike credential not working correctly ([#9108](https://github.com/n8n-io/n8n/issues/9108)) ([4c16000](https://github.com/n8n-io/n8n/commit/4c16000efadbfc5961ef2befd4f6501f9f2f0b2c))
* **HTTP Request Node:** Tolerate header name being empty ([#9138](https://github.com/n8n-io/n8n/issues/9138)) ([f6c9dbf](https://github.com/n8n-io/n8n/commit/f6c9dbf7b850e9b665bbc72090a41c45d125f996))
* **Respond to Webhook Node:** Continue on fail and error branch support ([#9115](https://github.com/n8n-io/n8n/issues/9115)) ([86a20f6](https://github.com/n8n-io/n8n/commit/86a20f656389474cb9fb26acf406de4e7af7b34c))


### Features

* **editor:** Add object keys that need bracket access to autocomplete ([#9088](https://github.com/n8n-io/n8n/issues/9088)) ([98bcd50](https://github.com/n8n-io/n8n/commit/98bcd50bab47e384ddcb6261aa91ba843cfa3f5a))
* **Github Node:** Add option to get pull requests ([#9094](https://github.com/n8n-io/n8n/issues/9094)) ([4d9000b](https://github.com/n8n-io/n8n/commit/4d9000bf27df5a2188a2d4a07d8e1e6a04f701d9))
* **Google Gemini Chat Model Node:** Add support for new Google Gemini models ([#9130](https://github.com/n8n-io/n8n/issues/9130)) ([f1215cd](https://github.com/n8n-io/n8n/commit/f1215cdb6bdfb18b7a170286c2d8e8c0deb617ff))
* **Summarize Node:** Option to continue when field to summarize can't be found in any items ([#9118](https://github.com/n8n-io/n8n/issues/9118)) ([d7abc30](https://github.com/n8n-io/n8n/commit/d7abc3010463ad21a9c162430485ebbb29d378b1))



# [1.37.0](https://github.com/n8n-io/n8n/compare/n8n@1.36.0...n8n@1.37.0) (2024-04-10)


### Bug Fixes

* **API:** Accept `settings.executionOrder` in workflow creation ([#9072](https://github.com/n8n-io/n8n/issues/9072)) ([0c90c7c](https://github.com/n8n-io/n8n/commit/0c90c7c8c1cde23c56b34fde264ea4e6ec0300b2))
* **AWS Bedrock Chat Model Node:** Improve filtering of Bedrock models & fix Claude 3 ([#9085](https://github.com/n8n-io/n8n/issues/9085)) ([cfaab0b](https://github.com/n8n-io/n8n/commit/cfaab0b829864f0d4900f7b36559c0bb1b2075a4))
* Continue on fail / error output support for chains and agents ([#9078](https://github.com/n8n-io/n8n/issues/9078)) ([f62800c](https://github.com/n8n-io/n8n/commit/f62800cd727ecd2b4a41fe6bbef411f8bc6f0a2e))
* **core:** Ensure `status` on Axios errors is available to the BE ([#9015](https://github.com/n8n-io/n8n/issues/9015)) ([744327c](https://github.com/n8n-io/n8n/commit/744327c20d909a0ccc2938dff8847d2b4756d9af))
* **core:** Ensure only leader handles waiting executions ([#9014](https://github.com/n8n-io/n8n/issues/9014)) ([217b07d](https://github.com/n8n-io/n8n/commit/217b07d735feab535916cff4baa72e500e3b80ee))
* **core:** Ensure TTL safeguard for test webhooks applies only to multi-main setup ([#9062](https://github.com/n8n-io/n8n/issues/9062)) ([ff81de3](https://github.com/n8n-io/n8n/commit/ff81de3313e8fd612104830b1b541b9dda392bb0))
* **core:** Fix `isLeader` check in `WaitTracker` constructor ([#9100](https://github.com/n8n-io/n8n/issues/9100)) ([c2f4d7d](https://github.com/n8n-io/n8n/commit/c2f4d7d7966db9fd7f7b19772757c71d493bf647))
* **core:** Remove binary data when deleting executions by filter ([#9056](https://github.com/n8n-io/n8n/issues/9056)) ([7bf0f90](https://github.com/n8n-io/n8n/commit/7bf0f900f193545c37849333e2964c89d96e25b2))
* **editor:** Add fallback for expression resolution in multi-output case ([#9045](https://github.com/n8n-io/n8n/issues/9045)) ([bcd39a1](https://github.com/n8n-io/n8n/commit/bcd39a110b4ca4c35b66340cec240dfc0c83132c))
* **editor:** Allow pinning of AI root nodes ([#9060](https://github.com/n8n-io/n8n/issues/9060)) ([32df171](https://github.com/n8n-io/n8n/commit/32df17104c13b713a36057ab9aaeef3fd03d9d24))
* **editor:** Canvas showing error toast when clicking outside of "import workflow by url" modal ([#9001](https://github.com/n8n-io/n8n/issues/9001)) ([f6ce81e](https://github.com/n8n-io/n8n/commit/f6ce81e7da74f80f81909b24f9675f7abcdb4265))
* **editor:** Connecting nodes to triggers when adding them together ([#9042](https://github.com/n8n-io/n8n/issues/9042)) ([f214362](https://github.com/n8n-io/n8n/commit/f2143620bab7c222e84e6cc0f5904805944e7163))
* **editor:** Drop outgoing connections on order changed event for nodes with dynamic outputs ([#9055](https://github.com/n8n-io/n8n/issues/9055)) ([3dd70a1](https://github.com/n8n-io/n8n/commit/3dd70a17e27fd312f949fb2fcccc0bf50ce9302e))
* **editor:** Expand range of allowed characters in expressions ([#9083](https://github.com/n8n-io/n8n/issues/9083)) ([3bcfef9](https://github.com/n8n-io/n8n/commit/3bcfef95f6c9e08b4429fd6b3fb9a67d7075b1aa))
* **editor:** Fix displaying logic of execution retry button ([#9061](https://github.com/n8n-io/n8n/issues/9061)) ([92f6cbf](https://github.com/n8n-io/n8n/commit/92f6cbfba36d1238e5b981c018b2a5365aabfe9c))
* **editor:** Fix execution with wait node ([#9051](https://github.com/n8n-io/n8n/issues/9051)) ([db4f8d4](https://github.com/n8n-io/n8n/commit/db4f8d49a3a87c4e893bb1496b0bc74bd804de64))
* **editor:** Fix issue with case insensitive tags ([#9071](https://github.com/n8n-io/n8n/issues/9071)) ([caea27d](https://github.com/n8n-io/n8n/commit/caea27dbb599fb81aee59e87236463127bcfab8c))
* **editor:** Fix issues in dark mode ([#9068](https://github.com/n8n-io/n8n/issues/9068)) ([7467aa3](https://github.com/n8n-io/n8n/commit/7467aa30e6c2a226cb9fee5f5d82fbd01db23e9e))
* **editor:** Issue showing Auth2 callback section when all properties are overriden ([#8999](https://github.com/n8n-io/n8n/issues/8999)) ([dff8f7a](https://github.com/n8n-io/n8n/commit/dff8f7ac94e0d215f4e2a204774857d240e7f79b))
* **editor:** Make share modal content scrollable ([#9025](https://github.com/n8n-io/n8n/issues/9025)) ([ec9fe98](https://github.com/n8n-io/n8n/commit/ec9fe98a357ad75349c6f64006ebbff7c95ff0fe))
* **editor:** Make Webhook node pinnable ([#9047](https://github.com/n8n-io/n8n/issues/9047)) ([042aa62](https://github.com/n8n-io/n8n/commit/042aa62fc2ddae2b9d39f4a92068c10bfe5bec14))
* **editor:** Prevent saving workflow while another save is in progress ([#9048](https://github.com/n8n-io/n8n/issues/9048)) ([3c9a1d2](https://github.com/n8n-io/n8n/commit/3c9a1d2da3aa7614ce1beec07654a8b2423f99bc))
* **editor:** Rerun failed nodes in manual executions ([#9050](https://github.com/n8n-io/n8n/issues/9050)) ([bc6575a](https://github.com/n8n-io/n8n/commit/bc6575afbb106ea22ae1ff7b1b9057ccb665a964))
* **editor:** UX improvements to mfa setup modal ([#9059](https://github.com/n8n-io/n8n/issues/9059)) ([4ac02dd](https://github.com/n8n-io/n8n/commit/4ac02dd5f46c78398186e94faabb2f8884c0f2ae))
* Fix missing input panel in node details view ([#9043](https://github.com/n8n-io/n8n/issues/9043)) ([71c54cb](https://github.com/n8n-io/n8n/commit/71c54cba52f5de26bd9c086390313c211ad0e574))
* **HTTP Request Node:** Duplicate key names support for form data  ([#9040](https://github.com/n8n-io/n8n/issues/9040)) ([3e231db](https://github.com/n8n-io/n8n/commit/3e231dbfe67b6dbe87f383daa8a52c5ae02edd92))
* **MySQL Node:** Query Parameters parse string to number ([#9011](https://github.com/n8n-io/n8n/issues/9011)) ([610ead9](https://github.com/n8n-io/n8n/commit/610ead9a3851eeee246313669d0ed9049c736a1a))
* **Summarization Chain Node:** 'Final Prompt to Combine' and 'Individual Summary Prompt' options ([#8391](https://github.com/n8n-io/n8n/issues/8391)) ([e47e4bf](https://github.com/n8n-io/n8n/commit/e47e4bf67152fae727374974fecf294aff56c257))
* Workflows executed from other workflows not stopping ([#9010](https://github.com/n8n-io/n8n/issues/9010)) ([0ac9851](https://github.com/n8n-io/n8n/commit/0ac985133be546f068f7f25b340c3bfdecadc08e))


### Features

* Add credential update and delete events to log streaming ([#9026](https://github.com/n8n-io/n8n/issues/9026)) ([f4f0a36](https://github.com/n8n-io/n8n/commit/f4f0a36fe1f8a792e3581849a0d8a78ce1e6f21a))
* Allow workflow execution even if it has errors ([#9037](https://github.com/n8n-io/n8n/issues/9037)) ([eaaefd7](https://github.com/n8n-io/n8n/commit/eaaefd76da6e9dbb86568aafdcb48b183b41fe40))
* Append item index suffix to an error message, if provided, and node has many input items ([#9070](https://github.com/n8n-io/n8n/issues/9070)) ([5793e56](https://github.com/n8n-io/n8n/commit/5793e5644aaf40abe620d8a0a4f76856b6c5ff83))
* **core:** Improve Langsmith traces for AI executions ([#9081](https://github.com/n8n-io/n8n/issues/9081)) ([936682e](https://github.com/n8n-io/n8n/commit/936682eeaae5f7cdbdb2afbf9c3bf9d85bcd964c))
* **core:** Prevent session hijacking ([#9057](https://github.com/n8n-io/n8n/issues/9057)) ([2826104](https://github.com/n8n-io/n8n/commit/28261047c399be0cc9c8d30015cc42b9410cebce))
* **Email Trigger (IMAP) Node:** Migrate from `imap-simple` to `@n8n/imap` ([#8899](https://github.com/n8n-io/n8n/issues/8899)) ([9f87cc2](https://github.com/n8n-io/n8n/commit/9f87cc25a020e03710bd64835c6547f9f12c1fe2))
* **JWT Node:** New node ([#9005](https://github.com/n8n-io/n8n/issues/9005)) ([0a9f6b3](https://github.com/n8n-io/n8n/commit/0a9f6b3de8f5548700e736b7d5f1d31c229595f5))
* **Postgres Node:** Options keepAlive and keepAliveInitialDelayMillis ([#9067](https://github.com/n8n-io/n8n/issues/9067)) ([58518b6](https://github.com/n8n-io/n8n/commit/58518b684b6c9495aa6efd0e815a8d01f102bbe4))



# [1.36.0](https://github.com/n8n-io/n8n/compare/n8n@1.35.0...n8n@1.36.0) (2024-04-03)


### Bug Fixes

* **editor:**  Issue with JSON editor getting cut off ([#9000](https://github.com/n8n-io/n8n/issues/9000)) ([4668db2](https://github.com/n8n-io/n8n/commit/4668db20fb6a47b4e417ab8f31407d13af9c70f8))
* **editor:** Fix canvas selection for touch devices that use mouse ([#9036](https://github.com/n8n-io/n8n/issues/9036)) ([286fa5c](https://github.com/n8n-io/n8n/commit/286fa5cd7eb5052d2c166145447f53b33174b62c))
* **editor:** Fix execution debug button ([#9018](https://github.com/n8n-io/n8n/issues/9018)) ([aac77e1](https://github.com/n8n-io/n8n/commit/aac77e1668d2b3fd96c2e77b4626b7b0ae7bf233))
* **editor:** Hover and active states not showing in execution list on dark mode ([#9002](https://github.com/n8n-io/n8n/issues/9002)) ([bead7eb](https://github.com/n8n-io/n8n/commit/bead7eb840b3c6c074364c6a44d001ea561fee1f))
* **editor:** UI enhancements and fixes for expression inputs ([#8996](https://github.com/n8n-io/n8n/issues/8996)) ([8788e2a](https://github.com/n8n-io/n8n/commit/8788e2a35bed261e13da5c92ee31bbb414d019a4))
* Prevent chat modal opening on 'Test workflow' click ([#9009](https://github.com/n8n-io/n8n/issues/9009)) ([3fd97e4](https://github.com/n8n-io/n8n/commit/3fd97e4c7299928a498e359b16f6f21eed9f0878))
* Stop listening button not working in NDV ([#9023](https://github.com/n8n-io/n8n/issues/9023)) ([02219dd](https://github.com/n8n-io/n8n/commit/02219dde2fa3c16145c3985272567b334b69dd54))


### Features

* Add Salesforce Trigger Node ([#8920](https://github.com/n8n-io/n8n/issues/8920)) ([571b613](https://github.com/n8n-io/n8n/commit/571b6135dd41ef983a822f210c09e3623e8ee605))
* Add Twilio Trigger Node ([#8859](https://github.com/n8n-io/n8n/issues/8859)) ([c204995](https://github.com/n8n-io/n8n/commit/c204995d9c5683d92cc7c7bd89c530ad3318b06d))
* **core:** Introduce AWS secrets manager as external secrets store ([#8982](https://github.com/n8n-io/n8n/issues/8982)) ([2aab78b](https://github.com/n8n-io/n8n/commit/2aab78b058f46c7b1692503a2b3b6bfb8939c128))
* **core:** Rate-limit login endpoint to mitigate brute force password guessing attacks ([#9028](https://github.com/n8n-io/n8n/issues/9028)) ([a6446fe](https://github.com/n8n-io/n8n/commit/a6446fe057749536344c4170395ce149340cd889))
* **editor:** Update templates links ([#9024](https://github.com/n8n-io/n8n/issues/9024)) ([4619dec](https://github.com/n8n-io/n8n/commit/4619dec285da14bb097df225a5682ed8babd82dd))
* **Webhook Node:** Overhaul ([#8889](https://github.com/n8n-io/n8n/issues/8889)) ([e84c27c](https://github.com/n8n-io/n8n/commit/e84c27c0cebd6fba135298ea18844045dcf55b4c))



# [1.35.0](https://github.com/n8n-io/n8n/compare/n8n@1.33.0...n8n@1.35.0) (2024-03-27)


### Bug Fixes

* **Anthropic Chat Model Node:** Fix detection of chat models in docker build & add support Claude Haiku ([#8953](https://github.com/n8n-io/n8n/issues/8953)) ([76041b8](https://github.com/n8n-io/n8n/commit/76041b8587fc5943ee80338774125d1fabb8e927))
* Chat Trigger exclude summarization node from valid ai nodes ([#8875](https://github.com/n8n-io/n8n/issues/8875)) ([4861556](https://github.com/n8n-io/n8n/commit/4861556a1c7da643fdc924f7f65dc89a7453744a))
* **Cohere Model Node:** Fix issue with credential test ([#8916](https://github.com/n8n-io/n8n/issues/8916)) ([4f0b52c](https://github.com/n8n-io/n8n/commit/4f0b52c45d1f165159787197fd41138059b13db6))
* **core:** Add missing `nodeCause` to paired item error ([#8976](https://github.com/n8n-io/n8n/issues/8976)) ([19d9e71](https://github.com/n8n-io/n8n/commit/19d9e71cb90d7085256496df8325564c13db3af4))
* **core:** Assign credential ownership correctly in source control import ([#8955](https://github.com/n8n-io/n8n/issues/8955)) ([260bc07](https://github.com/n8n-io/n8n/commit/260bc07ca9484b6e82cc9dc82c68a6c1c58f4a49))
* **core:** Ensure the generic OAuth2 API credential uses the OAuth2 credential test ([#8941](https://github.com/n8n-io/n8n/issues/8941)) ([079a114](https://github.com/n8n-io/n8n/commit/079a1147d41442bb7269d5e9da30e45019438ba2))
* **core:** Improve handling of invalid objects in `cleanupParameterData` (no-chanhelog) ([#8910](https://github.com/n8n-io/n8n/issues/8910)) ([33ab781](https://github.com/n8n-io/n8n/commit/33ab781aef1b9107f9ecc7ec22c9b264b4eaae63))
* **core:** Remove HTTP body for GET, HEAD, and OPTIONS requests ([#3621](https://github.com/n8n-io/n8n/issues/3621)) ([d85d0ec](https://github.com/n8n-io/n8n/commit/d85d0ecf45e8f256536bdd7cad6aab85971e8e43))
* **core:** Stringify all Luxon DateTimes in cleanupParameterData ([#8959](https://github.com/n8n-io/n8n/issues/8959)) ([1fb0dd4](https://github.com/n8n-io/n8n/commit/1fb0dd4f1c074ad6462d42bea030e3bafecef2ad))
* **core:** Update `follow-redirects` to address CVE-2024-28849 ([#8902](https://github.com/n8n-io/n8n/issues/8902)) ([a10120f](https://github.com/n8n-io/n8n/commit/a10120f74efa4c636f26eafc996e71bd372f8ee8))
* **editor:** Add proper scroll to Environments push modal ([#8883](https://github.com/n8n-io/n8n/issues/8883)) ([bcbff76](https://github.com/n8n-io/n8n/commit/bcbff760553058f8fb43b379130db0cd064fd869))
* **editor:** Fix accidental IDE code addition ([#8971](https://github.com/n8n-io/n8n/issues/8971)) ([117b57c](https://github.com/n8n-io/n8n/commit/117b57ccc5e3904d6ffc748d198d331f3008bcd3))
* **editor:** Fix an issue with an empty chat response if not in `output` property ([#8913](https://github.com/n8n-io/n8n/issues/8913)) ([024be62](https://github.com/n8n-io/n8n/commit/024be62693e96020c284116110944e90c7bcf1a8))
* **editor:** Fix design system component props ([#8923](https://github.com/n8n-io/n8n/issues/8923)) ([7176cd1](https://github.com/n8n-io/n8n/commit/7176cd1407e028ba8c543179b128c7e2ac9c0369))
* **editor:** Fix opening of chat window when executing a child node ([#8789](https://github.com/n8n-io/n8n/issues/8789)) ([5f53d76](https://github.com/n8n-io/n8n/commit/5f53d76e39395a8effdfeba0677f333b509ec8c8))
* **editor:** Fix source control docs link in add workflow button tooltip ([#8891](https://github.com/n8n-io/n8n/issues/8891)) ([a92d8bf](https://github.com/n8n-io/n8n/commit/a92d8bfc6e2fcc4bf79fc3f6564fdb864ccd3f41))
* **editor:** Improve expression editor performance by removing watchers ([#8900](https://github.com/n8n-io/n8n/issues/8900)) ([a5261d6](https://github.com/n8n-io/n8n/commit/a5261d6ebb8fa4ac8796b04920a4fa4bc43bb397))
* **editor:** Make inputs in the filter component regular inputs by default ([#8980](https://github.com/n8n-io/n8n/issues/8980)) ([295b650](https://github.com/n8n-io/n8n/commit/295b650fb8bd423eba506bc09a5746451db2c085))
* **editor:** Nodes connectors improvements ([#8945](https://github.com/n8n-io/n8n/issues/8945)) ([264f918](https://github.com/n8n-io/n8n/commit/264f918d9720e2a11ec011993df1e7a4cb776882))
* **editor:** Remove `isOwner` from IUser interface ([#8888](https://github.com/n8n-io/n8n/issues/8888)) ([6955e89](https://github.com/n8n-io/n8n/commit/6955e8991ca2ec13e6298c3c18ec2b28853ceda4))
* **editor:** Use bracket notation for all invalid identifiers in expressions ([#8933](https://github.com/n8n-io/n8n/issues/8933)) ([0e4216d](https://github.com/n8n-io/n8n/commit/0e4216d7afb6a09547ae575fcfd13e9fac22b350))
* **MySQL Node:** Set paired items correctly in single query batch mode ([#8940](https://github.com/n8n-io/n8n/issues/8940)) ([89df277](https://github.com/n8n-io/n8n/commit/89df277b80002f46d198d7b8bd3d81f5b815c116))
* OpenAI Node function to preserve original tools after node execution ([#8872](https://github.com/n8n-io/n8n/issues/8872)) ([054a4fc](https://github.com/n8n-io/n8n/commit/054a4fce1a8163f2201efd846938b909c7d0e394))
* Overhaul expression error messages related to paired item ([#8765](https://github.com/n8n-io/n8n/issues/8765)) ([45461c8](https://github.com/n8n-io/n8n/commit/45461c8cb57aa22697e58c6c52a25ab1d6d633d9))
* **Pinecone Vector Store Node:** Fix vector store nodes execution issue ([#8968](https://github.com/n8n-io/n8n/issues/8968)) ([323b901](https://github.com/n8n-io/n8n/commit/323b9016c8c2409d5b72c6cc2fdb0cf6f2ba118b))
* Validate custom tool names for forbidden chars ([#8878](https://github.com/n8n-io/n8n/issues/8878)) ([edce632](https://github.com/n8n-io/n8n/commit/edce632ee62fdb9485d1ed07ead7dd3c0d2afcf8))


### Features

* Add AI Error Debugging using OpenAI ([#8805](https://github.com/n8n-io/n8n/issues/8805)) ([948c383](https://github.com/n8n-io/n8n/commit/948c383999726278377f74987cd36ed6a5b39b7b))
* Add Onedrive Trigger Node ([#8742](https://github.com/n8n-io/n8n/issues/8742)) ([ff8dd4e](https://github.com/n8n-io/n8n/commit/ff8dd4e604216203800d9b12fd5f1105356cf03e))
* **core:** Add support for SQLite connection pooling ([#8722](https://github.com/n8n-io/n8n/issues/8722)) ([c4c319d](https://github.com/n8n-io/n8n/commit/c4c319d7cfb30772cca248a0039fd8e2b1c99eb7))
* **editor:** Add missing extension methods for expressions ([#8845](https://github.com/n8n-io/n8n/issues/8845)) ([5e84c2a](https://github.com/n8n-io/n8n/commit/5e84c2ab89c7d0e4365b32b1c94a9c10cea56cb9))
* **editor:** Add type information to autocomplete dropdown ([#8843](https://github.com/n8n-io/n8n/issues/8843)) ([d7bfd45](https://github.com/n8n-io/n8n/commit/d7bfd45333cc9780ae5f1424f33de2093bd1a2f9))
* **editor:** Block the frontend when trying to access n8n from another host over http ([#8906](https://github.com/n8n-io/n8n/issues/8906)) ([669bd83](https://github.com/n8n-io/n8n/commit/669bd830e9b1b0f986d8a8b4525d0bdc3e3c0bd7))
* **editor:** Refactor expression editors and mixins to composition API ([#8894](https://github.com/n8n-io/n8n/issues/8894)) ([0c179e4](https://github.com/n8n-io/n8n/commit/0c179e4e511e4e6075d390afc025c93630ef3241))
* **editor:** Release `@n8n/chat@0.9.1` ([#8918](https://github.com/n8n-io/n8n/issues/8918)) ([e0c303c](https://github.com/n8n-io/n8n/commit/e0c303c6c10145a2ef72daaf4142315cf65c839a))
* **editor:** Show tip when user can type dot after an expression ([#8931](https://github.com/n8n-io/n8n/issues/8931)) ([160dfd3](https://github.com/n8n-io/n8n/commit/160dfd383d79fc44be79e5a071dc5f6c6b67469b))
* Fetch user cloud role and pass it on in website links ([#8942](https://github.com/n8n-io/n8n/issues/8942)) ([666867a](https://github.com/n8n-io/n8n/commit/666867a236bce519dbd1a8f9162d4ced1b80d567))
* Telemetry include basic llm optional promps, trigger on save workflow event ([#8981](https://github.com/n8n-io/n8n/issues/8981)) ([335f363](https://github.com/n8n-io/n8n/commit/335f363ca16814d6ca1a8a92fc9da145b8eed990))



## [1.34.2](https://github.com/n8n-io/n8n/compare/n8n@1.34.1...n8n@1.34.2) (2024-03-26)


### Bug Fixes

* **editor:** Nodes connectors improvements ([#8945](https://github.com/n8n-io/n8n/issues/8945)) ([6310e36](https://github.com/n8n-io/n8n/commit/6310e36c8eaf331b4116666677a82b9a75f862dc))
* **Pinecone Vector Store Node:** Fix vector store nodes execution issue ([#8968](https://github.com/n8n-io/n8n/issues/8968)) ([9bd14c0](https://github.com/n8n-io/n8n/commit/9bd14c053c8b5410a49d3a5f3354e5ed0feed3b3))



## [1.34.1](https://github.com/n8n-io/n8n/compare/n8n@1.34.0...n8n@1.34.1) (2024-03-25)


### Bug Fixes

* **Anthropic Chat Model Node:** Fix detection of chat models in docker build & add support Claude Haiku ([#8953](https://github.com/n8n-io/n8n/issues/8953)) ([becc804](https://github.com/n8n-io/n8n/commit/becc8045646bfd6ace40895288f5f5a323c7fc8e))
* **core:** Ensure the generic OAuth2 API credential uses the OAuth2 credential test ([#8941](https://github.com/n8n-io/n8n/issues/8941)) ([578f01a](https://github.com/n8n-io/n8n/commit/578f01a02ccdef014938dfd3194bae182e02442a))
* **core:** Stringify all Luxon DateTimes in cleanupParameterData ([#8959](https://github.com/n8n-io/n8n/issues/8959)) ([58d9983](https://github.com/n8n-io/n8n/commit/58d9983d0efd50d01d8406b949a4e7a3db63e465))
* **editor:** Fix opening of chat window when executing a child node ([#8789](https://github.com/n8n-io/n8n/issues/8789)) ([e695927](https://github.com/n8n-io/n8n/commit/e69592784965f24a9c061f9a10bae58a72d2cc69))
* **editor:** Use bracket notation for all invalid identifiers in expressions ([#8933](https://github.com/n8n-io/n8n/issues/8933)) ([1316f2d](https://github.com/n8n-io/n8n/commit/1316f2d682d847d314e0175781a4fe7561205324))
* **MySQL Node:** Set paired items correctly in single query batch mode ([#8940](https://github.com/n8n-io/n8n/issues/8940)) ([5d129ba](https://github.com/n8n-io/n8n/commit/5d129baa2df3ff9cb2a608d4162e645e5dc64ae6))
* Overhaul expression error messages related to paired item ([#8765](https://github.com/n8n-io/n8n/issues/8765)) ([09654f9](https://github.com/n8n-io/n8n/commit/09654f9dcca77710d91b3a6543ce50fb933eb870))



# [1.34.0](https://github.com/n8n-io/n8n/compare/n8n@1.33.0...n8n@1.34.0) (2024-03-20)


### Bug Fixes

* Chat Trigger exclude summarization node from valid ai nodes ([#8875](https://github.com/n8n-io/n8n/issues/8875)) ([4861556](https://github.com/n8n-io/n8n/commit/4861556a1c7da643fdc924f7f65dc89a7453744a))
* **Cohere Model Node:** Fix issue with credential test ([#8916](https://github.com/n8n-io/n8n/issues/8916)) ([4f0b52c](https://github.com/n8n-io/n8n/commit/4f0b52c45d1f165159787197fd41138059b13db6))
* **core:** Improve handling of invalid objects in `cleanupParameterData` (no-chanhelog) ([#8910](https://github.com/n8n-io/n8n/issues/8910)) ([33ab781](https://github.com/n8n-io/n8n/commit/33ab781aef1b9107f9ecc7ec22c9b264b4eaae63))
* **core:** Remove HTTP body for GET, HEAD, and OPTIONS requests ([#3621](https://github.com/n8n-io/n8n/issues/3621)) ([d85d0ec](https://github.com/n8n-io/n8n/commit/d85d0ecf45e8f256536bdd7cad6aab85971e8e43))
* **core:** Update `follow-redirects` to address CVE-2024-28849 ([#8902](https://github.com/n8n-io/n8n/issues/8902)) ([a10120f](https://github.com/n8n-io/n8n/commit/a10120f74efa4c636f26eafc996e71bd372f8ee8))
* **editor:** Add proper scroll to Environments push modal ([#8883](https://github.com/n8n-io/n8n/issues/8883)) ([bcbff76](https://github.com/n8n-io/n8n/commit/bcbff760553058f8fb43b379130db0cd064fd869))
* **editor:** Fix an issue with an empty chat response if not in `output` property ([#8913](https://github.com/n8n-io/n8n/issues/8913)) ([024be62](https://github.com/n8n-io/n8n/commit/024be62693e96020c284116110944e90c7bcf1a8))
* **editor:** Fix design system component props ([#8923](https://github.com/n8n-io/n8n/issues/8923)) ([7176cd1](https://github.com/n8n-io/n8n/commit/7176cd1407e028ba8c543179b128c7e2ac9c0369))
* **editor:** Fix source control docs link in add workflow button tooltip ([#8891](https://github.com/n8n-io/n8n/issues/8891)) ([a92d8bf](https://github.com/n8n-io/n8n/commit/a92d8bfc6e2fcc4bf79fc3f6564fdb864ccd3f41))
* **editor:** Improve expression editor performance by removing watchers ([#8900](https://github.com/n8n-io/n8n/issues/8900)) ([a5261d6](https://github.com/n8n-io/n8n/commit/a5261d6ebb8fa4ac8796b04920a4fa4bc43bb397))
* **editor:** Remove `isOwner` from IUser interface ([#8888](https://github.com/n8n-io/n8n/issues/8888)) ([6955e89](https://github.com/n8n-io/n8n/commit/6955e8991ca2ec13e6298c3c18ec2b28853ceda4))
* OpenAI Node function to preserve original tools after node execution ([#8872](https://github.com/n8n-io/n8n/issues/8872)) ([054a4fc](https://github.com/n8n-io/n8n/commit/054a4fce1a8163f2201efd846938b909c7d0e394))
* Validate custom tool names for forbidden chars ([#8878](https://github.com/n8n-io/n8n/issues/8878)) ([edce632](https://github.com/n8n-io/n8n/commit/edce632ee62fdb9485d1ed07ead7dd3c0d2afcf8))


### Features

* Add AI Error Debugging using OpenAI ([#8805](https://github.com/n8n-io/n8n/issues/8805)) ([948c383](https://github.com/n8n-io/n8n/commit/948c383999726278377f74987cd36ed6a5b39b7b))
* Add Onedrive Trigger Node ([#8742](https://github.com/n8n-io/n8n/issues/8742)) ([ff8dd4e](https://github.com/n8n-io/n8n/commit/ff8dd4e604216203800d9b12fd5f1105356cf03e))
* **core:** Add support for SQLite connection pooling ([#8722](https://github.com/n8n-io/n8n/issues/8722)) ([c4c319d](https://github.com/n8n-io/n8n/commit/c4c319d7cfb30772cca248a0039fd8e2b1c99eb7))
* **editor:** Add missing extension methods for expressions ([#8845](https://github.com/n8n-io/n8n/issues/8845)) ([5e84c2a](https://github.com/n8n-io/n8n/commit/5e84c2ab89c7d0e4365b32b1c94a9c10cea56cb9))
* **editor:** Add type information to autocomplete dropdown ([#8843](https://github.com/n8n-io/n8n/issues/8843)) ([d7bfd45](https://github.com/n8n-io/n8n/commit/d7bfd45333cc9780ae5f1424f33de2093bd1a2f9))
* **editor:** Block the frontend when trying to access n8n from another host over http ([#8906](https://github.com/n8n-io/n8n/issues/8906)) ([669bd83](https://github.com/n8n-io/n8n/commit/669bd830e9b1b0f986d8a8b4525d0bdc3e3c0bd7))
* **editor:** Refactor expression editors and mixins to composition API ([#8894](https://github.com/n8n-io/n8n/issues/8894)) ([0c179e4](https://github.com/n8n-io/n8n/commit/0c179e4e511e4e6075d390afc025c93630ef3241))
* **editor:** Release `@n8n/chat@0.9.1` ([#8918](https://github.com/n8n-io/n8n/issues/8918)) ([e0c303c](https://github.com/n8n-io/n8n/commit/e0c303c6c10145a2ef72daaf4142315cf65c839a))

# [1.33.0](https://github.com/n8n-io/n8n/compare/n8n@1.32.0...n8n@1.33.0) (2024-03-13)


### Bug Fixes

* **core:** Always register webhooks on startup ([#8830](https://github.com/n8n-io/n8n/issues/8830)) ([c6f6254](https://github.com/n8n-io/n8n/commit/c6f6254c0e5197d4c0ba19aa52a1714e991a33b2))
* **core:** Add fallback for pairedItem info in runPartialWorkflow ([#8842](https://github.com/n8n-io/n8n/issues/8842)) ([bd465d3](https://github.com/n8n-io/n8n/commit/bd465d394aa9eb74a127748ebda1fc84a158d236))
* **core:** Display readable error when manual executions contains large payload ([#8834](https://github.com/n8n-io/n8n/issues/8834)) ([261b9c7](https://github.com/n8n-io/n8n/commit/261b9c73d6fbb06610839b80bb1f89125893b89b))
* **core:** Ignore semver range when upgrading comunity packages ([#8863](https://github.com/n8n-io/n8n/issues/8863)) ([11173a0](https://github.com/n8n-io/n8n/commit/11173a011468160999e2c3f4a380741edf3ba37e))
* **editor:** Allow sharee to use workflows with http request node without credential access ([#8841](https://github.com/n8n-io/n8n/issues/8841)) ([bde4c6c](https://github.com/n8n-io/n8n/commit/bde4c6c7a19b7275cabbbc3e4d0c5ec14be54769))
* **editor:** Disable pinning for root nodes from canvas ([#8848](https://github.com/n8n-io/n8n/issues/8848)) ([e10fa37](https://github.com/n8n-io/n8n/commit/e10fa379d3212fd9fd964d8468add07b257af7e1))
* **editor:** Fix workflow card open action ([#8839](https://github.com/n8n-io/n8n/issues/8839)) ([dd40570](https://github.com/n8n-io/n8n/commit/dd405700568acdc893358ef239e8f8637da66307))
* **editor:** Make inputs in the filter component expressions by default ([#8784](https://github.com/n8n-io/n8n/issues/8784)) ([6e2aa40](https://github.com/n8n-io/n8n/commit/6e2aa405fcdff3f9b1f75d9e22719f6c0c500aa9))
* **editor:** Improve filter component error handling ([#8832](https://github.com/n8n-io/n8n/issues/8832)) ([76fe960](https://github.com/n8n-io/n8n/commit/76fe960a7613b51a95720504537112fba13bb1d6))
* **GitHub Document Loader Node:** Fix issue with ignore paths not working correctly ([#8798](https://github.com/n8n-io/n8n/issues/8798)) ([c8d589c](https://github.com/n8n-io/n8n/commit/c8d589cce74dc1267d8058fc8f0b61b516969b79))
* **Notion Node:** Regex for block id ([#8860](https://github.com/n8n-io/n8n/issues/8860)) ([a1f6c57](https://github.com/n8n-io/n8n/commit/a1f6c570d63a8acd7b623fb039bfdbcd017dc022))
* **OpenAI Node:** text > message hide tools connector for unsupported models ([#8866](https://github.com/n8n-io/n8n/issues/8866)) ([cef7c24](https://github.com/n8n-io/n8n/commit/cef7c24b7779000386e45dae4c3ee25dd2d6251b))


### Features

* **editor:** Add more AI node info to telemetry ([#8827](https://github.com/n8n-io/n8n/issues/8827)) ([ed6dc86](https://github.com/n8n-io/n8n/commit/ed6dc86d60e30ed6e5992e0bd1b27e8cd59d689b))
* **editor:** Add sections to autocomplete dropdown ([#8720](https://github.com/n8n-io/n8n/issues/8720)) ([9b4618d](https://github.com/n8n-io/n8n/commit/9b4618dd5e58337b73e8804f11d7aca9a9bf1dc3))
* **editor:** Help users discover expressions when using drag n drop ([#8869](https://github.com/n8n-io/n8n/issues/8869)) ([e78cc2d](https://github.com/n8n-io/n8n/commit/e78cc2d8d2d22bdea30af45edd8e319d479deb55))
* **editor:** Improve errors in output panel ([#8644](https://github.com/n8n-io/n8n/issues/8644)) ([5301323](https://github.com/n8n-io/n8n/commit/5301323906663a64a3042bd2f8946e5f1e3f6293))
* **Pinecone Vector Store Node:** Support serverless environments ([#8849](https://github.com/n8n-io/n8n/issues/8849)) ([a136a73](https://github.com/n8n-io/n8n/commit/a136a73e4e15b5d2d1c11ef90caec75d0318f829))
* **Wordpress Node:** Support WordPress pages ([#8852](https://github.com/n8n-io/n8n/issues/8852)) ([a678e85](https://github.com/n8n-io/n8n/commit/a678e8570b72514b0b5da6fcac4da5534d05fee8))



# [1.32.0](https://github.com/n8n-io/n8n/compare/n8n@1.31.0...n8n@1.32.0) (2024-03-06)


### Bug Fixes

* AI agents, throw error on duplicate names in dynamic tools ([#8766](https://github.com/n8n-io/n8n/issues/8766)) ([75e4df1](https://github.com/n8n-io/n8n/commit/75e4df138fc103a3370239e906b9e600dc14c835))
* **Basic LLM Chain Node:** Fix retrieving of prompt parameter for v1.3 of the node ([#8817](https://github.com/n8n-io/n8n/issues/8817)) ([82f66c8](https://github.com/n8n-io/n8n/commit/82f66c87e0e6969535559aaa879fe1f66c6ff31f))
* **editor:** Fix NDV output tabs resetting on any click ([#8808](https://github.com/n8n-io/n8n/issues/8808)) ([c7c1767](https://github.com/n8n-io/n8n/commit/c7c17673cbdffd328032c9ec09be17c1f9018a4e))
* **editor:** Fix opening of node creator for sub-nodes connection hint link ([#8809](https://github.com/n8n-io/n8n/issues/8809)) ([df064af](https://github.com/n8n-io/n8n/commit/df064af6451cae0d5e389abae98fd9516b448272))
* **editor:** Fix retrieving of messages from memory in chat modal ([#8807](https://github.com/n8n-io/n8n/issues/8807)) ([bfda8ea](https://github.com/n8n-io/n8n/commit/bfda8ead0c449b262d57f14c1e8a077d21bac441))
* **editor:** Set correct type for right input in filter component ([#8771](https://github.com/n8n-io/n8n/issues/8771)) ([5d54663](https://github.com/n8n-io/n8n/commit/5d5466343e61125c0682d65a6829cbaf816d5a90))
* **editor:** Update assignment hint when user hovers table row ([#8782](https://github.com/n8n-io/n8n/issues/8782)) ([8c993aa](https://github.com/n8n-io/n8n/commit/8c993aa59dd6712703d5cc0a84949b0fa7dd874a))
* **editor:** Upgrade sanitize-html to address CVE-2024-21501 ([#8816](https://github.com/n8n-io/n8n/issues/8816)) ([a3e9e3d](https://github.com/n8n-io/n8n/commit/a3e9e3db62f9794fe4b3ae414a2d252edb6196aa))
* **Google Drive Node:** Add supportsAllDrives: true to update and download ([#8786](https://github.com/n8n-io/n8n/issues/8786)) ([11a5331](https://github.com/n8n-io/n8n/commit/11a5331e038fc383e454230dd9996015d7ce9b16))
* **HubSpot Node:** Include properties for contact and deal in getAll operation ([#8772](https://github.com/n8n-io/n8n/issues/8772)) ([08e2b06](https://github.com/n8n-io/n8n/commit/08e2b068fb241b3e44eebbc8d6053603d977ca32))
* **n8n Form Trigger Node:** Do not open pop up when data is pinned in trigger ([#8781](https://github.com/n8n-io/n8n/issues/8781)) ([0481e6e](https://github.com/n8n-io/n8n/commit/0481e6e6e7259cef5f4ac1c88dd0b45ef402f166))
* **OpenAI Node:** Message text operation parameters case fix ([#8804](https://github.com/n8n-io/n8n/issues/8804)) ([e38e96b](https://github.com/n8n-io/n8n/commit/e38e96bbec4a5f355ab0a8bb87bad3787032e9c5))
* Simplify Structured Output Parser wrapping and fix auto-fixing output parser ([#8778](https://github.com/n8n-io/n8n/issues/8778)) ([7d82dc1](https://github.com/n8n-io/n8n/commit/7d82dc1ea8c86c2a3575c3629b29af3cfb709f44))
* **TheHive 5 Node:** The Hive - Custom fields are no longer working ([#8780](https://github.com/n8n-io/n8n/issues/8780)) ([961d6b9](https://github.com/n8n-io/n8n/commit/961d6b9266344e221e21a771546b49c0c13ea80c))
* **Wait Node:** Change default wait period to 5 seconds ([#8783](https://github.com/n8n-io/n8n/issues/8783)) ([a521e7a](https://github.com/n8n-io/n8n/commit/a521e7a54d746189f098ae31fc06a92975dab5a9))


### Features

* Chat Memory Manager group messages option, on insert delete return confirmation of success instead of messages ([#8757](https://github.com/n8n-io/n8n/issues/8757)) ([246bfb9](https://github.com/n8n-io/n8n/commit/246bfb9ad4349cc17c2df64b357ddb96f794dfc5))
* **core:** Update hashing strategy for JWTs ([#8810](https://github.com/n8n-io/n8n/issues/8810)) ([cdec7c9](https://github.com/n8n-io/n8n/commit/cdec7c9334ef83a7e667a8bd5a649f165402f4e5))
* **Notion Node:** Continue on fail support ([#8788](https://github.com/n8n-io/n8n/issues/8788)) ([4850f6a](https://github.com/n8n-io/n8n/commit/4850f6a9cca3ae5b3a08e8b68d5404293367465a))
* Track node errors on PostHog ([#8774](https://github.com/n8n-io/n8n/issues/8774)) ([35f6826](https://github.com/n8n-io/n8n/commit/35f6826150ed91c679c855aa4ce5d1f5d5e072bd))


### Performance Improvements

* Upgrade Vue ([#8806](https://github.com/n8n-io/n8n/issues/8806)) ([1600433](https://github.com/n8n-io/n8n/commit/16004331b13d5d4cf3d379ab9c98fc898db14eeb))



# [1.31.0](https://github.com/n8n-io/n8n/compare/n8n@1.30.0...n8n@1.31.0) (2024-02-28)


### Bug Fixes

* **core:** Ensure `maxRedirects` is used for any http request defining it ([#8706](https://github.com/n8n-io/n8n/issues/8706)) ([246c988](https://github.com/n8n-io/n8n/commit/246c988b9373a838086f37e603ec2827cf849588))
* **core:** Fix pairedItem issue with partial manual executions ([#8575](https://github.com/n8n-io/n8n/issues/8575)) ([a29b41e](https://github.com/n8n-io/n8n/commit/a29b41ec55d8a0cf5610a53087e455b7e649b8bc))
* **Default Data Loader Node:** Fix binary data loader in s3 mode ([#8626](https://github.com/n8n-io/n8n/issues/8626)) ([a5e6f59](https://github.com/n8n-io/n8n/commit/a5e6f5928ae39f19d6cb55a234818e776141e325))
* **editor:** Do not break NDV for version-less nodes ([#8714](https://github.com/n8n-io/n8n/issues/8714)) ([8a88d15](https://github.com/n8n-io/n8n/commit/8a88d156847852b38e1fd13f3b9240887491a665))
* **editor:** Hide previous execution data for sub-nodes in debug mode if it has execution error ([#8710](https://github.com/n8n-io/n8n/issues/8710)) ([a973b9c](https://github.com/n8n-io/n8n/commit/a973b9c077d28faa45b527cf6e0f0e6644cf354a))
* **editor:** Update Filter component state when value is updated ([#8684](https://github.com/n8n-io/n8n/issues/8684)) ([3ba2cdc](https://github.com/n8n-io/n8n/commit/3ba2cdcadbf4df4e4521cb03bf63f13a32a926a5))
* Fix execution error when using AI chain nodes with non-chat model ([#8724](https://github.com/n8n-io/n8n/issues/8724)) ([0882dc0](https://github.com/n8n-io/n8n/commit/0882dc0ce9ad4c9260390f99be56df2d6f7b5e86))
* **Postgres Trigger Node:** `closeFunction` errors should not prevent a workflow from being deactivated ([#8738](https://github.com/n8n-io/n8n/issues/8738)) ([7012577](https://github.com/n8n-io/n8n/commit/7012577fce796c6d18ab8081f90014a8cded7391))
* Send user id when setting up an account ([#8639](https://github.com/n8n-io/n8n/issues/8639)) ([27f3166](https://github.com/n8n-io/n8n/commit/27f3166272455627a2d2f851a286126310a4d5b5))
* **Trello Node:** Remove GET request body ([#8715](https://github.com/n8n-io/n8n/issues/8715)) ([8c4a744](https://github.com/n8n-io/n8n/commit/8c4a744c56ce84984ed837583cdfd7a296de5090))
* Wrong prompt input key for sql agent ([#8708](https://github.com/n8n-io/n8n/issues/8708)) ([7c1cf33](https://github.com/n8n-io/n8n/commit/7c1cf33616eb1990a9d6d7f4b93e91575f2cddc8))


### Features

* Add env variables to support exposing `/workflows/demo` route and `/nodes.json` route ([#8506](https://github.com/n8n-io/n8n/issues/8506)) ([4b01335](https://github.com/n8n-io/n8n/commit/4b01335aa45d93b0e4f2b7c69503430f1bcca28a))
* Add Outlook Trigger Node ([#8656](https://github.com/n8n-io/n8n/issues/8656)) ([720ae1b](https://github.com/n8n-io/n8n/commit/720ae1b96b4c6fd644bad60191c35d8d598ad666))
* Add support for Ollama embeddings API ([#8732](https://github.com/n8n-io/n8n/issues/8732)) ([15490ad](https://github.com/n8n-io/n8n/commit/15490ad1d47c4f0d5c3f9eb350b2a1bcad4bbec0))
* **AI Agent Node:** Allow use of Azure Chat model for OpenAI Functions agent ([#8725](https://github.com/n8n-io/n8n/issues/8725)) ([d03d927](https://github.com/n8n-io/n8n/commit/d03d9276f923d541f9c9ef86b8dc232f2737e30b))
* Allow instance owners and admins to edit all credentials ([#8716](https://github.com/n8n-io/n8n/issues/8716)) ([7371708](https://github.com/n8n-io/n8n/commit/737170893d17108098c14db6be80071e8ef51930))
* **editor:** AI Floating Nodes ([#8703](https://github.com/n8n-io/n8n/issues/8703)) ([41b191e](https://github.com/n8n-io/n8n/commit/41b191e0552aa2d92d442d1dea05913e8b386d4d))
* **editor:** Retrieve previous chat message on arrow-up ([#8696](https://github.com/n8n-io/n8n/issues/8696)) ([246f8cf](https://github.com/n8n-io/n8n/commit/246f8cfcc3acdeb323849c94542fc4ad028c4f77))
* No expression error when node hasn’t executed ([#8448](https://github.com/n8n-io/n8n/issues/8448)) ([f9a99ec](https://github.com/n8n-io/n8n/commit/f9a99ec0295499d95534d64e016f70339a56956b))
* Session is selector for memory nodes ([#8736](https://github.com/n8n-io/n8n/issues/8736)) ([2aaf211](https://github.com/n8n-io/n8n/commit/2aaf211dfc270920a4885a2b086b98ab8a3c2af6))
* SQL agent improvements ([#8709](https://github.com/n8n-io/n8n/issues/8709)) ([0952430](https://github.com/n8n-io/n8n/commit/09524304e6a8d1fdcdfe6340b71a5a443b942d6d))



# [1.30.0](https://github.com/n8n-io/n8n/compare/n8n@1.29.0...n8n@1.30.0) (2024-02-21)


### Bug Fixes

* **AwsS3 Node:** Use location constrain ([#8654](https://github.com/n8n-io/n8n/issues/8654)) ([c73aeee](https://github.com/n8n-io/n8n/commit/c73aeeec3d296b3a6e203eba4513f6bd4bb65732))
* **core:** Apply correct hostname to redirected requests ([#8674](https://github.com/n8n-io/n8n/issues/8674)) ([0e36aeb](https://github.com/n8n-io/n8n/commit/0e36aeb421997948ef5d5170fa8d9b50d25b852d))
* **core:** Define `SHELL` env variable on docker images ([#8670](https://github.com/n8n-io/n8n/issues/8670)) ([e1a4fde](https://github.com/n8n-io/n8n/commit/e1a4fde207e392c372e3876946d6a5740721e253))
* **editor:** Correctly set condition operator when changed ([#8700](https://github.com/n8n-io/n8n/issues/8700)) ([23a1bc4](https://github.com/n8n-io/n8n/commit/23a1bc40a2eb8d340eea635a48c75f59369095bb))
* **editor:** Escape node names with quotes in autocomplete and drag'n'drop ([#8663](https://github.com/n8n-io/n8n/issues/8663)) ([890c2bd](https://github.com/n8n-io/n8n/commit/890c2bd52bd2ccd94fbc2e626dceda30554f9e82))
* **editor:** Filter component: do not clear expression when changing operator ([#8635](https://github.com/n8n-io/n8n/issues/8635)) ([66cbe54](https://github.com/n8n-io/n8n/commit/66cbe54e1d0ec48a36e6b6b15aaf7201970932e7))
* **editor:** Fix node runData and pinned data check on manual run ([#8669](https://github.com/n8n-io/n8n/issues/8669)) ([40c7f77](https://github.com/n8n-io/n8n/commit/40c7f77a35ef4e9bd4dbd9f28886b1b9e6af416f))
* **editor:** Fix SQL editors not always re-rendering when query changes ([#8621](https://github.com/n8n-io/n8n/issues/8621)) ([8e9d310](https://github.com/n8n-io/n8n/commit/8e9d3106a5792a182753e4030c135893f8bad27e))
* **editor:** Fix unnecessary execution of nodes when there is pin data ([#8567](https://github.com/n8n-io/n8n/issues/8567)) ([46fe544](https://github.com/n8n-io/n8n/commit/46fe544b9a38ea81093d846917af970141b8c86a))
* **editor:** Handle drag-n-dropping from other nodes in assignment component ([#8661](https://github.com/n8n-io/n8n/issues/8661)) ([c943a51](https://github.com/n8n-io/n8n/commit/c943a51a28953c2ecd0f3ae4849fd8a0de187bfc))
* **editor:** Send protocol and n8n version in templates destination parameter, stop redirecting template preview page to website ([#8691](https://github.com/n8n-io/n8n/issues/8691)) ([a573146](https://github.com/n8n-io/n8n/commit/a57314613586841c14e86f009bf42793545c33f8))
* **editor:** Use proper composable for localization ([#8660](https://github.com/n8n-io/n8n/issues/8660)) ([9c0fe41](https://github.com/n8n-io/n8n/commit/9c0fe413d9beb669b8b9807f98569f46a1682855))
* **editor:** Wrap expressions in resource locator component ([#8673](https://github.com/n8n-io/n8n/issues/8673)) ([e2f2fc9](https://github.com/n8n-io/n8n/commit/e2f2fc910df5ee06fa0b57b85689b5674b6774ba))
* **Extract From File Node:** Make binary data work with any backend  ([#8647](https://github.com/n8n-io/n8n/issues/8647)) ([d33d953](https://github.com/n8n-io/n8n/commit/d33d953497d25a50f17c71f7ecc7b9cc6332816e))
* **FTP Node:** Continue of fail looping support with paired item ([#8659](https://github.com/n8n-io/n8n/issues/8659)) ([3279762](https://github.com/n8n-io/n8n/commit/327976222114956584fdb2de51c914ad57382988))
* **FTP Node:** Fix "Maximum call stack size exceeded" error when dealing with too many files ([#8657](https://github.com/n8n-io/n8n/issues/8657)) ([5063674](https://github.com/n8n-io/n8n/commit/506367453c46485e5baff6510ce0c653ca4cc4e4))
* **Google Calendar Node:** Errors with after/before options ([#8628](https://github.com/n8n-io/n8n/issues/8628)) ([bee17dd](https://github.com/n8n-io/n8n/commit/bee17dd6cc4eaabc252602a02d4ec109f42ef926))
* **GraphQL Node:** Fix request format JSON error ([#8646](https://github.com/n8n-io/n8n/issues/8646)) ([bd4b50c](https://github.com/n8n-io/n8n/commit/bd4b50cf0882553b2ecb7f0b9bd93d154f775b4f))
* **Postgres Node:** Close connection pool only if it's not already closed or closing ([#8690](https://github.com/n8n-io/n8n/issues/8690)) ([457cac4](https://github.com/n8n-io/n8n/commit/457cac4cf9f7093d48e9f4ccb0021423c18f0b8b))


### Features

* **AI Agent Node:** Whitelist Azure Chat model for Agent ([#8699](https://github.com/n8n-io/n8n/issues/8699)) ([40aecd1](https://github.com/n8n-io/n8n/commit/40aecd1715d4fec7e5024167e89d4b2171ec19e8))
* **core:** Add support for $("NodeName").isExecuted ([#8683](https://github.com/n8n-io/n8n/issues/8683)) ([ad82f0c](https://github.com/n8n-io/n8n/commit/ad82f0c0c827e535a22b0a51e408f4cddea280e0))
* **core:** Move execution permission checks earlier in the lifecycle ([#8677](https://github.com/n8n-io/n8n/issues/8677)) ([059d281](https://github.com/n8n-io/n8n/commit/059d281fd1efdd281d3c9bf3f3a6c614d343e7ca))
* **editor:** Add chevron to filter component operator select ([#8633](https://github.com/n8n-io/n8n/issues/8633)) ([20446bd](https://github.com/n8n-io/n8n/commit/20446bdf11bd9f3528fd7b3bad61d522f1102f4d))
* **Google Sheets Node:** Option how to combine filters when reading rows ([#8652](https://github.com/n8n-io/n8n/issues/8652)) ([a5e522e](https://github.com/n8n-io/n8n/commit/a5e522e5360bd72a5567c96aaf0076baf0d95b35))
* **Google Workspace Admin Node:** Add support for error output branch ([#8499](https://github.com/n8n-io/n8n/issues/8499)) ([ef77571](https://github.com/n8n-io/n8n/commit/ef775711d01e77533775bd3c1e1f9bb1c508f2b2))
* Introduce prompt type option for Agent, Basic LLM Chain, and QA Chain nodes ([#8697](https://github.com/n8n-io/n8n/issues/8697)) ([2068f18](https://github.com/n8n-io/n8n/commit/2068f186ffd64766051294e8652689618a0df3fb))



# [1.29.0](https://github.com/n8n-io/n8n/compare/n8n@1.28.0...n8n@1.29.0) (2024-02-15)


### Bug Fixes

* **core:** Custom workflow tool tweaks  ([#8561](https://github.com/n8n-io/n8n/issues/8561)) ([ccc0ad5](https://github.com/n8n-io/n8n/commit/ccc0ad5009b2d547accfc34a9c0917114fd19c81))
* **core:** Give better error message if `executions.process` is still used in the configs ([#8618](https://github.com/n8n-io/n8n/issues/8618)) ([cd8ca84](https://github.com/n8n-io/n8n/commit/cd8ca8412d02090af07d8657283b7637178c975c))
* **core:** Improve the startup error when EXECUTIONS_PROCESS is set ([#8630](https://github.com/n8n-io/n8n/issues/8630)) ([a2a3ca1](https://github.com/n8n-io/n8n/commit/a2a3ca160f253b3b09f83bdc6dec11987971e464))
* **core:** Upgrade `@n8n/typeorm` to address postgres timestamp issues ([#8627](https://github.com/n8n-io/n8n/issues/8627)) ([68498cb](https://github.com/n8n-io/n8n/commit/68498cb72a16d587c4b24f9fe5e8ac2450cd78b9))
* **core:** Upgrade rudderstack sdk to address npm postInstall issues ([#8568](https://github.com/n8n-io/n8n/issues/8568)) ([5750e8e](https://github.com/n8n-io/n8n/commit/5750e8e88ed59b40d5115416c8afe227cb64c70e))
* **editor:** Debounce expression changes ([#8629](https://github.com/n8n-io/n8n/issues/8629)) ([9c7e026](https://github.com/n8n-io/n8n/commit/9c7e0266ee1c2112649772ca553bff429dcabc2d))
* **Execute Workflow Node:** Passing the workflow that is supposed to be executed as a paramter ([#8614](https://github.com/n8n-io/n8n/issues/8614)) ([b54488a](https://github.com/n8n-io/n8n/commit/b54488ada53a9941f5fd4d3cab8d39bd81b22f4a))
* Fix resolving of expressions of deeply nested sub-nodes ([#8612](https://github.com/n8n-io/n8n/issues/8612)) ([f527430](https://github.com/n8n-io/n8n/commit/f5274302f843c34f0a8a0b3eb51e7f9262fe0ea4))
* **FTP Node:** Fix issue with connections not closing properly ([#8619](https://github.com/n8n-io/n8n/issues/8619)) ([e597fbc](https://github.com/n8n-io/n8n/commit/e597fbc78ff60ce495eecd9ffdffda801ed90b66))
* **FTP Node:** Fix issue with paireditems not always working ([#8613](https://github.com/n8n-io/n8n/issues/8613)) ([d38a822](https://github.com/n8n-io/n8n/commit/d38a822b9501a8730c9cf097a9372e96080e8722))
* **Google Sheets Trigger Node:** First non-header row is ignored when using on row added event ([#8580](https://github.com/n8n-io/n8n/issues/8580)) ([2db8231](https://github.com/n8n-io/n8n/commit/2db8231af5baed941b5250af373898c3924d3baa))
* **HTTP Request Node:** Errorneous binary object without content-disposition response header ([#8583](https://github.com/n8n-io/n8n/issues/8583)) ([e28b374](https://github.com/n8n-io/n8n/commit/e28b374170725efeff59ac39e4ba6385bf834e7f))
* **HTTP Request Node:** Handle special characters in pagination expressions + improve hint text ([#8576](https://github.com/n8n-io/n8n/issues/8576)) ([3b2078c](https://github.com/n8n-io/n8n/commit/3b2078c3caf2a5acee48fed3055b47dbfe0af44a))
* **Jira Software Node:** Fix issue with not all issue types being supported ([#8571](https://github.com/n8n-io/n8n/issues/8571)) ([a6211c9](https://github.com/n8n-io/n8n/commit/a6211c9a5df9513ef057be1bfb78b4e0e2a75c2f))
* **Merge Node:** Fixing how paired items are handled in the merge node, when choosing a branch and selecting to return an empty object ([#8479](https://github.com/n8n-io/n8n/issues/8479)) ([a3bed97](https://github.com/n8n-io/n8n/commit/a3bed97883ece25ffb4ab3a8246418b123c92e52))
* **Microsoft Outlook Node:** Download executes more than once per incoming item ([#8566](https://github.com/n8n-io/n8n/issues/8566)) ([053fb5f](https://github.com/n8n-io/n8n/commit/053fb5ff7a3a4ce30b35fa6c830787b935ebaf63))
* **Notion Node:** Block with text results in a body validation error ([#8622](https://github.com/n8n-io/n8n/issues/8622)) ([6bc1c3d](https://github.com/n8n-io/n8n/commit/6bc1c3d7a83436ee3b3520adf4b52f59f2b4231c))
* **RSS Feed Trigger Node:** Save last item's date instead of last execution date ([#8572](https://github.com/n8n-io/n8n/issues/8572)) ([a822588](https://github.com/n8n-io/n8n/commit/a822588012b66711f37d3ca363fcd04742eda1b8))
* **Wait Node:** Account for workflow timezone in Wait node datetime ([#8578](https://github.com/n8n-io/n8n/issues/8578)) ([1116a28](https://github.com/n8n-io/n8n/commit/1116a28b4582cae93e9d44890cfe020cd813521c))


### Features

* Add support for AI log streaming ([#8526](https://github.com/n8n-io/n8n/issues/8526)) ([7501ad8](https://github.com/n8n-io/n8n/commit/7501ad8f3c56d9fcc5f4ec3d6fc468ab9cdb5024))
* Add telemetry event when users click on templates link ([#8625](https://github.com/n8n-io/n8n/issues/8625)) ([bf4f896](https://github.com/n8n-io/n8n/commit/bf4f896373acb2530a8f322cd612a3de616d6d15))
* **API:** Add tag support to public API ([#8588](https://github.com/n8n-io/n8n/issues/8588)) ([a743a40](https://github.com/n8n-io/n8n/commit/a743a4037674ccb68a311daa5511cb48de6c9bfa))
* **Convert to File Node:** Operation to convert a string in a plain text file, option to format JSON when creating file ([#8620](https://github.com/n8n-io/n8n/issues/8620)) ([d18cba3](https://github.com/n8n-io/n8n/commit/d18cba37a4a690cb3b4cd4259d27aedaa97193e4))
* **core:** Migrate to n8n's typeorm fork ([#8590](https://github.com/n8n-io/n8n/issues/8590)) ([8e392cf](https://github.com/n8n-io/n8n/commit/8e392cfc1dd103a00b3a0e7c186cbfad989a5080))
* **editor:** Use website as the main templates repository ([#8591](https://github.com/n8n-io/n8n/issues/8591)) ([79b09fd](https://github.com/n8n-io/n8n/commit/79b09fdf84860eee4c80e0c7eb7e320f6e05eabb))
* **HTML Extract Node:** Better text extraction, option to specify selectors to skip, option to clean up text data ([#8586](https://github.com/n8n-io/n8n/issues/8586)) ([32281d1](https://github.com/n8n-io/n8n/commit/32281d12d775281e4b8e419d76e46ca9e3b47267))
* **OpenAI Node:** Overhaul ([#8335](https://github.com/n8n-io/n8n/issues/8335)) ([941278d](https://github.com/n8n-io/n8n/commit/941278db6880ae3734a7a37aa03d7e6106ee5009))
* Upgrade typeorm, sqlite3, and pg/pg-promise ([#8579](https://github.com/n8n-io/n8n/issues/8579)) ([7826bd8](https://github.com/n8n-io/n8n/commit/7826bd842a8e1548c1eab8fff942d2efe8b3dc75))



# [1.28.0](https://github.com/n8n-io/n8n/compare/n8n@1.27.0...n8n@1.28.0) (2024-02-07)


### Bug Fixes

* Allow Date/Luxon objects and additional formats in DateTime validation ([#8525](https://github.com/n8n-io/n8n/issues/8525)) ([c419c85](https://github.com/n8n-io/n8n/commit/c419c8592f16a002d9f460c555db5f8bc04d95b8))
* **core:** Ensure AxiosError status always gets copied over to NodeApiError ([#8509](https://github.com/n8n-io/n8n/issues/8509)) ([76c5a62](https://github.com/n8n-io/n8n/commit/76c5a62f521fbd79a47d47f419fd90dcc6ca0275))
* **core:** Fix DropRoleMapping migration ([#8521](https://github.com/n8n-io/n8n/issues/8521)) ([4fed68e](https://github.com/n8n-io/n8n/commit/4fed68ee34c239ed3cae8541d5d4e7f86cf28d13))
* **core:** Fix new graceful shutdown env being always overridden by deprecated env ([#8503](https://github.com/n8n-io/n8n/issues/8503)) ([cc41fc7](https://github.com/n8n-io/n8n/commit/cc41fc7c801ecb1b0de4b7c5af5a03b3f30fdce8))
* **core:** Fix PermissionChecker.check, and add additional unit tests ([#8528](https://github.com/n8n-io/n8n/issues/8528)) ([5832d3c](https://github.com/n8n-io/n8n/commit/5832d3ca4695ec812e028e40b41811ca2215c0e2))
* **core:** Fix test runs of triggers that rely on static data ([#8524](https://github.com/n8n-io/n8n/issues/8524)) ([528c071](https://github.com/n8n-io/n8n/commit/528c07134a6705c8c7a5378f15f5e4a4b93234a9))
* **core:** Fix workflow tagging failure due to unique constraint check ([#8505](https://github.com/n8n-io/n8n/issues/8505)) ([92f939f](https://github.com/n8n-io/n8n/commit/92f939f82799975a5f9b859e7f342f3440961320))
* **core:** Upgrade nodemailer to address an exploit ([#8535](https://github.com/n8n-io/n8n/issues/8535)) ([ee5e422](https://github.com/n8n-io/n8n/commit/ee5e4220945fde5baaec9ad66ff08b8728912aa3))
* **core:** Use hostname from URL instead of Host header for SNI ([#8562](https://github.com/n8n-io/n8n/issues/8562)) ([7531f34](https://github.com/n8n-io/n8n/commit/7531f343861d91df075b8f3220f5bce8858b117f))
* **core:** Use trx manager instead of repository for tags overwrite ([#8557](https://github.com/n8n-io/n8n/issues/8557)) ([abddbb6](https://github.com/n8n-io/n8n/commit/abddbb622798bdc4a2b11347a09f10aaf03a4639))
* **editor:** Prune values that are not in the schema in the ResourceMapper component ([#8478](https://github.com/n8n-io/n8n/issues/8478)) ([612771e](https://github.com/n8n-io/n8n/commit/612771e0328f7e565d5f075cc20ad86bd1f13bce))
* **Embeddings OpenAI Node:** Fix dynamic models fetching ([#8533](https://github.com/n8n-io/n8n/issues/8533)) ([cccdfc7](https://github.com/n8n-io/n8n/commit/cccdfc73d6c13a37e395fdc2612f2ebf458a4f52))
* **HTTP Request Node:** Require parameter with filled name and value to avoid infinite loop ([#8454](https://github.com/n8n-io/n8n/issues/8454)) ([3128dca](https://github.com/n8n-io/n8n/commit/3128dca1faeff85d77a28640b7dfe8fbcd85db4f))
* **HTTP Request Node:** Support form data when using pagination ([#8497](https://github.com/n8n-io/n8n/issues/8497)) ([ca75744](https://github.com/n8n-io/n8n/commit/ca75744c7f93db827ece5bf3b17b82f07d4cffb1))
* **Microsoft Excel 365 Node:** Upsert append new rows at the end of used range, option to append at the end of selected range ([#8461](https://github.com/n8n-io/n8n/issues/8461)) ([1e02d73](https://github.com/n8n-io/n8n/commit/1e02d73ad782fb21cdd9b7350e34beb731a677c5))
* **MongoDB Node:** Fix "Maximum call stack size exceeded" error on too many rows ([#8530](https://github.com/n8n-io/n8n/issues/8530)) ([76cdf75](https://github.com/n8n-io/n8n/commit/76cdf75fb96fb55b4a6e7a1a9edc7c9674806391))
* **Slack Node:** Attachments fix ([#8471](https://github.com/n8n-io/n8n/issues/8471)) ([254700a](https://github.com/n8n-io/n8n/commit/254700a059a48a66dea8b9d80e61c8250e09d5b5))
* Update BaseChatModel import checks for MistralAI compatibility ([#8527](https://github.com/n8n-io/n8n/issues/8527)) ([c8b8379](https://github.com/n8n-io/n8n/commit/c8b83790150b9974d6d99f6a2b6b5b7be6fb8c53))


### Features

* Add assignment component with drag and drop to Set node ([#8283](https://github.com/n8n-io/n8n/issues/8283)) ([2799de4](https://github.com/n8n-io/n8n/commit/2799de491b753e6fb00f73b61393392b6fc8ad18))
* Azure Open AI chat model & embeddings ([#8522](https://github.com/n8n-io/n8n/issues/8522)) ([934d0d3](https://github.com/n8n-io/n8n/commit/934d0d35b1814c0a39595d61a30fb9c2e05fd995))
* **editor:** Add delete and disable button to nodes on hover ([#8482](https://github.com/n8n-io/n8n/issues/8482)) ([994754b](https://github.com/n8n-io/n8n/commit/994754bf39976c5bb33fd1c30a0eb82cc518850b))
* **Email Trigger (IMAP) Node:** Upgrade mailparser ([#8539](https://github.com/n8n-io/n8n/issues/8539)) ([da1fe44](https://github.com/n8n-io/n8n/commit/da1fe44d5246848e2ba7bb8bc5f4577685fbcee0))
* **RabbitMQ Trigger Node:** Add options to configure assert of exchanges and queues ([#8430](https://github.com/n8n-io/n8n/issues/8430)) ([4b3659f](https://github.com/n8n-io/n8n/commit/4b3659f04f84ef774d31cf2341c5dbb500a73afe))



# [1.27.0](https://github.com/n8n-io/n8n/compare/n8n@1.26.0...n8n@1.27.0) (2024-01-31)


### Bug Fixes

* **AwsS3 Node:** Fix handling of bucket with dot in name ([#8475](https://github.com/n8n-io/n8n/issues/8475)) ([0febe62](https://github.com/n8n-io/n8n/commit/0febe62ad03f82b85922e0cb66d60eeb22b3a919))
* **core:** Don't report executions that have been paused as failed to rudderstack and log streams ([#8501](https://github.com/n8n-io/n8n/issues/8501)) ([39e8754](https://github.com/n8n-io/n8n/commit/39e875478488f3c81147944bd6b52dc1f9def958))
* **core:** Fix stopping and retrying failed executions ([#8480](https://github.com/n8n-io/n8n/issues/8480)) ([238b54c](https://github.com/n8n-io/n8n/commit/238b54c77bba6f7abcc7fc2b3ac48a85206ce37e))
* **core:** Forward authorization header when on same domain ([#8507](https://github.com/n8n-io/n8n/issues/8507)) ([f1910a1](https://github.com/n8n-io/n8n/commit/f1910a10a6ac875b422d9efe9bfd3ca728ac8d96))
* **core:** Handle possibly invalid `updatedAt` timestamps in source-control ([#8485](https://github.com/n8n-io/n8n/issues/8485)) ([033fd34](https://github.com/n8n-io/n8n/commit/033fd344b5a09a7b9c0b941279da1744e182cc57))
* **core:** Handle zero execution statistics on metrics collection during license renewal ([#8463](https://github.com/n8n-io/n8n/issues/8463)) ([db48bdd](https://github.com/n8n-io/n8n/commit/db48bdd6d1110bfccc371ca490281c021227991f))
* **core:** Improve handling of wrapped errors ([#8510](https://github.com/n8n-io/n8n/issues/8510)) ([670af16](https://github.com/n8n-io/n8n/commit/670af167e6f2c0e4e45bcc7e0998a371d651f89d))
* **core:** Point users to the official documentation when they use `n8n --help` ([#8440](https://github.com/n8n-io/n8n/issues/8440)) ([9f11eba](https://github.com/n8n-io/n8n/commit/9f11eba0a4f726cc150b05c0f4b528bf25513e6f))
* **core:** Prevent calling internal hook email event if emailing is disabled ([#8462](https://github.com/n8n-io/n8n/issues/8462)) ([9e93980](https://github.com/n8n-io/n8n/commit/9e939809575592622f6bdca112da1905ac9205ef))
* **editor:** Disable expression editor modal opening on readonly field ([#8457](https://github.com/n8n-io/n8n/issues/8457)) ([eb27ed0](https://github.com/n8n-io/n8n/commit/eb27ed068ba21bbf4302686f0f0c0168e91c03f6))
* **editor:** Fix workflows filter resetting ([#8411](https://github.com/n8n-io/n8n/issues/8411)) ([ad4b298](https://github.com/n8n-io/n8n/commit/ad4b298be34915718b0415322e328a1b46ef5842))
* **editor:** Send template id as a number in telemetry events ([#8484](https://github.com/n8n-io/n8n/issues/8484)) ([327cc8d](https://github.com/n8n-io/n8n/commit/327cc8df7343b806bee87faaa86ed22d9d70127f))
* **editor:** Show pin button on binary output but disable it with tooltip ([#8388](https://github.com/n8n-io/n8n/issues/8388)) ([caab97e](https://github.com/n8n-io/n8n/commit/caab97e667df5d305aa1d2e15c0d31eb5f1a84eb))
* **Gotify Node:** Add option to set content type to support Markdown messages ([#8442](https://github.com/n8n-io/n8n/issues/8442)) ([c2ffd4e](https://github.com/n8n-io/n8n/commit/c2ffd4e6455b383e4ddc2eb310cefbcdf867d622))
* **HTML Node:** Escape data path value in JSON Property ([#8441](https://github.com/n8n-io/n8n/issues/8441)) ([fc5c562](https://github.com/n8n-io/n8n/commit/fc5c5627850bf618be4ca0d9cdb20adb0f8610e9))
* **Merge Node:** Passing on no items to "Input 2" results in wrong output items ([#8438](https://github.com/n8n-io/n8n/issues/8438)) ([dafacb9](https://github.com/n8n-io/n8n/commit/dafacb90c6b01e2f88c3de359ebb2d8d55e0aecc))
* **Microsoft Excel 365 Node:** Better error and description on unsupported range in upsert, update, getRange operations ([#8452](https://github.com/n8n-io/n8n/issues/8452)) ([8a595d1](https://github.com/n8n-io/n8n/commit/8a595d1527bf8cd97ce8293c6a52929eb3335750))
* Open executions with large number of execution items without crashing tab ([#8423](https://github.com/n8n-io/n8n/issues/8423)) ([56da2e4](https://github.com/n8n-io/n8n/commit/56da2e43528f157c421e97018366b8f2d854d11d))
* Properly iterate over credentials with expressions ([#8502](https://github.com/n8n-io/n8n/issues/8502)) ([0e9a5a2](https://github.com/n8n-io/n8n/commit/0e9a5a2ab2cde251cf106b149bdd4c3142e52b40))
* Use correct node version when pasting/importing nodes ([#8456](https://github.com/n8n-io/n8n/issues/8456)) ([70af67e](https://github.com/n8n-io/n8n/commit/70af67e744c709b85b600811b792def83518fa7c))


### Features

* Add model parameter to OpenAI embeddings ([#8481](https://github.com/n8n-io/n8n/issues/8481)) ([981ea39](https://github.com/n8n-io/n8n/commit/981ea3930e96c3b45267fa7ddac48710846e49ac))
* Add new 'is empty' and 'is not empty' operators to Filter ([#8445](https://github.com/n8n-io/n8n/issues/8445)) ([c21c4b9](https://github.com/n8n-io/n8n/commit/c21c4b9178b3ae328ff7a068663eeb64fed3e465))
* **core:** Upgrade Rudderstack SDK to address CVE-2023-45857 ([#8368](https://github.com/n8n-io/n8n/issues/8368)) ([2fba0e8](https://github.com/n8n-io/n8n/commit/2fba0e8d585aead43eaeb73fa49dc9b613900675))
* **editor:** Implement loading and error states for dynamically loaded components in node parameter list ([#8477](https://github.com/n8n-io/n8n/issues/8477)) ([e643a12](https://github.com/n8n-io/n8n/commit/e643a126f40dbad0634e5abb1e3ba355bad0275d))
* **editor:** Send template id as string in all telemetry events ([#8498](https://github.com/n8n-io/n8n/issues/8498)) ([2aed788](https://github.com/n8n-io/n8n/commit/2aed788dc354595b070e91fe76298f6702bbbe15))
* **Google Calendar Node:** Next occurrence property in recurring events  ([#8444](https://github.com/n8n-io/n8n/issues/8444)) ([bf11c7c](https://github.com/n8n-io/n8n/commit/bf11c7c1bd5826ba64acc665da4e3319f9a47174))

### ⚠️ BREAKING CHANGES
* **core:** Remove `own` execution-process mode ([#8490](https://github.com/n8n-io/n8n/issues/8490)) ([121a55b](https://github.com/n8n-io/n8n/commit/121a55b691469e7eb042737573c0ace276366ecb))



# [1.26.0](https://github.com/n8n-io/n8n/compare/n8n@1.25.0...n8n@1.26.0) (2024-01-24)


### Bug Fixes

* **AMQP Trigger Node:** Properly close connection after manual test step ([#8396](https://github.com/n8n-io/n8n/issues/8396)) ([2c14371](https://github.com/n8n-io/n8n/commit/2c143714817e62fcb2fec9b9cac208ef029f87fd))
* **Asana Node:** Fix issue when connecting to the new Asana environment ([#8404](https://github.com/n8n-io/n8n/issues/8404)) ([44f6ef2](https://github.com/n8n-io/n8n/commit/44f6ef2ed729ad39518cc85e068be03cd8b409ff))
* **AWS SQS Node:** Fix issue preventing data from being sent correctly ([#8382](https://github.com/n8n-io/n8n/issues/8382)) ([daba5bb](https://github.com/n8n-io/n8n/commit/daba5bb250c3bee338dde96e6e815835dd21e6f1))
* Change the UI text for some filter operations ([#8360](https://github.com/n8n-io/n8n/issues/8360)) ([976fe2e](https://github.com/n8n-io/n8n/commit/976fe2e6c8caf3f72c833af4447c46ddfa1d8e0a))
* **core:** Adjust starter node priority for manual executions with pinned activators ([#8386](https://github.com/n8n-io/n8n/issues/8386)) ([749ac2b](https://github.com/n8n-io/n8n/commit/749ac2b407d9477343c169ac26daba1a36cfcc6d))
* **core:** Errors are returned on the success branch if error item has other keys in addition to 'error' ([#8380](https://github.com/n8n-io/n8n/issues/8380)) ([25f51f4](https://github.com/n8n-io/n8n/commit/25f51f4fd79d14ccff8d35d92c11e47fe18f3e0d))
* **core:** Fix removal of triggers and pollers from memory on deactivation in multi-main setup ([#8416](https://github.com/n8n-io/n8n/issues/8416)) ([2257ec6](https://github.com/n8n-io/n8n/commit/2257ec63b3716598f85a5237bc147bb2c887fa33))
* **core:** Fix update workflow cli command being unable to activate all workflows ([#8412](https://github.com/n8n-io/n8n/issues/8412)) ([ae06fde](https://github.com/n8n-io/n8n/commit/ae06fdeb62d0cb982253f32956fdd55bd66058bd))
* **core:** Missing pairedItem fixes ([#8394](https://github.com/n8n-io/n8n/issues/8394)) ([284d965](https://github.com/n8n-io/n8n/commit/284d965b5acc0819ffc109729ce1d5d0b2352abb))
* **Discord Node:** Remove requirement on message for webhooks ([#8377](https://github.com/n8n-io/n8n/issues/8377)) ([c64e893](https://github.com/n8n-io/n8n/commit/c64e893b60143df6e9a752191adef0419811fe43))
* **editor:** Add pinned data for freshly added nodes ([#8323](https://github.com/n8n-io/n8n/issues/8323)) ([83228e2](https://github.com/n8n-io/n8n/commit/83228e26fb8f62676e15d59f65a43106487034da))
* **editor:** Enable ctrl/cmd click in workflow editor header ([#8387](https://github.com/n8n-io/n8n/issues/8387)) ([e43cf2f](https://github.com/n8n-io/n8n/commit/e43cf2fd715e21fd4e454c9e6b6d874306472360))
* **editor:** Fix copy to clipboard on insecure contexts ([#8425](https://github.com/n8n-io/n8n/issues/8425)) ([7386f79](https://github.com/n8n-io/n8n/commit/7386f79362673876509c27a2f6ddef08125a0b1e))
* **editor:** Fix doclines for `plus` and `minus` ([#8405](https://github.com/n8n-io/n8n/issues/8405)) ([ebf2b0d](https://github.com/n8n-io/n8n/commit/ebf2b0d55ccf3977269d4ea442f2ad210d1b375b))
* **editor:** Fix invisible community package update button ([#8406](https://github.com/n8n-io/n8n/issues/8406)) ([2ccb754](https://github.com/n8n-io/n8n/commit/2ccb754e52949e0d20925871f425eef92cd6aebc))
* **editor:** Fix secondary icon for environments on sidebar menu item ([#8407](https://github.com/n8n-io/n8n/issues/8407)) ([3544966](https://github.com/n8n-io/n8n/commit/35449667bfab7324350fe92e1f6538e3ae3cadb1))
* **editor:** Open native context menu when editing Sticky ([#8370](https://github.com/n8n-io/n8n/issues/8370)) ([ade7d30](https://github.com/n8n-io/n8n/commit/ade7d30053f897bd9269912565d86d33046e560e))
* **editor:** Use web native <a> element in nav menus ([#8385](https://github.com/n8n-io/n8n/issues/8385)) ([e606e84](https://github.com/n8n-io/n8n/commit/e606e841ee1086d737849dc33f4ced867ab2cb21))
* Fix issue preventing secrets with a - in the path from being imported ([#8378](https://github.com/n8n-io/n8n/issues/8378)) ([fc94377](https://github.com/n8n-io/n8n/commit/fc9437703687738091fdd072e03597358bd8f8d0))
* Force posthog recording to be disabled outside cloud ([#8374](https://github.com/n8n-io/n8n/issues/8374)) ([f31cc07](https://github.com/n8n-io/n8n/commit/f31cc0743ff94c9b29cdd0d498c87340beb29585))
* **Google Drive Node:** Fix issue preventing upload / update working in some configurations ([#8417](https://github.com/n8n-io/n8n/issues/8417)) ([4b3ea81](https://github.com/n8n-io/n8n/commit/4b3ea81028ae6dcbe3a4738dca7522b62685bb42))
* **Microsoft Outlook Node:** Message -> Send with attachments ([#8238](https://github.com/n8n-io/n8n/issues/8238)) ([0128081](https://github.com/n8n-io/n8n/commit/01280815c950413188905f5d17a13157685d0a27))
* **Microsoft SQL Node:** Prevent MSSQL max parameters error by chunking ([#8390](https://github.com/n8n-io/n8n/issues/8390)) ([1b0ba2c](https://github.com/n8n-io/n8n/commit/1b0ba2c02885a0dd9f548133efadcfc7485d666d))
* **Notion Node:** Fix is_empty query on formula fields ([#8397](https://github.com/n8n-io/n8n/issues/8397)) ([08e7db4](https://github.com/n8n-io/n8n/commit/08e7db4648cd2f820e0d63d012f42057a124dd82))
* **Switch Node:** Fix issue preventing some regex patterns from working ([#8422](https://github.com/n8n-io/n8n/issues/8422)) ([e9fea16](https://github.com/n8n-io/n8n/commit/e9fea16301cb9ee0ff7e3af45fc50d77e2cf6a23))


### Features

* **core:** Custom session timeout and refresh configuration ([#8342](https://github.com/n8n-io/n8n/issues/8342)) ([07e6705](https://github.com/n8n-io/n8n/commit/07e67052568dcb292dbf63bee8912110931726bc))
* **core:** Email recipients on resource shared ([#8408](https://github.com/n8n-io/n8n/issues/8408)) ([a0a1830](https://github.com/n8n-io/n8n/commit/a0a1830696eaa905d37fbd56e8bc5035d12b2aa5))
* **core:** Upgrade axios and follow-redirects to address CVE-2023-26159 ([#8366](https://github.com/n8n-io/n8n/issues/8366)) ([3912c5e](https://github.com/n8n-io/n8n/commit/3912c5e7abca98fe81d4c9c25894d30d8023ce56))
* **core:** Upgrade bull and ioredis to address CVE-2023-52079 ([#8365](https://github.com/n8n-io/n8n/issues/8365)) ([639d347](https://github.com/n8n-io/n8n/commit/639d34769e75096d0725f1f60861dc972b344abe))
* **editor:** Migrate `moveNodeWorkflow` mixin to `useCanvasPanning` composable ([#8322](https://github.com/n8n-io/n8n/issues/8322)) ([b6d7757](https://github.com/n8n-io/n8n/commit/b6d775768f927e69e7aa5f715c99f2fed4eaaa4c))
* **Execute Workflow Node:** Add 'Wait For Sub-Workflow Completion' option ([#8389](https://github.com/n8n-io/n8n/issues/8389)) ([ff92fc7](https://github.com/n8n-io/n8n/commit/ff92fc7fef39076e0846f2426ffdd86c761e7896))
* **LinkedIn Node:** Add support for Community Management API ([#7451](https://github.com/n8n-io/n8n/issues/7451)) ([7660d7e](https://github.com/n8n-io/n8n/commit/7660d7e735d248f3e731aca550c2973e85cdfebc))
* **Microsoft Teams Node:** Overhaul ([#7477](https://github.com/n8n-io/n8n/issues/7477)) ([2c146cc](https://github.com/n8n-io/n8n/commit/2c146cca62ec605f6d722fe6c4b90c7df9cf77f7))
* Nudge users to become template creators if eligible ([#8357](https://github.com/n8n-io/n8n/issues/8357)) ([9945701](https://github.com/n8n-io/n8n/commit/99457019f795636f56d80d3fc2c7e08055ace938))
* **Telegram Trigger Node:** Verify Webhook requests ([#8383](https://github.com/n8n-io/n8n/issues/8383)) ([1117612](https://github.com/n8n-io/n8n/commit/11176124b5b6157c7c17fd882691d2f9d6b41487))



# [1.25.0](https://github.com/n8n-io/n8n/compare/n8n@1.24.0...n8n@1.25.0) (2024-01-17)


### Bug Fixes

* Add fallback resolver for langchain modules ([#8308](https://github.com/n8n-io/n8n/issues/8308)) ([851060d](https://github.com/n8n-io/n8n/commit/851060dd3f38245da6e09c04ec0b12b24b63dca4))
* **API:** Fix manual chat trigger execution ([#8300](https://github.com/n8n-io/n8n/issues/8300)) ([884396e](https://github.com/n8n-io/n8n/commit/884396ea0d9f4a8d7987daf2b674f080056dd1d1))
* **AwsS3 Node:** Return confirmation of success after upload ([#8312](https://github.com/n8n-io/n8n/issues/8312)) ([c921665](https://github.com/n8n-io/n8n/commit/c921665f9abe19d9e8831062c1e7673d4d1ea694))
* **core:** Account for immediate confirmation request during test webhook creation ([#8329](https://github.com/n8n-io/n8n/issues/8329)) ([5fbd797](https://github.com/n8n-io/n8n/commit/5fbd7971e04640be3f877b3aa22d4aee61c1d40a))
* **core:** Ensure waiting executions account for workflow timezone ([#8340](https://github.com/n8n-io/n8n/issues/8340)) ([3734c89](https://github.com/n8n-io/n8n/commit/3734c89cf64514489831b5339d722c89b300cc54))
* **core:** Parse any readable stream response instead of only IncomingMessage ([#8359](https://github.com/n8n-io/n8n/issues/8359)) ([eb1320f](https://github.com/n8n-io/n8n/commit/eb1320fd7a4a67cd16de10c4174c7bcf2c177b06))
* **core:** Prevent invalid compressed responses from making executions stuck forever ([#8315](https://github.com/n8n-io/n8n/issues/8315)) ([0776814](https://github.com/n8n-io/n8n/commit/0776814ed8c520326a6447dcd7b6c53fda933054))
* **core:** Prevent issues with missing or mismatching encryption key ([#8332](https://github.com/n8n-io/n8n/issues/8332)) ([d4c93b1](https://github.com/n8n-io/n8n/commit/d4c93b16071081002b4bd316be0921bc7867dd82))
* **core:** Prevent NodeErrors from being wrapped multiple times ([#8301](https://github.com/n8n-io/n8n/issues/8301)) ([b267bf0](https://github.com/n8n-io/n8n/commit/b267bf07e365d8bb82a9847fb3c490437dc1010e))
* **core:** Replace all `moment` imports with `moment-timezone` ([#8337](https://github.com/n8n-io/n8n/issues/8337)) ([52a2e25](https://github.com/n8n-io/n8n/commit/52a2e25a25e9a009a536d8a371d9404e75d756f4))
* **core:** Report when waitTill is invalid and handle it  ([#8356](https://github.com/n8n-io/n8n/issues/8356)) ([d5455d7](https://github.com/n8n-io/n8n/commit/d5455d7accb193078b05a0f52386cf9303b6a00f))
* **editor:** Add read only mode to filter component ([#8285](https://github.com/n8n-io/n8n/issues/8285)) ([dcc76f3](https://github.com/n8n-io/n8n/commit/dcc76f348075b6e05e3f38bb9694d25ac9a5646b))
* **editor:** Capture indexed access expressions when building completions ([#8331](https://github.com/n8n-io/n8n/issues/8331)) ([159b328](https://github.com/n8n-io/n8n/commit/159b328587f3c57c73ae77c2a0c5d5c6ecc330aa))
* **editor:** Fix issue with synchronization table on LDAP not loading data ([#8327](https://github.com/n8n-io/n8n/issues/8327)) ([6b92d49](https://github.com/n8n-io/n8n/commit/6b92d49ea58b8e5797e4e938444b161a63137638))
* **editor:** Properly set colors for connections and labels on nodes with pinned data ([#8209](https://github.com/n8n-io/n8n/issues/8209)) ([3b8ccb9](https://github.com/n8n-io/n8n/commit/3b8ccb9fb903036a7d6e4b33f6b5a8933576e9e6))
* Fix node graph telemetry with default values ([#8297](https://github.com/n8n-io/n8n/issues/8297)) ([93b969a](https://github.com/n8n-io/n8n/commit/93b969a327e0770d9a0e81a95a5185b0fc12ebc6))
* **Google Drive Node:** Fix issue preventing service account from downloading files ([#7642](https://github.com/n8n-io/n8n/issues/7642)) ([cf7131d](https://github.com/n8n-io/n8n/commit/cf7131d766dfc7aec2c973525653ffec1ced03c1))
* **HTTP Request Node:** Delete `response.request` only when it's a valid circular references ([#8293](https://github.com/n8n-io/n8n/issues/8293)) ([05c43fa](https://github.com/n8n-io/n8n/commit/05c43faa2d7582a8ce58b9bb3338c00253ad3281))
* **Microsoft SQL Node:** Fix "Maximum call stack size exceeded" error on too many rows ([#8334](https://github.com/n8n-io/n8n/issues/8334)) ([bb2be8d](https://github.com/n8n-io/n8n/commit/bb2be8d70580896321641a49a3044165763eb9e1))
* **Ollama Model Node:** Use a simpler credentials test ([#8318](https://github.com/n8n-io/n8n/issues/8318)) ([63b738a](https://github.com/n8n-io/n8n/commit/63b738a542429934b3838bfc814ea2a4c51675c7))
* **OpenAI Node:** Load correct models for operation ([#8313](https://github.com/n8n-io/n8n/issues/8313)) ([a6a5372](https://github.com/n8n-io/n8n/commit/a6a5372b5f8e48e98788c4e3750ac4b63e91a96f))
* Properly output saml validation errors ([#8284](https://github.com/n8n-io/n8n/issues/8284)) ([8c7f399](https://github.com/n8n-io/n8n/commit/8c7f39907fa82fa37af4436511d4a2daaff13015))
* **Salesforce Node:** Upgrade to API version 59 ([#8346](https://github.com/n8n-io/n8n/issues/8346)) ([b51cbb3](https://github.com/n8n-io/n8n/commit/b51cbb325e03fd42be6dca99819d4cc7c4c1574b))
* **Supabase Node:** Pagination for get all rows ([#8311](https://github.com/n8n-io/n8n/issues/8311)) ([e080476](https://github.com/n8n-io/n8n/commit/e0804768e84aefe9d66ab683080f67bb15a1cb58))
* **Venafi TLS Protect Cloud Node:** Remove parameter `Application Server Type` ([#8325](https://github.com/n8n-io/n8n/issues/8325)) ([e3cedf7](https://github.com/n8n-io/n8n/commit/e3cedf7db038a70c9d48bb7c665b1be4beb872a9))
* **Venafi TLS Protect Cloud Trigger Node:** Handle new webhook payload format  ([#8326](https://github.com/n8n-io/n8n/issues/8326)) ([057d7d0](https://github.com/n8n-io/n8n/commit/057d7d031828ea8b6e779ca535ccd50d91bfa0cc))


### Features

* **core:** Implement inter-main communication for test webhooks in multi-main setup ([#8267](https://github.com/n8n-io/n8n/issues/8267)) ([1a0e285](https://github.com/n8n-io/n8n/commit/1a0e28555385f682aa335115c4d72e671c0bdc85))
* **editor:** Add new `/templates/search` endpoint ([#8227](https://github.com/n8n-io/n8n/issues/8227)) ([4277e92](https://github.com/n8n-io/n8n/commit/4277e92ec07671a679b0d9ab6e691ef9208585bd))
* Implement Chat Memory Manager node ([#8127](https://github.com/n8n-io/n8n/issues/8127)) ([464be93](https://github.com/n8n-io/n8n/commit/464be9332354620b2f1890136abf95dfdb71fd2e))



# [1.24.0](https://github.com/n8n-io/n8n/compare/n8n@1.23.0...n8n@1.24.0) (2024-01-10)


### Bug Fixes

* **core:** Do not add Authentication header when `authentication` type is `body` ([#8201](https://github.com/n8n-io/n8n/issues/8201)) ([ac1c642](https://github.com/n8n-io/n8n/commit/ac1c642fddfac3b0ed1144c7eccd7c88fbd5a1a5))
* **core:** Fix test webhook deregistration ([#8247](https://github.com/n8n-io/n8n/issues/8247)) ([5032bf0](https://github.com/n8n-io/n8n/commit/5032bf0e346dccf7cade17a1518b3031118af5e1))
* **editor:** Items count display in running workflow ([#8148](https://github.com/n8n-io/n8n/issues/8148)) ([8a3c87f](https://github.com/n8n-io/n8n/commit/8a3c87f69c20de7c713dff021e390ea4ea32b103)), closes [/github.com/n8n-io/n8n/pull/7763/files#diff-f5dae80a64b9951bb6691f1b9d439423cf84fa0cc9601b3f2c00904f3135e8deR48](https://github.com//github.com/n8n-io/n8n/pull/7763/files/issues/diff-f5dae80a64b9951bb6691f1b9d439423cf84fa0cc9601b3f2c00904f3135e8deR48)
* **editor:** Only load suggested templates for owners ([#8228](https://github.com/n8n-io/n8n/issues/8228)) ([8f22a26](https://github.com/n8n-io/n8n/commit/8f22a265d607047eff22ba957d627bbec7da7900))
* **editor:** Tweaking button sizes in execution preview ([#8206](https://github.com/n8n-io/n8n/issues/8206)) ([9d40ae8](https://github.com/n8n-io/n8n/commit/9d40ae8b74594d4368591a62f9b39dde28efc64d))
* **editor:** Unify canvas button positioning ([#8258](https://github.com/n8n-io/n8n/issues/8258)) ([b6c42cc](https://github.com/n8n-io/n8n/commit/b6c42cc08408d9d7cc49cc84245b4ad515fa3e6a))
* **editor:** Vertically center workflow preview loading state ([#8231](https://github.com/n8n-io/n8n/issues/8231)) ([2d6e406](https://github.com/n8n-io/n8n/commit/2d6e406e215188dbbbeb593ac09ccad3914aaf81))
* Fix issue with API key being required for the Qdrant Node ([#8237](https://github.com/n8n-io/n8n/issues/8237)) ([4401db3](https://github.com/n8n-io/n8n/commit/4401db3a2fad3464a5498e9a86fc6bba4f9c9f95))
* Fix template credential setup for nodes that dont have credentials ([#8208](https://github.com/n8n-io/n8n/issues/8208)) ([cd3f5b5](https://github.com/n8n-io/n8n/commit/cd3f5b5b1f48e42cb6fa5ebcc15527c28502ceb9))
* Fix user reinvites on FE and BE ([#8261](https://github.com/n8n-io/n8n/issues/8261)) ([0dabe5c](https://github.com/n8n-io/n8n/commit/0dabe5c74e5ad0969d4691b3db4a1e796ed8a08c))
* **FTP Node:** FTP connection failed due to missing password credential in node ([#8131](https://github.com/n8n-io/n8n/issues/8131)) ([e056aa9](https://github.com/n8n-io/n8n/commit/e056aa9c4dd6c6a7717202029b25f4f65ddecb0d))
* **Github Trigger Node:** Enforce SSL validation by default ([#8265](https://github.com/n8n-io/n8n/issues/8265)) ([1387541](https://github.com/n8n-io/n8n/commit/1387541e336e7311ba9c43907fa95d3196fae2eb))
* Make params panel double width for all SQL nodes ([#8236](https://github.com/n8n-io/n8n/issues/8236)) ([048b588](https://github.com/n8n-io/n8n/commit/048b588852f5fed1c976889ba54ef564ca7f4894))
* **Monday.com Node:** Migrate to api 2023-10 ([#8254](https://github.com/n8n-io/n8n/issues/8254)) ([ccde38a](https://github.com/n8n-io/n8n/commit/ccde38a8a8d65a21bf4d38ef7b09a5ffa3c7ad2d))
* **MySQL Node:** Only escape table names when needed ([#8246](https://github.com/n8n-io/n8n/issues/8246)) ([3b01eb6](https://github.com/n8n-io/n8n/commit/3b01eb60c98d51d0d7572342b8d6d40763293719))
* **Nextcloud Node:** Throw an actual error if server responded with Fatal error ([#8234](https://github.com/n8n-io/n8n/issues/8234)) ([b201ff8](https://github.com/n8n-io/n8n/commit/b201ff8f23b2bac6b00d5c16d91b4b2931f45ade))
* **NocoDB Node:** Download attachments ([#8235](https://github.com/n8n-io/n8n/issues/8235)) ([43e8e5e](https://github.com/n8n-io/n8n/commit/43e8e5e540b9fcbca663fcf17a78a7aba2abb475))
* **Postgres Node:** Stop marking autogenerated columns as required ([#8230](https://github.com/n8n-io/n8n/issues/8230)) ([bed04ec](https://github.com/n8n-io/n8n/commit/bed04ec122234b4329a5e415bf3627c115b3f32e)), closes [#7084](https://github.com/n8n-io/n8n/issues/7084)
* Resolve expressions in credentials following paired item ([#8250](https://github.com/n8n-io/n8n/issues/8250)) ([ccb2b07](https://github.com/n8n-io/n8n/commit/ccb2b076f8240b0712949b72ec57ae72a36ef62d))
* **Set Node:** Field not excluded if dot notation disabled and field was set by using drag-and-drop from ui ([#8233](https://github.com/n8n-io/n8n/issues/8233)) ([cda49a4](https://github.com/n8n-io/n8n/commit/cda49a4747ef4369ce7a971872c6fb8a74f4156d))
* Store workflow settings when saving an execution ([#8288](https://github.com/n8n-io/n8n/issues/8288)) ([8a7c629](https://github.com/n8n-io/n8n/commit/8a7c629ea183f75f9916003edf11cb8aeef445eb))
* **Webhook Node:** Fix handling of form-data files ([#8256](https://github.com/n8n-io/n8n/issues/8256)) ([fc29030](https://github.com/n8n-io/n8n/commit/fc2903096e6e64e5b2a14593418d5651e07ca9ee))


### Features

* Add Chat Trigger node ([#7409](https://github.com/n8n-io/n8n/issues/7409)) ([af49e95](https://github.com/n8n-io/n8n/commit/af49e95cc7ccf70f233f9bd1e34fbb57f7f08ccf))
* **core:** Cache test webhook registrations ([#8176](https://github.com/n8n-io/n8n/issues/8176)) ([22a5f52](https://github.com/n8n-io/n8n/commit/22a5f5258da0a973e1ad44c0d3d4f0fda1d23444)), closes [#8155](https://github.com/n8n-io/n8n/issues/8155)
* **core:** Validate shutdown handlers on startup ([#8260](https://github.com/n8n-io/n8n/issues/8260)) ([3b996a7](https://github.com/n8n-io/n8n/commit/3b996a7da0137a75c3047656a4bc8cc336ebfc1e))
* **editor:** Add fullscreen view to code editor ([#8084](https://github.com/n8n-io/n8n/issues/8084)) ([071e6d6](https://github.com/n8n-io/n8n/commit/071e6d6b6e32b7196f34043710c23331ad28fac0))
* **editor:** Update copy: `Execute` --> `Test` ([#8137](https://github.com/n8n-io/n8n/issues/8137)) ([df5d07b](https://github.com/n8n-io/n8n/commit/df5d07bcb8beba760bc17118b36ccd531bc3c755))
* **Google Sheets Node:** Add "By Name" option to selector for Sheets ([#8241](https://github.com/n8n-io/n8n/issues/8241)) ([dce28f9](https://github.com/n8n-io/n8n/commit/dce28f9cb98db33bf22bcfee181f8e9ca64dd2bc))
* **HTTP Request Node:** Interval Between Requests option for pagination ([#8224](https://github.com/n8n-io/n8n/issues/8224)) ([270328c](https://github.com/n8n-io/n8n/commit/270328ccf6e5502adc092f6f85d146ffb98e1208))
* Implement MistralCloud Chat & Embeddings nodes ([#8239](https://github.com/n8n-io/n8n/issues/8239)) ([d37b908](https://github.com/n8n-io/n8n/commit/d37b9084b2c657d8b5b8bae6dbb51b428db26e1e))
* **MongoDB Node:** Add support for TLS ([#8266](https://github.com/n8n-io/n8n/issues/8266)) ([e796e7f](https://github.com/n8n-io/n8n/commit/e796e7f06d73a74a403000c53942d56cab91781b))
* **Switch Node:** Overhaul ([#7855](https://github.com/n8n-io/n8n/issues/7855)) ([f4092a9](https://github.com/n8n-io/n8n/commit/f4092a9e49f66845612420ba59a013796ed80d45))


### Performance Improvements

* **core:** Improve caching service ([#8213](https://github.com/n8n-io/n8n/issues/8213)) ([f53c482](https://github.com/n8n-io/n8n/commit/f53c482939db938c47523ac11a9538e35e1926a9)), closes [#7747](https://github.com/n8n-io/n8n/issues/7747)
* **core:** Optimize workflow activation errors ([#8242](https://github.com/n8n-io/n8n/issues/8242)) ([f293956](https://github.com/n8n-io/n8n/commit/f2939568cf399e67214e89bc7f859323aaeda8dd))



# [1.23.0](https://github.com/n8n-io/n8n/compare/n8n@1.22.0...n8n@1.23.0) (2024-01-03)


### Bug Fixes

* **Asana Node:** Omit body from GET, HEAD, and DELETE requests ([#8057](https://github.com/n8n-io/n8n/issues/8057)) ([15ffd4f](https://github.com/n8n-io/n8n/commit/15ffd4fb9f967302e2444a873a804d2ccb64e748))
* **core:** Better input validation for the changeRole endpoint ([#8189](https://github.com/n8n-io/n8n/issues/8189)) ([cfe9525](https://github.com/n8n-io/n8n/commit/cfe9525dd4e2dbf2496bd86ad854bb744b5dc8fe))
* **core:** Fix issue that pinnedData is not used with Test-Webhooks ([#8123](https://github.com/n8n-io/n8n/issues/8123)) ([fa8bd8b](https://github.com/n8n-io/n8n/commit/fa8bd8b9eb202989229028cb6975cd2b50e5eef9))
* **core:** Handle empty executions table in pruning in migrations ([#8121](https://github.com/n8n-io/n8n/issues/8121)) ([ffaa30d](https://github.com/n8n-io/n8n/commit/ffaa30ddc4ee312f44726c17a7ec91b5551092ad))
* **core:** Remove circular dependency in WorkflowService and ActiveWorkflowRunner ([#8128](https://github.com/n8n-io/n8n/issues/8128)) ([21788d9](https://github.com/n8n-io/n8n/commit/21788d9153fb730965dabbce64c50c3b929ee728)), closes [#8122](https://github.com/n8n-io/n8n/issues/8122)
* **core:** Use pinned data only for manual mode ([#8164](https://github.com/n8n-io/n8n/issues/8164)) ([ea7e76f](https://github.com/n8n-io/n8n/commit/ea7e76fa3b3dc1f37b0415e14ea5ff90b8017b9a))
* **Discord Node:** Remove unnecessary requirement on parameters ([#8060](https://github.com/n8n-io/n8n/issues/8060)) ([ef3a577](https://github.com/n8n-io/n8n/commit/ef3a57719eb42777502cafdd38009e6cb5b484ce))
* **editor:** Avoid sanitizing output to search node data ([#8126](https://github.com/n8n-io/n8n/issues/8126)) ([c83d9f4](https://github.com/n8n-io/n8n/commit/c83d9f45bab986eb930e9da69eec970d3a72263d))
* **editor:** Enable explicit undo keyboard shortcut across all code editors ([#8178](https://github.com/n8n-io/n8n/issues/8178)) ([cf7f668](https://github.com/n8n-io/n8n/commit/cf7f6688bac5dd31dc3a45df4ecce579939141e2)), closes [#5297](https://github.com/n8n-io/n8n/issues/5297)
* **editor:** Fix operation change failing in certain conditions ([#8114](https://github.com/n8n-io/n8n/issues/8114)) ([711fa2b](https://github.com/n8n-io/n8n/commit/711fa2b9251154b50d8e5e7cd9a857ccb2c0bec6)), closes [/github.com/n8n-io/n8n/blob/7806a65229878a473f5526bad0b94614e8bfa8aa/packages/workflow/src/NodeHelpers.ts#L786](https://github.com//github.com/n8n-io/n8n/blob/7806a65229878a473f5526bad0b94614e8bfa8aa/packages/workflow/src/NodeHelpers.ts/issues/L786)
* **editor:** Fix templates view layout ([#8196](https://github.com/n8n-io/n8n/issues/8196)) ([d01e42a](https://github.com/n8n-io/n8n/commit/d01e42a2aabedfd4c0f79799bbfc9b1a235d4233))
* **editor:** Fix UI urls when hosted behind a path prefix ([#8198](https://github.com/n8n-io/n8n/issues/8198)) ([5c078f1](https://github.com/n8n-io/n8n/commit/5c078f1b3d78c7038bfdbb083fd029ef61bf2dfc)), closes [#8061](https://github.com/n8n-io/n8n/issues/8061)
* **editor:** Prevent browser zoom when scrolling inside sticky edit mode ([#8116](https://github.com/n8n-io/n8n/issues/8116)) ([e928210](https://github.com/n8n-io/n8n/commit/e928210ccdc00ad8a38e3f96ba5145c35e7b007b))
* **editor:** Prevent canvas undo/redo when NDV is open ([#8118](https://github.com/n8n-io/n8n/issues/8118)) ([39e45d8](https://github.com/n8n-io/n8n/commit/39e45d8b929d474f1e7587329b003fe15b61636d))
* **editor:** Prevent storing pairedItem data inside of pinData ([#8173](https://github.com/n8n-io/n8n/issues/8173)) ([405e267](https://github.com/n8n-io/n8n/commit/405e26757e2591b42a4bfeedd1fea997fbbb08c9))
* **GitHub Node:** Fix issue that File->Get did not run once per item ([#8190](https://github.com/n8n-io/n8n/issues/8190)) ([11cda41](https://github.com/n8n-io/n8n/commit/11cda41214100a1a3e65309434ab8be3ccef1898))
* **Invoice Ninja Node:** Fix issue with custom invoice numbers not working with v5 ([#8200](https://github.com/n8n-io/n8n/issues/8200)) ([3b6ae2d](https://github.com/n8n-io/n8n/commit/3b6ae2d0a510a57b27fc1a44cb3e710e2a783800))
* **Microsoft Excel 365 Node:** Ensure arg is string during worksheet table search ([#8154](https://github.com/n8n-io/n8n/issues/8154)) ([8e873ca](https://github.com/n8n-io/n8n/commit/8e873ca2f3c73ddd7bbef2218d8da82032f66cec))
* **Notion Node:** Ensure arg is string during page ID extraction ([#8153](https://github.com/n8n-io/n8n/issues/8153)) ([e94b8a6](https://github.com/n8n-io/n8n/commit/e94b8a6c30aaa2e59117d5a0cc03e1590d7ea8ca))
* **Redis Trigger Node:** Activating a workflow with a Redis trigger fails ([#8129](https://github.com/n8n-io/n8n/issues/8129)) ([a169b74](https://github.com/n8n-io/n8n/commit/a169b7406279de43dbd3fd7d13166d987c60d01a))
* **Schedule Trigger Node:** Use the correct `moment` import ([#8185](https://github.com/n8n-io/n8n/issues/8185)) ([17a4e2e](https://github.com/n8n-io/n8n/commit/17a4e2ea80c664e248c136b7e66eef710ccba7f2)), closes [#8184](https://github.com/n8n-io/n8n/issues/8184)
* Show public API upgrade CTA when feature is not enabled ([#8109](https://github.com/n8n-io/n8n/issues/8109)) ([e9c7fd7](https://github.com/n8n-io/n8n/commit/e9c7fd73975ced504d5a16a0dbbc313f15ccd8ab))


### Features

* **core:** Add closeFunction support to Sub-Nodes ([#7708](https://github.com/n8n-io/n8n/issues/7708)) ([bec0fae](https://github.com/n8n-io/n8n/commit/bec0faed9e51fe6ea20ab3b07b4dfa849b28516b))
* **core:** Add user.profile.beforeUpdate hook ([#8144](https://github.com/n8n-io/n8n/issues/8144)) ([e126ed7](https://github.com/n8n-io/n8n/commit/e126ed74f3d9ed3dae72252cb8c9e8a6f7620808))
* **core:** Improvements/overhaul for nodes working with binary data ([#7651](https://github.com/n8n-io/n8n/issues/7651)) ([5e16dd4](https://github.com/n8n-io/n8n/commit/5e16dd4ab4457acf21d3d7a3566d07944ff7f857))
* **core:** Remove discontinued crypto-js  ([#8104](https://github.com/n8n-io/n8n/issues/8104)) ([01e9a79](https://github.com/n8n-io/n8n/commit/01e9a79238bbd2c14ae77a12e54fc1c6f41e1246))
* **core:** Unify application components shutdown ([#8097](https://github.com/n8n-io/n8n/issues/8097)) ([3a881be](https://github.com/n8n-io/n8n/commit/3a881be6c25b3e16d8c53227dc851cb420f5f1bf))
* **editor:** Add node execution status indicator to output panel ([#8124](https://github.com/n8n-io/n8n/issues/8124)) ([ab74bad](https://github.com/n8n-io/n8n/commit/ab74bade05cb30e7fa65a491789a3df3ab7bf8b8))
* **editor:** Add template Id to workflow metadata ([#8088](https://github.com/n8n-io/n8n/issues/8088)) ([517b050](https://github.com/n8n-io/n8n/commit/517b050d0ae1a64987ac00d5795c5e59ed176f3f))
* **Home Assistant Node:** Use the new Home Assistant logo ([#8150](https://github.com/n8n-io/n8n/issues/8150)) ([518a99e](https://github.com/n8n-io/n8n/commit/518a99e5287dc648edafd34a4dd27c9205eb8629))
* **Qdrant Vector Store Node:** Qdrant vector store support ([#8080](https://github.com/n8n-io/n8n/issues/8080)) ([66460f6](https://github.com/n8n-io/n8n/commit/66460f66b0b02ae6f342e52500b29fe8b724e1dc))
* **Wordpress Node:** Add option to ignore error when using self signed certificates ([#8199](https://github.com/n8n-io/n8n/issues/8199)) ([65c8e12](https://github.com/n8n-io/n8n/commit/65c8e12b96ac8c1c53d3879d91982ca834f3cda1))



# [1.22.0](https://github.com/n8n-io/n8n/compare/n8n@1.21.0...n8n@1.22.0) (2023-12-21)


### Bug Fixes

* **ActiveCampaign Node:** Fix pagination issue when loading tags ([#8017](https://github.com/n8n-io/n8n/issues/8017)) ([1943857](https://github.com/n8n-io/n8n/commit/19438572312cf9354c333aeb52ccbf1ab81fc51f))
* **core:** Close db connection gracefully when exiting ([#8045](https://github.com/n8n-io/n8n/issues/8045)) ([e69707e](https://github.com/n8n-io/n8n/commit/e69707efd4bd947fdf6b9c66f373da63d34f41e9))
* **core:** Consider timeout in shutdown an error ([#8050](https://github.com/n8n-io/n8n/issues/8050)) ([4cae976](https://github.com/n8n-io/n8n/commit/4cae976a3b428bd528fe71ef0b240c0fd6e23bbf))
* **core:** Do not display error when stopping jobless execution in queue mode ([#8007](https://github.com/n8n-io/n8n/issues/8007)) ([8e6b951](https://github.com/n8n-io/n8n/commit/8e6b951a76e08b9ee9740fdd853f77553ad60cd6))
* **core:** Fix shutdown if terminating before hooks are initialized ([#8047](https://github.com/n8n-io/n8n/issues/8047)) ([6ae2f5e](https://github.com/n8n-io/n8n/commit/6ae2f5efea65e23029475ccdc5a65ec7c8152423))
* **core:** Handle multiple termination signals correctly ([#8046](https://github.com/n8n-io/n8n/issues/8046)) ([67bd8ad](https://github.com/n8n-io/n8n/commit/67bd8ad698bd0afe6ff7183d75da8bca4085598e))
* **core:** Initialize queue once in queue mode ([#8025](https://github.com/n8n-io/n8n/issues/8025)) ([53c0b49](https://github.com/n8n-io/n8n/commit/53c0b49d15047461e3b65baed65c9d76dff99539))
* **core:** Prevent axios from force setting a form-urlencoded content-type ([#8117](https://github.com/n8n-io/n8n/issues/8117)) ([bba9576](https://github.com/n8n-io/n8n/commit/bba95761e2f2b54af1fcab8a7b1d626ca10d537e)), closes [/github.com/axios/axios/blob/v1.x/lib/core/dispatchRequest.js#L45-L47](https://github.com//github.com/axios/axios/blob/v1.x/lib/core/dispatchRequest.js/issues/L45-L47)
* **core:** Remove circular references before serializing executions in public API ([#8043](https://github.com/n8n-io/n8n/issues/8043)) ([989888d](https://github.com/n8n-io/n8n/commit/989888d9bcec6f4eb3c811ce10d480737d96b102)), closes [#8030](https://github.com/n8n-io/n8n/issues/8030)
* **core:** Restore workflow ID during execution creation ([#8031](https://github.com/n8n-io/n8n/issues/8031)) ([c5e6ba8](https://github.com/n8n-io/n8n/commit/c5e6ba8cdd4a8f117ccc2e89e55497117156d8af)), closes [/github.com/n8n-io/n8n/pull/8002/files#diff-c8cbb62ca9ab2ae45e5f565cd8c63fff6475809a6241ea0b90acc575615224](https://github.com//github.com/n8n-io/n8n/pull/8002/files/issues/diff-c8cbb62ca9ab2ae45e5f565cd8c63fff6475809a6241ea0b90acc575615224)
* **core:** Use relative imports for dynamic imports in SecurityAuditService ([#8086](https://github.com/n8n-io/n8n/issues/8086)) ([785bf99](https://github.com/n8n-io/n8n/commit/785bf9974e38ea84c016e210a3108f4af567510d)), closes [#8085](https://github.com/n8n-io/n8n/issues/8085)
* **editor:** Add back credential `use` permission ([#8023](https://github.com/n8n-io/n8n/issues/8023)) ([329e5bf](https://github.com/n8n-io/n8n/commit/329e5bf9eed8556aba2bbd50bad9dbd6d3b373ad))
* **editor:** Cleanup Executions page component ([#8053](https://github.com/n8n-io/n8n/issues/8053)) ([2689c37](https://github.com/n8n-io/n8n/commit/2689c37e87c5b3ae5029121f4d3dc878841e8844))
* **editor:** Disable auto scroll and list size check when clicking on executions ([#7983](https://github.com/n8n-io/n8n/issues/7983)) ([fcb8b91](https://github.com/n8n-io/n8n/commit/fcb8b91f37e1fb0ef42f411c84390180e1ed7bbe))
* **editor:** Ensure execution data overrides pinned data when copying in executions view ([#8009](https://github.com/n8n-io/n8n/issues/8009)) ([1d1cb0d](https://github.com/n8n-io/n8n/commit/1d1cb0d3c530856e0c26d8f146f60b2555625ab6))
* **editor:** Fix copy/paste issue when switch node is in workflow ([#8103](https://github.com/n8n-io/n8n/issues/8103)) ([4b86926](https://github.com/n8n-io/n8n/commit/4b86926752fb1304a46385cb46bdf34fda0d53b6))
* **editor:** Make keyboard shortcuts more strict; don't accept extra Ctrl/Alt/Shift keys ([#8024](https://github.com/n8n-io/n8n/issues/8024)) ([8df49e1](https://github.com/n8n-io/n8n/commit/8df49e134d886267f9f7475573d013371220dcac))
* **editor:** Show credential share info only to appropriate users ([#8020](https://github.com/n8n-io/n8n/issues/8020)) ([b29b4d4](https://github.com/n8n-io/n8n/commit/b29b4d442bb0617aa516748ec48379eae0996cf0))
* **editor:** Turn off executions list auto-refresh after leaving the page ([#8005](https://github.com/n8n-io/n8n/issues/8005)) ([e3c363d](https://github.com/n8n-io/n8n/commit/e3c363d72cf4ee49086d012f92a7b34be958482f))
* **editor:** Update image sizes in template description not to be full width always ([#8037](https://github.com/n8n-io/n8n/issues/8037)) ([63a6e7e](https://github.com/n8n-io/n8n/commit/63a6e7e0340e1b00719f212ac620600a90d70ef1))
* **HTTP Request Node:** Do not create circular references in HTTP request node output ([#8030](https://github.com/n8n-io/n8n/issues/8030)) ([5b7ea16](https://github.com/n8n-io/n8n/commit/5b7ea16d9a20880c72779b02620e99ebe9f3617a))
* Stop binary data restoration from preventing execution from finishing ([#8082](https://github.com/n8n-io/n8n/issues/8082)) ([5ffff1b](https://github.com/n8n-io/n8n/commit/5ffff1bb22691c09c5ca8b3ada2a19d5ce155a0b))
* Upgrade axios to address CVE-2023-45857 ([#7713](https://github.com/n8n-io/n8n/issues/7713)) ([64eb9bb](https://github.com/n8n-io/n8n/commit/64eb9bbc3624ee8f2fa90812711ad568926fdca8))


### Features

* Add config option to prefer GET request over LIST when using Hashicorp Vault ([#8049](https://github.com/n8n-io/n8n/issues/8049)) ([439a22d](https://github.com/n8n-io/n8n/commit/439a22d68f7bf32f281b1078b71607307640a09b))
* Add option to `returnIntermediateSteps` for AI agents ([#8113](https://github.com/n8n-io/n8n/issues/8113)) ([7806a65](https://github.com/n8n-io/n8n/commit/7806a65229878a473f5526bad0b94614e8bfa8aa))
* **core:** Add N8N_GRACEFUL_SHUTDOWN_TIMEOUT env var ([#8068](https://github.com/n8n-io/n8n/issues/8068)) ([614f488](https://github.com/n8n-io/n8n/commit/614f48838626e2af8e3f2e76ee4a144af2d40f72))
* **editor:** Add lead enrichment suggestions to workflow list ([#8042](https://github.com/n8n-io/n8n/issues/8042)) ([36a923c](https://github.com/n8n-io/n8n/commit/36a923cf7bd4d42b8f8decbf01255c41d6dc1671)), closes [-update-workflows-list-page-to-show-fake-door-templates#comment-b6644c99](https://github.com/-update-workflows-list-page-to-show-fake-door-templates/issues/comment-b6644c99)
* **editor:** Finalize workers view ([#8052](https://github.com/n8n-io/n8n/issues/8052)) ([edfa784](https://github.com/n8n-io/n8n/commit/edfa78414d6bce901becc05e9d860f2521139688))
* **editor:** Gracefully ignore invalid payloads in postMessage handler ([#8096](https://github.com/n8n-io/n8n/issues/8096)) ([9d22c7a](https://github.com/n8n-io/n8n/commit/9d22c7a2782a1908f81bcf80260cd91cb296e239))
* **editor:** Upgrade frontend tooling to address a few vulnerabilities ([#8100](https://github.com/n8n-io/n8n/issues/8100)) ([19b7f1f](https://github.com/n8n-io/n8n/commit/19b7f1ffb17dcd6ac77839f97c2544f60f4ad55e))
* **Filter Node:** Overhaul UI by adding the new filter component ([#8016](https://github.com/n8n-io/n8n/issues/8016)) ([3d53052](https://github.com/n8n-io/n8n/commit/3d530522f828dfc985ae98e4bb551aa3a2bd44c6))
* **Respond to Webhook Node:** Overhaul with improvements like returning all items ([#8093](https://github.com/n8n-io/n8n/issues/8093)) ([32d397e](https://github.com/n8n-io/n8n/commit/32d397eff315fdc77677c0b134a7a25bcd8ca5d0))


### Performance Improvements

* **editor:** Improve canvas rendering performance ([#8022](https://github.com/n8n-io/n8n/issues/8022)) ([b780436](https://github.com/n8n-io/n8n/commit/b780436a6b445dc5951217b5a1f2c61b34961757))



# [1.21.0](https://github.com/n8n-io/n8n/compare/n8n@1.20.0...n8n@1.21.0) (2023-12-13)


### Bug Fixes

* **core:** Ensure inviter and invitee are set correctly in invite link ([#7943](https://github.com/n8n-io/n8n/issues/7943)) ([386bd61](https://github.com/n8n-io/n8n/commit/386bd619676e54e960ca0af3ff47fa3b9c16c813)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **core:** Fix user comparison in same-user subworkflow caller policy ([#7913](https://github.com/n8n-io/n8n/issues/7913)) ([92bab72](https://github.com/n8n-io/n8n/commit/92bab72cffb1083b495d211d0a31920e83e66769))
* **core:** Perform multi-main leader check against key ID ([#7964](https://github.com/n8n-io/n8n/issues/7964)) ([1a87f70](https://github.com/n8n-io/n8n/commit/1a87f70e8404218308072ee2f35c6ba2af34c23f)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **core:** Prevent workflow history saving error from happening ([#7812](https://github.com/n8n-io/n8n/issues/7812)) ([e5581ce](https://github.com/n8n-io/n8n/commit/e5581ce8023e21d3dcf140099f3a53e5ffb4584f))
* **editor:** Add missing string for worker in log streaming ([#7971](https://github.com/n8n-io/n8n/issues/7971)) ([148bc1d](https://github.com/n8n-io/n8n/commit/148bc1d303af3aafd73e73e11c3dd9cefd40a1dd)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **editor:** Allow SSH protocol in git repository URL for environments ([#7944](https://github.com/n8n-io/n8n/issues/7944)) ([bc1c72f](https://github.com/n8n-io/n8n/commit/bc1c72f992a47a9c263aec175ca820088cf340ec)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **editor:** Fix bug with node names with certain characters ([#8013](https://github.com/n8n-io/n8n/issues/8013)) ([26f0d57](https://github.com/n8n-io/n8n/commit/26f0d57f5fb71a06c92968a4997cceae62f32312))
* **editor:** Fix Webhook URL expansion icon ([#8011](https://github.com/n8n-io/n8n/issues/8011)) ([b00b905](https://github.com/n8n-io/n8n/commit/b00b9057a42f23cd9c4bb6675a3e6134610bf81b))
* **editor:** Prevent opening NDV search if `/` is typed in a contenteditable element ([#7968](https://github.com/n8n-io/n8n/issues/7968)) ([e8a493f](https://github.com/n8n-io/n8n/commit/e8a493f71863e6a5d2685b48a61a0d11daf5edc5))
* **editor:** Return early in ws message handler if no 'command' keyword is found ([#7946](https://github.com/n8n-io/n8n/issues/7946)) ([5b2defc](https://github.com/n8n-io/n8n/commit/5b2defc867a0627a861bf0fb98abfd99f8efe934))
* Ensure external hooks post workflow execute run in queue mode ([#7947](https://github.com/n8n-io/n8n/issues/7947)) ([3ba7deb](https://github.com/n8n-io/n8n/commit/3ba7deb337963d40ae70f40ffb2f4eb23cac89b7)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **FileMaker Node:** Prevent erroring on zero fields loaded ([#7955](https://github.com/n8n-io/n8n/issues/7955)) ([10ad386](https://github.com/n8n-io/n8n/commit/10ad3866048ad06d0e8455ed2c52c618ae9e5032)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* Fix issue preventing secrets from loading if the path contains - or / ([#7988](https://github.com/n8n-io/n8n/issues/7988)) ([0ac9594](https://github.com/n8n-io/n8n/commit/0ac959463f25187c5be4116a2209411afd903d87))
* **Google Sheets Node:** Prevent erroring on zero sheet search results ([#7957](https://github.com/n8n-io/n8n/issues/7957)) ([9b877a9](https://github.com/n8n-io/n8n/commit/9b877a942787c855c3a3a011c19c5d1d30b8da67)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **Google Sheets Node:** Prevent erroring when fetching mapping columns ([#7972](https://github.com/n8n-io/n8n/issues/7972)) ([29a1066](https://github.com/n8n-io/n8n/commit/29a10668d17cdeb8b0e93c912f59c5976b6fc6c6)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **Postgres Node:** Do not include id column in upsert fields selection if it's not unique ([#7975](https://github.com/n8n-io/n8n/issues/7975)) ([435392c](https://github.com/n8n-io/n8n/commit/435392cbfe150c5e85d092686b3b7e20273421cc))
* **Postgres Trigger Node:** Increase manual trigger timeout from 30 to 60 seconds ([#8015](https://github.com/n8n-io/n8n/issues/8015)) ([09a5729](https://github.com/n8n-io/n8n/commit/09a5729305a8072f5e98a320c85ad1c83a6946ed))
* Restrict updating/deleting of shared but not owned credentials ([#7950](https://github.com/n8n-io/n8n/issues/7950)) ([42e828d](https://github.com/n8n-io/n8n/commit/42e828d5c655e54b6a4ec83c398c684996b9cc3e)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **Webhook Node:** Binary data handling ([#7804](https://github.com/n8n-io/n8n/issues/7804)) ([565b409](https://github.com/n8n-io/n8n/commit/565b409a82ca6173efd19f26a5f5b27a359a3b87))
* **Webhook Node:** Do not create binary data when there is no data in the request ([#8000](https://github.com/n8n-io/n8n/issues/8000)) ([70f0755](https://github.com/n8n-io/n8n/commit/70f0755278e0a2bdb61c29623f27623b65473ab4)), closes [/github.com/n8n-io/n8n/pull/7804/files#r1422641833](https://github.com//github.com/n8n-io/n8n/pull/7804/files/issues/r1422641833)


### Features

* Add config option for external secret update interval ([#7995](https://github.com/n8n-io/n8n/issues/7995)) ([b6c1c04](https://github.com/n8n-io/n8n/commit/b6c1c04b541d0944c5baac1ab021539c8f020f10))
* AI nodes usability fixes + Summarization Chain V2 ([#7949](https://github.com/n8n-io/n8n/issues/7949)) ([dcf1286](https://github.com/n8n-io/n8n/commit/dcf12867b3c49596cd214812caee3292d2e794de)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* Data transformation nodes and actions in Nodes Panel ([#7760](https://github.com/n8n-io/n8n/issues/7760)) ([675ec21](https://github.com/n8n-io/n8n/commit/675ec21d335af2b2c9598bc2bec18194506ef71a))
* **editor:** Add AppCues tracking for onboarding event ([#7945](https://github.com/n8n-io/n8n/issues/7945)) ([04cabaf](https://github.com/n8n-io/n8n/commit/04cabafef7acbc30cba647732e2ca8ae8a02d29a)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **editor:** Add option to disable NDV in workflow previews  ([#7990](https://github.com/n8n-io/n8n/issues/7990)) ([393afef](https://github.com/n8n-io/n8n/commit/393afef1747f168d5fa42be2424fd02125f1bbac)), closes [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **editor:** Filter component + implement in If node ([#7490](https://github.com/n8n-io/n8n/issues/7490)) ([8a53434](https://github.com/n8n-io/n8n/commit/8a5343401dd355436120a9a424ae455e80b50da6))
* **editor:** Show template credential setup based on feature flag ([#7989](https://github.com/n8n-io/n8n/issues/7989)) ([08ee307](https://github.com/n8n-io/n8n/commit/08ee3072093fb26b14b48e2b35d8c8d018317f13))
* **Google Ads Node:** Update to support v15 ([#7962](https://github.com/n8n-io/n8n/issues/7962)) ([7f01269](https://github.com/n8n-io/n8n/commit/7f0126915aae514a0ab515a4baf5582da2aeb1e3))
* Introduce advanced permissions ([#7844](https://github.com/n8n-io/n8n/issues/7844)) ([dbd62a4](https://github.com/n8n-io/n8n/commit/dbd62a4992ab8aca59e3cb50d3d970454e462238))
* **Local File Trigger Node:** Add polling option typically good to watch network files/folders ([#7942](https://github.com/n8n-io/n8n/issues/7942)) ([2fbdfec](https://github.com/n8n-io/n8n/commit/2fbdfec0c0a3f5da64764e7821e84db30b664e49))
* **n8n Form Trigger Node:** Improvements ([#7571](https://github.com/n8n-io/n8n/issues/7571)) ([953a58f](https://github.com/n8n-io/n8n/commit/953a58f18bfdd36fa8b526ca6213631aacab49cb))



# [1.20.0](https://github.com/n8n-io/n8n/compare/n8n@1.19.0...n8n@1.20.0) (2023-12-06)


### Bug Fixes

* **AWS DynamoDB Node:** Improve error message parsing ([#7793](https://github.com/n8n-io/n8n/issues/7793)) ([5ba5ed8](https://github.com/n8n-io/n8n/commit/5ba5ed8e3c8ba2f909859bde129d92576fbda46f))
* **core:** Allow grace period for binary data deletion after manual execution ([#7889](https://github.com/n8n-io/n8n/issues/7889)) ([61d8aeb](https://github.com/n8n-io/n8n/commit/61d8aebeaf6487269b252b353fdf16dcb67f41ff))
* **core:** Consolidate ownership and sharing data on workflows and credentials ([#7920](https://github.com/n8n-io/n8n/issues/7920)) ([38b88b9](https://github.com/n8n-io/n8n/commit/38b88b946bab67dc1a964bb3c980a627d4a32595))
* **core:** Fix hard deletes stopping if database query throws ([#7848](https://github.com/n8n-io/n8n/issues/7848)) ([46dd4d3](https://github.com/n8n-io/n8n/commit/46dd4d3105db3a15c81903ae81c9bbb21a45397b))
* **core:** Make sure mfa secret and recovery codes are not returned on login ([#7936](https://github.com/n8n-io/n8n/issues/7936)) ([f5502cc](https://github.com/n8n-io/n8n/commit/f5502cc628f6b348f7fe3325b96ec9dc3360beaf)), closes [/github.com/n8n-io/n8n/pull/6994/files#diff-95a87cb029a3d26e6722df2e68132453fc254fc1f4540cbdaa95cfdbda1893deL91](https://github.com//github.com/n8n-io/n8n/pull/6994/files/issues/diff-95a87cb029a3d26e6722df2e68132453fc254fc1f4540cbdaa95cfdbda1893deL91) [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **editor:** Fix deletion of last execution at execution preview ([#7883](https://github.com/n8n-io/n8n/issues/7883)) ([ce2d388](https://github.com/n8n-io/n8n/commit/ce2d388f059c0bb32d27f4b29e901d1a70083610))
* **editor:** Replace isInstanceOwner checks with scopes where applicable ([#7858](https://github.com/n8n-io/n8n/issues/7858)) ([132d691](https://github.com/n8n-io/n8n/commit/132d691cbf983f60293c7423de0077fb7c97e0af))
* **Google Sheets Node:** Fix issue with paired items not being set correctly ([#7862](https://github.com/n8n-io/n8n/issues/7862)) ([5207a2f](https://github.com/n8n-io/n8n/commit/5207a2fe5210e40d3b2aedd95182a18e497c72ab))
* **Notion Node:** Fix broken Notion node parameters ([#7864](https://github.com/n8n-io/n8n/issues/7864)) ([51d1f5b](https://github.com/n8n-io/n8n/commit/51d1f5b82070542d45c3d57387343959a3f0abb2)), closes [#7791](https://github.com/n8n-io/n8n/issues/7791)


### Features

* **BambooHR Node:** Add support for Only Current on company reports ([#7878](https://github.com/n8n-io/n8n/issues/7878)) ([4175801](https://github.com/n8n-io/n8n/commit/4175801c90ad4f744d1a7c331d4fb20891ed2e9e))
* **core:** Allow admin creation ([#7837](https://github.com/n8n-io/n8n/issues/7837)) ([476806e](https://github.com/n8n-io/n8n/commit/476806ebb0f31f656992fb67aba37116f10e1475))
* **editor:** Add sections to create node panel ([#7831](https://github.com/n8n-io/n8n/issues/7831)) ([39fa8d2](https://github.com/n8n-io/n8n/commit/39fa8d21bbee5d870b2620ec65401a5ca134c4f1))
* **editor:** Open template credential setup from collection ([#7882](https://github.com/n8n-io/n8n/issues/7882)) ([627ddb9](https://github.com/n8n-io/n8n/commit/627ddb91fb6c00796671a1f72f59a251cd89004d))
* **editor:** Select credentials in template setup if theres only one ([#7879](https://github.com/n8n-io/n8n/issues/7879)) ([fe3417a](https://github.com/n8n-io/n8n/commit/fe3417a615534a01cb0c7b5e8f47bc18abd5cd4d))


### Performance Improvements

* **editor:** Improve node rendering performance when opening large workflows ([#7904](https://github.com/n8n-io/n8n/issues/7904)) ([a8049a0](https://github.com/n8n-io/n8n/commit/a8049a0def21506ebf4fb1d3b69ae28ec35fdc21)), closes [#7901](https://github.com/n8n-io/n8n/issues/7901) [4#a39f9e5ba64a48b58a71d81c837e8227](https://github.com/4/issues/a39f9e5ba64a48b58a71d81c837e8227) [4#f6a177d32bde4b57ae2da0b8e454](https://github.com/4/issues/f6a177d32bde4b57ae2da0b8e454) [4#fef2d36ab02247e1a0f65a74f6fb534](https://github.com/4/issues/fef2d36ab02247e1a0f65a74f6fb534)
* **editor:** Improve performance when opening large workflows with node issues ([#7901](https://github.com/n8n-io/n8n/issues/7901)) ([4bd7ae2](https://github.com/n8n-io/n8n/commit/4bd7ae29f7c82b8817420e617a123024147c6c70))



# [1.19.0](https://github.com/n8n-io/n8n/compare/n8n@1.18.0...n8n@1.19.0) (2023-11-29)


### Bug Fixes

* **core:** Ensure member and admin cannot be promoted to owner ([#7830](https://github.com/n8n-io/n8n/issues/7830)) ([9b87a59](https://github.com/n8n-io/n8n/commit/9b87a596ca4aec462faedcca1ba4655b168bc3bc)), closes [/linear.app/n8n/issue/PAY-985/add-user-role-modification-endpoint#comment-62355f6](https://github.com//linear.app/n8n/issue/PAY-985/add-user-role-modification-endpoint/issues/comment-62355f6)
* **core:** Prevent error messages due to statistics about data loading ([#7824](https://github.com/n8n-io/n8n/issues/7824)) ([847f6ac](https://github.com/n8n-io/n8n/commit/847f6ac771316eea270d2e83adac5d8a6483475a))
* **core:** Tighten checks for multi-main setup usage ([#7788](https://github.com/n8n-io/n8n/issues/7788)) ([fdb2c18](https://github.com/n8n-io/n8n/commit/fdb2c18ecc49d1e8759e809d2e2c2e4aa17009da))
* **core:** Use AbortController to notify nodes to abort execution ([#6141](https://github.com/n8n-io/n8n/issues/6141)) ([d2c18c5](https://github.com/n8n-io/n8n/commit/d2c18c57274cac02e70cf1cc9e533a6ca98f0ec6))
* **editor:** Add telemetry to workflow history ([#7811](https://github.com/n8n-io/n8n/issues/7811)) ([d497041](https://github.com/n8n-io/n8n/commit/d4970410e1ba328b05ddc23abcbf33c719de5624))
* **editor:** Allow owners and admins to share workflows and credentials they don't own ([#7833](https://github.com/n8n-io/n8n/issues/7833)) ([3ab3ec9](https://github.com/n8n-io/n8n/commit/3ab3ec9da88f7b7ae07a98d7ef7c4f9892079048))
* **editor:** Disable context menu actions in read-only mode ([#7789](https://github.com/n8n-io/n8n/issues/7789)) ([902beff](https://github.com/n8n-io/n8n/commit/902beffce51d547094ea249d1fbbb70a879165d6))
* **editor:** Fix cloud plan data loading on instance ([#7841](https://github.com/n8n-io/n8n/issues/7841)) ([8b99384](https://github.com/n8n-io/n8n/commit/8b99384367161a47b3de13b7e83bcf6d07e3bf19))
* **editor:** Fix credential icon for old node type version ([#7843](https://github.com/n8n-io/n8n/issues/7843)) ([4074107](https://github.com/n8n-io/n8n/commit/40741075117dd8018ca1c6d03c050c3959142ebd))
* **editor:** Fix icon for unknown node type ([#7842](https://github.com/n8n-io/n8n/issues/7842)) ([28ac5a7](https://github.com/n8n-io/n8n/commit/28ac5a750eb28e9ab41611a76fa5fb9c30ce64dc))
* **editor:** Fix mouse position in workflow previews ([#7853](https://github.com/n8n-io/n8n/issues/7853)) ([c063398](https://github.com/n8n-io/n8n/commit/c0633987bfd6de24db0efc4bcb73adba9e9b6a74))
* **editor:** Show nice error when environment is not set up ([#7778](https://github.com/n8n-io/n8n/issues/7778)) ([5835e05](https://github.com/n8n-io/n8n/commit/5835e055d39921cdf2aa9799e427931bec8e5e2c))
* **editor:** Suppress dev server websocket messages in workflow view ([#7808](https://github.com/n8n-io/n8n/issues/7808)) ([685ffd7](https://github.com/n8n-io/n8n/commit/685ffd74137199f5e10145a33f3e0f03dabc2e7f))
* **Google Sheets Node:** Read operation execute for each item ([#7800](https://github.com/n8n-io/n8n/issues/7800)) ([d548872](https://github.com/n8n-io/n8n/commit/d5488725a83f6705b95c9de9d8736adf1b870134))
* **HTTP Request Node:** Enable expressions for binary input data fields ([#7782](https://github.com/n8n-io/n8n/issues/7782)) ([6208af0](https://github.com/n8n-io/n8n/commit/6208af07eb393b0fb8483b8ae4949a63423cc409))
* **Microsoft SQL Node:** Prevent double escaping table name ([#7801](https://github.com/n8n-io/n8n/issues/7801)) ([73ec753](https://github.com/n8n-io/n8n/commit/73ec7533ce4724940c2b23f677a9dfcf75de6a16))


### Features

* Add AI tool building capabilities  ([#7336](https://github.com/n8n-io/n8n/issues/7336)) ([87def60](https://github.com/n8n-io/n8n/commit/87def60979bd6525b59df4bd811571a2afe83bec))
* Add initial scope checks via decorators ([#7737](https://github.com/n8n-io/n8n/issues/7737)) ([a37f1cb](https://github.com/n8n-io/n8n/commit/a37f1cb0bad87c486c387383f8179aa42f0b9e1a))
* Add user role select to users list settings page ([#7796](https://github.com/n8n-io/n8n/issues/7796)) ([137e238](https://github.com/n8n-io/n8n/commit/137e23853fdbd3e62037a6cb7f742811af41a03d))
* Ado 1296 spike credential setup in templates ([#7786](https://github.com/n8n-io/n8n/issues/7786)) ([aae45b0](https://github.com/n8n-io/n8n/commit/aae45b043b9e1427f9ffc44ef88d719782fccee5))
* **core:** Add Support for custom CORS origins for webhooks ([#7455](https://github.com/n8n-io/n8n/issues/7455)) ([99a9ea4](https://github.com/n8n-io/n8n/commit/99a9ea497a3d21739f911da5c88c076f60471bed))
* **core:** Allow user role modification ([#7797](https://github.com/n8n-io/n8n/issues/7797)) ([7a86d36](https://github.com/n8n-io/n8n/commit/7a86d3606852fcbc537533af24eef34279b229c6))
* **core:** Set up endpoint for all existing roles with license flag ([#7834](https://github.com/n8n-io/n8n/issues/7834)) ([2356fb0](https://github.com/n8n-io/n8n/commit/2356fb0f0c247271ffa00d1cf25460e06212f1c4))
* **editor:** Add node name and version to NDV node settings ([#7731](https://github.com/n8n-io/n8n/issues/7731)) ([da85198](https://github.com/n8n-io/n8n/commit/da851986f6f7cd4375b06c28a149dcb375fe8b83))
* **editor:** Add routing middleware, permission checks, RBAC store, RBAC component ([#7702](https://github.com/n8n-io/n8n/issues/7702)) ([67a8891](https://github.com/n8n-io/n8n/commit/67a88914f2f2d11c413e7f627d659333d8419af8))
* **editor:** Replace middleware for Role checks with Scope checks ([#7847](https://github.com/n8n-io/n8n/issues/7847)) ([72852a6](https://github.com/n8n-io/n8n/commit/72852a60eb15cbf45ebcdd390770c4cd9929a457))
* **editor:** Show avatars for users currently working on the same workflow ([#7763](https://github.com/n8n-io/n8n/issues/7763)) ([77bc8ec](https://github.com/n8n-io/n8n/commit/77bc8ecd4b1552f7253bc1348087db518ce7ce07))
* **Notion Node:** Option to simplify output in getChildBlocks operation ([#7791](https://github.com/n8n-io/n8n/issues/7791)) ([d667bca](https://github.com/n8n-io/n8n/commit/d667bca658a2b79fa5d0afba9ef25f26a10cdfc2))
* **Slack Node:** Add support for getting the profile of a user ([#7829](https://github.com/n8n-io/n8n/issues/7829)) ([90bb6ba](https://github.com/n8n-io/n8n/commit/90bb6ba4174a71f0d42e8dc9f009b879ca9d4616))



# [1.18.0](https://github.com/n8n-io/n8n/compare/n8n@1.17.0...n8n@1.18.0) (2023-11-22)


### Bug Fixes

* **core:** Account for non-ASCII chars in filename on binary data download ([#7742](https://github.com/n8n-io/n8n/issues/7742)) ([b4ebb1a](https://github.com/n8n-io/n8n/commit/b4ebb1a28dc87c297721299a635e836dcaa273b7))
* **core:** Correct permissions for getstatus ([#7724](https://github.com/n8n-io/n8n/issues/7724)) ([f96c1d2](https://github.com/n8n-io/n8n/commit/f96c1d204400028c55a2120d0569180379c0649f))
* **core:** Ensure failed executions are saved in queue mode ([#7744](https://github.com/n8n-io/n8n/issues/7744)) ([b7c5c74](https://github.com/n8n-io/n8n/commit/b7c5c7406f6f978bbd84737de34114e9492ae5f6))
* **core:** Guard against node not found on cancelling test webhook ([#7750](https://github.com/n8n-io/n8n/issues/7750)) ([6be453b](https://github.com/n8n-io/n8n/commit/6be453b716eff14df420ef565ea1b5ffb3ce73f0))
* **editor:** Handle permission edge cases (empty scopes) ([#7723](https://github.com/n8n-io/n8n/issues/7723)) ([e2ffd39](https://github.com/n8n-io/n8n/commit/e2ffd397fc0ab8d88128ba78d02c5df003af4a9d))
* **editor:** Make sure LineController is registered with chart.js ([#7730](https://github.com/n8n-io/n8n/issues/7730)) ([ebee1a5](https://github.com/n8n-io/n8n/commit/ebee1a590873aa56c23fd610616196ee27fe657a))
* **editor:** Move workerview entry into settings menu ([#7761](https://github.com/n8n-io/n8n/issues/7761)) ([366cd67](https://github.com/n8n-io/n8n/commit/366cd672a74649a19fc927e0327ae7c19ed5a1fc))
* **editor:** Only show push to git menu item to owners ([#7766](https://github.com/n8n-io/n8n/issues/7766)) ([0d3d33d](https://github.com/n8n-io/n8n/commit/0d3d33dd1f2354248ac341a0c9f2553812f404e0))
* **editor:** Show v1 banner dismiss button if owner ([#7722](https://github.com/n8n-io/n8n/issues/7722)) ([44d3b3e](https://github.com/n8n-io/n8n/commit/44d3b3ed7ee77715006591a4f49049388fcd4035))
* **editor:** Use project diagram icon for worker view ([#7764](https://github.com/n8n-io/n8n/issues/7764)) ([ff0b651](https://github.com/n8n-io/n8n/commit/ff0b6511f74831c499ab032910dfa9cf38356e8c))
* **editor:** Validate user info before submiting ([#7608](https://github.com/n8n-io/n8n/issues/7608)) ([2064f7f](https://github.com/n8n-io/n8n/commit/2064f7f251913a0cc22b4e27bb38df921f711109))
* **GitHub Node:** Fix issue preventing file edits on branches ([#7734](https://github.com/n8n-io/n8n/issues/7734)) ([ce002a6](https://github.com/n8n-io/n8n/commit/ce002a6cc672d1e13cc3d3470add78781d1ef20e))
* **Google Sheets Node:** Check for `null` before destructuring ([#7729](https://github.com/n8n-io/n8n/issues/7729)) ([5d4a52d](https://github.com/n8n-io/n8n/commit/5d4a52d3b7e35924e1a8c9a2c808418bdf224d2c))
* **Item Lists Node:** Don't check same type in remove duplicates operation ([#7678](https://github.com/n8n-io/n8n/issues/7678)) ([4f30764](https://github.com/n8n-io/n8n/commit/4f307646f3a5691331c7c610c62f562921a005f8))
* **JotForm Trigger Node:** Fix iteration on form loader ([#7751](https://github.com/n8n-io/n8n/issues/7751)) ([82f3202](https://github.com/n8n-io/n8n/commit/82f3202a2de2863f01abe3cf84d6f37eba4fb6fa))


### Features

* Add Creator hub link to Templates page ([#7721](https://github.com/n8n-io/n8n/issues/7721)) ([4dbae0e](https://github.com/n8n-io/n8n/commit/4dbae0e2e95d1b5f46cfc50a5a9fc6bb761defde))
* **core:** Coordinate manual workflow activation and deactivation in multi-main scenario ([#7643](https://github.com/n8n-io/n8n/issues/7643)) ([4c40825](https://github.com/n8n-io/n8n/commit/4c4082503c916d654758da738321f9e78a098ce5)), closes [#7566](https://github.com/n8n-io/n8n/issues/7566)
* **editor:** Add node context menu ([#7620](https://github.com/n8n-io/n8n/issues/7620)) ([8d12c1a](https://github.com/n8n-io/n8n/commit/8d12c1ad8d9283764647836bdd50224259d506e9))
* **editor:** Node IO filter ([#7503](https://github.com/n8n-io/n8n/issues/7503)) ([1881765](https://github.com/n8n-io/n8n/commit/18817651ec5d9ed5e774379ae5cf8f57c5461e43))



# [1.17.0](https://github.com/n8n-io/n8n/compare/n8n@1.16.0...n8n@1.17.0) (2023-11-15)


### Bug Fixes

* **Convert to/from binary data Node:** Better mime type defaults ([#7693](https://github.com/n8n-io/n8n/issues/7693)) ([9b3be0c](https://github.com/n8n-io/n8n/commit/9b3be0cfd8b0b58903d89ea3bf0b73be579a4f89))
* **core:** Consider subworkflows successfully run when in waiting state ([#7699](https://github.com/n8n-io/n8n/issues/7699)) ([0e00dab](https://github.com/n8n-io/n8n/commit/0e00dab9f5d5a6622cdc22fa8bfbecc039f6b67a))
* **core:** Fix named parameter resolution in migrations ([#7688](https://github.com/n8n-io/n8n/issues/7688)) ([4441ed5](https://github.com/n8n-io/n8n/commit/4441ed51169e8be930c548b17f54147ff6bd8e7d)), closes [#7628](https://github.com/n8n-io/n8n/issues/7628)
* **core:** Initialize JWT Secret before it's used anywhere ([#7707](https://github.com/n8n-io/n8n/issues/7707)) ([3460eb5](https://github.com/n8n-io/n8n/commit/3460eb5eeba95e51ccdac05084daf883c9750022))
* **core:** Reduce memory usage in credentials risk auditing ([#7663](https://github.com/n8n-io/n8n/issues/7663)) ([9fd6319](https://github.com/n8n-io/n8n/commit/9fd6319583d0446e41de4fb80d4bc5a6c5e1ca07))
* **Date & Time Node:** Add fromFormat option to solve ambiguous date strings ([#7675](https://github.com/n8n-io/n8n/issues/7675)) ([d2d11e0](https://github.com/n8n-io/n8n/commit/d2d11e0208e8a20145910bbdd02e7b273fb0aa13))
* **editor:** Fix resource mapper component being truncated ([#7664](https://github.com/n8n-io/n8n/issues/7664)) ([00dff50](https://github.com/n8n-io/n8n/commit/00dff50140d12e37bfeecdf1300ff313c179ec89))
* **editor:** More securely clear executions tab auto refresh timer ([#7685](https://github.com/n8n-io/n8n/issues/7685)) ([37dd658](https://github.com/n8n-io/n8n/commit/37dd658dc5bc1128c91d86105bf7f49dfcf96985))
* **editor:** Redirect to workflow editor after saving in debug mode ([#7645](https://github.com/n8n-io/n8n/issues/7645)) ([020042e](https://github.com/n8n-io/n8n/commit/020042ef1a329e805035061fbf6743bde892e3b1))
* **Google Sheets Node:** Append exceeding grid limits ([#7684](https://github.com/n8n-io/n8n/issues/7684)) ([88efb99](https://github.com/n8n-io/n8n/commit/88efb9958711bac446b6a698dfba50afd2b46132))
* **HTTP Request Node:** Support generic credentials when using pagination ([#7686](https://github.com/n8n-io/n8n/issues/7686)) ([48b240b](https://github.com/n8n-io/n8n/commit/48b240b0269858adb8fde8abb8a7211b2a3e78e0)), closes [#7653](https://github.com/n8n-io/n8n/issues/7653)
* **HubSpot Node:** Fetching available parameters fails when using expressions ([#7672](https://github.com/n8n-io/n8n/issues/7672)) ([a9ab738](https://github.com/n8n-io/n8n/commit/a9ab73896e6a42b2fd5df296c9ee95ac82936b7e))
* **HubSpot Node:** Update deal owner on Hubspot Deal ([#7673](https://github.com/n8n-io/n8n/issues/7673)) ([3c0734b](https://github.com/n8n-io/n8n/commit/3c0734bd2d92e9d2b9e99658c2e14710f57f36ef))
* **Spreadsheet File Node:** Read file as utf-8 in v1 ([#7701](https://github.com/n8n-io/n8n/issues/7701)) ([786b4ad](https://github.com/n8n-io/n8n/commit/786b4adcce910fa52104550d90a688c4046628f9))


### Features

* **core:** Expression function $ifEmpty ([#7660](https://github.com/n8n-io/n8n/issues/7660)) ([1c7225e](https://github.com/n8n-io/n8n/commit/1c7225ebdb1d92ce45313bbab27b0839d963fc4c))
* **Date & Time Node:** Option to include other fields in output item ([#7661](https://github.com/n8n-io/n8n/issues/7661)) ([aea3c50](https://github.com/n8n-io/n8n/commit/aea3c501313debaf1cf2b194023a534f829290ea))
* **Discord Node:** Overhaul ([#5351](https://github.com/n8n-io/n8n/issues/5351)) ([6a53c2a](https://github.com/n8n-io/n8n/commit/6a53c2a375ca71ffad1491da5ae7e6ec461a1a56))
* **Discourse Node:** Add new options to Get Users ([#7674](https://github.com/n8n-io/n8n/issues/7674)) ([2e8c841](https://github.com/n8n-io/n8n/commit/2e8c841277c2ba45ab2ab3e823135f2b15a7e570))
* **editor:** Add color selector to sticky node ([#7453](https://github.com/n8n-io/n8n/issues/7453)) ([8359364](https://github.com/n8n-io/n8n/commit/8359364536809e667be86f4b4df0838c94a801d7))
* **editor:** Add HTTP request nodes for credentials without a node ([#7157](https://github.com/n8n-io/n8n/issues/7157)) ([14035e1](https://github.com/n8n-io/n8n/commit/14035e1244fee5bc49b9afe57d63d9e887f25dd0))
* **editor:** Add workflow filters to querystring ([#7456](https://github.com/n8n-io/n8n/issues/7456)) ([afd637b](https://github.com/n8n-io/n8n/commit/afd637b5eab2bba33fd9ec8b24104bef5e2a4cc0))
* **editor:** Adds a EE view to show worker details and job status ([#7600](https://github.com/n8n-io/n8n/issues/7600)) ([cbc6909](https://github.com/n8n-io/n8n/commit/cbc690907fa36e2fde0218dd6f7737d00498c674))
* **GitLab Node:** Add support for pagination on getIssues ([#7529](https://github.com/n8n-io/n8n/issues/7529)) ([0a0798e](https://github.com/n8n-io/n8n/commit/0a0798e48500b0c159aa37deae7ce5d144f4f4c7))
* **OpenAI Node:** Add dall-e-3 support ([#7655](https://github.com/n8n-io/n8n/issues/7655)) ([a9c7188](https://github.com/n8n-io/n8n/commit/a9c7188c4d9d3a020cb26647c9030f6ffd47a35a))
* **RabbitMQ Trigger Node:** Add exchange and routing key options ([#7547](https://github.com/n8n-io/n8n/issues/7547)) ([5aee2b7](https://github.com/n8n-io/n8n/commit/5aee2b768f7743c6508c518bab35206577035380))
* **Telegram Node:** Add support for markdownv2 ([#7679](https://github.com/n8n-io/n8n/issues/7679)) ([819b3a7](https://github.com/n8n-io/n8n/commit/819b3a746a1cfbb785c97d0c681734211a599852))
* **Venafi TLS Protect Cloud Node:** Add region parameter to Venafi protect cloud ([#7689](https://github.com/n8n-io/n8n/issues/7689)) ([a08fca5](https://github.com/n8n-io/n8n/commit/a08fca51d928b7bfb7c0081287a38274048892bb))


### Performance Improvements

* **core:** Lazyload security audit reporters ([#7696](https://github.com/n8n-io/n8n/issues/7696)) ([b2ca050](https://github.com/n8n-io/n8n/commit/b2ca0500311d85742ef8abf8f9f0d1436e6d9ba1))



# [1.16.0](https://github.com/n8n-io/n8n/compare/n8n@1.15.1...n8n@1.16.0) (2023-11-08)


### Bug Fixes

* **core:** Comply with custom default for workflow saving settings ([#7634](https://github.com/n8n-io/n8n/issues/7634)) ([48c068f](https://github.com/n8n-io/n8n/commit/48c068f97b6c7df08fec9fd9d80a0e7eaacc95f5))
* **core:** Decrease reset password token expire time ([#7598](https://github.com/n8n-io/n8n/issues/7598)) ([2aa7f63](https://github.com/n8n-io/n8n/commit/2aa7f6375a01625980278aee714bdc06002b0948))
* **core:** Ensure `init` before checking leader or follower in multi-main scenario ([#7621](https://github.com/n8n-io/n8n/issues/7621)) ([a994ba5](https://github.com/n8n-io/n8n/commit/a994ba5e8d7092edeae05e7aa5fdfbb9fd854034))
* **core:** Ensure pruning starts only after migrations have completed ([#7626](https://github.com/n8n-io/n8n/issues/7626)) ([f748de9](https://github.com/n8n-io/n8n/commit/f748de9567ed1ecebea0ee35e9c71f8ea0e2d450))
* **core:** Fix accessor error when running partial execution ([#7618](https://github.com/n8n-io/n8n/issues/7618)) ([26361df](https://github.com/n8n-io/n8n/commit/26361dfcd31c9952c8ef109314ca88f5f03e40f4)), closes [#6229](https://github.com/n8n-io/n8n/issues/6229)
* **core:** Make password-reset urls valid only for single-use ([#7622](https://github.com/n8n-io/n8n/issues/7622)) ([6031424](https://github.com/n8n-io/n8n/commit/60314248f4b021f451eb744184fe150ddc03bc6e))
* **Crypto Node:** Fix issue with value not appearing for Sign action ([#7619](https://github.com/n8n-io/n8n/issues/7619)) ([5df583f](https://github.com/n8n-io/n8n/commit/5df583f783731e46500600e6a23ff3b7fdfb4e52))
* **editor:** Allow overriding theme from query params ([#7591](https://github.com/n8n-io/n8n/issues/7591)) ([2854a0c](https://github.com/n8n-io/n8n/commit/2854a0cf467258c6dacc15c2b200cf6480b6ecef))
* **editor:** Fix issue that frontend breaks with unkown nodes ([#7596](https://github.com/n8n-io/n8n/issues/7596)) ([db56a9e](https://github.com/n8n-io/n8n/commit/db56a9ee37e8b041ea8958fc8400b9e5b6b81316))
* **editor:** Fix local storage flags defaulting to undefined string ([#7603](https://github.com/n8n-io/n8n/issues/7603)) ([151e60f](https://github.com/n8n-io/n8n/commit/151e60f829663e79982aae6ac1cd8489f3083224))
* **editor:** Fix workflow history prune time limit (getting hours instead of days) ([#7644](https://github.com/n8n-io/n8n/issues/7644)) ([3d5a485](https://github.com/n8n-io/n8n/commit/3d5a485bcf7fef4c6b7d96df3a77c041178951a6))
* **editor:** Hide not supported node options ([#7597](https://github.com/n8n-io/n8n/issues/7597)) ([b532a7b](https://github.com/n8n-io/n8n/commit/b532a7bdb7d33d5ffb20665dfde58cb664d39b4a))
* **editor:** Remove unknown credentials on pasting workflow ([#7582](https://github.com/n8n-io/n8n/issues/7582)) ([d633753](https://github.com/n8n-io/n8n/commit/d63375368713b31e15735721c7a7603fe08a6645))
* **editor:** Reset canvas zoom before workspace reset in node view ([#7625](https://github.com/n8n-io/n8n/issues/7625)) ([78b84af](https://github.com/n8n-io/n8n/commit/78b84af8d1cfed005c7d9c715d832e8c91fd9e3f))
* **editor:** Zoom in/out on canvas the same amount on scroll/gesture ([#7602](https://github.com/n8n-io/n8n/issues/7602)) ([c92402a](https://github.com/n8n-io/n8n/commit/c92402a3cabfdc227f3c929bc7731d42f4516776))
* **Facebook Lead Ads Trigger Node:** Fix issue with missing scope for business management  ([#7616](https://github.com/n8n-io/n8n/issues/7616)) ([32b85ba](https://github.com/n8n-io/n8n/commit/32b85ba2fec6e74d8648be7e718b52140c1bc4fc))


### Features

* **core:** Add the node version to telemetry in node_graph_string ([#7449](https://github.com/n8n-io/n8n/issues/7449)) ([59dc36a](https://github.com/n8n-io/n8n/commit/59dc36abd9141a863cb41c17a9115410b27bdb16))
* **core:** Coordinate workflow activation in multiple main scenario in internal API ([#7566](https://github.com/n8n-io/n8n/issues/7566)) ([c857e42](https://github.com/n8n-io/n8n/commit/c857e42677ef0d415caf66f00d7af029546dfd79))
* **core:** Initial support for two-way communication over websockets ([#7570](https://github.com/n8n-io/n8n/issues/7570)) ([ac87701](https://github.com/n8n-io/n8n/commit/ac877014eda83eb2ee61c87f29e2583f3fbfd125))
* **core:** Log executed migrations with info level ([#7586](https://github.com/n8n-io/n8n/issues/7586)) ([7dac9ab](https://github.com/n8n-io/n8n/commit/7dac9ab82c2f91cfbb66a57f175c1865e8c8107a))
* **core:** Rate limit forgot password endpoint ([#7604](https://github.com/n8n-io/n8n/issues/7604)) ([5790e25](https://github.com/n8n-io/n8n/commit/5790e251b8072679d7c061e2d2fa1f4229e03cf8))
* **LinkedIn Node:** Add support for Article thumbnails ([#7489](https://github.com/n8n-io/n8n/issues/7489)) ([e6d3d1a](https://github.com/n8n-io/n8n/commit/e6d3d1a4c2dd6a860e935df4b0ce3f13e23030c7))
* **NocoDB Node:** Add new data apis and workspace support ([#7329](https://github.com/n8n-io/n8n/issues/7329)) ([da2d2a8](https://github.com/n8n-io/n8n/commit/da2d2a83bbfb05db3a10aef99bfde3ccaf160d60))



## [1.15.1](https://github.com/n8n-io/n8n/compare/n8n@1.14.0...n8n@1.15.1) (2023-11-02)


### Bug Fixes

* **core:** Ensure execution deletion in worker lifecycle hook ([#7481](https://github.com/n8n-io/n8n/issues/7481)) ([742c8a8](https://github.com/n8n-io/n8n/commit/742c8a8534098522fe103fad09fa95f70c460b3d))
* **core:** Fix data encryption on credentials import ([#7560](https://github.com/n8n-io/n8n/issues/7560)) ([b350568](https://github.com/n8n-io/n8n/commit/b350568505d48ec880fe98d2b62ef090d5399c5f))
* **core:** Fix issue that prevents owner logging in when using ldap ([#7408](https://github.com/n8n-io/n8n/issues/7408)) ([479f902](https://github.com/n8n-io/n8n/commit/479f90231d0a03c69b17189384812b5a1d81ef3d))
* **core:** Handle missing resultData in runData  ([#7523](https://github.com/n8n-io/n8n/issues/7523)) ([1055bd3](https://github.com/n8n-io/n8n/commit/1055bd3762b90b013a300bd87e3fa902e902cb9e))
* **core:** Permission check for subworkflow properly checking for workflow settings ([#7576](https://github.com/n8n-io/n8n/issues/7576)) ([437c95e](https://github.com/n8n-io/n8n/commit/437c95e84e144cc77f2866a74d6b670c415895cd))
* **core:** Prevent executions from becoming forever running ([#7569](https://github.com/n8n-io/n8n/issues/7569)) ([9bdb85c](https://github.com/n8n-io/n8n/commit/9bdb85c4ced96fde75435e334dc757d6c7679926))
* **core:** Upgrade crypto-js to address CVE-2023-46233  ([#7519](https://github.com/n8n-io/n8n/issues/7519)) ([65e5593](https://github.com/n8n-io/n8n/commit/65e559323371e8235b92e2134d9908d69043fac4))
* **editor:** Do not truncate form inputs ([#7528](https://github.com/n8n-io/n8n/issues/7528)) ([ae616f1](https://github.com/n8n-io/n8n/commit/ae616f146bc2ce8d37f8cf5116c6c4c8682a91a6))
* **editor:** Fix NDV close after using input select ([#7544](https://github.com/n8n-io/n8n/issues/7544)) ([3b5e181](https://github.com/n8n-io/n8n/commit/3b5e181e66f8d7e3860e3078dae7cbb20e92551a))
* **editor:** Fix NDV unexpected re-render ([#7532](https://github.com/n8n-io/n8n/issues/7532)) ([2853fcf](https://github.com/n8n-io/n8n/commit/2853fcff735fd0b98c19c1192349ef2c659d2493))
* **editor:** Fix route component caching, incorrect use of array reduce method and enable WF history feature  ([#7434](https://github.com/n8n-io/n8n/issues/7434)) ([12a89e6](https://github.com/n8n-io/n8n/commit/12a89e6d1441f81380d5e477274a5e2d3eb29f2d))
* **editor:** Fixes the issue that Switch Node can not be created ([#7516](https://github.com/n8n-io/n8n/issues/7516)) ([df89685](https://github.com/n8n-io/n8n/commit/df89685e1548219f4c06614287abafbc96697817))
* **editor:** Handle `localStorage` being blocked/unavailable ([#7348](https://github.com/n8n-io/n8n/issues/7348)) ([c05bc67](https://github.com/n8n-io/n8n/commit/c05bc6728d3227af4931ddcda5ed8bc6a3539dd0))
* Fix dark mode small issues ([#7573](https://github.com/n8n-io/n8n/issues/7573)) ([1d81afc](https://github.com/n8n-io/n8n/commit/1d81afcbdf17166f3ebf468673e3ba348ae7fecb))
* **Jira Software Node:** Handle missing issue types in issue types loader ([#7534](https://github.com/n8n-io/n8n/issues/7534)) ([9762705](https://github.com/n8n-io/n8n/commit/9762705833c809fd2781de179279a15c1be988eb))
* **Switch Node:** Allow sortable Switch rules ([#7555](https://github.com/n8n-io/n8n/issues/7555)) ([7a56e58](https://github.com/n8n-io/n8n/commit/7a56e58a608132ef795d8c5cdaccb8caa49c0e8f))


### Features

* **core:** Add optional Error-Output ([#7460](https://github.com/n8n-io/n8n/issues/7460)) ([655efea](https://github.com/n8n-io/n8n/commit/655efeaf669e9722895b66fef47f000507459210))
* **core:** Make queue mode settings configurable ([#7526](https://github.com/n8n-io/n8n/issues/7526)) ([3d95b24](https://github.com/n8n-io/n8n/commit/3d95b243e935e4eba97a418d05fa687169ab7d07))
* **core:** Set up leader selection for multiple main instances ([#7527](https://github.com/n8n-io/n8n/issues/7527)) ([442c73e](https://github.com/n8n-io/n8n/commit/442c73e63bb54f50657a511d88912a80cab64c7f))
* **editor:** Implement the `UserStack` design system component ([#7559](https://github.com/n8n-io/n8n/issues/7559)) ([ce14f62](https://github.com/n8n-io/n8n/commit/ce14f6266b30caadb477b08d4257b82c769a74c3))
* **HTTP Request Node:** Add pagination support ([#5993](https://github.com/n8n-io/n8n/issues/5993)) ([cc2bd2e](https://github.com/n8n-io/n8n/commit/cc2bd2e19c8b75320b236de215d389220fbe24ae))
* **HTTP Request Node:** Update icon and default color ([#7572](https://github.com/n8n-io/n8n/issues/7572)) ([ff279ab](https://github.com/n8n-io/n8n/commit/ff279ab4112435c341b84081d68b976ff03bf261))
* **n8n Form Trigger Node:** Add text area and password input types ([#7474](https://github.com/n8n-io/n8n/issues/7474)) ([b72040a](https://github.com/n8n-io/n8n/commit/b72040aa5423aa6cb16dea2e7c6ea6439376b653))
* **editor:** Dark mode is here! You can change it under personal settings.([#6980](https://github.com/n8n-io/n8n/pull/6980)) ([0746783](https://github.com/n8n-io/n8n/commit/0746783e027ebe6715588a68db399a34e0211a96))



# [1.15.0](https://github.com/n8n-io/n8n/compare/n8n@1.14.0...n8n@1.15.0) (2023-11-02)


### Bug Fixes

* **core:** Ensure execution deletion in worker lifecycle hook ([#7481](https://github.com/n8n-io/n8n/issues/7481)) ([742c8a8](https://github.com/n8n-io/n8n/commit/742c8a8534098522fe103fad09fa95f70c460b3d))
* **core:** Fix data encryption on credentials import ([#7560](https://github.com/n8n-io/n8n/issues/7560)) ([b350568](https://github.com/n8n-io/n8n/commit/b350568505d48ec880fe98d2b62ef090d5399c5f))
* **core:** Fix issue that prevents owner logging in when using ldap ([#7408](https://github.com/n8n-io/n8n/issues/7408)) ([479f902](https://github.com/n8n-io/n8n/commit/479f90231d0a03c69b17189384812b5a1d81ef3d))
* **core:** Handle missing resultData in runData  ([#7523](https://github.com/n8n-io/n8n/issues/7523)) ([1055bd3](https://github.com/n8n-io/n8n/commit/1055bd3762b90b013a300bd87e3fa902e902cb9e))
* **core:** Permission check for subworkflow properly checking for workflow settings ([#7576](https://github.com/n8n-io/n8n/issues/7576)) ([437c95e](https://github.com/n8n-io/n8n/commit/437c95e84e144cc77f2866a74d6b670c415895cd))
* **core:** Prevent executions from becoming forever running ([#7569](https://github.com/n8n-io/n8n/issues/7569)) ([9bdb85c](https://github.com/n8n-io/n8n/commit/9bdb85c4ced96fde75435e334dc757d6c7679926))
* **core:** Upgrade crypto-js to address CVE-2023-46233  ([#7519](https://github.com/n8n-io/n8n/issues/7519)) ([65e5593](https://github.com/n8n-io/n8n/commit/65e559323371e8235b92e2134d9908d69043fac4))
* **editor:** Do not truncate form inputs ([#7528](https://github.com/n8n-io/n8n/issues/7528)) ([ae616f1](https://github.com/n8n-io/n8n/commit/ae616f146bc2ce8d37f8cf5116c6c4c8682a91a6))
* **editor:** Fix NDV close after using input select ([#7544](https://github.com/n8n-io/n8n/issues/7544)) ([3b5e181](https://github.com/n8n-io/n8n/commit/3b5e181e66f8d7e3860e3078dae7cbb20e92551a))
* **editor:** Fix NDV unexpected re-render ([#7532](https://github.com/n8n-io/n8n/issues/7532)) ([2853fcf](https://github.com/n8n-io/n8n/commit/2853fcff735fd0b98c19c1192349ef2c659d2493))
* **editor:** Fix route component caching, incorrect use of array reduce method and enable WF history feature  ([#7434](https://github.com/n8n-io/n8n/issues/7434)) ([12a89e6](https://github.com/n8n-io/n8n/commit/12a89e6d1441f81380d5e477274a5e2d3eb29f2d))
* **editor:** Fixes the issue that Switch Node can not be created ([#7516](https://github.com/n8n-io/n8n/issues/7516)) ([df89685](https://github.com/n8n-io/n8n/commit/df89685e1548219f4c06614287abafbc96697817))
* **editor:** Handle `localStorage` being blocked/unavailable ([#7348](https://github.com/n8n-io/n8n/issues/7348)) ([c05bc67](https://github.com/n8n-io/n8n/commit/c05bc6728d3227af4931ddcda5ed8bc6a3539dd0))
* Fix dark mode small issues ([#7573](https://github.com/n8n-io/n8n/issues/7573)) ([1d81afc](https://github.com/n8n-io/n8n/commit/1d81afcbdf17166f3ebf468673e3ba348ae7fecb))
* **Jira Software Node:** Handle missing issue types in issue types loader ([#7534](https://github.com/n8n-io/n8n/issues/7534)) ([9762705](https://github.com/n8n-io/n8n/commit/9762705833c809fd2781de179279a15c1be988eb))
* **Switch Node:** Allow sortable Switch rules ([#7555](https://github.com/n8n-io/n8n/issues/7555)) ([7a56e58](https://github.com/n8n-io/n8n/commit/7a56e58a608132ef795d8c5cdaccb8caa49c0e8f))


### Features

* **core:** Add optional Error-Output ([#7460](https://github.com/n8n-io/n8n/issues/7460)) ([655efea](https://github.com/n8n-io/n8n/commit/655efeaf669e9722895b66fef47f000507459210))
* **core:** Make queue mode settings configurable ([#7526](https://github.com/n8n-io/n8n/issues/7526)) ([3d95b24](https://github.com/n8n-io/n8n/commit/3d95b243e935e4eba97a418d05fa687169ab7d07))
* **core:** Set up leader selection for multiple main instances ([#7527](https://github.com/n8n-io/n8n/issues/7527)) ([442c73e](https://github.com/n8n-io/n8n/commit/442c73e63bb54f50657a511d88912a80cab64c7f))
* **editor:** Implement the `UserStack` design system component ([#7559](https://github.com/n8n-io/n8n/issues/7559)) ([ce14f62](https://github.com/n8n-io/n8n/commit/ce14f6266b30caadb477b08d4257b82c769a74c3))
* **HTTP Request Node:** Add pagination support ([#5993](https://github.com/n8n-io/n8n/issues/5993)) ([cc2bd2e](https://github.com/n8n-io/n8n/commit/cc2bd2e19c8b75320b236de215d389220fbe24ae))
* **HTTP Request Node:** Update icon and default color ([#7572](https://github.com/n8n-io/n8n/issues/7572)) ([ff279ab](https://github.com/n8n-io/n8n/commit/ff279ab4112435c341b84081d68b976ff03bf261))
* **n8n Form Trigger Node:** Add text area and password input types ([#7474](https://github.com/n8n-io/n8n/issues/7474)) ([b72040a](https://github.com/n8n-io/n8n/commit/b72040aa5423aa6cb16dea2e7c6ea6439376b653))
* * **editor:** Dark mode is here! You can change it under personal settings.([#6980](https://github.com/n8n-io/n8n/pull/6980)) ([0746783](https://github.com/n8n-io/n8n/commit/0746783e027ebe6715588a68db399a34e0211a96))



# [1.14.0](https://github.com/n8n-io/n8n/compare/n8n@1.13.0...n8n@1.14.0) (2023-10-25)


### Features

* **Switch Node:** Add support for infinite Switch outputs ([#7499](https://github.com/n8n-io/n8n/issues/7499)) ([2febc61](https://github.com/n8n-io/n8n/commit/2febc61ec94928eb196e1b5f815fffa13f8bae07))



# [1.13.0](https://github.com/n8n-io/n8n/compare/n8n@1.12.0...n8n@1.13.0) (2023-10-25)


### Bug Fixes

* **core:** Always derive `instanceId` from the encryption key (no-changlog) ([#7501](https://github.com/n8n-io/n8n/issues/7501)) ([a9fdd01](https://github.com/n8n-io/n8n/commit/a9fdd018f4f5ba1e11cc10dc3a3b7929a586f818))
* **core:** Do not return `inviteAcceptUrl` in response if email was sent ([#7465](https://github.com/n8n-io/n8n/issues/7465)) ([55c6a1b](https://github.com/n8n-io/n8n/commit/55c6a1b0d394265fa4018a7023971589d8e61b4a))
* **core:** Ensure nodes post-processors run in the correct order ([#7500](https://github.com/n8n-io/n8n/issues/7500)) ([6f45298](https://github.com/n8n-io/n8n/commit/6f45298d3d61b33e762f520129f4775e216707c8)), closes [#7497](https://github.com/n8n-io/n8n/issues/7497)
* **core:** Fix `frontend.settings` external hook execution ([#7496](https://github.com/n8n-io/n8n/issues/7496)) ([774fe20](https://github.com/n8n-io/n8n/commit/774fe202bfde4f2c5cc95f28a33185e261b031a5))
* **core:** Handle gzip and deflate compressed request payloads ([#7461](https://github.com/n8n-io/n8n/issues/7461)) ([83762e0](https://github.com/n8n-io/n8n/commit/83762e051d5e34d9e43caebd6275780da05c6a46))
* **core:** Reduce logging overhead for levels that do not output ([#7479](https://github.com/n8n-io/n8n/issues/7479)) ([76c0481](https://github.com/n8n-io/n8n/commit/76c04815f7f53bf6b4c06bbe5afa52f51f28750d))
* **Customer.io Node:** Fix api endpoint when using EU region ([#7485](https://github.com/n8n-io/n8n/issues/7485)) ([519680c](https://github.com/n8n-io/n8n/commit/519680c2cf37f3b7341e87e71b911ac2fee8bdfa)), closes [#7484](https://github.com/n8n-io/n8n/issues/7484)
* **editor:** Allow importing the same workflow multiple times ([#7458](https://github.com/n8n-io/n8n/issues/7458)) ([3c0a166](https://github.com/n8n-io/n8n/commit/3c0a166f7f1cf225e5d1b4da91f7449f2deed5ca)), closes [#7457](https://github.com/n8n-io/n8n/issues/7457)
* **editor:** Fix canvas selection breaking after interacting with node actions ([#7466](https://github.com/n8n-io/n8n/issues/7466)) ([bc47365](https://github.com/n8n-io/n8n/commit/bc473655fbc09b1172cd6949236ca2871c9d3b8e))
* **editor:** Fix connections disappearing after reactivating canvas and renaming a node ([#7483](https://github.com/n8n-io/n8n/issues/7483)) ([450e0cc](https://github.com/n8n-io/n8n/commit/450e0cc66abbe57697f66835a837e53b5eb883a3))
* **Google Sheets Node:** Append or update runs forever when without column headers ([#7463](https://github.com/n8n-io/n8n/issues/7463)) ([ab6a9bb](https://github.com/n8n-io/n8n/commit/ab6a9bbac29a2caf34f4dd8211cd18116f659804))
* **Microsoft SQL Node:** Prevent SQL injection ([#7467](https://github.com/n8n-io/n8n/issues/7467)) ([a739245](https://github.com/n8n-io/n8n/commit/a7392453323fe06371988fd5bb28d659a7a00cd8))
* **MQTT Trigger Node:** Fix node causing a start up hang when active ([#7498](https://github.com/n8n-io/n8n/issues/7498)) ([baecb93](https://github.com/n8n-io/n8n/commit/baecb93bef30ac00f09b46ea987bb4c9a2fca394))
* **MySQL Node:** Resolve expressions in v1 ([#7464](https://github.com/n8n-io/n8n/issues/7464)) ([5c46bb0](https://github.com/n8n-io/n8n/commit/5c46bb09c137023608119093cabdf896555b22b9))
* **Redis Node:** Fix adding sets data types ([#7444](https://github.com/n8n-io/n8n/issues/7444)) ([4e66023](https://github.com/n8n-io/n8n/commit/4e66023cd428513b76626795c27ba0713c6c4ea9)), closes [#6339](https://github.com/n8n-io/n8n/issues/6339)
* **Spreadsheet File Node:** Fix include empty cells not working with v2 ([#7505](https://github.com/n8n-io/n8n/issues/7505)) ([05e6f2a](https://github.com/n8n-io/n8n/commit/05e6f2a6ac43fb4059e7e6cc40af6c5d75e01c8b)), closes [Ticket#763644](https://github.com/Ticket/issues/763644)


### Features

* **core:** Add support for oauth based service accounts with UM SMTP ([#7311](https://github.com/n8n-io/n8n/issues/7311)) ([647372b](https://github.com/n8n-io/n8n/commit/647372be275c46e9963c96163c9e913a17f13e5f))
* **editor:** Add PH tracking to event ([#7511](https://github.com/n8n-io/n8n/issues/7511)) ([c47d27d](https://github.com/n8n-io/n8n/commit/c47d27dd6da9420add7dad243b2701876f39a95b))
* **Facebook Lead Ads Trigger Node:** Add Facebook Lead Ads Trigger Node ([#7113](https://github.com/n8n-io/n8n/issues/7113)) ([ac814a9](https://github.com/n8n-io/n8n/commit/ac814a9c613f6f9943be8002110ca9e2433918b2))
* **Ghost Node:** Add support for lexical format ([#7488](https://github.com/n8n-io/n8n/issues/7488)) ([7b1973c](https://github.com/n8n-io/n8n/commit/7b1973c058e0cb7dfa436953c6f046c2b3b145eb))
* **RSS Feed Trigger Node:** Add RSS feed trigger node ([#7386](https://github.com/n8n-io/n8n/issues/7386)) ([689360e](https://github.com/n8n-io/n8n/commit/689360ee069043415838f1488486ce8deaef9e38))



# [1.12.0](https://github.com/n8n-io/n8n/compare/n8n@1.11.0...n8n@1.12.0) (2023-10-18)


### Bug Fixes

* **core:** Add check that queue is defined and remove cyclic dependency ([#7404](https://github.com/n8n-io/n8n/issues/7404)) ([45f2ef3](https://github.com/n8n-io/n8n/commit/45f2ef373ee76abb0d4b9ad805beb02d8969ebd6))
* **core:** Do not throw when deleting workflows with executions without binary-data ([#7411](https://github.com/n8n-io/n8n/issues/7411)) ([2b6a15e](https://github.com/n8n-io/n8n/commit/2b6a15e478fd1a6041be4eac19dcf1c5e5583886))
* **core:** Fix expression with paired item with multi-input node ([#7424](https://github.com/n8n-io/n8n/issues/7424)) ([ec14141](https://github.com/n8n-io/n8n/commit/ec141416e29540a2bf6ce99be1b13d76517eca13))
* **core:** Fix ignoring crashed executions without event msgs ([#7368](https://github.com/n8n-io/n8n/issues/7368)) ([2f4d91b](https://github.com/n8n-io/n8n/commit/2f4d91b2cd2b87ae4aceb06a4170cd86802c9bbf))
* **core:** Pg-promise de-initialization fix ([#7417](https://github.com/n8n-io/n8n/issues/7417)) ([7703904](https://github.com/n8n-io/n8n/commit/77039044ebd74b907a44a08ae5421517fc74b46e))
* **core:** Prevent false stalled jobs in queue mode from displaying as errored ([#7435](https://github.com/n8n-io/n8n/issues/7435)) ([e01b9e5](https://github.com/n8n-io/n8n/commit/e01b9e5ae1bf6ccdec422c2767fdf870b2e159b0))
* **core:** Prevent undefined issues when restoring binary data ([#7419](https://github.com/n8n-io/n8n/issues/7419)) ([46977a2](https://github.com/n8n-io/n8n/commit/46977a2aff342bc7568f5a378b78689a5c3d8e95))
* **editor:** Fix remote options fetching on every keystroke ([#7320](https://github.com/n8n-io/n8n/issues/7320)) ([367255a](https://github.com/n8n-io/n8n/commit/367255ab2c13b4a33a746d3d4b9f3164309a11c8))
* **editor:** Open only one tab with plans page ([#7377](https://github.com/n8n-io/n8n/issues/7377)) ([c599006](https://github.com/n8n-io/n8n/commit/c599006b917e681fca918b789a80d79883bd69a9))
* **Google Sheets Node:** Update by row_number, restored 'Handling Extra Data Option', updated Cell Format default ([#7357](https://github.com/n8n-io/n8n/issues/7357)) ([d8531a5](https://github.com/n8n-io/n8n/commit/d8531a53b9a256095157129b64adde7749aa84c9))
* **Ldap Node:** Fix issue with connections not closing correctly ([#7432](https://github.com/n8n-io/n8n/issues/7432)) ([c3f0be8](https://github.com/n8n-io/n8n/commit/c3f0be809f3ea09573fec26648ef030c7d8ddc16))
* **Set Node:** Null should not throw an error ([#7416](https://github.com/n8n-io/n8n/issues/7416)) ([e9b6ab0](https://github.com/n8n-io/n8n/commit/e9b6ab04cd4b292c291b77e66aa717605e72f852))
* **TheHive 5 Node:** Observable encoding in alert > create fix ([#7450](https://github.com/n8n-io/n8n/issues/7450)) ([a2d2e3d](https://github.com/n8n-io/n8n/commit/a2d2e3dda798d166cfc2a49b0c4f0eb164a666dc))


### Features

* **core:** Make executions pruning interval configurable ([#7439](https://github.com/n8n-io/n8n/issues/7439)) ([40707fa](https://github.com/n8n-io/n8n/commit/40707fa6926776aa806221df8edee05ee7e9f3ed))
* **Google Calendar Trigger Node:** Add support for cancelled events ([#7436](https://github.com/n8n-io/n8n/issues/7436)) ([9d241a0](https://github.com/n8n-io/n8n/commit/9d241a0d6dbfd990920708c718ff3de83c9b5883))
* **HubSpot Trigger Node:** Add support for ticket related events ([#7156](https://github.com/n8n-io/n8n/issues/7156)) ([57c6093](https://github.com/n8n-io/n8n/commit/57c609384af7c583c213c639add7170e0bbb24fd))
* **n8n Form Trigger Node:** New node ([#7130](https://github.com/n8n-io/n8n/issues/7130)) ([3ddc176](https://github.com/n8n-io/n8n/commit/3ddc176dfa2d3d99a328a29a3a8613e35ff456a0))
* **Spreadsheet File Node:** Improve CSV parsing ([#7448](https://github.com/n8n-io/n8n/issues/7448)) ([79f23fb](https://github.com/n8n-io/n8n/commit/79f23fb93979aa1ef3a9bbf7049b93d1e6a0e95a))



# [1.11.0](https://github.com/n8n-io/n8n/compare/n8n@1.10.0...n8n@1.11.0) (2023-10-11)


### Bug Fixes

* Add role check for upgrade path ([#7374](https://github.com/n8n-io/n8n/issues/7374)) ([a43f720](https://github.com/n8n-io/n8n/commit/a43f720658aedf8a52f713c28b29ed08bfad33c8))
* **core:** Add an option to enable postgres ssl with default certs ([#6889](https://github.com/n8n-io/n8n/issues/6889)) ([789e1e7](https://github.com/n8n-io/n8n/commit/789e1e7ed41838bdadb5e8cb429aa76610fa5749))
* **core:** Fix error on missing paired item data ([#7399](https://github.com/n8n-io/n8n/issues/7399)) ([47e8953](https://github.com/n8n-io/n8n/commit/47e8953ec9cccaddc603aff4c6e6fce88258e6d0))
* **core:** Missing pairing info ([#7326](https://github.com/n8n-io/n8n/issues/7326)) ([e2c3c7a](https://github.com/n8n-io/n8n/commit/e2c3c7acebdae2014b32620277fce70d0db85dd0))
* **core:** Prevent object deletion request on no prefix match ([#7366](https://github.com/n8n-io/n8n/issues/7366)) ([63e11e4](https://github.com/n8n-io/n8n/commit/63e11e4be93a50fe753d84771dbc72ead38fdc0e))
* **editor:** Fix completions for `.json` on quoted node name in Code node ([#7382](https://github.com/n8n-io/n8n/issues/7382)) ([86e7ec7](https://github.com/n8n-io/n8n/commit/86e7ec796acd9d8fbe8e42a5beba687cd6133a2f)), closes [/linear.app/n8n/issue/PAY-635/autocomplete-only-supports-3-levels-of-children#comment-234f738](https://github.com//linear.app/n8n/issue/PAY-635/autocomplete-only-supports-3-levels-of-children/issues/comment-234f738)
* **editor:** Implement canvas zoom UX improvements ([#7376](https://github.com/n8n-io/n8n/issues/7376)) ([7e06b31](https://github.com/n8n-io/n8n/commit/7e06b31a5f3de8f073e7ef42be24e04899091486))
* **editor:** Make workflow history button available only for dev builds ([#7392](https://github.com/n8n-io/n8n/issues/7392)) ([7ed466d](https://github.com/n8n-io/n8n/commit/7ed466db7faa9af88e54276bc6cb9a6dc9e80493))
* **editor:** Remove excess margin below run data editor ([#7372](https://github.com/n8n-io/n8n/issues/7372)) ([3fa2764](https://github.com/n8n-io/n8n/commit/3fa27647d8e8a39812d9802d4c0954b3135db847))
* **editor:** Sanitize HTML binary-data before rendering in the UI ([#7400](https://github.com/n8n-io/n8n/issues/7400)) ([2b075bf](https://github.com/n8n-io/n8n/commit/2b075bfc2da02afc43c1ebfee565b849c87aee49))
* **editor:** Use display option's @Version specifier  ([#7351](https://github.com/n8n-io/n8n/issues/7351)) ([afbf0c3](https://github.com/n8n-io/n8n/commit/afbf0c3d5e50976ca5d9f4c08051ea7bd3d2b354))
* **Google BigQuery Node:** Location default to jobReference ([#7354](https://github.com/n8n-io/n8n/issues/7354)) ([97bb703](https://github.com/n8n-io/n8n/commit/97bb703d0a13cf979a2c462c87570707d5032867))
* **Google Drive Trigger Node:** Add Shared Drives support ([#7369](https://github.com/n8n-io/n8n/issues/7369)) ([3e7a4d3](https://github.com/n8n-io/n8n/commit/3e7a4d3b2cc12fcb1b011fccd0773bb807986884))
* **Google Sheets Node:** Fix "Maximum call stack size exceeded" error on too many rows ([#7384](https://github.com/n8n-io/n8n/issues/7384)) ([732b15a](https://github.com/n8n-io/n8n/commit/732b15a1faeab5b802dfddb282418601f34ade27))
* **HTML Node:** Update property fields to not use expressions on drag ([#7379](https://github.com/n8n-io/n8n/issues/7379)) ([77643e5](https://github.com/n8n-io/n8n/commit/77643e5ccbc2f68cd240c7aa7e21c0efbcc08b63))
* **Notion Node:** Handle empty values correctly for Notion selects + multi selects ([#7383](https://github.com/n8n-io/n8n/issues/7383)) ([fbcd1d4](https://github.com/n8n-io/n8n/commit/fbcd1d40edfa8737a8786a8f961723c42f84a851))
* **Set Node:** Increase search priority ([#7358](https://github.com/n8n-io/n8n/issues/7358)) ([e5ad1e7](https://github.com/n8n-io/n8n/commit/e5ad1e7e4df33a06c9649fe0652edfc80f7cb818))
* **Webhook Node:** Backward compatible form-data parsing for non-array files ([#7385](https://github.com/n8n-io/n8n/issues/7385)) ([6479eb1](https://github.com/n8n-io/n8n/commit/6479eb180ff9a43791b5211157f5c450e1463ffd))


### Features

* **core:** Add Job Summary to Worker response ([#7360](https://github.com/n8n-io/n8n/issues/7360)) ([b8608ce](https://github.com/n8n-io/n8n/commit/b8608cee6d5ab96ec38a8a7f5428d02ce01366ee))
* **core:** Integrate object store as binary data manager ([#7253](https://github.com/n8n-io/n8n/issues/7253)) ([1a661e6](https://github.com/n8n-io/n8n/commit/1a661e6d00e907b9bc4bdc248db6dbc25972294b)), closes [#7225](https://github.com/n8n-io/n8n/issues/7225)
* **core:** Switch binary filesystem mode to nested path structure ([#7307](https://github.com/n8n-io/n8n/issues/7307)) ([0847623](https://github.com/n8n-io/n8n/commit/0847623f85192232d129778ab4295be3cd685877)), closes [#7253](https://github.com/n8n-io/n8n/issues/7253)
* **editor:** Make PDF and Audio binary-data viewable in the UI ([#7367](https://github.com/n8n-io/n8n/issues/7367)) ([8187be1](https://github.com/n8n-io/n8n/commit/8187be1b7dd723fec9591e2fc4f57a782f3ca398)), closes [#7361](https://github.com/n8n-io/n8n/issues/7361)
* **editor:** Support autologin for upgrade path ([#7316](https://github.com/n8n-io/n8n/issues/7316)) ([1dfa052](https://github.com/n8n-io/n8n/commit/1dfa052301c4580838bc17830676c8fb383a00b4))
* **Execute Workflow Node:** Run once for each item mode ([#7289](https://github.com/n8n-io/n8n/issues/7289)) ([c8c14ca](https://github.com/n8n-io/n8n/commit/c8c14ca0af1faaf680c97868210b7372ac8ac61e))
* **Item Lists Node:** Split merge binary data ([#7297](https://github.com/n8n-io/n8n/issues/7297)) ([965db8f](https://github.com/n8n-io/n8n/commit/965db8f7f272056d10515a94a3b0b69b75913a9a))
* **Loop Over Items (Split in Batches) Node:** Automatically add a loop + rename ([#7228](https://github.com/n8n-io/n8n/issues/7228)) ([7b773cc](https://github.com/n8n-io/n8n/commit/7b773cc5cc77853f73db186f7f7a7fbc6379db31))
* **Notion Node:** Fetch child blocks recursively ([#7304](https://github.com/n8n-io/n8n/issues/7304)) ([193181a](https://github.com/n8n-io/n8n/commit/193181a9c62d21812e5452b06606c63f26f6b9d0))



# [1.10.0](https://github.com/n8n-io/n8n/compare/n8n@1.9.0...n8n@1.10.0) (2023-10-05)


### Bug Fixes

* **Convert to/from binary data Node:** Rename 'Move Binary Data' to 'Convert to/from binary data' ([#7318](https://github.com/n8n-io/n8n/issues/7318)) ([5e6c1d4](https://github.com/n8n-io/n8n/commit/5e6c1d4f4bc049d366dbc9b66d5481f6ed43190e))
* **core:** Account for itemless case on restoring binary data ID ([#7305](https://github.com/n8n-io/n8n/issues/7305)) ([1691223](https://github.com/n8n-io/n8n/commit/169122378968b4d4c73d921ee2d5d86b76e1cd01))
* **core:** Fix pruning of non-finished executions ([#7333](https://github.com/n8n-io/n8n/issues/7333)) ([1b4848a](https://github.com/n8n-io/n8n/commit/1b4848afcb817621e0977186c7400945758bee96))
* **editor:** Disable email confirmation banner for trialing users ([#7340](https://github.com/n8n-io/n8n/issues/7340)) ([6d3d178](https://github.com/n8n-io/n8n/commit/6d3d1789dbd800a6ef75aab3a69e5b5ef5dba933))
* **editor:** Display value of selected matching column in RMC ([#7298](https://github.com/n8n-io/n8n/issues/7298)) ([3aac22b](https://github.com/n8n-io/n8n/commit/3aac22b4c1d472b8470346bfc4df99b7794c3692))
* **editor:** Fix canvas endpoint snapping when dragging connection ([#7346](https://github.com/n8n-io/n8n/issues/7346)) ([b59b908](https://github.com/n8n-io/n8n/commit/b59b9086d769b859156f4f8f99411afe5e4b9108))
* **editor:** Fix disappearing NDV header in code nodes ([#7290](https://github.com/n8n-io/n8n/issues/7290)) ([7ebf8f3](https://github.com/n8n-io/n8n/commit/7ebf8f327ad433acc949034cd070f2362dfacd4e))
* **editor:** Fix RLC not loading when an expression can't resolve ([#7295](https://github.com/n8n-io/n8n/issues/7295)) ([ddc26c2](https://github.com/n8n-io/n8n/commit/ddc26c21bd8da6c95cbe447bf7e479ddc449e6a4))
* **editor:** Separate cloud endpoint calls ([#7312](https://github.com/n8n-io/n8n/issues/7312)) ([04dfcd7](https://github.com/n8n-io/n8n/commit/04dfcd73bee2c1ea0d47fd7102383719827d53d0))
* **Jira Software Node:** Get all users in dropdown/RLC ([#7322](https://github.com/n8n-io/n8n/issues/7322)) ([3704760](https://github.com/n8n-io/n8n/commit/370476072471da6b3b849d8f5acc5cf1380a5ba8)), closes [#2670](https://github.com/n8n-io/n8n/issues/2670)
* **Notion Node:** Rename Notion API Key to Internal Integration Token ([#7176](https://github.com/n8n-io/n8n/issues/7176)) ([ec2aa38](https://github.com/n8n-io/n8n/commit/ec2aa3819c1e9624c4692d5f6942f096aae900e7))
* **Postgres Node:** Node requires comma-separated string even when using a single parameter through an expression ([#7300](https://github.com/n8n-io/n8n/issues/7300)) ([763d451](https://github.com/n8n-io/n8n/commit/763d4514fafe489c169cd0513bf3b2c4cf7f7f12))
* **Set Node:** Do not stringify null and undefined ([#7313](https://github.com/n8n-io/n8n/issues/7313)) ([f0a6687](https://github.com/n8n-io/n8n/commit/f0a66873b94b032792f30bc279118cdb13210505))
* **Typeform Trigger Node:** Change output format for TypeForm trigger to object instead of array ([#7315](https://github.com/n8n-io/n8n/issues/7315)) ([b3fc00e](https://github.com/n8n-io/n8n/commit/b3fc00e045dc16f758b684b71591ec2d1f889d73))


### Features

* **core:** Add "Sent by n8n" attribution ([#7183](https://github.com/n8n-io/n8n/issues/7183)) ([8f9fe62](https://github.com/n8n-io/n8n/commit/8f9fe6269b5608346b0ac3612aa2e3af4a7baae1))
* **core:** Add support for building LLM applications ([#7235](https://github.com/n8n-io/n8n/issues/7235)) ([00a4b8b](https://github.com/n8n-io/n8n/commit/00a4b8b0c62883f2a36559a939f9c32c5d1c048e)), closes [#7246](https://github.com/n8n-io/n8n/issues/7246) [#7137](https://github.com/n8n-io/n8n/issues/7137)
* Workflow History pruning and prune time settings ([#7343](https://github.com/n8n-io/n8n/issues/7343)) ([0adc533](https://github.com/n8n-io/n8n/commit/0adc53371969ac3f759d06d9fbb095267fffe95e))



# [1.9.0](https://github.com/n8n-io/n8n/compare/n8n@1.8.0...n8n@1.9.0) (2023-09-28)


### Bug Fixes

* **Airtable Node:** Attachments field type fix ([#7227](https://github.com/n8n-io/n8n/issues/7227)) ([2af967c](https://github.com/n8n-io/n8n/commit/2af967cf88a4d6e795ff1641f9946f9fcbf49a03))
* **core:** Change WorkflowHistory nodes/connections columns to be json ([#7282](https://github.com/n8n-io/n8n/issues/7282)) ([a80abad](https://github.com/n8n-io/n8n/commit/a80abad3af8fed3a40b6f713cd94a16f44d84f60))
* **core:** Fix binary data manager check on pruning ([#7251](https://github.com/n8n-io/n8n/issues/7251)) ([484035e](https://github.com/n8n-io/n8n/commit/484035eb519ab28de31488484caaa4bf9a77d095))
* **core:** Fix missing execution ID in webhook-based workflow producing binary data ([#7244](https://github.com/n8n-io/n8n/issues/7244)) ([33991e9](https://github.com/n8n-io/n8n/commit/33991e92d0aabd13a44ba103de43a6ec2b90ca46))
* **core:** Handle filename* with quotes in Content-Disposition header ([#7229](https://github.com/n8n-io/n8n/issues/7229)) ([67b985f](https://github.com/n8n-io/n8n/commit/67b985fe89cc45e40f66b38bd2e0c310a4b3504c))
* **core:** Make DNS resolution order configurable ([#7272](https://github.com/n8n-io/n8n/issues/7272)) ([5b3121c](https://github.com/n8n-io/n8n/commit/5b3121c415ec96535eae4ed2adc28461311b6c6e))
* **core:** Make senderId required for all command messages ([#7252](https://github.com/n8n-io/n8n/issues/7252)) ([4b01428](https://github.com/n8n-io/n8n/commit/4b014286cf66e5f9b660fc145274be7caccbf34c))
* **core:** Prevent executions from displaying Running status incorrectly ([#7261](https://github.com/n8n-io/n8n/issues/7261)) ([861cac5](https://github.com/n8n-io/n8n/commit/861cac5257f5e0d3cc2a010f09481ab93b8241e6)), closes [/linear.app/n8n/issue/HELP-338/large-number-of-long-running-executions-for-nadjalemlist#comment-18d1fc96](https://github.com//linear.app/n8n/issue/HELP-338/large-number-of-long-running-executions-for-nadjalemlist/issues/comment-18d1fc96)
* **core:** Use consistent timezone-aware timestamps in postgres ([#6948](https://github.com/n8n-io/n8n/issues/6948)) ([0132514](https://github.com/n8n-io/n8n/commit/0132514f8b7005a895880bab9f547484e2e90710)), closes [#2178](https://github.com/n8n-io/n8n/issues/2178) [#2810](https://github.com/n8n-io/n8n/issues/2810) [#3855](https://github.com/n8n-io/n8n/issues/3855) [#2813](https://github.com/n8n-io/n8n/issues/2813)
* **editor:** Add debug feature docs link ([#7240](https://github.com/n8n-io/n8n/issues/7240)) ([4614e1e](https://github.com/n8n-io/n8n/commit/4614e1e1c90f1c7630ccc58e8400380afedba585))
* **editor:** Fix SQL editor issue ([#7236](https://github.com/n8n-io/n8n/issues/7236)) ([647fc6c](https://github.com/n8n-io/n8n/commit/647fc6c555702bb3222871fb50f8916c6d2ae3f3))
* Ensure new Set node is on top of search list ([#7215](https://github.com/n8n-io/n8n/issues/7215)) ([2491ccf](https://github.com/n8n-io/n8n/commit/2491ccf4d9f36ecc93e559918cf68c690ae149db))
* **HTTP Request Node:** Add suggestion how to fix '429 - too many requests' errors ([#7293](https://github.com/n8n-io/n8n/issues/7293)) ([0bc33b1](https://github.com/n8n-io/n8n/commit/0bc33b1cc2c2d3ae8db0342545b3a4a2b4931af9))
* Issue enforcing user limits on start plan ([#7188](https://github.com/n8n-io/n8n/issues/7188)) ([303bc8e](https://github.com/n8n-io/n8n/commit/303bc8e71e60c3ee8ccd6b823814945d892e3726))
* **Item Lists Node:** Concatenate operation pairedItems fix ([#7286](https://github.com/n8n-io/n8n/issues/7286)) ([cde23a1](https://github.com/n8n-io/n8n/commit/cde23a1bb1934bebe8e19308745910d625e3ca73))
* **Respond to Webhook Node:** JSON output from expression fix ([#7294](https://github.com/n8n-io/n8n/issues/7294)) ([8bc369d](https://github.com/n8n-io/n8n/commit/8bc369dd40836472502dc7b36c503a04db3f480c))


### Features

* Add onboarding flow ([#7212](https://github.com/n8n-io/n8n/issues/7212)) ([01e9340](https://github.com/n8n-io/n8n/commit/01e93406219f6c1712247d9855590ea06df3e965))
* Add user cloud it to telemetry ([#7232](https://github.com/n8n-io/n8n/issues/7232)) ([60c152d](https://github.com/n8n-io/n8n/commit/60c152dc72c27862f50304b8a824e2ec5e201787))
* **core:** Add secrets provider reload and refactor ([#7277](https://github.com/n8n-io/n8n/issues/7277)) ([53a7502](https://github.com/n8n-io/n8n/commit/53a7502d20eb95055e842e0450e9daea308443a1))
* **core:** Add Tournament as the new default expression evaluator ([#6964](https://github.com/n8n-io/n8n/issues/6964)) ([bf74f09](https://github.com/n8n-io/n8n/commit/bf74f09d69014da3c3fb2a56288b010670a4b982))
* **core:** Initial workflow history API ([#7234](https://github.com/n8n-io/n8n/issues/7234)) ([0083a9e](https://github.com/n8n-io/n8n/commit/0083a9e45d21928be259664532528706d0a57ecf))
* **core:** Introduce object store service ([#7225](https://github.com/n8n-io/n8n/issues/7225)) ([fa84545](https://github.com/n8n-io/n8n/commit/fa845453bb3d2ef72ef555bc8b8fa3f8bb703e1f))
* **editor:** Rework banners framework and add email confirmation banner ([#7205](https://github.com/n8n-io/n8n/issues/7205)) ([b0e98b5](https://github.com/n8n-io/n8n/commit/b0e98b59a6500b11f306403c563191749478c3fb)), closes [4#6afd052ec8d146a1b0fab8884a19add7](https://github.com/4/issues/6afd052ec8d146a1b0fab8884a19add7) [/github.com/n8n-io/n8n/blob/f9f122d46d26565a4cc5dcf63060e7ed9f359e53/packages/editor-ui/src/components/banners/BannerStack.vue#L14](https://github.com//github.com/n8n-io/n8n/blob/f9f122d46d26565a4cc5dcf63060e7ed9f359e53/packages/editor-ui/src/components/banners/BannerStack.vue/issues/L14) [/github.com/n8n-io/n8n/blob/b80d2e3bec59a9abe141a4c808ea2b7f5d9fecce/packages/editor-ui/src/stores/cloudPlan.store.ts#L59](https://github.com//github.com/n8n-io/n8n/blob/b80d2e3bec59a9abe141a4c808ea2b7f5d9fecce/packages/editor-ui/src/stores/cloudPlan.store.ts/issues/L59)
* **MISP Node:** Update credential to support HTTP Request node ([#7268](https://github.com/n8n-io/n8n/issues/7268)) ([e4c302c](https://github.com/n8n-io/n8n/commit/e4c302c6833c2a9cc6a5fc46d21272266222dd63))


### Performance Improvements

* **core:** Skip unneeded calls on every pruning cycle ([#7260](https://github.com/n8n-io/n8n/issues/7260)) ([db01164](https://github.com/n8n-io/n8n/commit/db01164ce11c2c1574899a60541d13712bb39324))



# [1.8.0](https://github.com/n8n-io/n8n/compare/n8n@1.7.0...n8n@1.8.0) (2023-09-20)


### Bug Fixes

* **core:** Make parsing of content-type and content-disposition headers more flexible ([#7217](https://github.com/n8n-io/n8n/issues/7217)) ([d41546b](https://github.com/n8n-io/n8n/commit/d41546b899e75c0decbf2fe2f0841b33c9b39bc9)), closes [#7149](https://github.com/n8n-io/n8n/issues/7149)
* **core:** Resolve domains to IPv4 first ([#7206](https://github.com/n8n-io/n8n/issues/7206)) ([e9ce531](https://github.com/n8n-io/n8n/commit/e9ce5312106e550c15eb4adc049e4b0151a7c40c))
* **editor:** Add ssh key type selection to source control settings when regenerating key ([#7172](https://github.com/n8n-io/n8n/issues/7172)) ([54bf66d](https://github.com/n8n-io/n8n/commit/54bf66d335060e866b4f120269b156c4690a8246))
* **editor:** No need to add click emitting click events, VUE delegates the handler to the root element of the component ([#7182](https://github.com/n8n-io/n8n/issues/7182)) ([3c055e4](https://github.com/n8n-io/n8n/commit/3c055e4d8d77addea014d8da363518c4c14c9a98))
* **editor:** Prevent duplicate creation of credential for OAuth2 ([#7163](https://github.com/n8n-io/n8n/issues/7163)) ([07a6417](https://github.com/n8n-io/n8n/commit/07a6417f0f52988e3dfac4583aab84426fc471cc))
* **editor:** Testing flaky resource mapper feature in e2e tests ([#7165](https://github.com/n8n-io/n8n/issues/7165)) ([aaf87c3](https://github.com/n8n-io/n8n/commit/aaf87c3edd434ab464f3ec4a4001c07895370cb0))
* **HTML Node:** Add pairedItem support for 'Convert to HTML Table' operation ([#7196](https://github.com/n8n-io/n8n/issues/7196)) ([6bc477b](https://github.com/n8n-io/n8n/commit/6bc477b50ebcb31eae6068b2218fea56349a64a9))
* **HTTP Request Node:** Decrease default timeout to 5min ([#7177](https://github.com/n8n-io/n8n/issues/7177)) ([321780d](https://github.com/n8n-io/n8n/commit/321780d4a2a1f7e5e7ab0ea23e0b2fc28d539330))
* **seven Node:** Rename sms77 to seven, fix credentials test ([#7180](https://github.com/n8n-io/n8n/issues/7180)) ([cf776b8](https://github.com/n8n-io/n8n/commit/cf776b8f1756c3e20ed39fe882ebaba05f12eb6a))
* **X (Formerly Twitter) Node:** Rename Twitter to X (keep Twitter alias) ([#7179](https://github.com/n8n-io/n8n/issues/7179)) ([d317e09](https://github.com/n8n-io/n8n/commit/d317e09c597a37fbb099ed1f032d27225e655eb9))


### Features

* **core:** Add command to trigger license refresh on workers ([#7184](https://github.com/n8n-io/n8n/issues/7184)) ([9f797b9](https://github.com/n8n-io/n8n/commit/9f797b96d818a5ae74ad82917347c99f3c249688))
* **core:** Add rsa option to ssh key generation ([#7154](https://github.com/n8n-io/n8n/issues/7154)) ([fdac2c8](https://github.com/n8n-io/n8n/commit/fdac2c85729e19be0fd18f6807a7f5f99dfca002))
* **Linear Node:** Add support for OAuth2 ([#7201](https://github.com/n8n-io/n8n/issues/7201)) ([12a3168](https://github.com/n8n-io/n8n/commit/12a3168367e3208665ab78fe52b00cf508f7a50d))
* **Microsoft Outlook Node:** Node overhaul ([#4449](https://github.com/n8n-io/n8n/issues/4449)) ([556a613](https://github.com/n8n-io/n8n/commit/556a6132bafc3eeb574fbd753a438a5e0f2c466d))
* **Set Node:** Overhaul ([#6348](https://github.com/n8n-io/n8n/issues/6348)) ([3a47455](https://github.com/n8n-io/n8n/commit/3a474552b211fad8939a19492f34c5e7b3137002))



# [1.7.0](https://github.com/n8n-io/n8n/compare/n8n@1.6.0...n8n@1.7.0) (2023-09-13)


### Bug Fixes

* Account for nanoid workflow ids for subworkflow execute policy ([#7094](https://github.com/n8n-io/n8n/issues/7094)) ([67092c0](https://github.com/n8n-io/n8n/commit/67092c0a1bf98ccc5ceadc3d582fac7bff2dc46c))
* **Code Node:** Disable WASM to address CVE-2023-37903 ([#7122](https://github.com/n8n-io/n8n/issues/7122)) ([36a8e91](https://github.com/n8n-io/n8n/commit/36a8e911e6f58d0b87816fae0443c6ce8f5ea45a))
* **Code Node:** Upgrade vm2 to address CVE-2023-37466 ([#7123](https://github.com/n8n-io/n8n/issues/7123)) ([0a35025](https://github.com/n8n-io/n8n/commit/0a35025e5e6669661bdfcc16378453ec9109a347))
* **core:** Disable Node.js custom inspection to address CVE-2023-37903 ([#7125](https://github.com/n8n-io/n8n/issues/7125)) ([a223734](https://github.com/n8n-io/n8n/commit/a223734a4a781834bee1a1484dffc47c56e8d50e)), closes [#7122](https://github.com/n8n-io/n8n/issues/7122)
* **editor:** Tweak hover area of workflow / cred cards ([#7108](https://github.com/n8n-io/n8n/issues/7108)) ([217de21](https://github.com/n8n-io/n8n/commit/217de21605beca57f087921231ae929279071686))
* **editor:** Unbind workflow endpoint events in case of workspace reset  ([#7129](https://github.com/n8n-io/n8n/issues/7129)) ([c9b7948](https://github.com/n8n-io/n8n/commit/c9b79485cf7d361174aeba175ccb98de7d918693))
* **editor:** Update git repo url validation regex ([#7151](https://github.com/n8n-io/n8n/issues/7151)) ([e51f173](https://github.com/n8n-io/n8n/commit/e51f173608dd79bfe53eb86eeaed976109f74410))
* **Google Cloud Firestore Node:** Fix empty string interpreted as number ([#7136](https://github.com/n8n-io/n8n/issues/7136)) ([915cfa0](https://github.com/n8n-io/n8n/commit/915cfa0f6a0311ca34d2f8eeb471c601473314aa))
* **HubSpot Node:** Fix issue with contact lists not working ([#5582](https://github.com/n8n-io/n8n/issues/5582)) ([6e5a4f6](https://github.com/n8n-io/n8n/commit/6e5a4f6a589550a816f421ffa966cfeea3cac64d))
* **Postgres Node:** Fix automatic column mapping ([#7121](https://github.com/n8n-io/n8n/issues/7121)) ([92af131](https://github.com/n8n-io/n8n/commit/92af1314fe60560cdfb52b3307cc74559ba530a8))
* **Zoho CRM Node:** Fix issue with Sales Order not updating ([#6959](https://github.com/n8n-io/n8n/issues/6959)) ([fd800b6](https://github.com/n8n-io/n8n/commit/fd800b674b52079eb2572a4d2465774759e9b31d))


### Features

* **core:** Add an option to enable WAL mode for SQLite ([#7118](https://github.com/n8n-io/n8n/issues/7118)) ([1d1a022](https://github.com/n8n-io/n8n/commit/1d1a022defefc790905cfb8fcb9dd364ffb063bb))
* **core:** Add commands to workers to respond with current state ([#7029](https://github.com/n8n-io/n8n/issues/7029)) ([7b49cf2](https://github.com/n8n-io/n8n/commit/7b49cf2a2c750d685af6cff464401f38482dac5a))
* **Salesforce Node:** Add fax field to lead option ([#7030](https://github.com/n8n-io/n8n/issues/7030)) ([01f875a](https://github.com/n8n-io/n8n/commit/01f875a94d193ba1e709bf6cfe31a3951f3af81a))



# [1.6.0](https://github.com/n8n-io/n8n/compare/n8n@1.5.1...n8n@1.6.0) (2023-09-06)


### Bug Fixes

* **core:** Add support for in-transit encryption (TLS) on Redis connections ([#7047](https://github.com/n8n-io/n8n/issues/7047)) ([a910757](https://github.com/n8n-io/n8n/commit/a910757cc5ac7e47f9e0ca6a57c8b624e269aaa4))
* **core:** Disallow orphan executions ([#7069](https://github.com/n8n-io/n8n/issues/7069)) ([8a28e98](https://github.com/n8n-io/n8n/commit/8a28e98ec811952163c58feaad608ec14ffc9243))
* **core:** Split event bus controller into community and ee ([#7107](https://github.com/n8n-io/n8n/issues/7107)) ([011ee2e](https://github.com/n8n-io/n8n/commit/011ee2e04b62e0182e9d6787064dea70654cb4ab))
* **editor:** Standardize save text ([#7093](https://github.com/n8n-io/n8n/issues/7093)) ([58b3492](https://github.com/n8n-io/n8n/commit/58b3492b0dcf140920ec97ce6d50e91a6d3a01a6))
* Ensure all new executions are saved ([#7061](https://github.com/n8n-io/n8n/issues/7061)) ([b8e06d2](https://github.com/n8n-io/n8n/commit/b8e06d245f5b8bc969d2eb29793e9d98a33e69a8))
* Load remote resources even if expressions in non requried parameters resolve ([#6987](https://github.com/n8n-io/n8n/issues/6987)) ([8a8d4e8](https://github.com/n8n-io/n8n/commit/8a8d4e8bb32588e79c3fcda2317c491ade9b3637))
* **Postgres Node:** Connection pool of the database object has been destroyed ([#7074](https://github.com/n8n-io/n8n/issues/7074)) ([9dd5f0e](https://github.com/n8n-io/n8n/commit/9dd5f0e579ccfd5144ddb547977f15b45dd7c9ce))
* **Postgres Node:** Tunnel doesn't always close ([#7087](https://github.com/n8n-io/n8n/issues/7087)) ([58e55ba](https://github.com/n8n-io/n8n/commit/58e55ba6691dc73a9f475a1989dccb51144e1825))


### Features

* **core:** Add list query middleware to credentials ([#7041](https://github.com/n8n-io/n8n/issues/7041)) ([fd78021](https://github.com/n8n-io/n8n/commit/fd78021b68a261291d76811a2a01d7336577bca7))
* **core:** Add support for floating licenses ([#7090](https://github.com/n8n-io/n8n/issues/7090)) ([e26553f](https://github.com/n8n-io/n8n/commit/e26553f1981d2788f4f2e1e5f5ce23ff8a4a7c8d))
* **core:** Migration for soft deletions for executions ([#7088](https://github.com/n8n-io/n8n/issues/7088)) ([413e0bc](https://github.com/n8n-io/n8n/commit/413e0bccb4d0144e5bdcf9221762e3f2b4428194))
* **HTTP Request Node:** Determine binary file name from content-disposition headers ([#7032](https://github.com/n8n-io/n8n/issues/7032)) ([273d091](https://github.com/n8n-io/n8n/commit/273d0913fe5f45c0fe074e6a788e475d5a1d50bd))
* **TheHive Node:** Overhaul ([#6457](https://github.com/n8n-io/n8n/issues/6457)) ([73e782e](https://github.com/n8n-io/n8n/commit/73e782e2cf9d4b96d8b3748e74ad93570663e536))



## [1.5.1](https://github.com/n8n-io/n8n/compare/n8n@1.5.0...n8n@1.5.1) (2023-08-31)


### Features

* **Strapi Node:** Add token credentials ([#7048](https://github.com/n8n-io/n8n/issues/7048)) ([c01bca5](https://github.com/n8n-io/n8n/commit/c01bca562b71d8b524e29edd37e8397d0689b180))



# [1.5.0](https://github.com/n8n-io/n8n/compare/n8n@1.4.0...n8n@1.5.0) (2023-08-31)


### Bug Fixes

* **Agile CRM Node:** Fix issue with company address not working ([#6997](https://github.com/n8n-io/n8n/issues/6997)) ([2f81652](https://github.com/n8n-io/n8n/commit/2f81652400b6a793fa610728519fd992c03c3d0d))
* **Code Node:** Switch over to vm2 fork ([#7018](https://github.com/n8n-io/n8n/issues/7018)) ([dfe0fa6](https://github.com/n8n-io/n8n/commit/dfe0fa65f8111cd534387e26197cb3836d694e27))
* **core:** Invalid NODES_INCLUDE should not crash the app ([#7038](https://github.com/n8n-io/n8n/issues/7038)) ([04e3178](https://github.com/n8n-io/n8n/commit/04e31789019aad6fe122ed81b06552a61d7f3a6d)), closes [#6683](https://github.com/n8n-io/n8n/issues/6683)
* **core:** Setup websocket keep-live messages ([#6866](https://github.com/n8n-io/n8n/issues/6866)) ([8bdb07d](https://github.com/n8n-io/n8n/commit/8bdb07d33ded48eab0b8f892a06e18f37bee9372)), closes [#6757](https://github.com/n8n-io/n8n/issues/6757)
* **core:** Throw `NodeSSLError` only for nodes that allow ignoring SSL issues ([#6928](https://github.com/n8n-io/n8n/issues/6928)) ([a01c3fb](https://github.com/n8n-io/n8n/commit/a01c3fbc19d66cf8b1dac3e34e0999dd36d81e7c))
* **Date & Time Node:** Dont parse date if it's not set (null or undefined) ([#7050](https://github.com/n8n-io/n8n/issues/7050)) ([d72f79f](https://github.com/n8n-io/n8n/commit/d72f79ffb393a096f510f0c41bb66d987fe8cb0d))
* **editor:** Fix sending of Ask AI tracking events ([#7002](https://github.com/n8n-io/n8n/issues/7002)) ([fb05afa](https://github.com/n8n-io/n8n/commit/fb05afa16560c3c837abf46824f8dc7fa3bb1c83))
* **Microsoft Excel 365 Node:** Support for more extensions in workbook rlc ([#7020](https://github.com/n8n-io/n8n/issues/7020)) ([d6e1cf2](https://github.com/n8n-io/n8n/commit/d6e1cf232f86ddc69cceb69c8971c3373dab454c))
* **MongoDB Node:** Stringify response ObjectIDs ([#6990](https://github.com/n8n-io/n8n/issues/6990)) ([9ca990b](https://github.com/n8n-io/n8n/commit/9ca990b9936ee80972952d0a1ad73c2926809ba2))
* **MongoDB Node:** Upgrade mongodb package to address  CVE-2021-32050 ([#7054](https://github.com/n8n-io/n8n/issues/7054)) ([d3f6356](https://github.com/n8n-io/n8n/commit/d3f635657c7514296fd0a473ba13672db2717490))
* **Postgres Node:** Empty return data fix for Postgres and MySQL ([#7016](https://github.com/n8n-io/n8n/issues/7016)) ([176ccd6](https://github.com/n8n-io/n8n/commit/176ccd62bc1d6f28958c0fc894ee647f1e3a5f6e))
* **Webhook Node:** Fix URL params for webhooks ([#6986](https://github.com/n8n-io/n8n/issues/6986)) ([596b569](https://github.com/n8n-io/n8n/commit/596b5695cdcca33da02bec428d58de8b2a13297e))


### Features

* **core:** Add filtering, selection and pagination to users ([#6994](https://github.com/n8n-io/n8n/issues/6994)) ([b716241](https://github.com/n8n-io/n8n/commit/b716241b428ef09cf6bdf32cb3a8680e9ba8f25f))
* **core:** Add MFA ([#4767](https://github.com/n8n-io/n8n/issues/4767)) ([2b7ba6f](https://github.com/n8n-io/n8n/commit/2b7ba6fdf100ef78b60358648d773e2f200847b8))
* **editor:** Debug executions in the editor ([#6834](https://github.com/n8n-io/n8n/issues/6834)) ([c833078](https://github.com/n8n-io/n8n/commit/c833078c87adeadb1e701f17d3f380c669eb1460))
* External Secrets storage for credentials ([#6477](https://github.com/n8n-io/n8n/issues/6477)) ([ed927d3](https://github.com/n8n-io/n8n/commit/ed927d34b25b4ddd7048b622c141e32a8a57b6b7))
* **RSS Read Node:** Add support for self signed certificates ([#7039](https://github.com/n8n-io/n8n/issues/7039)) ([3b9f0fe](https://github.com/n8n-io/n8n/commit/3b9f0fed7af2d3a234049ab7d50d883ee4608007))



# [1.4.0](https://github.com/n8n-io/n8n/compare/n8n@1.3.0...n8n@1.4.0) (2023-08-23)


### Bug Fixes

* **core:** Add recoveryInProgress flag file ([#6962](https://github.com/n8n-io/n8n/issues/6962)) ([7b96820](https://github.com/n8n-io/n8n/commit/7b96820218449958180d4c34bebdc4c4de9172e1))
* **core:** Fix `continueOnFail` for expression error in Set ([#6939](https://github.com/n8n-io/n8n/issues/6939)) ([d4fac05](https://github.com/n8n-io/n8n/commit/d4fac0527b7a34aace9ea0ff89dde152026d6c17))
* **core:** Fix `import:workflow` command ([#6996](https://github.com/n8n-io/n8n/issues/6996)) ([8c38d85](https://github.com/n8n-io/n8n/commit/8c38d85e765114df03afb5e221b3d4ae4e6c0fc7))
* **core:** Replace throw with warning when deactivating a non-active workflow ([#6969](https://github.com/n8n-io/n8n/issues/6969)) ([b6a00fe](https://github.com/n8n-io/n8n/commit/b6a00febbdd62560fa68321fbcd6e44c92a82ddd))
* **core:** Set up OAuth2 cred test ([#6960](https://github.com/n8n-io/n8n/issues/6960)) ([4fc69b7](https://github.com/n8n-io/n8n/commit/4fc69b776ccea91c2a38249dc4f4ef0b191ce374))
* **editor:** Do not flag dynamic load options issue on expression ([#6932](https://github.com/n8n-io/n8n/issues/6932)) ([60a1ef0](https://github.com/n8n-io/n8n/commit/60a1ef09934608afbe171bf3cf18ca5e95987153))
* **editor:** Ensure community node install button tracks user agreement ([#6976](https://github.com/n8n-io/n8n/issues/6976)) ([0ddfc73](https://github.com/n8n-io/n8n/commit/0ddfc73bee88c994876787a41540ef847f4fcd4f))
* **editor:** Fix parsing for single quoted resolvables ([#6982](https://github.com/n8n-io/n8n/issues/6982)) ([f32e993](https://github.com/n8n-io/n8n/commit/f32e9932275bb51a724c6ae681ed9ca0683a8e8e))
* **editor:** Fix Remove all fields not removing values in resource mapper ([#6940](https://github.com/n8n-io/n8n/issues/6940)) ([e6cff3f](https://github.com/n8n-io/n8n/commit/e6cff3fce4de1644b75b07318fe561f721aee51c))
* **editor:** Prevent Code node linter from erroring on `null` parse ([#6934](https://github.com/n8n-io/n8n/issues/6934)) ([40d3a29](https://github.com/n8n-io/n8n/commit/40d3a295d3c5ddcf5c034c02b3584532c395a12c))
* **Google Sheets Node:** Fix short sheet name interpreted as range ([#6989](https://github.com/n8n-io/n8n/issues/6989)) ([00268a0](https://github.com/n8n-io/n8n/commit/00268a019a1b09ba49971504bb38cd81a281236e))
* **Google Sheets Trigger Node:** Support sheet names with non-latin characters ([#6970](https://github.com/n8n-io/n8n/issues/6970)) ([052dd7c](https://github.com/n8n-io/n8n/commit/052dd7cc9d10b2365b38001c6e091bd52bf45873))
* **GraphQL Node:** Improve error handling ([#6955](https://github.com/n8n-io/n8n/issues/6955)) ([41db637](https://github.com/n8n-io/n8n/commit/41db6371f0d7a736bf7e1c13e2a3acd678bec246))
* **Mautic Node:** Fix issue with owner not being set correctly ([#6991](https://github.com/n8n-io/n8n/issues/6991)) ([64b950f](https://github.com/n8n-io/n8n/commit/64b950f2944f8fe352e6832f4059047d14ba9485))
* **Salesforce Node:** Fix Account update owner operation ([#6958](https://github.com/n8n-io/n8n/issues/6958)) ([9b27878](https://github.com/n8n-io/n8n/commit/9b27878d8fe8755d76d09db07be01bcab83b8772))
* **Shopify Node:** Fix pagination when using options ([#6972](https://github.com/n8n-io/n8n/issues/6972)) ([475d9c9](https://github.com/n8n-io/n8n/commit/475d9c98e8281e62e3566671bb6ddb1d028b543f))
* **Webhook Node:** Backward compatible form-data parsing for non-array fields ([#6967](https://github.com/n8n-io/n8n/issues/6967)) ([9455bcf](https://github.com/n8n-io/n8n/commit/9455bcfef5383ee351b620f12a0f5fba2447a839))


### Features

* **core:** Add a warning to error workflows that cannot be started due to permission or settings ([#6961](https://github.com/n8n-io/n8n/issues/6961)) ([67b88f7](https://github.com/n8n-io/n8n/commit/67b88f75f424011e3e49ebe3a37e36871a2253ae))
* **core:** Add support for ready hooks, and credentials overwrite endpoint in workers ([#6954](https://github.com/n8n-io/n8n/issues/6954)) ([8f8a1de](https://github.com/n8n-io/n8n/commit/8f8a1de3dd478e2e7b33b4b8a64bb0e3b7cda1f3))
* **editor:** Show banner for non-production licenses ([#6943](https://github.com/n8n-io/n8n/issues/6943)) ([413570c](https://github.com/n8n-io/n8n/commit/413570c49dc800cfed0581b8ae1798aa0b4bbd50))
* Remove PostHog event calls ([#6915](https://github.com/n8n-io/n8n/issues/6915)) ([270946a](https://github.com/n8n-io/n8n/commit/270946a93bc61ae3953a3dd9b2835e458565e12c))
* **Send Email Node:** Add support for sending text and html email simultaneously ([#6978](https://github.com/n8n-io/n8n/issues/6978)) ([3860d41](https://github.com/n8n-io/n8n/commit/3860d41d737d56a616e3a8c61a90d3ec956b89cd))



# [1.3.0](https://github.com/n8n-io/n8n/compare/n8n@1.2.0...n8n@1.3.0) (2023-08-16)


### Bug Fixes

* **core:** Don't let bull override the default redis config ([#6897](https://github.com/n8n-io/n8n/issues/6897)) ([cfeb322](https://github.com/n8n-io/n8n/commit/cfeb322b3b19405e2788e3ca3325fd491d5ebd28))
* **core:** Fix fetching of EE executions ([#6901](https://github.com/n8n-io/n8n/issues/6901)) ([f3fce48](https://github.com/n8n-io/n8n/commit/f3fce48155d4a1ed262efce16cbe537b19aa6963))
* **core:** Update frontend urls when using the `--tunnel` option ([#6898](https://github.com/n8n-io/n8n/issues/6898)) ([718e613](https://github.com/n8n-io/n8n/commit/718e61354dc62e6aa1af69050eea52de6aa3c350))
* **editor:** Disable telemetry in dev mode and in E2E tests ([#6869](https://github.com/n8n-io/n8n/issues/6869)) ([808a928](https://github.com/n8n-io/n8n/commit/808a92809e4d389d902249646d5dc146de1d4e98))
* **editor:** Fix code node’s content property to be reactive ([#6931](https://github.com/n8n-io/n8n/issues/6931)) ([3b75bc6](https://github.com/n8n-io/n8n/commit/3b75bc6bc1c954c4d4a899edddda214f0a2245fb))
* **editor:** Fix event emit on credential sharing ([#6922](https://github.com/n8n-io/n8n/issues/6922)) ([297c3c9](https://github.com/n8n-io/n8n/commit/297c3c91f23a47b1aa78323d2b6e5677fbab8402))
* **editor:** Fix multiOptions parameters resetting on initial load ([#6903](https://github.com/n8n-io/n8n/issues/6903)) ([49867c2](https://github.com/n8n-io/n8n/commit/49867c2b176a5e76c4b9e7caafc29a44633332bf))
* **editor:** Update execution view layout ([#6882](https://github.com/n8n-io/n8n/issues/6882)) ([0339732](https://github.com/n8n-io/n8n/commit/03397323784809eb64c30b2ee535e8516ab06fbf))
* **Email Trigger (IMAP) Node:** Fix connection issue with unexpected spaces in host ([#6886](https://github.com/n8n-io/n8n/issues/6886)) ([f3248e4](https://github.com/n8n-io/n8n/commit/f3248e46e478e5ac061c3d69da988b0db8acf553))
* Fix issue with key formatting if null or undefined ([#6924](https://github.com/n8n-io/n8n/issues/6924)) ([4e4a3cf](https://github.com/n8n-io/n8n/commit/4e4a3cf7ab8dee45cc15e8948f8628c5915cc841))
* Fix issue with key formatting introduced in 1.2.0 ([#6896](https://github.com/n8n-io/n8n/issues/6896)) ([0e075c9](https://github.com/n8n-io/n8n/commit/0e075c9cb540d78209aaa3c8240259f074c31846))
* Fix lag when node parameters are updated ([#6941](https://github.com/n8n-io/n8n/issues/6941)) ([3eb65e0](https://github.com/n8n-io/n8n/commit/3eb65e08c4f22334aeae172504991a688273528e))
* **HTTP Request Node:** Improve error handling for TCP socket errors when `Continue On Fail` is enabled ([#6925](https://github.com/n8n-io/n8n/issues/6925)) ([96ff1f8](https://github.com/n8n-io/n8n/commit/96ff1f847d2672ecf6604dde6c3b5c594c3b1e2f))
* Prevent workflow breaking when credential type is unknown ([#6923](https://github.com/n8n-io/n8n/issues/6923)) ([e83b93f](https://github.com/n8n-io/n8n/commit/e83b93f293ab8df37f896cc315afab50a477bbef))
* **Respond to Webhook Node:** Return headers in response ([#6921](https://github.com/n8n-io/n8n/issues/6921)) ([a82107f](https://github.com/n8n-io/n8n/commit/a82107fb05120f7365086032c9b05ea316716327))


### Features

* **core:** Add support for not requiring SMTP auth with user management ([#3742](https://github.com/n8n-io/n8n/issues/3742)) ([eead6d4](https://github.com/n8n-io/n8n/commit/eead6d49f238f41714911d1488b75515472c34a0))
* **core:** Descriptive message for common nodeJS errors ([#6841](https://github.com/n8n-io/n8n/issues/6841)) ([3adb0b6](https://github.com/n8n-io/n8n/commit/3adb0b66ea2c1e929850345bc31e5b0a708eabd0))
* **editor:** Ask AI in Code node ([#6672](https://github.com/n8n-io/n8n/issues/6672)) ([fde6ad1](https://github.com/n8n-io/n8n/commit/fde6ad1e7fa6236c6c1ac1e3ff6d8e959012543a))
* Enable parallel processing on multiple queue nodes ([#6295](https://github.com/n8n-io/n8n/issues/6295)) ([44afcff](https://github.com/n8n-io/n8n/commit/44afcff95916cd00df66391e54440d3f96788913))



# [1.2.0](https://github.com/n8n-io/n8n/compare/n8n@1.1.0...n8n@1.2.0) (2023-08-09)


### Bug Fixes

* Auth.api user limit test expecting incorrect status ([#6836](https://github.com/n8n-io/n8n/issues/6836)) ([371bfa0](https://github.com/n8n-io/n8n/commit/371bfa0f488f0a240bd1a8854759d6f6639e6eea))
* **Code Node:** Consistent redirection of stdout for JS and Python sandboxes ([#6818](https://github.com/n8n-io/n8n/issues/6818)) ([f718c22](https://github.com/n8n-io/n8n/commit/f718c2291f0385bfb60ea70e7b7a943a4c6b5149))
* **core:** Add missing primary key on the `execution_data` table on postgres ([#6797](https://github.com/n8n-io/n8n/issues/6797)) ([dc295ac](https://github.com/n8n-io/n8n/commit/dc295ac5bfe8a62ce208656a8b25a89376af276a))
* **core:** Add sharing data to workflows in EE executions ([#6872](https://github.com/n8n-io/n8n/issues/6872)) ([6796d9e](https://github.com/n8n-io/n8n/commit/6796d9e5d676a7e76206462ef18640c246f0dc5a))
* **core:** Allow ignoring SSL issues on generic oauth2 credentials ([#6702](https://github.com/n8n-io/n8n/issues/6702)) ([feac369](https://github.com/n8n-io/n8n/commit/feac369f6c5590f30e63bed6d5569a57710a8d2e))
* **core:** Change VariablesService to DI and use caching ([#6827](https://github.com/n8n-io/n8n/issues/6827)) ([659ca26](https://github.com/n8n-io/n8n/commit/659ca26fe7cf7d1b9403f6c20b63b598f7dfa7b5))
* **core:** Fix loading of scoped-community packages ([#6807](https://github.com/n8n-io/n8n/issues/6807)) ([53e58b4](https://github.com/n8n-io/n8n/commit/53e58b408a8ef6a0f911593180d818ccee92cc1d))
* **core:** Fix property existence checks on AugmentObject ([#6842](https://github.com/n8n-io/n8n/issues/6842)) ([732416f](https://github.com/n8n-io/n8n/commit/732416f52f49eeb542401439e5b96b4b1a083c05))
* **core:** Fix source control name and email being switched ([#6839](https://github.com/n8n-io/n8n/issues/6839)) ([6ec7033](https://github.com/n8n-io/n8n/commit/6ec7033bb711648c8c2d93f4f2b15b3b6dfdcaea))
* **core:** Fix WebSocket close codes ([a8bfb46](https://github.com/n8n-io/n8n/commit/a8bfb4618323731de8bc9bc265b3bbb9de69c50c))
* **core:** Log crash causes to console when sentry is disabled ([#6890](https://github.com/n8n-io/n8n/issues/6890)) ([6553d92](https://github.com/n8n-io/n8n/commit/6553d92c7c128b117b6bdbd33182002f6cf24fa1))
* **core:** OAuth1 authentication fix for Clever Cloud API ([#6847](https://github.com/n8n-io/n8n/issues/6847)) ([5ab30fd](https://github.com/n8n-io/n8n/commit/5ab30fdd95c766e57f8c2cf7c7a9951bbf3d7c2d))
* **core:** Restrict read/write file paths access ([#6582](https://github.com/n8n-io/n8n/issues/6582)) ([f6bf9e9](https://github.com/n8n-io/n8n/commit/f6bf9e9887bb46bb884fd06f3e789f8585445501))
* **core:** Serialize BigInts ([#6805](https://github.com/n8n-io/n8n/issues/6805)) ([7b27fa5](https://github.com/n8n-io/n8n/commit/7b27fa5898cd3c8c9882cbec0c36ff703510b57d))
* **core:** Update packages to address CVE-2023-2142 and CVE-2020-28469 ([#6844](https://github.com/n8n-io/n8n/issues/6844)) ([a5667e6](https://github.com/n8n-io/n8n/commit/a5667e6c42fae96a48e39464cbcec808d36bb5ee))
* Correct typos in Taiga and ServiceNow nodes ([#6814](https://github.com/n8n-io/n8n/issues/6814)) ([803b152](https://github.com/n8n-io/n8n/commit/803b1521facb7908c34fbb729d15aaaf5680e471))
* Display source control buttons properly ([#6756](https://github.com/n8n-io/n8n/issues/6756)) ([d050b99](https://github.com/n8n-io/n8n/commit/d050b99fb218ae31dfd0ec7dea88884e14021495))
* **editor:** Close tags dropdown when modal is opened ([#6766](https://github.com/n8n-io/n8n/issues/6766)) ([cf00ba7](https://github.com/n8n-io/n8n/commit/cf00ba708941bebceda8278a359b0badaa111f2c)), closes [#6571](https://github.com/n8n-io/n8n/issues/6571)
* **editor:** Do not show mapping discoverability tooltip after dismiss ([#6862](https://github.com/n8n-io/n8n/issues/6862)) ([08982ed](https://github.com/n8n-io/n8n/commit/08982ede4c3dd2b38b1a0ce91adf8198f0af1776))
* **editor:** Fix code node highlight error ([#6791](https://github.com/n8n-io/n8n/issues/6791)) ([50b0dc2](https://github.com/n8n-io/n8n/commit/50b0dc21fd0a698f87538e5458274ed50ab6774e))
* **editor:** Fix collapsed sub menu elements ([#6778](https://github.com/n8n-io/n8n/issues/6778)) ([d33528d](https://github.com/n8n-io/n8n/commit/d33528dab399bc01461ab5e3af1fbb75e5d89d91))
* **editor:** Fix credential errors in executions view for workflow sharee  ([#6875](https://github.com/n8n-io/n8n/issues/6875)) ([a0f9b2e](https://github.com/n8n-io/n8n/commit/a0f9b2eefe6050264b0c892c6e79e2140ab05825))
* **editor:** Fix redo when adding node on connection ([#6833](https://github.com/n8n-io/n8n/issues/6833)) ([4ac4b85](https://github.com/n8n-io/n8n/commit/4ac4b850dd7187e4e4ef50bbe442ebf273e51eb9))
* **editor:** Fix tooltip opening delay prop name ([#6776](https://github.com/n8n-io/n8n/issues/6776)) ([e19b0d7](https://github.com/n8n-io/n8n/commit/e19b0d7748765570903831d5e676e6c4deba2fef))
* **editor:** Fix value syncing in SQL and HTML editor ([#6848](https://github.com/n8n-io/n8n/issues/6848)) ([90e825f](https://github.com/n8n-io/n8n/commit/90e825f74368588073b1403b0681a89704eced06))
* **editor:** Improve displaying and hiding of connections actions ([#6823](https://github.com/n8n-io/n8n/issues/6823)) ([369a2e9](https://github.com/n8n-io/n8n/commit/369a2e97968c6d40d827d8e780a8d3f1fd2188f7))
* **editor:** Prevent text edit dialog from re-opening in same tick ([#6781](https://github.com/n8n-io/n8n/issues/6781)) ([c9f3acc](https://github.com/n8n-io/n8n/commit/c9f3acc8485edd0adbde4a633318a01b018d6fc0))
* **editor:** Remove additional margin on tooltip ([#6802](https://github.com/n8n-io/n8n/issues/6802)) ([651cf34](https://github.com/n8n-io/n8n/commit/651cf34da60fb3842132905adfee3cd5e1395c75))
* **editor:** Resolve vue 3 related console-warnings ([#6779](https://github.com/n8n-io/n8n/issues/6779)) ([30484a0](https://github.com/n8n-io/n8n/commit/30484a0615c90525fa0604b8b0df16159f18a6d4))
* **editor:** Vue3 - Fix modal positioning and multi-select tag sizing ([#6783](https://github.com/n8n-io/n8n/issues/6783)) ([4e491b7](https://github.com/n8n-io/n8n/commit/4e491b754fe74ebdffdc292f4358ee98ad99e01d))
* **Email Trigger (IMAP) Node:**  UTF-8 attachments are not correctly named ([#6856](https://github.com/n8n-io/n8n/issues/6856)) ([72814d1](https://github.com/n8n-io/n8n/commit/72814d1f0fb5dfce19a89397a6a1cd5829563222))
* Fix all modal sizes ([#6820](https://github.com/n8n-io/n8n/issues/6820)) ([7525cfe](https://github.com/n8n-io/n8n/commit/7525cfe2dcd03e5050ffb32e8fef64132788d62e))
* Fix horizontal overflow for dialogs ([#6830](https://github.com/n8n-io/n8n/issues/6830)) ([41d8a18](https://github.com/n8n-io/n8n/commit/41d8a18d47dfeb0119034efe0e5779a9bfb0edce))
* Fix issue with key based credentials not being read correctly ([#6824](https://github.com/n8n-io/n8n/issues/6824)) ([db21a8d](https://github.com/n8n-io/n8n/commit/db21a8db75833c86ab3d662c6c864f9f5e47c436))
* Fix tags overflow handler in workflows header ([#6784](https://github.com/n8n-io/n8n/issues/6784)) ([7cd4588](https://github.com/n8n-io/n8n/commit/7cd45885bf13479948a4c5bb441d24b3c042a624))
* **GoToWebinar Node:** Fix issue with timezone incorrectly being required ([#6865](https://github.com/n8n-io/n8n/issues/6865)) ([905eef8](https://github.com/n8n-io/n8n/commit/905eef85594bb10f27c7c97f24ac7f9fcedcc5cf))
* Handle subtitle errors when pasting workflow ([#6826](https://github.com/n8n-io/n8n/issues/6826)) ([31a4cfc](https://github.com/n8n-io/n8n/commit/31a4cfc9698666bb69b2fd54d7af3644a31b69c2))
* **Lemlist Node:** Fix pagination issues with campaigns and activities ([#6734](https://github.com/n8n-io/n8n/issues/6734)) ([c3e76ec](https://github.com/n8n-io/n8n/commit/c3e76ec697991f4a184e51cb7753a5c89064f7f9))
* **Linear Node:** Fix issue creation priority ([#6813](https://github.com/n8n-io/n8n/issues/6813)) ([fce8cc4](https://github.com/n8n-io/n8n/commit/fce8cc427579c9098359b9d1ecc420650299b229))
* **Postgres Trigger Node:** Imposible to cancell execution manually ([#6709](https://github.com/n8n-io/n8n/issues/6709)) ([491378d](https://github.com/n8n-io/n8n/commit/491378de772670b640be23e3b9bc7eadad6d3ebe))
* Remove tag animation ([#6821](https://github.com/n8n-io/n8n/issues/6821)) ([52aafe0](https://github.com/n8n-io/n8n/commit/52aafe07372dd3dd46ddc8e4ad14de08f02fb4e8))
* Respect set modal widths ([#6771](https://github.com/n8n-io/n8n/issues/6771)) ([3aaf1ac](https://github.com/n8n-io/n8n/commit/3aaf1ac0fd9cb7db6e074c1dca421de066c0793b)), closes [#6571](https://github.com/n8n-io/n8n/issues/6571)
* Show NodeIcon tooltips by removing pointer-events: none ([#6777](https://github.com/n8n-io/n8n/issues/6777)) ([eb898f7](https://github.com/n8n-io/n8n/commit/eb898f744f7c3df92635409a136809473b4de0c1))
* **TheHive Node:** Treat  `ApiKey` as a secret ([#6786](https://github.com/n8n-io/n8n/issues/6786)) ([11a3965](https://github.com/n8n-io/n8n/commit/11a3965ba89e75daaccf39596272eef70f1fc316))
* **Todoist Node:** Fix issue with section id being ignored ([#6799](https://github.com/n8n-io/n8n/issues/6799)) ([749468e](https://github.com/n8n-io/n8n/commit/749468e4fa3d823785a01e79b02f4897bc40c943))


### Features

* Clean up onboarding experiment ([#6873](https://github.com/n8n-io/n8n/issues/6873)) ([3619345](https://github.com/n8n-io/n8n/commit/36193451692b878cea703e3a743d9ac8f3ba5086))
* **core:** Add metrics option to cache ([#6846](https://github.com/n8n-io/n8n/issues/6846)) ([adcf5a9](https://github.com/n8n-io/n8n/commit/adcf5a96e83d8b43b155f5a834a74b3a1fd4274b))
* **core:** Add unique id to instances ([#6863](https://github.com/n8n-io/n8n/issues/6863)) ([6499f42](https://github.com/n8n-io/n8n/commit/6499f424811188fa4785db9d86b1299e4fb39540))
* **core:** Create a dsl for writing db agnostic migrations ([#6853](https://github.com/n8n-io/n8n/issues/6853)) ([75be1a9](https://github.com/n8n-io/n8n/commit/75be1a9c0d223a5d866551e836d7ab1b952d03ca))
* **core:** Credentials for popular SecOps services, Part 1 ([#6775](https://github.com/n8n-io/n8n/issues/6775)) ([11567f9](https://github.com/n8n-io/n8n/commit/11567f946be411f081b2ba25c2ac60d5dcf56835))
* **core:** Make Redis available for backend communication ([#6719](https://github.com/n8n-io/n8n/issues/6719)) ([3cad60e](https://github.com/n8n-io/n8n/commit/3cad60e9184de7ad73893062964366a09d4487df))
* **editor:** Add "Download" button if JSON data is to large ([#6850](https://github.com/n8n-io/n8n/issues/6850)) ([efe08cc](https://github.com/n8n-io/n8n/commit/efe08cced3979e40bbf011301f51f9f2f69117de))
* **editor:** Migrate Design System and Editor UI to Vue 3 ([#6476](https://github.com/n8n-io/n8n/issues/6476)) ([dd6a4c9](https://github.com/n8n-io/n8n/commit/dd6a4c956adb997b59ee0174eedd9b8f6265ec6b)), closes [#6571](https://github.com/n8n-io/n8n/issues/6571)
* **Facebook Graph API Node:** Add support for v16 and v17 ([#6808](https://github.com/n8n-io/n8n/issues/6808)) ([46a41c1](https://github.com/n8n-io/n8n/commit/46a41c1c91c7ebadd72fb51b6f749a542a7393fc))
* **Pipedrive Node:** Add option to update the file name and description ([#6883](https://github.com/n8n-io/n8n/issues/6883)) ([f8ad543](https://github.com/n8n-io/n8n/commit/f8ad543af5c5d680d23d5dab861a6b3fe47b4ccc))


### Performance Improvements

* **core:** Add filtering and pagination to `GET /workflows` ([#6845](https://github.com/n8n-io/n8n/issues/6845)) ([dceff67](https://github.com/n8n-io/n8n/commit/dceff675ecd1d9f72ca2614c42da2bfaa758f305)), closes [#6876](https://github.com/n8n-io/n8n/issues/6876)
* **core:** Cache roles ([#6803](https://github.com/n8n-io/n8n/issues/6803)) ([e4f0418](https://github.com/n8n-io/n8n/commit/e4f041815a9a919add9ad616e17ed31d4b645c2c))
* **core:** Cache webhooks ([#6825](https://github.com/n8n-io/n8n/issues/6825)) ([0511458](https://github.com/n8n-io/n8n/commit/0511458d41c65f81edc17b5ff58a0be911a7629d))
* **editor:** Memoize locale translate calls during actions generation ([#6773](https://github.com/n8n-io/n8n/issues/6773)) ([2d47e8d](https://github.com/n8n-io/n8n/commit/2d47e8dc4ad2ec75d25cd5e67ab89f29766e0a7f))



# [1.1.0](https://github.com/n8n-io/n8n/compare/n8n@1.0.1...n8n@1.1.0) (2023-07-26)


### Bug Fixes

* Add missing indices on sqlite ([#6673](https://github.com/n8n-io/n8n/issues/6673)) ([b1838f7](https://github.com/n8n-io/n8n/commit/b1838f7fab3e6d2983fa4d2ba1a480c79f8fe2c5))
* **API:** Do not add starting node on workflow creation ([#6686](https://github.com/n8n-io/n8n/issues/6686)) ([92192fb](https://github.com/n8n-io/n8n/commit/92192fbd6108a71fca591e5284269239d4347621))
* **API:** Fix issue with workflow setting not supporting newer nanoids ([#6699](https://github.com/n8n-io/n8n/issues/6699)) ([c7e1013](https://github.com/n8n-io/n8n/commit/c7e10130d694347982f50bc0ad1024101e27beea))
* **AwsS3 Node:** Fix issue if bucket name contains a '.' ([#6542](https://github.com/n8n-io/n8n/issues/6542)) ([540d32d](https://github.com/n8n-io/n8n/commit/540d32dee4b8927199e047c77acf516d5b824bc3))
* **Brevo Node:** Rename SendInBlue node to Brevo node ([#6521](https://github.com/n8n-io/n8n/issues/6521)) ([e63b398](https://github.com/n8n-io/n8n/commit/e63b3982d200ade34461b9159eb1e988f494c025))
* **Code Node:** Install python modules always in a user-writable folder ([#6568](https://github.com/n8n-io/n8n/issues/6568)) ([bf35124](https://github.com/n8n-io/n8n/commit/bf351243dfa69095699596e8828904fda025d45c))
* **core:** Add empty credential value marker to show empty pw field ([#6532](https://github.com/n8n-io/n8n/issues/6532)) ([9294e2d](https://github.com/n8n-io/n8n/commit/9294e2da3c7c99c2099f5865e610fa7217bf06be))
* **core:** Deleting manual executions should defer deleting binary data ([#6680](https://github.com/n8n-io/n8n/issues/6680)) ([462a674](https://github.com/n8n-io/n8n/commit/462a674d1759dc5ae9849daa48cc8c4130dd030e))
* **core:** Filter out workflows that failed to activate on startup ([#6676](https://github.com/n8n-io/n8n/issues/6676)) ([667c15d](https://github.com/n8n-io/n8n/commit/667c15d0dfbdab0c29114d5002eed75031c79b42))
* **core:** Fix credentials test ([#6569](https://github.com/n8n-io/n8n/issues/6569)) ([1abd172](https://github.com/n8n-io/n8n/commit/1abd172f73e171e37c4cc3ccfaa395c6a46bdf48))
* **core:** Fix migrations for MySQL/MariaDB ([#6591](https://github.com/n8n-io/n8n/issues/6591)) ([29882a6](https://github.com/n8n-io/n8n/commit/29882a6f39dddcd1c8c107c20a548ce8dc665cba))
* **core:** Handle all uncaught exception, not just the ones from Axios ([#6666](https://github.com/n8n-io/n8n/issues/6666)) ([ff07595](https://github.com/n8n-io/n8n/commit/ff0759530df3780e8eb53a29ec4ab4e98e5755c6))
* **core:** Improve the performance of last 2 sqlite migrations ([#6522](https://github.com/n8n-io/n8n/issues/6522)) ([31cba87](https://github.com/n8n-io/n8n/commit/31cba87d307183d613890c7e6d627636b5280b52))
* **core:** Load SAML libraries dynamically ([#6690](https://github.com/n8n-io/n8n/issues/6690)) ([fce5609](https://github.com/n8n-io/n8n/commit/fce5609fa32b81ff8e44567233c77a7a1d6232df))
* **core:** Redirect user to previous url after SSO signin ([#6710](https://github.com/n8n-io/n8n/issues/6710)) ([08331c6](https://github.com/n8n-io/n8n/commit/08331c63fbc0d69d2203f14165b15e1a596788b0))
* **core:** Reduce memory consumption on `BinaryDataManager.init` ([#6633](https://github.com/n8n-io/n8n/issues/6633)) ([329d22f](https://github.com/n8n-io/n8n/commit/329d22f5d1f484d899df885a871f0f32839f0098))
* **core:** Remove typeorm patches, but still enforce transactions on every migration ([#6594](https://github.com/n8n-io/n8n/issues/6594)) ([9def7a7](https://github.com/n8n-io/n8n/commit/9def7a729b52cd6b4698c47e190e9e2bd7894da5)), closes [#6519](https://github.com/n8n-io/n8n/issues/6519)
* **core:** Rename to credential_stubs and variable_stubs.json ([#6528](https://github.com/n8n-io/n8n/issues/6528)) ([b06462f](https://github.com/n8n-io/n8n/commit/b06462f4415bd1143a00b4a66e6e626da8c52196))
* **core:** Support redis cluster in queue mode ([#6708](https://github.com/n8n-io/n8n/issues/6708)) ([4029386](https://github.com/n8n-io/n8n/commit/40293863492d73865f805870937e46f3d0bdaa56))
* **core:** Update docker compose setup for V1 images ([#6642](https://github.com/n8n-io/n8n/issues/6642)) ([05007d8](https://github.com/n8n-io/n8n/commit/05007d894e1bfa3550cfd865f85c2844b3db6eea))
* **core:** Upgrade semver to address CVE-2022-25883 ([#6689](https://github.com/n8n-io/n8n/issues/6689)) ([9daf944](https://github.com/n8n-io/n8n/commit/9daf944ba53937ddd41bd640a6d473d235f0e16f))
* **core:** Use `exec` in docker images to forward signals correctly ([#6732](https://github.com/n8n-io/n8n/issues/6732)) ([ed9f86b](https://github.com/n8n-io/n8n/commit/ed9f86bb95f7080335a336c866cd477669b02002))
* **core:** Use JWT as reset password token ([#6714](https://github.com/n8n-io/n8n/issues/6714)) ([89f4402](https://github.com/n8n-io/n8n/commit/89f44021b919181ad58c555a31071c286b866975))
* **core:** Use lower cased email for SAML email attribute ([#6663](https://github.com/n8n-io/n8n/issues/6663)) ([eedde24](https://github.com/n8n-io/n8n/commit/eedde24cc046ea517c6d6e455bcdd46a97e4c05b))
* **core:** Use owners file to export wf owners ([#6547](https://github.com/n8n-io/n8n/issues/6547)) ([4b755fb](https://github.com/n8n-io/n8n/commit/4b755fb0b441a37eb804c9e70d4b071a341f7155))
* **crowd.dev Node:** Fix documentation urls for crowd.dev credentials and nodes ([#6696](https://github.com/n8n-io/n8n/issues/6696)) ([acda7f2](https://github.com/n8n-io/n8n/commit/acda7f269f7b227d430e2308767e1676fda8e165))
* **editor:** Add default author name and email to source control settings ([#6543](https://github.com/n8n-io/n8n/issues/6543)) ([e1a02c7](https://github.com/n8n-io/n8n/commit/e1a02c76257de30e08878279dea33d7854d46938))
* **editor:** Add paywall state to non owner users for Variables ([#6679](https://github.com/n8n-io/n8n/issues/6679)) ([e7091d6](https://github.com/n8n-io/n8n/commit/e7091d6726eb98a194bc2614c0da332d348180dc))
* **editor:** Change default branchColor and remove label ([#6541](https://github.com/n8n-io/n8n/issues/6541)) ([186271e](https://github.com/n8n-io/n8n/commit/186271e939bca19ec9c94d9455e9430d8b8cf9d7))
* **editor:** Ensure default credential values are not detected as dirty state ([#6677](https://github.com/n8n-io/n8n/issues/6677)) ([c7b74c3](https://github.com/n8n-io/n8n/commit/c7b74c3c1fdd2f11b8650adf79052681c2f1e248))
* **editor:** Extend menu item and use it as a recursive component ([#6618](https://github.com/n8n-io/n8n/issues/6618)) ([d617f63](https://github.com/n8n-io/n8n/commit/d617f63ae9155c03dbf5e597db8e102c1f7a025f))
* **editor:** Hide Execute Node button for unknown nodes ([#6684](https://github.com/n8n-io/n8n/issues/6684)) ([6887b4e](https://github.com/n8n-io/n8n/commit/6887b4edeae6536f5b670c55637fde1c5dbd6e40))
* **editor:** Increase contrast ratio in execution list workflow names ([#6661](https://github.com/n8n-io/n8n/issues/6661)) ([c0b1cb2](https://github.com/n8n-io/n8n/commit/c0b1cb273e56c04abff5d9893a5e37cda6eb3383))
* **editor:** Make Source control branch select required ([#6619](https://github.com/n8n-io/n8n/issues/6619)) ([20737b5](https://github.com/n8n-io/n8n/commit/20737b532423c964bd70e0aa2aac2c9533b5c3d4))
* **editor:** Prevent keyboard shortcuts to edit workflows in readonly mode ([#6613](https://github.com/n8n-io/n8n/issues/6613)) ([7383e7f](https://github.com/n8n-io/n8n/commit/7383e7fd48b5c86d43fab4fa47cb1e7a4a4b4043))
* **editor:** Prevent RMC from loading schema if it's already cached ([#6695](https://github.com/n8n-io/n8n/issues/6695)) ([a79aa19](https://github.com/n8n-io/n8n/commit/a79aa198330808b7e45b217748fffdabb68098e2))
* **editor:** Remove global link styling in v1 banner ([#6705](https://github.com/n8n-io/n8n/issues/6705)) ([76a765a](https://github.com/n8n-io/n8n/commit/76a765a1517f53cb0c4f16a57bdd6f55bc3be0bd))
* **editor:** Show appropriate empty workflow list content when instance environment is readonly ([#6610](https://github.com/n8n-io/n8n/issues/6610)) ([7515f7d](https://github.com/n8n-io/n8n/commit/7515f7d52ae72fa1361687c43a9c29f585b3c6ce))
* **editor:** Show retry information in execution list only when it exists ([#6587](https://github.com/n8n-io/n8n/issues/6587)) ([3ca66be](https://github.com/n8n-io/n8n/commit/3ca66be38082e7a3866d53d07328be58e913067f))
* **editor:** Skip error line highlighting if out of range ([#6721](https://github.com/n8n-io/n8n/issues/6721)) ([a62d00a](https://github.com/n8n-io/n8n/commit/a62d00a4795d02a5905c5ddbae569f122a46a023))
* **editor:** Update design system menu item component ([#6659](https://github.com/n8n-io/n8n/issues/6659)) ([84466e9](https://github.com/n8n-io/n8n/commit/84466e983336a3cfa8c20b30ead8d58abbf07cf0))
* **FileMaker Node:** Improve returned error responses ([#6585](https://github.com/n8n-io/n8n/issues/6585)) ([91a052e](https://github.com/n8n-io/n8n/commit/91a052e4c53b6717d3a4e4d1034339012ce39c41))
* **FTP Node:** List recursive ignore . and .. to prevent infinite loops ([#6707](https://github.com/n8n-io/n8n/issues/6707)) ([995d5cc](https://github.com/n8n-io/n8n/commit/995d5cc47095e584c2a064dd5aa3841b3054ffd4))
* **GitLab Trigger Node:** Fix trigger activation 404 error  ([#6711](https://github.com/n8n-io/n8n/issues/6711)) ([8ceb832](https://github.com/n8n-io/n8n/commit/8ceb8322ebfc1384291e8a0d5d07ee5c22d52142))
* **Gmail Trigger Node:** Early returns in case of no data ([#6727](https://github.com/n8n-io/n8n/issues/6727)) ([c2511a8](https://github.com/n8n-io/n8n/commit/c2511a829cfa40d4d9d570ad7724845c93544c3b))
* **Google BigQuery Node:** Error description improvement ([#6715](https://github.com/n8n-io/n8n/issues/6715)) ([95837d2](https://github.com/n8n-io/n8n/commit/95837d260466e8a4bd19c44390ce4557fa5c51cb))
* **Google Drive Node:** Fix regex in file RLC ([#6607](https://github.com/n8n-io/n8n/issues/6607)) ([5672146](https://github.com/n8n-io/n8n/commit/56721468dff51bb60ececc0472e2b9ca0740fcb1))
* **Google Drive Node:** URL parsing ([#6527](https://github.com/n8n-io/n8n/issues/6527)) ([d9ed0b3](https://github.com/n8n-io/n8n/commit/d9ed0b31b538320a67ee4e5c0cae34656c9f4334))
* **Google Sheets Node:** Incorrect read of 0 and false ([#6525](https://github.com/n8n-io/n8n/issues/6525)) ([806d134](https://github.com/n8n-io/n8n/commit/806d13460240abe94843e569b1820cd8d0d8edd1))
* **HTTP Request Node:** Cleanup circular references in response ([#6590](https://github.com/n8n-io/n8n/issues/6590)) ([aecc05b](https://github.com/n8n-io/n8n/commit/aecc05b787d09ba778adc5b4bf96abacc5a64204))
* **Merge Node:** Enrich input 2 fix ([#6526](https://github.com/n8n-io/n8n/issues/6526)) ([c82c7f1](https://github.com/n8n-io/n8n/commit/c82c7f19128df3a11d6d0f18e8d8dab57e6a3b8f))
* **Microsoft Outlook Node:** Fix issue with category not correctly applying ([#6583](https://github.com/n8n-io/n8n/issues/6583)) ([fc8ed55](https://github.com/n8n-io/n8n/commit/fc8ed55c0de7db4cf17f4f1bf417f6cbf48444c2))
* **Notion Node:** Version fix ([#6531](https://github.com/n8n-io/n8n/issues/6531)) ([38dc784](https://github.com/n8n-io/n8n/commit/38dc784d2eed25aae777c5c3c3fda1a35e20bd24))
* **Postgres Node:** Arrays in query replacement fix ([#6718](https://github.com/n8n-io/n8n/issues/6718)) ([4cae091](https://github.com/n8n-io/n8n/commit/4cae091cfb54701dfa51b5204799df0a8b4929cd))
* **Postgres Node:** For select queries, empty result should be be replaced with `{"success":true}` ([#6703](https://github.com/n8n-io/n8n/issues/6703)) ([250175d](https://github.com/n8n-io/n8n/commit/250175d066d6759f4a787371b47ed91ee62aab71))
* **Postgres Node:** Upsert does not fetch columns when schema other then public ([#6643](https://github.com/n8n-io/n8n/issues/6643)) ([aaa9ee3](https://github.com/n8n-io/n8n/commit/aaa9ee3949529a745e3b624716da1549ed571604))
* **Salesforce Node:** Fix typo for adding a contact to a campaign ([#6598](https://github.com/n8n-io/n8n/issues/6598)) ([7ffe3cb](https://github.com/n8n-io/n8n/commit/7ffe3cb36adeecaca6cc6ddf067a701ee55c18d1))
* **Sendy Node:** Fix issue with brand id not being sent ([#6530](https://github.com/n8n-io/n8n/issues/6530)) ([2e8dfb8](https://github.com/n8n-io/n8n/commit/2e8dfb86d4636781b319d6190e8be12e7661ee16))
* Stop n8n from complaining about credentials when saving a new workflow form a template ([#6671](https://github.com/n8n-io/n8n/issues/6671)) ([486d16b](https://github.com/n8n-io/n8n/commit/486d16bcdb6be12dd85f4af5f7de878d9d178fd6))
* **Strapi Node:** Fix issue with pagination ([#4991](https://github.com/n8n-io/n8n/issues/4991)) ([54444fa](https://github.com/n8n-io/n8n/commit/54444fa388da12d75553e66e53a8cf6f8a99b6fc))
* **Telegram Trigger Node:** Add guard to 'include' call on null or undefined ([#6730](https://github.com/n8n-io/n8n/issues/6730)) ([533b0ba](https://github.com/n8n-io/n8n/commit/533b0bac13d275753fee329bb4abe0c7aae5b48b))
* **XML Node:** Fix issue with not returning valid data ([#6565](https://github.com/n8n-io/n8n/issues/6565)) ([cdd215f](https://github.com/n8n-io/n8n/commit/cdd215f642b47413c05f229e641074d0d4048f68))


### Features

* Add crowd.dev node and trigger node ([#6082](https://github.com/n8n-io/n8n/issues/6082)) ([238a78f](https://github.com/n8n-io/n8n/commit/238a78f0582dbf439a9799de0edcb2e9bef29978))
* Add missing input panels to some trigger nodes ([#6518](https://github.com/n8n-io/n8n/issues/6518)) ([fdf8a42](https://github.com/n8n-io/n8n/commit/fdf8a428ed38bb3ceb2bc0e50b002b34843d8fc4))
* Add various source control improvements ([#6533](https://github.com/n8n-io/n8n/issues/6533)) ([68fdc20](https://github.com/n8n-io/n8n/commit/68fdc2078928be478a286774f2889feba1c3f5fe))
* **Airtable Node:** Overhaul ([#6200](https://github.com/n8n-io/n8n/issues/6200)) ([b69d20c](https://github.com/n8n-io/n8n/commit/b69d20c12ec1ad0395e23747ce5f1d437de0231b))
* Allow `eslint-config` to be externally consumable ([#6694](https://github.com/n8n-io/n8n/issues/6694)) ([3566c13](https://github.com/n8n-io/n8n/commit/3566c13afc9795206b5a4af7b06159e35b046e12))
* Allow hiding credential params on cloud ([#6687](https://github.com/n8n-io/n8n/issues/6687)) ([2af1c24](https://github.com/n8n-io/n8n/commit/2af1c24ead4c02e0588d4c2dfcf4a289f54388d4))
* **API:** Implement users account quota guards  ([#6434](https://github.com/n8n-io/n8n/issues/6434)) ([e5620ab](https://github.com/n8n-io/n8n/commit/e5620ab1e49548e4c2ffd296e055f1caee94d2ba)), closes [#6636](https://github.com/n8n-io/n8n/issues/6636)
* **core:** Add cache service ([#6729](https://github.com/n8n-io/n8n/issues/6729)) ([c0d2bac](https://github.com/n8n-io/n8n/commit/c0d2bac94d732d4166633adf9c3b8eaf5d8046be))
* **core:** Only show V1 banner to users who migrated ([#6622](https://github.com/n8n-io/n8n/issues/6622)) ([071e56f](https://github.com/n8n-io/n8n/commit/071e56f7fde2fc4ffc7e3da92a069d8ed593bc60))
* **editor:** Implement new banners framework ([#6603](https://github.com/n8n-io/n8n/issues/6603)) ([4240e76](https://github.com/n8n-io/n8n/commit/4240e76253e02da13942d4b84a83ec22fd30aca3))
* **editor:** Load fixed template list as experiment ([#6632](https://github.com/n8n-io/n8n/issues/6632)) ([e996622](https://github.com/n8n-io/n8n/commit/e9966224ea555ce8f3a48872887a73ef879e47c3))
* **editor:** Prevent saving of workflow when canvas is loading ([#6497](https://github.com/n8n-io/n8n/issues/6497)) ([f89ef83](https://github.com/n8n-io/n8n/commit/f89ef83c766fafb1d0497ed91a74b93e8d2af1ec))
* **editor:** Removing `ph-no-capture` class from some elements ([#6674](https://github.com/n8n-io/n8n/issues/6674)) ([c3455a4](https://github.com/n8n-io/n8n/commit/c3455a4ad82d965c41267fea173feaad4800c43f))
* Environments release using source control ([#6653](https://github.com/n8n-io/n8n/issues/6653)) ([fc7aa8b](https://github.com/n8n-io/n8n/commit/fc7aa8bd664553c463536b6abe58a488e5e11147))
* **Google Cloud Storage Node:** Use streaming for file uploads ([#6462](https://github.com/n8n-io/n8n/issues/6462)) ([cd0e41a](https://github.com/n8n-io/n8n/commit/cd0e41a6b49a58bee95721363dd7e6c43de28725))
* **Google Drive Node:** Overhaul ([#5941](https://github.com/n8n-io/n8n/issues/5941)) ([d70a1cb](https://github.com/n8n-io/n8n/commit/d70a1cb0c82ee0a4b92776684c6c9079020d028f))
* **HTML Node:** 'Convert to table operation ([#6540](https://github.com/n8n-io/n8n/issues/6540)) ([8abb03d](https://github.com/n8n-io/n8n/commit/8abb03d7cf02ad7f03a0adffa646870df5f1a02c))
* **HTTP Request Node:** New http request generic custom auth credential ([#5798](https://github.com/n8n-io/n8n/issues/5798)) ([b17b458](https://github.com/n8n-io/n8n/commit/b17b4582a059104665888a2369c3e2256db4c1ed))
* **Matrix Node:** Allow setting filename if the binary data has none ([#6536](https://github.com/n8n-io/n8n/issues/6536)) ([8b76e98](https://github.com/n8n-io/n8n/commit/8b76e980852062b192a95593035697c43d6f808e))
* **Microsoft To Do Node:** Add an option to set a reminder when creating a task ([#5757](https://github.com/n8n-io/n8n/issues/5757)) ([b19833d](https://github.com/n8n-io/n8n/commit/b19833d673bd554ba86c0b234e8d13633912563a))
* **Notion Node:** Add option to update icon when updating a page ([#5670](https://github.com/n8n-io/n8n/issues/5670)) ([225e849](https://github.com/n8n-io/n8n/commit/225e849960ce65d7f85b482f05fb3d7ffb4f9427))
* **OpenAI Node:** Update max token limit to support newer model limits ([#6644](https://github.com/n8n-io/n8n/issues/6644)) ([26046f6](https://github.com/n8n-io/n8n/commit/26046f6fe8df9e6fe799f6253d086142f6ce7e53))
* **Read PDF Node:** Replace pdf-parse with pdfjs, and add support for streaming and encrypted PDFs ([#6640](https://github.com/n8n-io/n8n/issues/6640)) ([0a31b8e](https://github.com/n8n-io/n8n/commit/0a31b8e2b4aab8d74d80f76598900109fe19a0e8))
* **Rundeck Node:** Add support for node filters  ([#5633](https://github.com/n8n-io/n8n/issues/5633)) ([1f70f49](https://github.com/n8n-io/n8n/commit/1f70f49ce5784baba7fd779b23209bae4f6b039a))
* **Slack Node:** Add option to include link to workflow in Slack node ([#6611](https://github.com/n8n-io/n8n/issues/6611)) ([aa53c46](https://github.com/n8n-io/n8n/commit/aa53c46367480e31642e807ad1abf149fd13eb28))
* **Strava Node:** Add hide_from_home field in Activity Update ([#5883](https://github.com/n8n-io/n8n/issues/5883)) ([7495e31](https://github.com/n8n-io/n8n/commit/7495e31a5b25e97683c7ea38225ba253d8fae8b7))
* **Telegram Node:** Add support for sending messages to forum topics ([#5746](https://github.com/n8n-io/n8n/issues/5746)) ([e6a81f0](https://github.com/n8n-io/n8n/commit/e6a81f0008fddfcfd5f1102c8e6e58650020d930))
* **Twitter Node:** Node overhaul ([#4788](https://github.com/n8n-io/n8n/issues/4788)) ([42721db](https://github.com/n8n-io/n8n/commit/42721dba80077fb796086a2bf0ecce256bf3a50f))


### Reverts

* Revert "test(editor): Add canvas actions E2E tests" (#6736) ([ed09e9c](https://github.com/n8n-io/n8n/commit/ed09e9c695109a715a4c8d47338bbb0b794eb009)), closes [#6736](https://github.com/n8n-io/n8n/issues/6736) [#6723](https://github.com/n8n-io/n8n/issues/6723)



## [1.0.1](https://github.com/n8n-io/n8n/compare/n8n@1.0.0...n8n@1.0.1) (2023-07-05)


### Bug Fixes

* **core:** Fix credentials test ([#6569](https://github.com/n8n-io/n8n/issues/6569)) ([8f244df](https://github.com/n8n-io/n8n/commit/8f244df0f9efcb087a78dd8d9481489c484c77b7))
* **core:** Fix migrations for MySQL/MariaDB ([#6591](https://github.com/n8n-io/n8n/issues/6591)) ([b9da67b](https://github.com/n8n-io/n8n/commit/b9da67b653bf19f39d0d1506d3140c71432efaed))
* **core:** Make node execution order configurable, and backward-compatible ([#6507](https://github.com/n8n-io/n8n/issues/6507)) ([d97edbc](https://github.com/n8n-io/n8n/commit/d97edbcffa966a693548eed033ac41d4a404fc23))
* **core:** Update pruning related config defaults for v1 ([#6577](https://github.com/n8n-io/n8n/issues/6577)) ([ffb4e47](https://github.com/n8n-io/n8n/commit/ffb4e470b56222ae11891d478e96ea9c31675afe))
* **editor:** Restore expression completions ([#6566](https://github.com/n8n-io/n8n/issues/6566)) ([516e572](https://github.com/n8n-io/n8n/commit/516e5728f73da6393defe7633533cc142c531c7a))
* **editor:** Show retry information in execution list only when it exists ([#6587](https://github.com/n8n-io/n8n/issues/6587)) ([2580286](https://github.com/n8n-io/n8n/commit/2580286a198e53c3bf3db6e56faed301b606db07))
* **Sendy Node:** Fix issue with brand id not being sent ([#6530](https://github.com/n8n-io/n8n/issues/6530)) ([b9e5211](https://github.com/n8n-io/n8n/commit/b9e52117355d939e77a2e3c59a7f67ac21e31b22))
* **Strapi Node:** Fix issue with pagination ([#4991](https://github.com/n8n-io/n8n/issues/4991)) ([4253b48](https://github.com/n8n-io/n8n/commit/4253b48b26d1625cd2fb7f38159f9528cea45f34))
* **XML Node:** Fix issue with not returning valid data ([#6565](https://github.com/n8n-io/n8n/issues/6565)) ([c2b9d5a](https://github.com/n8n-io/n8n/commit/c2b9d5ac506375ecc316e8c79a3ce0bf143e9406))


### Features

* Add missing input panels to some trigger nodes ([#6518](https://github.com/n8n-io/n8n/issues/6518)) ([3b12864](https://github.com/n8n-io/n8n/commit/3b12864460a458f23b57a6f3f4b40d0d364ef6e6))



# [1.0.0](https://github.com/n8n-io/n8n/compare/n8n@0.234.0...n8n@1.0.0) (2023-06-27)


### ⚠️ BREAKING CHANGES
* **core** Docker containers now run as the user `node` instead of `root` ([#6365](https://github.com/n8n-io/n8n/pull/6365)) ([f636616](https://github.com/n8n-io/n8n/commit/f6366160a476f42cb0612d10c5777a154d8665dd))
* **core** Drop `debian` and `rhel7` images ([#6365](https://github.com/n8n-io/n8n/pull/6365)) ([f636616](https://github.com/n8n-io/n8n/commit/f6366160a476f42cb0612d10c5777a154d8665dd))
* **core** Drop support for deprecated `WEBHOOK_TUNNEL_URL` env variable ([#6363](https://github.com/n8n-io/n8n/pull/6363))
* **core** Execution mode defaults to `main` now, instead of `own` ([#6363](https://github.com/n8n-io/n8n/pull/6363))
* **core** Default push backend is `websocket` now, instead of `sse` ([#6363](https://github.com/n8n-io/n8n/pull/6363))
* **core** Stop loading custom/community nodes from n8n's `node_modules` folder ([#6396](https://github.com/n8n-io/n8n/pull/6396)) ([a45a2c8](https://github.com/n8n-io/n8n/commit/a45a2c8c41eb7ffb2d62d5a8877c34eb45799fa9))
* **core** User management is mandatory now. basic-auth, external-jwt-auth, and no-auth options are removed ([#6362](https://github.com/n8n-io/n8n/pull/6362)) ([8c008f5](https://github.com/n8n-io/n8n/commit/8c008f5d2217030e93d79e2baca0f2965d4d643e))
* **core** Allow syntax errors and expression errors to fail executions ([#6352](https://github.com/n8n-io/n8n/pull/6352)) ([1197811](https://github.com/n8n-io/n8n/commit/1197811a1e3bc4ad7464d53d7e4860d0e62335a3))
* **core** Drop support for `request` library and `N8N_USE_DEPRECATED_REQUEST_LIB` env variable ([#6413](https://github.com/n8n-io/n8n/pull/6413)) ([632ea27](https://github.com/n8n-io/n8n/commit/632ea275b7fa352d4af23339208bed66bb948da8))
* **core** Make date extensions outputs match inputs ([#6435](https://github.com/n8n-io/n8n/pull/6435)) ([85372aa](https://github.com/n8n-io/n8n/commit/85372aabdfc52493504d4723ee1829e2ea15151d))
* **core** Drop support for `executeSingle` method on nodes ([#4853](https://github.com/n8n-io/n8n/pull/4853)) ([9194d8b](https://github.com/n8n-io/n8n/commit/9194d8bb0ecf81e52d47ddfc4b75dc4e0efd492d))
* **core** Change data processing for multi-input-nodes ([#4238](https://github.com/n8n-io/n8n/pull/4238)) ([b8458a5](https://github.com/n8n-io/n8n/commit/b8458a53f66b79903f0fdb168f6febdefb36d13a))


### Bug Fixes

* **core:** All migrations should run in a transaction ([#6519](https://github.com/n8n-io/n8n/issues/6519)) ([e152cfe](https://github.com/n8n-io/n8n/commit/e152cfe27cf3396f4b278614f1d46d9dd723f36e))
* **Edit Image Node:** Fix transparent operation ([#6513](https://github.com/n8n-io/n8n/issues/6513)) ([4a4bcbc](https://github.com/n8n-io/n8n/commit/4a4bcbca298bf90c54d3597103e6a231855abbd2))
* **Google Drive Node:** URL parsing ([#6527](https://github.com/n8n-io/n8n/issues/6527)) ([18aa9f3](https://github.com/n8n-io/n8n/commit/18aa9f3c62149cd603c560c2944c3146cd31e9e7))
* **Google Sheets Node:** Incorrect read of 0 and false ([#6525](https://github.com/n8n-io/n8n/issues/6525)) ([b6202b5](https://github.com/n8n-io/n8n/commit/b6202b5585f864d97dc114e1e49a6a7dae5c674a))
* **Merge Node:** Enrich input 2 fix ([#6526](https://github.com/n8n-io/n8n/issues/6526)) ([70822ce](https://github.com/n8n-io/n8n/commit/70822ce988543476719089c132e1d10af0d03e78))
* **Notion Node:** Version fix ([#6531](https://github.com/n8n-io/n8n/issues/6531)) ([d3d8522](https://github.com/n8n-io/n8n/commit/d3d8522e8f0c702f56997667a252892296540450))
* Show error when referencing node that exist but has not been executed ([#6496](https://github.com/n8n-io/n8n/issues/6496)) ([3db2707](https://github.com/n8n-io/n8n/commit/3db2707b8e47ea539f4f6c40497a928b51b40274))


### Features

* **core:** Change node execution order (most top-left one first) ([#6246](https://github.com/n8n-io/n8n/issues/6246)) ([0287d5b](https://github.com/n8n-io/n8n/commit/0287d5becdce30a9c0de2a0d6ad4a0db50e198d7))
* **core:** Remove conditional defaults in V1 release ([#6363](https://github.com/n8n-io/n8n/issues/6363)) ([f636616](https://github.com/n8n-io/n8n/commit/f6366160a476f42cb0612d10c5777a154d8665dd))
* **editor:** Add v1 banner ([#6443](https://github.com/n8n-io/n8n/issues/6443)) ([0fe415a](https://github.com/n8n-io/n8n/commit/0fe415add2baa8e70e29087f7a90312bd1ab38af))
* **editor:** SQL editor overhaul ([#6282](https://github.com/n8n-io/n8n/issues/6282)) ([beedfb6](https://github.com/n8n-io/n8n/commit/beedfb609ccde2ef202e08566580a2e1a6b6eafa))
* **HTTP Request Node:** Notice about dev console ([#6516](https://github.com/n8n-io/n8n/issues/6516)) ([d431117](https://github.com/n8n-io/n8n/commit/d431117c9e5db9ff0ec6a1e7371bbf58698957c9))



# [0.236.0](https://github.com/n8n-io/n8n/compare/n8n@0.235.0...n8n@0.236.0) (2023-07-05)


### Bug Fixes

* **Brevo Node:** Rename SendInBlue node to Brevo node ([#6521](https://github.com/n8n-io/n8n/issues/6521)) ([e63b398](https://github.com/n8n-io/n8n/commit/e63b3982d200ade34461b9159eb1e988f494c025))
* **core:** Fix credentials test ([#6569](https://github.com/n8n-io/n8n/issues/6569)) ([1abd172](https://github.com/n8n-io/n8n/commit/1abd172f73e171e37c4cc3ccfaa395c6a46bdf48))
* **core:** Fix migrations for MySQL/MariaDB ([#6591](https://github.com/n8n-io/n8n/issues/6591)) ([29882a6](https://github.com/n8n-io/n8n/commit/29882a6f39dddcd1c8c107c20a548ce8dc665cba))
* **core:** Improve the performance of last 2 sqlite migrations ([#6522](https://github.com/n8n-io/n8n/issues/6522)) ([31cba87](https://github.com/n8n-io/n8n/commit/31cba87d307183d613890c7e6d627636b5280b52))
* **core:** Remove typeorm patches, but still enforce transactions on every migration ([#6594](https://github.com/n8n-io/n8n/issues/6594)) ([9def7a7](https://github.com/n8n-io/n8n/commit/9def7a729b52cd6b4698c47e190e9e2bd7894da5)), closes [#6519](https://github.com/n8n-io/n8n/issues/6519)
* **core:** Use owners file to export wf owners ([#6547](https://github.com/n8n-io/n8n/issues/6547)) ([4b755fb](https://github.com/n8n-io/n8n/commit/4b755fb0b441a37eb804c9e70d4b071a341f7155))
* **editor:** Show retry information in execution list only when it exists ([#6587](https://github.com/n8n-io/n8n/issues/6587)) ([3ca66be](https://github.com/n8n-io/n8n/commit/3ca66be38082e7a3866d53d07328be58e913067f))
* **Salesforce Node:** Fix typo for adding a contact to a campaign ([#6598](https://github.com/n8n-io/n8n/issues/6598)) ([7ffe3cb](https://github.com/n8n-io/n8n/commit/7ffe3cb36adeecaca6cc6ddf067a701ee55c18d1))
* **Strapi Node:** Fix issue with pagination ([#4991](https://github.com/n8n-io/n8n/issues/4991)) ([54444fa](https://github.com/n8n-io/n8n/commit/54444fa388da12d75553e66e53a8cf6f8a99b6fc))
* **XML Node:** Fix issue with not returning valid data ([#6565](https://github.com/n8n-io/n8n/issues/6565)) ([cdd215f](https://github.com/n8n-io/n8n/commit/cdd215f642b47413c05f229e641074d0d4048f68))


### Features

* Add crowd.dev node and trigger node ([#6082](https://github.com/n8n-io/n8n/issues/6082)) ([238a78f](https://github.com/n8n-io/n8n/commit/238a78f0582dbf439a9799de0edcb2e9bef29978))
* Add various source control improvements ([#6533](https://github.com/n8n-io/n8n/issues/6533)) ([68fdc20](https://github.com/n8n-io/n8n/commit/68fdc2078928be478a286774f2889feba1c3f5fe))
* **HTTP Request Node:** New http request generic custom auth credential ([#5798](https://github.com/n8n-io/n8n/issues/5798)) ([b17b458](https://github.com/n8n-io/n8n/commit/b17b4582a059104665888a2369c3e2256db4c1ed))
* **Microsoft To Do Node:** Add an option to set a reminder when creating a task ([#5757](https://github.com/n8n-io/n8n/issues/5757)) ([b19833d](https://github.com/n8n-io/n8n/commit/b19833d673bd554ba86c0b234e8d13633912563a))
* **Notion Node:** Add option to update icon when updating a page ([#5670](https://github.com/n8n-io/n8n/issues/5670)) ([225e849](https://github.com/n8n-io/n8n/commit/225e849960ce65d7f85b482f05fb3d7ffb4f9427))
* **Strava Node:** Add hide_from_home field in Activity Update ([#5883](https://github.com/n8n-io/n8n/issues/5883)) ([7495e31](https://github.com/n8n-io/n8n/commit/7495e31a5b25e97683c7ea38225ba253d8fae8b7))
* **Twitter Node:** Node overhaul ([#4788](https://github.com/n8n-io/n8n/issues/4788)) ([42721db](https://github.com/n8n-io/n8n/commit/42721dba80077fb796086a2bf0ecce256bf3a50f))



# [0.235.0](https://github.com/n8n-io/n8n/compare/n8n@0.234.0...n8n@0.235.0) (2023-06-28)


### Bug Fixes

* **core:** Add empty credential value marker to show empty pw field ([#6532](https://github.com/n8n-io/n8n/issues/6532)) ([9294e2d](https://github.com/n8n-io/n8n/commit/9294e2da3c7c99c2099f5865e610fa7217bf06be))
* **core:** All migrations should run in a transaction ([#6519](https://github.com/n8n-io/n8n/issues/6519)) ([e152cfe](https://github.com/n8n-io/n8n/commit/e152cfe27cf3396f4b278614f1d46d9dd723f36e))
* **core:** Rename to credential_stubs and variable_stubs.json ([#6528](https://github.com/n8n-io/n8n/issues/6528)) ([b06462f](https://github.com/n8n-io/n8n/commit/b06462f4415bd1143a00b4a66e6e626da8c52196))
* **Edit Image Node:** Fix transparent operation ([#6513](https://github.com/n8n-io/n8n/issues/6513)) ([4a4bcbc](https://github.com/n8n-io/n8n/commit/4a4bcbca298bf90c54d3597103e6a231855abbd2))
* **editor:** Add default author name and email to source control settings ([#6543](https://github.com/n8n-io/n8n/issues/6543)) ([e1a02c7](https://github.com/n8n-io/n8n/commit/e1a02c76257de30e08878279dea33d7854d46938))
* **editor:** Change default branchColor and remove label ([#6541](https://github.com/n8n-io/n8n/issues/6541)) ([186271e](https://github.com/n8n-io/n8n/commit/186271e939bca19ec9c94d9455e9430d8b8cf9d7))
* **Google Drive Node:** URL parsing ([#6527](https://github.com/n8n-io/n8n/issues/6527)) ([d9ed0b3](https://github.com/n8n-io/n8n/commit/d9ed0b31b538320a67ee4e5c0cae34656c9f4334))
* **Google Sheets Node:** Incorrect read of 0 and false ([#6525](https://github.com/n8n-io/n8n/issues/6525)) ([806d134](https://github.com/n8n-io/n8n/commit/806d13460240abe94843e569b1820cd8d0d8edd1))
* **Merge Node:** Enrich input 2 fix ([#6526](https://github.com/n8n-io/n8n/issues/6526)) ([c82c7f1](https://github.com/n8n-io/n8n/commit/c82c7f19128df3a11d6d0f18e8d8dab57e6a3b8f))
* **Notion Node:** Version fix ([#6531](https://github.com/n8n-io/n8n/issues/6531)) ([38dc784](https://github.com/n8n-io/n8n/commit/38dc784d2eed25aae777c5c3c3fda1a35e20bd24))
* **Sendy Node:** Fix issue with brand id not being sent ([#6530](https://github.com/n8n-io/n8n/issues/6530)) ([2e8dfb8](https://github.com/n8n-io/n8n/commit/2e8dfb86d4636781b319d6190e8be12e7661ee16))


### Features

* Add missing input panels to some trigger nodes ([#6518](https://github.com/n8n-io/n8n/issues/6518)) ([fdf8a42](https://github.com/n8n-io/n8n/commit/fdf8a428ed38bb3ceb2bc0e50b002b34843d8fc4))
* **editor:** Prevent saving of workflow when canvas is loading ([#6497](https://github.com/n8n-io/n8n/issues/6497)) ([f89ef83](https://github.com/n8n-io/n8n/commit/f89ef83c766fafb1d0497ed91a74b93e8d2af1ec))
* **editor:** SQL editor overhaul ([#6282](https://github.com/n8n-io/n8n/issues/6282)) ([beedfb6](https://github.com/n8n-io/n8n/commit/beedfb609ccde2ef202e08566580a2e1a6b6eafa))
* **Google Drive Node:** Overhaul ([#5941](https://github.com/n8n-io/n8n/issues/5941)) ([d70a1cb](https://github.com/n8n-io/n8n/commit/d70a1cb0c82ee0a4b92776684c6c9079020d028f))
* **HTTP Request Node:** Notice about dev console ([#6516](https://github.com/n8n-io/n8n/issues/6516)) ([d431117](https://github.com/n8n-io/n8n/commit/d431117c9e5db9ff0ec6a1e7371bbf58698957c9))
* **Matrix Node:** Allow setting filename if the binary data has none ([#6536](https://github.com/n8n-io/n8n/issues/6536)) ([8b76e98](https://github.com/n8n-io/n8n/commit/8b76e980852062b192a95593035697c43d6f808e))



# [0.234.0](https://github.com/n8n-io/n8n/compare/n8n@0.233.0...n8n@0.234.0) (2023-06-22)


### Bug Fixes

* **core:** Fix OAuth2 callback for `grantType=clientCredentials` ([#6500](https://github.com/n8n-io/n8n/issues/6500)) ([25b9216](https://github.com/n8n-io/n8n/commit/25b92169aefc47dc028a11dc008abb4a36d037d3))
* **core:** Fix pairedItem for alwaysOutputData & multi identical resolve ([#6405](https://github.com/n8n-io/n8n/issues/6405)) ([4b0e0b7](https://github.com/n8n-io/n8n/commit/4b0e0b797071cb20bd2b042eb0d8591fe801ae76))
* **core:** Fix the url sent in the password-reset emails ([#6466](https://github.com/n8n-io/n8n/issues/6466)) ([9978e27](https://github.com/n8n-io/n8n/commit/9978e2760bc0b8f8c7e5c1ef6610670611d8efe9))
* **core:** Improve the error returned to users on SSL issues ([#6494](https://github.com/n8n-io/n8n/issues/6494)) ([1b084bc](https://github.com/n8n-io/n8n/commit/1b084bc56b90a25b399c084b69efdb48ff01dfb5))
* **core:** Use correct scopes-separator when generating authorization urls ([#6502](https://github.com/n8n-io/n8n/issues/6502)) ([5bf83f8](https://github.com/n8n-io/n8n/commit/5bf83f8bf6889e0154000ad774f292e98b87729d))
* **editor:** Fix DNV header disappearing when scrolling the code editor content ([#6459](https://github.com/n8n-io/n8n/issues/6459)) ([ad9fd12](https://github.com/n8n-io/n8n/commit/ad9fd12615a7050c6fec0caf041e49c972693d1f))
* **editor:** Fix resource mapper dropdown width and disabled styling ([#6493](https://github.com/n8n-io/n8n/issues/6493)) ([da330f0](https://github.com/n8n-io/n8n/commit/da330f0648b85c39e89ca2eeaba94f9b2c3a1b13))
* **editor:** Remove `$if`, `$min` and `$max` from code node autocomplete ([#6460](https://github.com/n8n-io/n8n/issues/6460)) ([16f707d](https://github.com/n8n-io/n8n/commit/16f707d5c479c72f87c129ec870fd00c329a9ade))
* **editor:** Show confirm on pull only when http response status is 409 ([#6451](https://github.com/n8n-io/n8n/issues/6451)) ([5819be5](https://github.com/n8n-io/n8n/commit/5819be5ced53adc643b2bb18dbd1be0096a05395))
* **editor:** Show execution error as message ([#6431](https://github.com/n8n-io/n8n/issues/6431)) ([d3b78e2](https://github.com/n8n-io/n8n/commit/d3b78e291ece5355b0829c935a3142b6078287c9))
* **editor:** Update data pinning tooltip to match current behaviour ([#6436](https://github.com/n8n-io/n8n/issues/6436)) ([ee10ac8](https://github.com/n8n-io/n8n/commit/ee10ac8da9ad6533995361f51cab97da35501855))
* **editor:** Update git repo URL validation to prevent using https protocol ([#6475](https://github.com/n8n-io/n8n/issues/6475)) ([8b50625](https://github.com/n8n-io/n8n/commit/8b50625fb15fc86840485e167627a2ab1802d512))
* **editor:** Update version control docs links ([#6440](https://github.com/n8n-io/n8n/issues/6440)) ([da105f4](https://github.com/n8n-io/n8n/commit/da105f468bd69b3d572f422d7270204e5823200e))
* **Google Sheets Node:** Return empty response if no rows updated ([#6407](https://github.com/n8n-io/n8n/issues/6407)) ([32fb419](https://github.com/n8n-io/n8n/commit/32fb4190111c60c8bd05d47d5bace2f9043d1f06))
* **HTML Node:** Prevent XSS in execution-data preview ([#6432](https://github.com/n8n-io/n8n/issues/6432)) ([16e0df5](https://github.com/n8n-io/n8n/commit/16e0df553c4e068768bf7dd7bbac1d7c2b88fec2))
* **HTTP Request Node:** "Ignore SSL issues" should also ignore legacy renegotiation issues ([#6492](https://github.com/n8n-io/n8n/issues/6492)) ([7a95e08](https://github.com/n8n-io/n8n/commit/7a95e08bfd04cd53a9d531fdb715f289bfdd64b6))
* **LinkedIn Node:** Remove unsupported description from image posts ([#6446](https://github.com/n8n-io/n8n/issues/6446)) ([529f0e4](https://github.com/n8n-io/n8n/commit/529f0e499670450f8cb0dda539176d1b07c39190))
* Make MySQL migration for nano id change compatible with version 5.7 ([#6498](https://github.com/n8n-io/n8n/issues/6498)) ([044c710](https://github.com/n8n-io/n8n/commit/044c710a8ecca3d705ebfb53cef204482428fbec))
* **Split In Batches Node:** Add "done" context to allow simple reset ([#6437](https://github.com/n8n-io/n8n/issues/6437)) ([ffd13f4](https://github.com/n8n-io/n8n/commit/ffd13f4541794832792ecf33e24d5dc4960ff005))
* **Zendesk Node:** Fix issue with group assignment not working ([#6501](https://github.com/n8n-io/n8n/issues/6501)) ([772ed7f](https://github.com/n8n-io/n8n/commit/772ed7ff10f6071816ad8cb4543ae9bcaf3813d3))
* **Zulip Node:** Remove trailing slash from the url ([#6427](https://github.com/n8n-io/n8n/issues/6427)) ([cc1b249](https://github.com/n8n-io/n8n/commit/cc1b249d58618c11bb22ae4458aaf22ef77e6493))


### Features

* Add support for large files with declarative nodes ([#6461](https://github.com/n8n-io/n8n/issues/6461)) ([e0f109f](https://github.com/n8n-io/n8n/commit/e0f109fa7ee3b1502d68f648504e12a61bff7c93))
* **AwsS3 Node:** Small overhaul of the node with multipart uploading ([#6017](https://github.com/n8n-io/n8n/issues/6017)) ([109442f](https://github.com/n8n-io/n8n/commit/109442f38f9868d51d85ba4f88d185910f4f2688))
* **core:** Add GET /users endpoints to public API ([#6360](https://github.com/n8n-io/n8n/issues/6360)) ([6ab3502](https://github.com/n8n-io/n8n/commit/6ab350209d0fa7ee37c9e4425d987517aeba3d98))
* **core:** Add PKCE for OAuth2 ([#6324](https://github.com/n8n-io/n8n/issues/6324)) ([fc7261a](https://github.com/n8n-io/n8n/commit/fc7261aca6485141fca95b6eccffe1f1a9a8c0c4))
* **DebugHelper Node:** Fix and include in main app ([#6406](https://github.com/n8n-io/n8n/issues/6406)) ([18f5884](https://github.com/n8n-io/n8n/commit/18f588444f7f126ec1c4867d2ac1f2d3cbc99b88))
* **Gmail Node:** Add reply to email ([#6453](https://github.com/n8n-io/n8n/issues/6453)) ([fddc69e](https://github.com/n8n-io/n8n/commit/fddc69ee2c2324aff783172c959af9e40ad89696))
* **Item Lists Node:** Improvements ([#6190](https://github.com/n8n-io/n8n/issues/6190)) ([1dbca44](https://github.com/n8n-io/n8n/commit/1dbca4402579ce1e323ab30c5caebef247a19c8d))
* Migrate integer primary keys to nanoids ([#6345](https://github.com/n8n-io/n8n/issues/6345)) ([c3ba012](https://github.com/n8n-io/n8n/commit/c3ba0123ad0913140707dbf56fafa1d4dd0f3de3)), closes [#6323](https://github.com/n8n-io/n8n/issues/6323)
* **Stripe Trigger Node:** Add action required trigger for payment intents ([#6490](https://github.com/n8n-io/n8n/issues/6490)) ([f2154fb](https://github.com/n8n-io/n8n/commit/f2154fba60cbbaa9b6c9e72523801573fe3b6baf))
* **Webhook Node:** Stream binary response in `lastNode.firstEntryBinary` mode ([#6463](https://github.com/n8n-io/n8n/issues/6463)) ([6ccab3e](https://github.com/n8n-io/n8n/commit/6ccab3eaaa883e17d00607e180e14edf9ce33688))



# [0.233.0](https://github.com/n8n-io/n8n/compare/n8n@0.232.0...n8n@0.233.0) (2023-06-14)


### Bug Fixes

* **core:** Allow all executions to be stopped ([#6386](https://github.com/n8n-io/n8n/issues/6386)) ([cc44af9](https://github.com/n8n-io/n8n/commit/cc44af9243457a5dfa904c205ad5428f793104b4))
* **core:** Prevent arbitrary code execution via expressions ([#6420](https://github.com/n8n-io/n8n/issues/6420)) ([da7ae2b](https://github.com/n8n-io/n8n/commit/da7ae2beef0375aa914aee251aeff5f7ff334b34))
* **editor:** Hide version control main menu component if no feature flag ([#6419](https://github.com/n8n-io/n8n/issues/6419)) ([75c0ab0](https://github.com/n8n-io/n8n/commit/75c0ab03f8379bb5426cef87045b67b458c97d70))
* **LinkedIn Node:** Fix issue with posting as user or organization ([#6414](https://github.com/n8n-io/n8n/issues/6414)) ([d041602](https://github.com/n8n-io/n8n/commit/d041602754a694e67e81c1bbff87c13bf91bdd5d))
* **Schedule Trigger Node:** Follow the correct Unix cron format for month and days of the week ([#6401](https://github.com/n8n-io/n8n/issues/6401)) ([2aef9de](https://github.com/n8n-io/n8n/commit/2aef9de14830c56199fd19bc09382424c55a2b9b))



# [0.232.0](https://github.com/n8n-io/n8n/compare/n8n@0.231.0...n8n@0.232.0) (2023-06-07)


### Bug Fixes

* **core:** RMC boolean value fix ([#6397](https://github.com/n8n-io/n8n/issues/6397)) ([28bb797](https://github.com/n8n-io/n8n/commit/28bb797bb0ea59b66a7641fc116f47c25564c21a))
* **Date & Time Node:** Reset responseData at end of loop ([#6385](https://github.com/n8n-io/n8n/issues/6385)) ([eaa8648](https://github.com/n8n-io/n8n/commit/eaa8648f2bf61074eae6dcd7355f8f107a31388e))
* **editor:** Add button to refresh branches ([#6387](https://github.com/n8n-io/n8n/issues/6387)) ([ce57816](https://github.com/n8n-io/n8n/commit/ce578162f4e44a6cc1774ab217967110b254ab3f))
* **editor:** Add secondary icon to menu items ([#6351](https://github.com/n8n-io/n8n/issues/6351)) ([3dd2601](https://github.com/n8n-io/n8n/commit/3dd260168eb627fd7fbed740bc97fa7f6289628f))
* **editor:** Add Set up version control CTA ([#6356](https://github.com/n8n-io/n8n/issues/6356)) ([e72521d](https://github.com/n8n-io/n8n/commit/e72521d5ec7a5e57dc311defb70f1fe19054b0f0))
* **editor:** Adding branch color ([#6380](https://github.com/n8n-io/n8n/issues/6380)) ([dba3f44](https://github.com/n8n-io/n8n/commit/dba3f44bc00de68113cc98db9afc6267f56ec04c))
* **editor:** Fix an issue with connections breaking during renaming ([#6358](https://github.com/n8n-io/n8n/issues/6358)) ([0f2bc6b](https://github.com/n8n-io/n8n/commit/0f2bc6b73711597fdf008ee54665d9bed82a1a9e))
* **editor:** Fix hard-coded parameter names for code editors ([#6372](https://github.com/n8n-io/n8n/issues/6372)) ([f61b776](https://github.com/n8n-io/n8n/commit/f61b776beac961fa58c6c69371c69ae1e74ef83e))
* **editor:** Fix typing `$` in inline expression field reloading node parameters form ([#6374](https://github.com/n8n-io/n8n/issues/6374)) ([4c0d4eb](https://github.com/n8n-io/n8n/commit/4c0d4ebd9917e52512e85a5cad2c93b554e0e212))
* **editor:** Pin all data regardless of pagination ([#6346](https://github.com/n8n-io/n8n/issues/6346)) ([f88029f](https://github.com/n8n-io/n8n/commit/f88029f308356c1c8271d7345ecbbd6e91c41b3d))
* **editor:** Remove explicit parameter name scanning for code editors ([#6390](https://github.com/n8n-io/n8n/issues/6390)) ([97295f6](https://github.com/n8n-io/n8n/commit/97295f67f0f8509ac6ba0d4ce38ce12582dff074))
* **editor:** Remove root level tag selector from css module to avoid making it a global style ([#6392](https://github.com/n8n-io/n8n/issues/6392)) ([cc37f21](https://github.com/n8n-io/n8n/commit/cc37f21aa27f3536f2043b5ff5da944388ac5504))
* **editor:** Update version control setup CTA tooltip ([#6393](https://github.com/n8n-io/n8n/issues/6393)) ([385b3e8](https://github.com/n8n-io/n8n/commit/385b3e871a9307c36428f8239a5db318d71948c1))
* Improve executions list polling performance ([#6355](https://github.com/n8n-io/n8n/issues/6355)) ([b5cabfe](https://github.com/n8n-io/n8n/commit/b5cabfef54e186f59580112a90566099bb79305e))
* **Ldap Node:** Add DN field to update operation ([#6371](https://github.com/n8n-io/n8n/issues/6371)) ([9396e7e](https://github.com/n8n-io/n8n/commit/9396e7eb585ab9d6fda742b0d234c4262570af93))
* Show actual execution data for production executions even if pin data exists ([#6302](https://github.com/n8n-io/n8n/issues/6302)) ([4eb8437](https://github.com/n8n-io/n8n/commit/4eb8437196a298a64f039aff51ba030dc21abb08))


### Features

* **Crypto Node:** Add support for hash and hmac on binary data ([#6359](https://github.com/n8n-io/n8n/issues/6359)) ([406a405](https://github.com/n8n-io/n8n/commit/406a405dd153833057286a27d04278ef71ceef3d))
* **editor:** Make WF name a link on /executions ([#6354](https://github.com/n8n-io/n8n/issues/6354)) ([6ddf161](https://github.com/n8n-io/n8n/commit/6ddf16128b4ab47db716eeab89f7526558073f56))
* New trigger PostgreSQL  ([#5495](https://github.com/n8n-io/n8n/issues/5495)) ([4488f93](https://github.com/n8n-io/n8n/commit/4488f93c39b0ec0b4a0eff98391b46db6a2eed78))
* Version control mvp ([#6271](https://github.com/n8n-io/n8n/issues/6271)) ([1b32141](https://github.com/n8n-io/n8n/commit/1b321416c0ba5371e0016398ae660ce298b8cdd6))


# [0.231.0](https://github.com/n8n-io/n8n/compare/n8n@0.230.0...n8n@0.231.0) (2023-05-31)


### Bug Fixes

* **Code Node:** Fix `item` and `items` alias regression ([#6331](https://github.com/n8n-io/n8n/issues/6331)) ([54e3838](https://github.com/n8n-io/n8n/commit/54e3838daed1f0931a04ba76cfd1ea7519c0e382))
* **Code Node:** Update vm2 to address CVE-2023-32313 ([#6318](https://github.com/n8n-io/n8n/issues/6318)) ([bcbec52](https://github.com/n8n-io/n8n/commit/bcbec52552d52b0509659cab13112e1377a256b3))
* **core:** Optimize getSharedWorkflowIds query ([#6314](https://github.com/n8n-io/n8n/issues/6314)) ([0631f69](https://github.com/n8n-io/n8n/commit/0631f69d98e5420faebba1a54d9ad47a2664d110))
* **core:** Prevent prototype pollution on injectable services ([#6309](https://github.com/n8n-io/n8n/issues/6309)) ([d94c20a](https://github.com/n8n-io/n8n/commit/d94c20ada543767f700475b40ef7174c433c26c5))
* **editor:** Fix locale plularisation if count is 0 ([#6312](https://github.com/n8n-io/n8n/issues/6312)) ([0d88bd7](https://github.com/n8n-io/n8n/commit/0d88bd7c1ae95cf077c2fa231d942204ff3b8f68))
* **editor:** Fix Luxon date parsing of ExecutionsUsage component ([#6333](https://github.com/n8n-io/n8n/issues/6333)) ([8f0ff46](https://github.com/n8n-io/n8n/commit/8f0ff460b11999f4d78f8313910358aa87311713))
* **editor:** Update SSO settings styles ([#6342](https://github.com/n8n-io/n8n/issues/6342)) ([5ae1124](https://github.com/n8n-io/n8n/commit/5ae1124106e7597d0943c371eae6aba6c105fd6b))
* **Execute Command Node:** Block executions when `command` is empty ([#6308](https://github.com/n8n-io/n8n/issues/6308)) ([011d577](https://github.com/n8n-io/n8n/commit/011d5778b15232cff94a321dfee18c3d7489f93d))
* Show `Ask AI` only on Code Node ([#6336](https://github.com/n8n-io/n8n/issues/6336)) ([da856d1](https://github.com/n8n-io/n8n/commit/da856d1c6593b43e1ce8d1becb1464c19c908e78))


### Features

* Add manual login option and password reset link for SSO ([#6328](https://github.com/n8n-io/n8n/issues/6328)) ([77e3f15](https://github.com/n8n-io/n8n/commit/77e3f1551dd7473a69f8833be5678d98964142e1))
* **core:** Add metadata (customdata) to event log ([#6334](https://github.com/n8n-io/n8n/issues/6334)) ([792b1c1](https://github.com/n8n-io/n8n/commit/792b1c1ffb0eb279bc3451787891ca3835f59d9f))
* **editor:** Implement Resource Mapper component ([#6207](https://github.com/n8n-io/n8n/issues/6207)) ([04cfa54](https://github.com/n8n-io/n8n/commit/04cfa548af3c7a25f1f0a36ddfb1de6a9e3f2169)), closes [#5752](https://github.com/n8n-io/n8n/issues/5752) [#5814](https://github.com/n8n-io/n8n/issues/5814)



# [0.230.0](https://github.com/n8n-io/n8n/compare/n8n@0.229.0...n8n@0.230.0) (2023-05-24)


### Bug Fixes

* **core:** Optimize SharedWorkflow queries ([#6297](https://github.com/n8n-io/n8n/issues/6297)) ([ed7f3b8](https://github.com/n8n-io/n8n/commit/ed7f3b845fe9a7aa0f6e1ff57ae9197057cd8aa1))
* **core:** Prevent app crashes because of unhandled promises in poll and trigger nodes ([#6278](https://github.com/n8n-io/n8n/issues/6278)) ([3750605](https://github.com/n8n-io/n8n/commit/37506050c3f49cececa9da3cf7d420b367f2e055))
* **editor:** Fix canvas loading when page gets restored from bfcache ([#6304](https://github.com/n8n-io/n8n/issues/6304)) ([11477f0](https://github.com/n8n-io/n8n/commit/11477f0a20f82b02d763dbf53e29083dd1e95e87))
* **editor:** Fix design system button with icon vertical alignment ([#6284](https://github.com/n8n-io/n8n/issues/6284)) ([fc580f7](https://github.com/n8n-io/n8n/commit/fc580f7ee80b48a62fc2bebaec9902cd15944ad7))
* **editor:** Fix inverted checks on modal confirmation results ([#6285](https://github.com/n8n-io/n8n/issues/6285)) ([5d2f474](https://github.com/n8n-io/n8n/commit/5d2f4746ea5da977a6532db90c624ded1520ec3e))
* **ERPNext Node:** Fix issue with credential test and add frappe cloud url ([#6283](https://github.com/n8n-io/n8n/issues/6283)) ([2a2b645](https://github.com/n8n-io/n8n/commit/2a2b6452dc326d8979bed0cf47fc54becd746619))
* **Google Calendar Node:** All day option fix ([#6274](https://github.com/n8n-io/n8n/issues/6274)) ([5bef91e](https://github.com/n8n-io/n8n/commit/5bef91e3c84a15a30a893ce3b321b7a8ea926963))
* Initialize license in queue mode correctly ([#6301](https://github.com/n8n-io/n8n/issues/6301)) ([42c79cd](https://github.com/n8n-io/n8n/commit/42c79cd6f1e495e60a9f038403d9a8a761318f52))
* **OpenAI Node:** Descriptive errors ([#6270](https://github.com/n8n-io/n8n/issues/6270)) ([8fdfa3b](https://github.com/n8n-io/n8n/commit/8fdfa3b6b83c6a008d1be778dadcc2172e8a708d))
* Prevent removing manual executions when setting says to save ([#6300](https://github.com/n8n-io/n8n/issues/6300)) ([55b755c](https://github.com/n8n-io/n8n/commit/55b755cb44a3bf9fc9d41af37b7818d3626baf0d))
* **SSH Node:** Private key field as password and credential test ([#6298](https://github.com/n8n-io/n8n/issues/6298)) ([d5c7e6f](https://github.com/n8n-io/n8n/commit/d5c7e6f2cff63337948122a11c3707316c937b9f))
* **SSH Node:** Replace ~ with /home/username ([#6269](https://github.com/n8n-io/n8n/issues/6269)) ([4219490](https://github.com/n8n-io/n8n/commit/421949067b47a25e859fbd45364ba657e7286599))
* **Strapi Node:** Strapi credentials notice ([#6289](https://github.com/n8n-io/n8n/issues/6289)) ([bbe6d4c](https://github.com/n8n-io/n8n/commit/bbe6d4c4dbda0b2cba447cf1b0aa4a7f808096fb))
* **Strava Trigger Node:** Fix issue with delete events failing to display data ([#6277](https://github.com/n8n-io/n8n/issues/6277)) ([8a8fed0](https://github.com/n8n-io/n8n/commit/8a8fed08407f20791ae01ab83e1ce3d99715dc5c))
* **Wekan Node:** Handle response correctly ([#6296](https://github.com/n8n-io/n8n/issues/6296)) ([4d9c8b0](https://github.com/n8n-io/n8n/commit/4d9c8b07a93ea4f2e5ad913358bafb682f6f5506))


### Features

* Add SSO SAML metadataUrl support and various improvements ([#6139](https://github.com/n8n-io/n8n/issues/6139)) ([e3a53fd](https://github.com/n8n-io/n8n/commit/e3a53fd19d8c258a08baab9c090968104327a13b))
* **core:** Remove all floating promises. Enforce `@typescript-eslint/no-floating-promises` ([#6281](https://github.com/n8n-io/n8n/issues/6281)) ([e046f65](https://github.com/n8n-io/n8n/commit/e046f656fefe951af71ab031a440729a5eb1c7cb))
* **core:** Replace client-oauth2 with an in-repo package ([#6266](https://github.com/n8n-io/n8n/issues/6266)) ([a1b1f24](https://github.com/n8n-io/n8n/commit/a1b1f24ddfd4da36f8dd04e34e2675a3993755ca))
* **Execution Data Node:** New node ([#6247](https://github.com/n8n-io/n8n/issues/6247)) ([3f7c4f0](https://github.com/n8n-io/n8n/commit/3f7c4f0ad485a0a4049f371723b01847077f7ccd))
* **Gotify Node:** Add support for self signed certificates ([#6053](https://github.com/n8n-io/n8n/issues/6053)) ([401cffd](https://github.com/n8n-io/n8n/commit/401cffde57aa153bc2d1589bc8d11d7951f2ade1))
* **Ldap Node:** Add LDAP node ([#4783](https://github.com/n8n-io/n8n/issues/4783)) ([ec393bc](https://github.com/n8n-io/n8n/commit/ec393bc041e9e7590e7b0a2821976f104f5c23bb))
* **LoneScale Node:** Add LoneScale node and Trigger node ([#5146](https://github.com/n8n-io/n8n/issues/5146)) ([4b85433](https://github.com/n8n-io/n8n/commit/4b854333d49c661fe11f19a176a147dbf28e697f))
* **RabbitMQ Node:** Add mode for acknowledging and deleting from queue later in workflow ([#6225](https://github.com/n8n-io/n8n/issues/6225)) ([f5950b2](https://github.com/n8n-io/n8n/commit/f5950b201c6ff412b9a304052f05eb2c3b8a7c51))
* **Send Email Node:** Add content-id for email attachments ([#3632](https://github.com/n8n-io/n8n/issues/3632)) ([8fe8aad](https://github.com/n8n-io/n8n/commit/8fe8aad6a77bbec7a26c87f8bad9593852e8d464))
* **SSH Node:** Credentials test ([#6279](https://github.com/n8n-io/n8n/issues/6279)) ([3569d53](https://github.com/n8n-io/n8n/commit/3569d53917b41b758a96293a2b33a06cbf2c0a70))



# [0.229.0](https://github.com/n8n-io/n8n/compare/n8n@0.228.0...n8n@0.229.0) (2023-05-17)


### Bug Fixes

* **Code Node:** Restore help text ([#6231](https://github.com/n8n-io/n8n/issues/6231)) ([e72d564](https://github.com/n8n-io/n8n/commit/e72d564bf84460ce085f022f186e8101524f2e7b))
* **core:** Make sure that special polling parameters are available on community nodes as well ([#6230](https://github.com/n8n-io/n8n/issues/6230)) ([9db49d0](https://github.com/n8n-io/n8n/commit/9db49d0c18f007b974594b918728e430ec510f54))
* Remove workflow execution credential error message when instance owner ([#6116](https://github.com/n8n-io/n8n/issues/6116)) ([e81a964](https://github.com/n8n-io/n8n/commit/e81a96483af6e0d0a3cf62481f5e9a37d6a62b6e))


### Features

* **core:** Reduce the number of events sent to Sentry ([#6235](https://github.com/n8n-io/n8n/issues/6235)) ([a4c0cc9](https://github.com/n8n-io/n8n/commit/a4c0cc9b5c56639067918f1bad1baf4eb201e48b))
* **core:** Return OAuth2 error body if available ([#5794](https://github.com/n8n-io/n8n/issues/5794)) ([79d0a0f](https://github.com/n8n-io/n8n/commit/79d0a0f2470905f98b71fb5c8ca007244004f99a))
* **editor:** Add cloud ExecutionsUsage and API blocking using licenses ([#6159](https://github.com/n8n-io/n8n/issues/6159)) ([cd7c312](https://github.com/n8n-io/n8n/commit/cd7c312fbd172b5d3c8bbeaf775f7b5bb4611aa5)), closes [#6187](https://github.com/n8n-io/n8n/issues/6187)
* **editor:** Add color picker design system component ([#6179](https://github.com/n8n-io/n8n/issues/6179)) ([823e885](https://github.com/n8n-io/n8n/commit/823e88500c35508d6322242bca5749d711fb2b31))
* **editor:** Drop support for legacy browsers that do not have native ESM support ([#6239](https://github.com/n8n-io/n8n/issues/6239)) ([9182d15](https://github.com/n8n-io/n8n/commit/9182d1558a1f98e0ea1b9fbaddabf7c8b4836e94))
* **editor:** Updating node reference pattern in expression editor ([#6228](https://github.com/n8n-io/n8n/issues/6228)) ([13bcec1](https://github.com/n8n-io/n8n/commit/13bcec1661e1da736ff9c93869bc49a3038bdf1b))
* **editor:** Version Control settings update (WIP) ([#6233](https://github.com/n8n-io/n8n/issues/6233)) ([0666377](https://github.com/n8n-io/n8n/commit/0666377ef8074ad093391d41e08e194704a25dbd))
* **Google Ads Node:** Update to support v13 ([#6212](https://github.com/n8n-io/n8n/issues/6212)) ([bd1bffc](https://github.com/n8n-io/n8n/commit/bd1bffcd536eedde8582a354c11349dbddd2b9a2))
* **Respond to Webhook Node:** Move from Binary Buffer to Binary streaming ([#5613](https://github.com/n8n-io/n8n/issues/5613)) ([8ae2d80](https://github.com/n8n-io/n8n/commit/8ae2d801d8e2c881fcff5f7cf4fcb699c10b2be2))



# [0.228.0](https://github.com/n8n-io/n8n/compare/n8n@0.227.0...n8n@0.228.0) (2023-05-11)


### Bug Fixes

* **AWS Rekognition Node:** Fix all different action type ([#6136](https://github.com/n8n-io/n8n/issues/6136)) ([22b82a4](https://github.com/n8n-io/n8n/commit/22b82a43a24bb8415eb8f4a941b05647ef8904c2))
* **core:** Ensure DB repositories are initialized before the DB migrations are run  ([#6220](https://github.com/n8n-io/n8n/issues/6220)) ([500c0eb](https://github.com/n8n-io/n8n/commit/500c0ebce34dc2d21a531176dee965a70abec5f8))
* **core:** Move nodeExecute InternalHook calls to hookFunctionsSave ([#6193](https://github.com/n8n-io/n8n/issues/6193)) ([f00b2ae](https://github.com/n8n-io/n8n/commit/f00b2ae3eaa225e483abc8defdc58d27b7d2c5e8))
* Correctly save executions that failed when polling as error instead of new ([#6192](https://github.com/n8n-io/n8n/issues/6192)) ([06948b5](https://github.com/n8n-io/n8n/commit/06948b5ba5775b4f03d1ce46d57a461014317d51))
* **editor:** Add loading skeletons to Executions list page ([#6184](https://github.com/n8n-io/n8n/issues/6184)) ([eae3a55](https://github.com/n8n-io/n8n/commit/eae3a55cc6b87bc8998d18d3d32d0d03013996b1))
* **editor:** Display SSO entry in Settings on Cloud ([#6181](https://github.com/n8n-io/n8n/issues/6181)) ([b0a1899](https://github.com/n8n-io/n8n/commit/b0a1899e7141e5726d4fcbca6bba47e8e4b5cef7))
* **editor:** Fix polling trigger check for `runData` ([#6130](https://github.com/n8n-io/n8n/issues/6130)) ([80831cd](https://github.com/n8n-io/n8n/commit/80831cd7c60f77557c37317600690a289d966448))
* **editor:** Fix viewing and downloading of binary data ([#6218](https://github.com/n8n-io/n8n/issues/6218)) ([b9779c3](https://github.com/n8n-io/n8n/commit/b9779c32936c8b5e2385226ecab1025ff88d7044))
* **editor:** Flag issues only on workflow activation ([#6127](https://github.com/n8n-io/n8n/issues/6127)) ([1b49c17](https://github.com/n8n-io/n8n/commit/1b49c17f38e97547430c407e21284b0c508469fa))
* **editor:** Remove duplicate mapping of `item.json` key in data pinning ([#6135](https://github.com/n8n-io/n8n/issues/6135)) ([91fee0c](https://github.com/n8n-io/n8n/commit/91fee0ca667f233c0bde0dc6089bbed7d7db5b5f))
* **editor:** Show the correct actions count in the nodes list ([#6183](https://github.com/n8n-io/n8n/issues/6183)) ([751e132](https://github.com/n8n-io/n8n/commit/751e132968470144cfca1c1b7ca22caf2c4c1de4))
* **editor:** Update and add design system checkbox component to Editor ([#6178](https://github.com/n8n-io/n8n/issues/6178)) ([13c143e](https://github.com/n8n-io/n8n/commit/13c143eb6df41457fbd361674f2063b983a0e077))
* **editor:** Update and fix storybook (was failing to run in local dev mode) ([#6180](https://github.com/n8n-io/n8n/issues/6180)) ([1e6a75f](https://github.com/n8n-io/n8n/commit/1e6a75f3416cdfcce1299dc9d242e23d0ea97ad3))
* **FTP Node:** Use filename instead of remote filepath for downloaded binary data ([#6170](https://github.com/n8n-io/n8n/issues/6170)) ([be08933](https://github.com/n8n-io/n8n/commit/be089331b372e029ab5516b91e63a2d5d9033719))
* **Google Sheets Node:** Upgrade xlsx to address CVE-2023-30533 ([#6172](https://github.com/n8n-io/n8n/issues/6172)) ([45dc985](https://github.com/n8n-io/n8n/commit/45dc985af742b049dc5673cf972da704d1f1f220))
* **HTTP Request Node:** Correctly doesn't redirect on non GET method ([#6132](https://github.com/n8n-io/n8n/issues/6132)) ([3f5c606](https://github.com/n8n-io/n8n/commit/3f5c6062542f3b2b8a02cf0820e03da3f01d8bf2))
* **MySQL Node:** Node should return date types as strings ([#6169](https://github.com/n8n-io/n8n/issues/6169)) ([5d77ec7](https://github.com/n8n-io/n8n/commit/5d77ec76e3c47fe9f9d7f31fe6c03827685ec576))
* **Postgres Node:** Always return TIMESTAMP and TIMESTAMPZ as ISO string ([#6145](https://github.com/n8n-io/n8n/issues/6145)) ([0eb4d9f](https://github.com/n8n-io/n8n/commit/0eb4d9fc16aad1d1a350ba074c4b86712fbd90a1))
* Prevent overflow when rendering expression hints ([#6214](https://github.com/n8n-io/n8n/issues/6214)) ([c717771](https://github.com/n8n-io/n8n/commit/c7177719e5f60813f4d15f7f97f1b4f253e29b07))
* Prevent unnecessary error messages also for data loaded flag ([#6201](https://github.com/n8n-io/n8n/issues/6201)) ([d5e62ff](https://github.com/n8n-io/n8n/commit/d5e62ff096ddefd52dae742166fe92ceef17ded6))


### Features

* **Airtable Node:** Access token support ([#6160](https://github.com/n8n-io/n8n/issues/6160)) ([f9fd820](https://github.com/n8n-io/n8n/commit/f9fd82040ac09914a03e5b9f8f84fce5f6a99835))
* **Code Node:** Add Python support ([#4295](https://github.com/n8n-io/n8n/issues/4295)) ([35c8510](https://github.com/n8n-io/n8n/commit/35c8510ab6d607fe59056a4aa1d8d148e194d12c))
* **core:** Improve health check ([#6205](https://github.com/n8n-io/n8n/issues/6205)) ([9e7b9fb](https://github.com/n8n-io/n8n/commit/9e7b9fb443046c73135efb70d0d1894207125f66))
* Create NPM node ([#6177](https://github.com/n8n-io/n8n/issues/6177)) ([f3bc6f1](https://github.com/n8n-io/n8n/commit/f3bc6f19b68f6bd4bd99614f60bd6833bd15813f))
* **Date & Time Node:** Overhaul of the node ([#5904](https://github.com/n8n-io/n8n/issues/5904)) ([7d1d1f7](https://github.com/n8n-io/n8n/commit/7d1d1f7872163cecb468c317670da2d8b89a7651))
* **HubSpot Node:** Overhaul the HubSpot Node ([#4337](https://github.com/n8n-io/n8n/issues/4337)) ([2913e67](https://github.com/n8n-io/n8n/commit/2913e676e639757cdf1a513ad35a7df0e494fa6f))
* **JotForm Trigger Node:** Add support for hipaa-api.jotform.com ([#6171](https://github.com/n8n-io/n8n/issues/6171)) ([3074f42](https://github.com/n8n-io/n8n/commit/3074f42b3b98cf0dbdc13ad7b927d6b7fc726fab))
* **Kafka Trigger Node:** Add non-parallel execution ([#6175](https://github.com/n8n-io/n8n/issues/6175)) ([814ea51](https://github.com/n8n-io/n8n/commit/814ea5185ce82e0a7687b41161602b45f92bee93))



# [0.227.0](https://github.com/n8n-io/n8n/compare/n8n@0.226.0...n8n@0.227.0) (2023-05-03)


### Bug Fixes

* **AWS S3 Node:** Fix File upload, and add node tests ([#6153](https://github.com/n8n-io/n8n/issues/6153)) ([deb4c04](https://github.com/n8n-io/n8n/commit/deb4c04f346f8e5985b5f6c3f3a3e929fde13e5b))
* **Compression Node:** Fix issue with decompression failing with uppercase extensions ([#6098](https://github.com/n8n-io/n8n/issues/6098)) ([aa59329](https://github.com/n8n-io/n8n/commit/aa593298365eabd6eb1dda9fe3f06e7eae7c5ea9))
* **core:** Account for nodes with renamable content ([#6109](https://github.com/n8n-io/n8n/issues/6109)) ([c99f158](https://github.com/n8n-io/n8n/commit/c99f158120b3c1ffca1718be337afc73d6ec9e65))
* **core:** Assign Unknown Error only if message or description not present in error ([8aedc03](https://github.com/n8n-io/n8n/commit/8aedc03ddad3f83ffd2569be5b61710f27d2f672))
* **core:** Avoid using `Object.keys` on Buffer and other non-plain objects ([#6131](https://github.com/n8n-io/n8n/issues/6131)) ([a3aba83](https://github.com/n8n-io/n8n/commit/a3aba835a15a8a32acc1e1ff0b972007df2b2b34))
* **core:** Better error message in Webhook node when using the POST method ([a0dd17e](https://github.com/n8n-io/n8n/commit/a0dd17e1151e668b95dc57367a0b100d00913ea3))
* **core:** Better errors for common status codes fix ([700cc39](https://github.com/n8n-io/n8n/commit/700cc39cbc7da3c70513ff586dc97319456308ae))
* **core:** Fix `hasOwnProperty` on augmented objects ([#6124](https://github.com/n8n-io/n8n/issues/6124)) ([206b6b9](https://github.com/n8n-io/n8n/commit/206b6b90b860ceaab58b9bdd5ff20ffc741c13fa))
* **core:** Fix bug running addUserActivatedColumn migration on MariaDB ([#6157](https://github.com/n8n-io/n8n/issues/6157)) ([570790e](https://github.com/n8n-io/n8n/commit/570790ed0c9521e09b6414bc1da2c596f17ff072))
* **core:** Fix canceled execution status ([#6142](https://github.com/n8n-io/n8n/issues/6142)) ([839a56a](https://github.com/n8n-io/n8n/commit/839a56a682674baf44d5beececdbe677d18c0d89))
* **core:** Improve saml endpoints and audit events ([#6107](https://github.com/n8n-io/n8n/issues/6107)) ([c0b1cdd](https://github.com/n8n-io/n8n/commit/c0b1cddc91fe199377c301f02f230827f231ba73))
* **core:** Remove SAML config metadataUrl if XML metadata is set directly ([#6143](https://github.com/n8n-io/n8n/issues/6143)) ([25fe14b](https://github.com/n8n-io/n8n/commit/25fe14be56482477c00a360914730b25c9028443))
* **core:** Skip auth for controllers/routes that don't use the `Authorized` decorator, or use `Authorized('none')` ([#6106](https://github.com/n8n-io/n8n/issues/6106)) ([59aee22](https://github.com/n8n-io/n8n/commit/59aee2270bdc0c8360aa534237b7f6015d382346))
* Correctly allow sharees to test credential when opening the modal ([#6111](https://github.com/n8n-io/n8n/issues/6111)) ([2e73f4a](https://github.com/n8n-io/n8n/commit/2e73f4abd04ba7ab929b0fce57bf12651a0a2e49))
* **Date & Time Node:** Numbers conversions fix ([14f7114](https://github.com/n8n-io/n8n/commit/14f71146e21026721fc9d5883bb9d73d38afcf8c))
* **editor:** Change execution list tab loader design ([#6120](https://github.com/n8n-io/n8n/issues/6120)) ([188ef04](https://github.com/n8n-io/n8n/commit/188ef042cd58b9194dadef4cc68deb3510688c26))
* **editor:** Disable changing of email and pw when SAML login enabled ([#6104](https://github.com/n8n-io/n8n/issues/6104)) ([3e9ecd9](https://github.com/n8n-io/n8n/commit/3e9ecd939742df8d8ced9179aaa26b081139befa))
* **editor:** Fix `Show details` summary ([#6113](https://github.com/n8n-io/n8n/issues/6113)) ([90a62cc](https://github.com/n8n-io/n8n/commit/90a62ccfb5b4a959d72336d284ad4ac3b17af582))
* **editor:** Fix copy selection behavior ([#6112](https://github.com/n8n-io/n8n/issues/6112)) ([1607aeb](https://github.com/n8n-io/n8n/commit/1607aeb9f94700793d58604ea4f89c5555d43981))
* **editor:** Fix cropped off completions docstrings ([#6129](https://github.com/n8n-io/n8n/issues/6129)) ([85e8145](https://github.com/n8n-io/n8n/commit/85e8145439f89e76fe5fe3a659430c03738d6e2b))
* **editor:** Fix focus jumping when using chrome autofill ([#6140](https://github.com/n8n-io/n8n/issues/6140)) ([c63181b](https://github.com/n8n-io/n8n/commit/c63181b3171040c3dd3051c2a1358aea0af6bae0))
* **editor:** Fix missing `Stop Listening` button ([#6125](https://github.com/n8n-io/n8n/issues/6125)) ([20a72bb](https://github.com/n8n-io/n8n/commit/20a72bb28b981e9c8d12dd6398d843b39d80daac))
* **editor:** Fix quote handling on dollar-sign variable completions ([#6128](https://github.com/n8n-io/n8n/issues/6128)) ([51f5990](https://github.com/n8n-io/n8n/commit/51f59905591fa492017fc3ced46601eeca5fb057))
* **editor:** Fix sidebar button styling ([#6138](https://github.com/n8n-io/n8n/issues/6138)) ([a72a511](https://github.com/n8n-io/n8n/commit/a72a5112f34a0d8ab248f687c74b758c8db6729c))
* **editor:** Fix unique names for node duplication ([#6134](https://github.com/n8n-io/n8n/issues/6134)) ([71ae6c6](https://github.com/n8n-io/n8n/commit/71ae6c66ef32ba86edf0bb9cdb9f24a6d40ee80c))
* **editor:** Fix unscrollable node settings ([#6133](https://github.com/n8n-io/n8n/issues/6133)) ([c8ff368](https://github.com/n8n-io/n8n/commit/c8ff368fc7be58e7c42746f7e7a4c5f6a4149d3e))
* **editor:** Loading state for executions tab ([#6100](https://github.com/n8n-io/n8n/issues/6100)) ([4cbb05b](https://github.com/n8n-io/n8n/commit/4cbb05b0017ffd77eca51fc5b9c5c4868515a60d))
* **editor:** Remove pagination from binary data output ([#6093](https://github.com/n8n-io/n8n/issues/6093)) ([c6e665a](https://github.com/n8n-io/n8n/commit/c6e665a975958c433d7991c057a3e4be644daff1))
* **editor:** Restrict `[empty]` in parameter input hint to zero-length string ([#6003](https://github.com/n8n-io/n8n/issues/6003)) ([8862e1e](https://github.com/n8n-io/n8n/commit/8862e1e7df0be62ab3746b70e613ffd2ab26bc4a))
* **editor:** Show error in RLC if credentials are not set ([#6108](https://github.com/n8n-io/n8n/issues/6108)) ([2c240a0](https://github.com/n8n-io/n8n/commit/2c240a0e4ecd9157dca612d98a8a7c68a65a9909))
* **HTTP Request Node:** Add description for 'Specify Body' option ([#6114](https://github.com/n8n-io/n8n/issues/6114)) ([af097ae](https://github.com/n8n-io/n8n/commit/af097ae22c7e87918ada2527c6a2fe62cb8f318a))
* **HTTP Request Node:** Always lowercase headers ([983e6e1](https://github.com/n8n-io/n8n/commit/983e6e124eb9557eec55c5f2e2b834a926243955))
* **Mattermost Node:** Fix base url trailing slash error ([#6097](https://github.com/n8n-io/n8n/issues/6097)) ([25a386d](https://github.com/n8n-io/n8n/commit/25a386dd70df516090e622d921a79456fc7d16e3))
* **Merge Node:** Do not error if expected key is missing ([d219af7](https://github.com/n8n-io/n8n/commit/d219af75cf37c603c34b1ca5851cafd4a490889c))
* Prevent displaying an endless timer in the execution list for finished executions ([#6137](https://github.com/n8n-io/n8n/issues/6137)) ([701105e](https://github.com/n8n-io/n8n/commit/701105edcf5284f276fe146d8267e1a5560ab186))
* Prevent invocations of 'GET /rest/license' from returning an error when ephemeral licenses are used ([#6154](https://github.com/n8n-io/n8n/issues/6154)) ([a3d26ef](https://github.com/n8n-io/n8n/commit/a3d26eff79013642865fa59078732526850b96a6))
* **Slack Node:** Restore ability to send text in addition of blocks or attachments ([8669f95](https://github.com/n8n-io/n8n/commit/8669f95736797da4f3efd33468cdeac5d28667b0))


### Features

* **core:** Add notice to alert users a new version is available ([cb497fb](https://github.com/n8n-io/n8n/commit/cb497fbbecdba670d5121fa2c6eaf7c66d8a8a38))
* **editor:** Add support for `loadOptionsDependsOn` to RLC ([#6101](https://github.com/n8n-io/n8n/issues/6101)) ([b17d5f9](https://github.com/n8n-io/n8n/commit/b17d5f9aa086bf408e8450244460ada57de0d7c3))
* **editor:** Add version controls settings (WIP) ([#6036](https://github.com/n8n-io/n8n/issues/6036)) ([0c9ce3a](https://github.com/n8n-io/n8n/commit/0c9ce3a2ec9487b4eb9130651927e91dcd0f85af))
* **Item Lists Node:** Split out items work on objects as well as arrays ([c65ac03](https://github.com/n8n-io/n8n/commit/c65ac0336821868c289adc55abab40017b1856da))
* **Microsoft Excel 365 Node:** Overhaul ([5364a2d](https://github.com/n8n-io/n8n/commit/5364a2dff32e05147b8e9dd392038eb36791e5dc))



## [0.226.2](https://github.com/n8n-io/n8n/compare/n8n@0.226.1...n8n@0.226.2) (2023-05-03)


### Bug Fixes

* **core:** Fix bug running addUserActivatedColumn migration on MariaDB ([#6157](https://github.com/n8n-io/n8n/issues/6157)) ([aa8e96d](https://github.com/n8n-io/n8n/commit/aa8e96dd6b19f105a957da71a5c4d7ab5caecc01))



## [0.226.1](https://github.com/n8n-io/n8n/compare/n8n@0.226.0...n8n@0.226.1) (2023-05-02)


### Bug Fixes

* **Compression Node:** Fix issue with decompression failing with uppercase extensions ([#6098](https://github.com/n8n-io/n8n/issues/6098)) ([7136500](https://github.com/n8n-io/n8n/commit/71365002daa71c5fa5e68a5bb373ee200a05b7b9))
* **core:** Account for nodes with renamable content ([#6109](https://github.com/n8n-io/n8n/issues/6109)) ([b561d46](https://github.com/n8n-io/n8n/commit/b561d463265831f3cd370ec99982847f2bddca41))
* **core:** Fix `hasOwnProperty` on augmented objects ([#6124](https://github.com/n8n-io/n8n/issues/6124)) ([2f015c0](https://github.com/n8n-io/n8n/commit/2f015c0f153785384b009e71bf4994e18b5d06b8))
* **core:** Fix canceled execution status ([#6142](https://github.com/n8n-io/n8n/issues/6142)) ([1796101](https://github.com/n8n-io/n8n/commit/1796101fed03d04906f2341a0488b60b7b5bf71c))
* **core:** Skip auth for controllers/routes that don't use the `Authorized` decorator, or use `Authorized('none')` ([#6106](https://github.com/n8n-io/n8n/issues/6106)) ([9d44991](https://github.com/n8n-io/n8n/commit/9d44991b2a8c9384e2bf32204ac47a4ecb0131be))
* Correctly allow sharees to test credential when opening the modal ([#6111](https://github.com/n8n-io/n8n/issues/6111)) ([240bb47](https://github.com/n8n-io/n8n/commit/240bb47e8e2cd99c56b8837079073bbf2bf5f687))
* **Date & Time Node:** Numbers conversions fix ([e11e7cd](https://github.com/n8n-io/n8n/commit/e11e7cd603a145c83c36f6a6deb821a56ccabd6f))
* **editor:** Change execution list tab loader design ([#6120](https://github.com/n8n-io/n8n/issues/6120)) ([ffc033f](https://github.com/n8n-io/n8n/commit/ffc033ff8ff391be09da8dbd62f8eb06a94f6cb0))
* **editor:** Fix `Show details` summary ([#6113](https://github.com/n8n-io/n8n/issues/6113)) ([e12bafb](https://github.com/n8n-io/n8n/commit/e12bafb9473393dd9e139d0e0a4a21241b417645))
* **editor:** Fix copy selection behavior ([#6112](https://github.com/n8n-io/n8n/issues/6112)) ([0efd94a](https://github.com/n8n-io/n8n/commit/0efd94a875fe9e3cac5da3421effcf6c8f6eaae8))
* **editor:** Fix cropped off completions docstrings ([#6129](https://github.com/n8n-io/n8n/issues/6129)) ([06594cc](https://github.com/n8n-io/n8n/commit/06594cc36f1a0d4069e556d6dbb4e268a78301c6))
* **editor:** Fix missing `Stop Listening` button ([#6125](https://github.com/n8n-io/n8n/issues/6125)) ([dcbd2d2](https://github.com/n8n-io/n8n/commit/dcbd2d2bc1c59ca8bbe6a802a2a8f482b3d20d74))
* **editor:** Fix quote handling on dollar-sign variable completions ([#6128](https://github.com/n8n-io/n8n/issues/6128)) ([c23ad35](https://github.com/n8n-io/n8n/commit/c23ad3502d0a8c4bcbd60cce2fc13a91981fb119))
* **editor:** Fix sidebar button styling ([#6138](https://github.com/n8n-io/n8n/issues/6138)) ([d3f4bc1](https://github.com/n8n-io/n8n/commit/d3f4bc1859104f11d2cf38ef3f3405d62c88bc6d))
* **editor:** Fix unique names for node duplication ([#6134](https://github.com/n8n-io/n8n/issues/6134)) ([48a4068](https://github.com/n8n-io/n8n/commit/48a4068d7ec1ddf5d5a4d10620dce1c89cb8fa34))
* **editor:** Fix unscrollable node settings ([#6133](https://github.com/n8n-io/n8n/issues/6133)) ([f762f16](https://github.com/n8n-io/n8n/commit/f762f16afb7b9ea54e29950c06133a292dc87b3f))
* **editor:** Loading state for executions tab ([#6100](https://github.com/n8n-io/n8n/issues/6100)) ([2e12c50](https://github.com/n8n-io/n8n/commit/2e12c50477014c57fa665ba36f48ff658cf7ee94))
* **editor:** Remove pagination from binary data output ([#6093](https://github.com/n8n-io/n8n/issues/6093)) ([7b7d9de](https://github.com/n8n-io/n8n/commit/7b7d9de7586905b2740541e7f0289bc78f8f2ad7))
* **editor:** Show error in RLC if credentials are not set ([#6108](https://github.com/n8n-io/n8n/issues/6108)) ([5bf3400](https://github.com/n8n-io/n8n/commit/5bf3400ca7ffa04bb51214bc539435b847614cbb))
* **HTTP Request Node:** Add description for 'Specify Body' option ([#6114](https://github.com/n8n-io/n8n/issues/6114)) ([69b6ba8](https://github.com/n8n-io/n8n/commit/69b6ba85202c5a28052a56c041b880bfa9fcf0a0))
* **HTTP Request Node:** Always lowercase headers ([31c56a1](https://github.com/n8n-io/n8n/commit/31c56a12f273d5569ed3ac4d72cf74c90cc24b31))
* **Mattermost Node:** Fix base url trailing slash error ([#6097](https://github.com/n8n-io/n8n/issues/6097)) ([788fda1](https://github.com/n8n-io/n8n/commit/788fda1b7dbf29d7a7e614a959ac3630b2a6559f))
* **Merge Node:** Do not error if expected key is missing ([8b59564](https://github.com/n8n-io/n8n/commit/8b59564776ebaf2c54b9e2dae5b77109895da883))
* Prevent displaying an endless timer in the execution list for finished executions ([#6137](https://github.com/n8n-io/n8n/issues/6137)) ([2672896](https://github.com/n8n-io/n8n/commit/2672896c8e2de7d1f92899a392a3f2b3f60aaef3))
* **Slack Node:** Restore ability to send text in addition of blocks or attachments ([625d672](https://github.com/n8n-io/n8n/commit/625d6729b4158fbc811941ce45819f32372e6265))



# [0.226.0](https://github.com/n8n-io/n8n/compare/n8n@0.225.0...n8n@0.226.0) (2023-04-26)


### Bug Fixes

* **Code Node:** Update vm2 to address CVE-2023-30547 ([#6039](https://github.com/n8n-io/n8n/issues/6039)) ([8268f23](https://github.com/n8n-io/n8n/commit/8268f235abf5277480c215ea953fc3db1c275c95))
* **core:** Improve domain and url matching for extractDomain and extractUrl ([#6010](https://github.com/n8n-io/n8n/issues/6010)) ([33fb732](https://github.com/n8n-io/n8n/commit/33fb73217dca68244c93296f1a4be96cc83e4480))
* **core:** Serialize dates and regexps when reading from augmented objects ([#6086](https://github.com/n8n-io/n8n/issues/6086)) ([a4eb46a](https://github.com/n8n-io/n8n/commit/a4eb46acc178533e3c63fedcf0d884a5b66bae28))
* **core:** Skip license activation when instance was already activated ([#6064](https://github.com/n8n-io/n8n/issues/6064)) ([eaf7090](https://github.com/n8n-io/n8n/commit/eaf70909197ed511efe9add956eb5e4f78b27e20))
* **editor:** Clean up demo and template callouts from workflows page ([#6023](https://github.com/n8n-io/n8n/issues/6023)) ([4ee5083](https://github.com/n8n-io/n8n/commit/4ee508385ab5ac379925b315006a2d9389183751))
* **editor:** Fix memory leak in Node Detail View by correctly unsubscribing from event buses ([#6021](https://github.com/n8n-io/n8n/issues/6021)) ([0970ec0](https://github.com/n8n-io/n8n/commit/0970ec066d8f80082f49f0b0f8987b95392102bf))
* **editor:** Fix typo in SSO upgrade link ([#6031](https://github.com/n8n-io/n8n/issues/6031)) ([9b59f1d](https://github.com/n8n-io/n8n/commit/9b59f1df9c358d3677b4cbc3e80a73af03b7981d))
* **editor:** Resolve expressions for grandparent nodes ([#5859](https://github.com/n8n-io/n8n/issues/5859)) ([a19d444](https://github.com/n8n-io/n8n/commit/a19d4447ac38e40d1fd1da83beb6c20fb7b2d0ed))
* **editor:** SettingsSidebar should disconnect from push when navigating away ([#6025](https://github.com/n8n-io/n8n/issues/6025)) ([41660d9](https://github.com/n8n-io/n8n/commit/41660d9e281432b87d875c98992bfaf54d25b37f))
* **editor:** Update LDAP and Log streaming paywalls ([#6069](https://github.com/n8n-io/n8n/issues/6069)) ([8a3b3e5](https://github.com/n8n-io/n8n/commit/8a3b3e53e1ac0a2a1864b42b24ab46f25253a9d3))
* **editor:** Update SSO upgrade link ([#6016](https://github.com/n8n-io/n8n/issues/6016)) ([953198e](https://github.com/n8n-io/n8n/commit/953198e092a44029805ff85e4607355444ea8b2c))
* **Notion Node:** Update credential test to not require user permissions ([#6022](https://github.com/n8n-io/n8n/issues/6022)) ([a68330f](https://github.com/n8n-io/n8n/commit/a68330ff66744551270f40399a6fd7fe330e6f27))


### Features

* **core:** Add license:info command ([#6047](https://github.com/n8n-io/n8n/issues/6047)) ([ab12d3e](https://github.com/n8n-io/n8n/commit/ab12d3e3278745b290de82c16f358841b20850b4))
* **core:** Add SSH key generation ([#6006](https://github.com/n8n-io/n8n/issues/6006)) ([71ed1f4](https://github.com/n8n-io/n8n/commit/71ed1f410c5a80f35ecaf913a5522b7788998695))
* **core:** Add support for digestAuth to httpRequest and declarative style ([#5676](https://github.com/n8n-io/n8n/issues/5676)) ([62f993c](https://github.com/n8n-io/n8n/commit/62f993c84f6ecf2f4d0431d505ba18a0253bd244))
* **core:** Manage version control settings ([#6079](https://github.com/n8n-io/n8n/issues/6079)) ([f3b4701](https://github.com/n8n-io/n8n/commit/f3b470186360dc3c3a3df599f0a9740183e86696))
* **core:** Upgrade google-timezones-json to use the correct timezone for Sao Paulo ([#6042](https://github.com/n8n-io/n8n/issues/6042)) ([b8cb5d7](https://github.com/n8n-io/n8n/commit/b8cb5d7f0b11fb138d5c4714bcc9e1d9b6366d76)), closes [#2647](https://github.com/n8n-io/n8n/issues/2647)
* **editor:** Add disable template experiment ([#5963](https://github.com/n8n-io/n8n/issues/5963)) ([a74284b](https://github.com/n8n-io/n8n/commit/a74284bac387338e870dc81ac33748af55521274))
* **editor:** Add SQL editor support ([#5517](https://github.com/n8n-io/n8n/issues/5517)) ([70aaf24](https://github.com/n8n-io/n8n/commit/70aaf2478461d9ceea98bc91dc935493fd6dbe24))
* **editor:** Enhance Node Creator actions view ([#5954](https://github.com/n8n-io/n8n/issues/5954)) ([390841b](https://github.com/n8n-io/n8n/commit/390841bbf0fdd4d536101593711a6658ea2784e4))
* **editor:** Version control (WIP) ([#6013](https://github.com/n8n-io/n8n/issues/6013)) ([0e0a064](https://github.com/n8n-io/n8n/commit/0e0a064fa7ae54a8a6b695bd4bb19da71334fea0))
* **editor:** Version control paywall (WIP) ([#6030](https://github.com/n8n-io/n8n/issues/6030)) ([ef79b03](https://github.com/n8n-io/n8n/commit/ef79b03f38460a20658c62fd35dbcaf6d266582f))
* **Google BigQuery Node:** Node improvements ([#4877](https://github.com/n8n-io/n8n/issues/4877)) ([9817a15](https://github.com/n8n-io/n8n/commit/9817a15da4c80425fb77273ed7c9acbe020f0f48))



## [0.225.2](https://github.com/n8n-io/n8n/compare/n8n@0.225.1...n8n@0.225.2) (2023-04-25)


### Bug Fixes

* **core:** Upgrade google-timezones-json to use the correct timezone for Sao Paulo ([#6042](https://github.com/n8n-io/n8n/issues/6042)) ([f93fd5a](https://github.com/n8n-io/n8n/commit/f93fd5aba2583e1c62efe8dcb423559413cf9c6a)), closes [#2647](https://github.com/n8n-io/n8n/issues/2647)
* **Code Node:** Update vm2 to address CVE-2023-30547 ([#6039](https://github.com/n8n-io/n8n/issues/6039)) ([f1ca4e2](https://github.com/n8n-io/n8n/commit/f1ca4e232865a0ee6ac178b11515de115b0bfd09))



# [0.224.4](https://github.com/n8n-io/n8n/compare/n8n@0.224.2...n8n@0.224.4) (2023-04-24)


### Bug Fixes

* **core:** Upgrade google-timezones-json to use the correct timezone for Sao Paulo ([#6042](https://github.com/n8n-io/n8n/issues/6042)) ([c23a592](https://github.com/n8n-io/n8n/commit/c23a5923f8df787758f756c529518c9e8b93b96e)), closes [#2647](https://github.com/n8n-io/n8n/issues/2647)
* **Code Node:** Update vm2 to address CVE-2023-30547 ([#6039](https://github.com/n8n-io/n8n/issues/6039)) ([6cd15bd](https://github.com/n8n-io/n8n/commit/6cd15bd889b6eec3b050cfe3c3b190707a09e898))



## [0.225.1](https://github.com/n8n-io/n8n/compare/n8n@0.225.0...n8n@0.225.1) (2023-04-20)


### Bug Fixes

* **editor:** Clean up demo and template callouts from workflows page ([#6023](https://github.com/n8n-io/n8n/issues/6023)) ([6ec1c45](https://github.com/n8n-io/n8n/commit/6ec1c45355807e62f31a707bada823cdc73bc719))
* **editor:** Fix memory leak in Node Detail View by correctly unsubscribing from event buses ([#6021](https://github.com/n8n-io/n8n/issues/6021)) ([1b9e047](https://github.com/n8n-io/n8n/commit/1b9e047ef5745f479e6693dca9696efbec32a7a6))
* **editor:** SettingsSidebar should disconnect from push when navigating away ([#6025](https://github.com/n8n-io/n8n/issues/6025)) ([e9f8cfe](https://github.com/n8n-io/n8n/commit/e9f8cfe82182ee0d7c8c2394551791793cc71f47))
* **Notion Node:** Update credential test to not require user permissions ([#6022](https://github.com/n8n-io/n8n/issues/6022)) ([6d02ae5](https://github.com/n8n-io/n8n/commit/6d02ae53cf1ec616abd47e434018bdf5e998f916))



## [0.224.2](https://github.com/n8n-io/n8n/compare/n8n@0.224.1...n8n@0.224.2) (2023-04-20)


### Bug Fixes

* **core:** Fix paired item returning wrong data ([#5898](https://github.com/n8n-io/n8n/issues/5898)) ([2a45441](https://github.com/n8n-io/n8n/commit/2a45441d8aa1e9069af09eb28b9b26b0c4abf96e))
* **core:** Make `getExecutionId` available on all nodes types ([#5990](https://github.com/n8n-io/n8n/issues/5990)) ([8373aab](https://github.com/n8n-io/n8n/commit/8373aab1fffc6f15e2a79462c97cd52cff277784))
* **editor:** Fix memory leak in Node Detail View by correctly unsubscribing from event buses ([#6021](https://github.com/n8n-io/n8n/issues/6021)) ([d8fce5b](https://github.com/n8n-io/n8n/commit/d8fce5b1cbcded5dcb652b1b5bf252555343d4b1))
* **editor:** Fix moving canvas on middle click preventing lasso selection ([#5996](https://github.com/n8n-io/n8n/issues/5996)) ([a7a5778](https://github.com/n8n-io/n8n/commit/a7a57782bbaadad342f592331b7b9d49aa0e62de))
* **editor:** SettingsSidebar should disconnect from push when navigating away ([#6025](https://github.com/n8n-io/n8n/issues/6025)) ([b475c8f](https://github.com/n8n-io/n8n/commit/b475c8f26aea9c108a8ea29826619925516c372f))
* **Google Sheets Trigger Node:** Return actual error message ([5e59141](https://github.com/n8n-io/n8n/commit/5e59141ec60566dbacea246402e57b13328a94b3))
* **HTTP Request Node:** Fix itemIndex in HTTP Request errors ([#5991](https://github.com/n8n-io/n8n/issues/5991)) ([4a521a4](https://github.com/n8n-io/n8n/commit/4a521a416e3fb85ba58d4ca4ad420b485c220d96))
* **Notion Node:** Update credential test to not require user permissions ([#6022](https://github.com/n8n-io/n8n/issues/6022)) ([14c9b5e](https://github.com/n8n-io/n8n/commit/14c9b5e6295a59b5ddbde0e07ba94250b50bcedf))



# [0.225.0](https://github.com/n8n-io/n8n/compare/n8n@0.224.0...n8n@0.225.0) (2023-04-19)


### Bug Fixes

* **core:** Fix broken API permissions in public API ([#5978](https://github.com/n8n-io/n8n/issues/5978)) ([49d838f](https://github.com/n8n-io/n8n/commit/49d838f628a124f3497165437a384e78d8a8ff63))
* **core:** Fix paired item returning wrong data ([#5898](https://github.com/n8n-io/n8n/issues/5898)) ([b13b7d7](https://github.com/n8n-io/n8n/commit/b13b7d73e7857fe9a264d9400adfa337907f659a))
* **core:** Improve SAML connection test result views ([#5981](https://github.com/n8n-io/n8n/issues/5981)) ([4c994fa](https://github.com/n8n-io/n8n/commit/4c994faec1ed6173d99f5b01efd9678e54e7eb49))
* **core:** Make `getExecutionId` available on all nodes types ([#5990](https://github.com/n8n-io/n8n/issues/5990)) ([c42820e](https://github.com/n8n-io/n8n/commit/c42820e82efe7365b5d7344bb3f474ba420ea7c9))
* **core:** Skip SAML onboarding for users with first- and lastname ([#5966](https://github.com/n8n-io/n8n/issues/5966)) ([8474cd3](https://github.com/n8n-io/n8n/commit/8474cd386ddfca9e9078b45af65af9299d63eb85))
* **editor:** Add padding to prepend input ([#5874](https://github.com/n8n-io/n8n/issues/5874)) ([cd89489](https://github.com/n8n-io/n8n/commit/cd894893aafe1fc25e0e556a9651ab458b50ae99))
* **editor:** Cleanup demo/video experiment ([#5974](https://github.com/n8n-io/n8n/issues/5974)) ([c171365](https://github.com/n8n-io/n8n/commit/c171365d2a613ea1fb9b08c22c54be29d1c8ade7))
* **editor:** Enterprise features missing with UM ([#5995](https://github.com/n8n-io/n8n/issues/5995)) ([f9a810a](https://github.com/n8n-io/n8n/commit/f9a810aaf7fd56beba1342016a96922e8b332951))
* **editor:** Fix moving canvas on middle click preventing lasso selection ([#5996](https://github.com/n8n-io/n8n/issues/5996)) ([3c2a569](https://github.com/n8n-io/n8n/commit/3c2a56928b46425822795cf1594133a538f47c21))
* **editor:** Make sure to redirect to blank canvas after personalisation modal ([#5980](https://github.com/n8n-io/n8n/issues/5980)) ([7c474d3](https://github.com/n8n-io/n8n/commit/7c474d3c92ecca8e44e8eea76ada69aa7e8f5987))
* **editor:** Only treat as CTRL pressed by default on touch devices for MouseEvent ([#5968](https://github.com/n8n-io/n8n/issues/5968)) ([536d810](https://github.com/n8n-io/n8n/commit/536d8109b02d1a0f771055c36ff0f45dae08281e))
* **editor:** Fix n8n-checkbox alignment ([#6004](https://github.com/n8n-io/n8n/issues/6004)) ([f544826](https://github.com/n8n-io/n8n/commit/f5448269ee9277f19b0943035d23ad0df1dcde67))
* **Code Node:** Handle user code returning `null` and `undefined` ([#5989](https://github.com/n8n-io/n8n/issues/5989)) ([a3664de](https://github.com/n8n-io/n8n/commit/a3664de3556f9f8159ed310a289ec12a4cd2c5c5))
* **Github Trigger Node:** Remove content_reference event ([#5830](https://github.com/n8n-io/n8n/issues/5830)) ([d288a91](https://github.com/n8n-io/n8n/commit/d288a918f17dad2d0e32cf2d66f94037c77679b3))
* **Google Sheets Trigger Node:** Return actual error message ([ba5b4eb](https://github.com/n8n-io/n8n/commit/ba5b4eb42fa1b609ddbe726d3e8655c1f9d28a2e))
* **HTTP Request Node:** Fix itemIndex in HTTP Request errors ([#5991](https://github.com/n8n-io/n8n/issues/5991)) ([b351c62](https://github.com/n8n-io/n8n/commit/b351c6265938a908f90237c834012cc19cf70dc3))
* **NocoDB Node:** Fix for updating or deleting rows with not default primary keys ([ee7f863](https://github.com/n8n-io/n8n/commit/ee7f86394eaf7aceee5521a4178c80a3c05cc27d))
* **OpenAI Node:** Update models to only show those supported ([#5805](https://github.com/n8n-io/n8n/issues/5805)) ([29959be](https://github.com/n8n-io/n8n/commit/29959be6883d48c0385f333b3d9798a8c7c91c43))
* **OpenAI Node:** Update OpenAI Text Moderate input placeholder text ([#5823](https://github.com/n8n-io/n8n/issues/5823)) ([6b9909b](https://github.com/n8n-io/n8n/commit/6b9909bd80f4b04ec877fe7ee9b8a2619392d220))


### Features

* **core:** Add variables feature ([#5602](https://github.com/n8n-io/n8n/issues/5602)) ([1bb9871](https://github.com/n8n-io/n8n/commit/1bb987140af8e835770a0ca45403e274a793f22c))
* **core:** Add versionControl feature flag ([#6000](https://github.com/n8n-io/n8n/issues/6000)) ([33299ca](https://github.com/n8n-io/n8n/commit/33299ca61aaec94714431a58286da4bb2cf829c1))
* **core:** Support for google service account in HTTP node ([0b48088](https://github.com/n8n-io/n8n/commit/0b48088296a7f826be3664f10c847b9dca753732))
* **editor:** Add Ask AI preview ([#5916](https://github.com/n8n-io/n8n/issues/5916)) ([f8f8374](https://github.com/n8n-io/n8n/commit/f8f8374506c3d0c2ad7cea73bb461b3f64a81be1))
* **GitLab Node:** Add Additional parameters for File List ([#5621](https://github.com/n8n-io/n8n/issues/5621)) ([3810039](https://github.com/n8n-io/n8n/commit/3810039da032ecbd038255316b3d8fa5ce5ef2df))
* **MySQL Node:** Overhaul ([0a53c95](https://github.com/n8n-io/n8n/commit/0a53c957c4d69270e10058cdd384e47c8e3c987e))



## [0.224.1](https://github.com/n8n-io/n8n/compare/n8n@0.224.0...n8n@0.224.1) (2023-04-14)


### Bug Fixes

* **core:** Fix broken API permissions in public API ([#5978](https://github.com/n8n-io/n8n/issues/5978)) ([b76ab31](https://github.com/n8n-io/n8n/commit/b76ab318f8919138391850738de99e592aa020a7))
* **editor:** Only treat as CTRL pressed by default on touch devices for MouseEvent ([#5968](https://github.com/n8n-io/n8n/issues/5968)) ([471be3b](https://github.com/n8n-io/n8n/commit/471be3b4a89e9967524a5d06212153bbf2b56537))



# [0.224.0](https://github.com/n8n-io/n8n/compare/n8n@0.223.0...n8n@0.224.0) (2023-04-12)


### Bug Fixes

* **Code Node:** Update vm2 to address CVE-2023-29017 ([#5947](https://github.com/n8n-io/n8n/issues/5947)) ([f0eba0a](https://github.com/n8n-io/n8n/commit/f0eba0a2f3be584363163abe2e30e8a57c9632f9))
* **core:** App should not crash with a custom rest endpoint ([#5911](https://github.com/n8n-io/n8n/issues/5911)) ([2881ee9](https://github.com/n8n-io/n8n/commit/2881ee9ecc0e3258cf025ad7f1f571be4f21d320)), closes [#5880](https://github.com/n8n-io/n8n/issues/5880)
* **core:** Do not execute `workflowExecuteBefore` hook when resuming executions from a waiting state ([#5727](https://github.com/n8n-io/n8n/issues/5727)) ([6689451](https://github.com/n8n-io/n8n/commit/6689451e8c939bb2714c42ada83acdc0a9af62b7))
* **core:** Fix issue where sub workflows would display as running forever after failure to start ([#5905](https://github.com/n8n-io/n8n/issues/5905)) ([3e382ef](https://github.com/n8n-io/n8n/commit/3e382ef85e966419dc71744b772d80c648583c5c))
* **core:** Update xml2js to address CVE-2023-0842 ([#5948](https://github.com/n8n-io/n8n/issues/5948)) ([3085ed9](https://github.com/n8n-io/n8n/commit/3085ed9beee603cdb496fc7fb39357f15e0710d0))
* **editor:** Drop mergeDeep in favor of lodash merge ([#5943](https://github.com/n8n-io/n8n/issues/5943)) ([0570514](https://github.com/n8n-io/n8n/commit/0570514b789c9fa020e96533b7c65bf45614c4d0))
* **HTTP Request Node:** Show detailed error message in the UI again ([#5959](https://github.com/n8n-io/n8n/issues/5959)) ([e79679c](https://github.com/n8n-io/n8n/commit/e79679c023d127458227d904dbdb4824a755b956))


### Features

* Create TOTP node ([#5901](https://github.com/n8n-io/n8n/issues/5901)) ([6cf74e4](https://github.com/n8n-io/n8n/commit/6cf74e412a87ccb255efea950cb458712554391d))
* **editor:** Add user activation survey ([#5677](https://github.com/n8n-io/n8n/issues/5677)) ([725393d](https://github.com/n8n-io/n8n/commit/725393dae625285ed91a7e4662eec1a425cf53f1))
* **editor:** SAML login disables Invite button ([#5922](https://github.com/n8n-io/n8n/issues/5922)) ([3fdc441](https://github.com/n8n-io/n8n/commit/3fdc4413c20f1fd345a5864d9a237b30e20813f0))
* **editor:** SAML paywall state ([#5906](https://github.com/n8n-io/n8n/issues/5906)) ([d40e86a](https://github.com/n8n-io/n8n/commit/d40e86aabc8c66a17b04cfe669ac27b4b281762a))



## [0.222.2](https://github.com/n8n-io/n8n/compare/n8n@0.222.1...n8n@0.222.2) (2023-04-11)


### Bug Fixes

* **Code Node:** Update vm2 to address CVE-2023-29017 ([#5947](https://github.com/n8n-io/n8n/issues/5947)) ([fc1fb28](https://github.com/n8n-io/n8n/commit/fc1fb2863f6df697ca4a098054f9638cf2bc97bc))
* **core:** Update xml2js to address CVE-2023-0842 ([#5948](https://github.com/n8n-io/n8n/issues/5948)) ([e903d61](https://github.com/n8n-io/n8n/commit/e903d6107112fca64b54dec76019720c9df6a66a))



## [0.221.3](https://github.com/n8n-io/n8n/compare/n8n@0.221.2...n8n@0.221.3) (2023-04-11)


### Bug Fixes

* **Code Node:** Update vm2 to address CVE-2023-29017 ([#5947](https://github.com/n8n-io/n8n/issues/5947)) ([4127e3f](https://github.com/n8n-io/n8n/commit/4127e3ff9d1d1ef8b76c557bf3b4799ab7aba7f7))
* **core:** Update xml2js to address CVE-2023-0842 ([#5948](https://github.com/n8n-io/n8n/issues/5948)) ([cf7a4b6](https://github.com/n8n-io/n8n/commit/cf7a4b65d3d828fbacd027de9c2bf2481883efa7))



# [0.223.0](https://github.com/n8n-io/n8n/compare/n8n@0.222.1...n8n@0.223.0) (2023-04-05)


### Bug Fixes

* Add droppable state for booleans when mapping ([#5838](https://github.com/n8n-io/n8n/issues/5838)) ([e3884ce](https://github.com/n8n-io/n8n/commit/e3884ce378e488905735fbfdb986aa26f1cf952b))
* **AWS SNS Node:** Fix an issue with messages failing to send if they contain certain characters ([#5807](https://github.com/n8n-io/n8n/issues/5807)) ([32c4eef](https://github.com/n8n-io/n8n/commit/32c4eef574a14ed599554382496a99a8240be74b))
* **Compare Datasets Node:** Fuzzy compare not comparing keys missing in one of inputs ([d1945d9](https://github.com/n8n-io/n8n/commit/d1945d9b72fc11e7201e22a7ae0399acf2ffd5f1))
* **Compare Datasets Node:** Support for dot notation in skip fields ([83e25c0](https://github.com/n8n-io/n8n/commit/83e25c066a845fc95c3474ae93f36993ca7ce699))
* **core:** `augmentObject` should clone Buffer/Uint8Array instead of wrapping them in a proxy ([#5902](https://github.com/n8n-io/n8n/issues/5902)) ([a721734](https://github.com/n8n-io/n8n/commit/a72173414d9d31ab1824f87713709818955b8956))
* **core:** `augmentObject` should use existing property descriptors whenever possible ([#5872](https://github.com/n8n-io/n8n/issues/5872)) ([6a1b7c3](https://github.com/n8n-io/n8n/commit/6a1b7c306bc9b7c469c5299af6beaf5af568b6b6))
* **core:** Deactivate active workflows during import ([#5840](https://github.com/n8n-io/n8n/issues/5840)) ([fa5bc81](https://github.com/n8n-io/n8n/commit/fa5bc814b04273cff817d4a94b1d1ec6685807e0))
* **core:** Do not mark duplicates as circular references in `jsonStringify` ([#5789](https://github.com/n8n-io/n8n/issues/5789)) ([18efaf3](https://github.com/n8n-io/n8n/commit/18efaf397a6bab8bd5dba881bbdfeceef8dbafb0))
* **core:** Do not user `util.types.isProxy` for tracking of augmented objects ([#5836](https://github.com/n8n-io/n8n/issues/5836)) ([aacbb54](https://github.com/n8n-io/n8n/commit/aacbb54bef0743a1c5c5e2467dd7e00e50e325de))
* **core:** Fix curl import error when no data ([085660d](https://github.com/n8n-io/n8n/commit/085660d7d7faf475b695724cabb6387c46adcc5f))
* **core:** Fix the issue of nodes not loading when run via npx ([#5888](https://github.com/n8n-io/n8n/issues/5888)) ([e47190b](https://github.com/n8n-io/n8n/commit/e47190b5607dfd1284a1d2c3b8f678e8032627de))
* **core:** Handle Date and RegExp correctly in jsonStringify ([#5812](https://github.com/n8n-io/n8n/issues/5812)) ([4f91525](https://github.com/n8n-io/n8n/commit/4f91525022716e7c1745185fae6fc2582a4252fb))
* **core:** Handle Date and RegExp objects in AugmentObject ([#5809](https://github.com/n8n-io/n8n/issues/5809)) ([6c35ffa](https://github.com/n8n-io/n8n/commit/6c35ffa82c45434dadee0354b75a901d3f3d6e98))
* **core:** Improve axios error handling in nodes ([#5891](https://github.com/n8n-io/n8n/issues/5891)) ([a260c05](https://github.com/n8n-io/n8n/commit/a260c05fa859c0bdd90f9abdecac59fd35978c55))
* **core:** Password reset should pass in the correct values to external hooks ([#5842](https://github.com/n8n-io/n8n/issues/5842)) ([5bcab8f](https://github.com/n8n-io/n8n/commit/5bcab8fcbea546cd57ef728131f9e16cc57e675d))
* **core:** Prevent augmentObject from creating infinitely deep proxies ([#5893](https://github.com/n8n-io/n8n/issues/5893)) ([31cd04c](https://github.com/n8n-io/n8n/commit/31cd04c4769b92c7f19ae8babf5df2deddef1fb3)), closes [#5848](https://github.com/n8n-io/n8n/issues/5848)
* **core:** Service account private key as a password field ([739b9b0](https://github.com/n8n-io/n8n/commit/739b9b07f0e364f98d3c2d0ce8911cd4f53e8455))
* **core:** Update lock file ([#5801](https://github.com/n8n-io/n8n/issues/5801)) ([06d7a46](https://github.com/n8n-io/n8n/commit/06d7a46bdcd2173835ede762aff3c37b21f0a530))
* **core:** Use table-prefixes in queries in import commands ([#5887](https://github.com/n8n-io/n8n/issues/5887)) ([ddbfcc7](https://github.com/n8n-io/n8n/commit/ddbfcc7d93cc3645fc3bb0f0de059ac76adaa475))
* **core:** Waiting workflows not stopping ([#5811](https://github.com/n8n-io/n8n/issues/5811)) ([744c3fd](https://github.com/n8n-io/n8n/commit/744c3fd21130b6ee3c722df3fab096b169fd0ff8))
* **Date & Time Node:** Add info box at top of date and time explaining expressions ([b7a20dd](https://github.com/n8n-io/n8n/commit/b7a20dd3a2e69a8e4e8ba76c63a6b1f4c26b6a87))
* **Date & Time Node:** Convert luxon DateTime object to ISO ([7710652](https://github.com/n8n-io/n8n/commit/77106520c8942c746bb1ddffcddcde68a7059805))
* **editor:** Add $if, $min, $max to root expression autocomplete ([#5858](https://github.com/n8n-io/n8n/issues/5858)) ([a13866e](https://github.com/n8n-io/n8n/commit/a13866e233430ec6aa9fcaa5f3861b3a4470b458))
* **editor:** Curb overeager item access linting ([#5865](https://github.com/n8n-io/n8n/issues/5865)) ([3ae6933](https://github.com/n8n-io/n8n/commit/3ae69337eeb1f8a4d698f2099bb190c49cc5f8fd))
* **editor:** Disable Grammarly in expression editors ([#5826](https://github.com/n8n-io/n8n/issues/5826)) ([ddc8f30](https://github.com/n8n-io/n8n/commit/ddc8f30e6d410f7453395f17754b8ee9a546d9b7))
* **editor:** Disable password reset on desktop with no user management ([#5853](https://github.com/n8n-io/n8n/issues/5853)) ([96533a9](https://github.com/n8n-io/n8n/commit/96533a995c1e7ac653d3f135f954619b098bb609))
* **editor:** Fix connection lost hover text not showing ([#5828](https://github.com/n8n-io/n8n/issues/5828)) ([b69129b](https://github.com/n8n-io/n8n/commit/b69129bd78689bd56c3a9b07c2e30f58735347d1))
* **editor:** Fix focused state in Code node editor ([#5869](https://github.com/n8n-io/n8n/issues/5869)) ([48446f5](https://github.com/n8n-io/n8n/commit/48446f5d674c335716c86e30079eb35c75e32b66))
* **editor:** Fix issue preventing execution preview loading when in an iframe ([#5817](https://github.com/n8n-io/n8n/issues/5817)) ([d86e693](https://github.com/n8n-io/n8n/commit/d86e693019db1fa034d43f8e7e18df09f785b2e1))
* **editor:** Fix loading executions in long execution list ([#5843](https://github.com/n8n-io/n8n/issues/5843)) ([5c9343c](https://github.com/n8n-io/n8n/commit/5c9343c7c0febdeb3dfa449d6b18d744d909724a))
* **editor:** Fix mapping with special characters ([#5837](https://github.com/n8n-io/n8n/issues/5837)) ([f8f584c](https://github.com/n8n-io/n8n/commit/f8f584c136da8ad8b17f82f6f4e95f0d69014b40))
* **editor:** Prevent error from showing-up when duplicating unsaved workflow ([#5833](https://github.com/n8n-io/n8n/issues/5833)) ([0b0024d](https://github.com/n8n-io/n8n/commit/0b0024d7222ac1f6f7872b26eceefab93a17ef22))
* **editor:** Prevent NDV schema view pagination ([#5844](https://github.com/n8n-io/n8n/issues/5844)) ([1eba478](https://github.com/n8n-io/n8n/commit/1eba4788f26d0f5472fa4156b317d8b14d19b927))
* **editor:** Show correct status on canceled executions ([#5813](https://github.com/n8n-io/n8n/issues/5813)) ([d0788ee](https://github.com/n8n-io/n8n/commit/d0788ee8e150167a65561552494046d8e506f93c))
* **editor:** Support backspacing with modifier key ([#5845](https://github.com/n8n-io/n8n/issues/5845)) ([11692c5](https://github.com/n8n-io/n8n/commit/11692c55f381f17a7a137262d85dfd6c7fda7ad5))
* **Gmail Node:** Gmail luxon object support, fix for timestamp ([2b9ca0d](https://github.com/n8n-io/n8n/commit/2b9ca0d240b403a5f12b115956bbc11672f3a04a))
* **Google Sheets Node:** Fix insertOrUpdate cell update with object ([0625e2e](https://github.com/n8n-io/n8n/commit/0625e2e6bc67092848f719f8fede87af0f3df891))
* **HTML Extract Node:** Support for dot notation in JSON property ([0da3b96](https://github.com/n8n-io/n8n/commit/0da3b96cfc943bf8036a48df946873fb32f3f5d9))
* **HTTP Request Node:** Detect mime-type from streaming responses ([#5896](https://github.com/n8n-io/n8n/issues/5896)) ([69efde7](https://github.com/n8n-io/n8n/commit/69efde7a094b0bf3e3ca04b456ba3a792838a0b9))
* **HTTP Request Node:** Fix AWS credentials to stop removing url params for STS ([#5790](https://github.com/n8n-io/n8n/issues/5790)) ([a1306c6](https://github.com/n8n-io/n8n/commit/a1306c690398828ed9acb72af0161c4ff827b217))
* **HTTP Request Node:** Refresh token properly on never fail option ([#5861](https://github.com/n8n-io/n8n/issues/5861)) ([33c67f4](https://github.com/n8n-io/n8n/commit/33c67f45ba959b90c8bebbe0b27b2a7c4152a116))
* **HTTP Request Node:** Support for dot notation in JSON body ([b29cf9a](https://github.com/n8n-io/n8n/commit/b29cf9a2492a444cb1dd72e74c9ed1d8722bbc5a))
* **HubSpot Trigger Node:** Developer API key is required for webhooks ([e11a30a](https://github.com/n8n-io/n8n/commit/e11a30a640700d2bc53919422cb8ddbf66aafddd))
* **LinkedIn Node:** Update the version of the API ([#5720](https://github.com/n8n-io/n8n/issues/5720)) ([18d2e7c](https://github.com/n8n-io/n8n/commit/18d2e7cd57745f0969b0df383572b3874fe65f2c))
* **Redis Node:** Fix issue with hash set not working as expected ([#5832](https://github.com/n8n-io/n8n/issues/5832)) ([db25441](https://github.com/n8n-io/n8n/commit/db2544146f646ec9a2c38787bc94eafc1edb1228))
* **Set Node:** Convert string to number ([b408550](https://github.com/n8n-io/n8n/commit/b408550e9f486351198f0ce5c10895c42df45835))


### Features

* **core:** Convert eventBus controller to decorator style and improve permissions ([#5779](https://github.com/n8n-io/n8n/issues/5779)) ([f15f4bd](https://github.com/n8n-io/n8n/commit/f15f4bdcf204fa43a652022babf03e577602b2b5))
* **core:** Prevent non owners password reset when saml is enabled ([#5788](https://github.com/n8n-io/n8n/issues/5788)) ([2216455](https://github.com/n8n-io/n8n/commit/221645576087e4cd828b34ea33e874e1bff5f34a))
* **core:** Read ephemeral license from environment and clean up ee flags ([#5808](https://github.com/n8n-io/n8n/issues/5808)) ([83aef17](https://github.com/n8n-io/n8n/commit/83aef1712070c29fea5d0522c95b1208af4cd2e4))
* **editor:** Allow `tab` to accept completion ([#5855](https://github.com/n8n-io/n8n/issues/5855)) ([1b8c35a](https://github.com/n8n-io/n8n/commit/1b8c35ab87ce7ea24d00d13faddba9daf9f2ab39))
* **editor:** Enable saving workflow when node details view is open ([#5856](https://github.com/n8n-io/n8n/issues/5856)) ([0a59002](https://github.com/n8n-io/n8n/commit/0a59002ef878ff8836d3ca63956f7a444d329d0b))
* **editor:** SSO onboarding ([#5756](https://github.com/n8n-io/n8n/issues/5756)) ([04f8600](https://github.com/n8n-io/n8n/commit/04f8600bbd220204b5e5a90f22c3dc9c137afb54))
* **editor:** SSO setup ([#5736](https://github.com/n8n-io/n8n/issues/5736)) ([f4e5949](https://github.com/n8n-io/n8n/commit/f4e59499fc0168295c5df20b1525c7ecea4ea15b)), closes [#5899](https://github.com/n8n-io/n8n/issues/5899)
* **Filter Node:** Show discarded items ([f7f9d91](https://github.com/n8n-io/n8n/commit/f7f9d915b174d5c17efa918032741d4fa6da85e9))
* **HTTP Request Node:** Follow redirects by default ([#5895](https://github.com/n8n-io/n8n/issues/5895)) ([f7e610b](https://github.com/n8n-io/n8n/commit/f7e610b15c4699880edffd7f10f223e820052784))
* **Postgres Node:** Overhaul node ([07dc0e4](https://github.com/n8n-io/n8n/commit/07dc0e4b4075f1fac98d5685a99a38187bca741b))
* **ServiceNow Node:** Add support for work notes when updating an incident ([#5791](https://github.com/n8n-io/n8n/issues/5791)) ([1409f5d](https://github.com/n8n-io/n8n/commit/1409f5d65262b9783e690408f5dabd074c709f22))
* **SSH Node:** Hide the private key within the ssh credential ([#5871](https://github.com/n8n-io/n8n/issues/5871)) ([d877361](https://github.com/n8n-io/n8n/commit/d87736103d09042d2f74e74b57be429f2ca3550d))



## [0.222.1](https://github.com/n8n-io/n8n/compare/n8n@0.222.0...n8n@0.222.1) (2023-04-04)


### Bug Fixes

* **AWS SNS Node:** Fix an issue with messages failing to send if they contain certain characters ([#5807](https://github.com/n8n-io/n8n/issues/5807)) ([f0954b9](https://github.com/n8n-io/n8n/commit/f0954b94e164f0ff3e809849731137cf479670a4))
* **core:** `augmentObject` should clone Buffer/Uint8Array instead of wrapping them in a proxy ([#5902](https://github.com/n8n-io/n8n/issues/5902)) ([a877b02](https://github.com/n8n-io/n8n/commit/a877b025b8c93a31822e7ccb5b935dca00595439))
* **core:** `augmentObject` should use existing property descriptors whenever possible ([#5872](https://github.com/n8n-io/n8n/issues/5872)) ([b1ee8f4](https://github.com/n8n-io/n8n/commit/b1ee8f4d991ffc5017894f588e9bd21f652f23c6))
* **core:** Fix the issue of nodes not loading when run via npx ([#5888](https://github.com/n8n-io/n8n/issues/5888)) ([163446c](https://github.com/n8n-io/n8n/commit/163446c674d07c060eaa0d7ec54a087a4cb671d5))
* **core:** Improve axios error handling in nodes ([#5891](https://github.com/n8n-io/n8n/issues/5891)) ([f0a51a0](https://github.com/n8n-io/n8n/commit/f0a51a0b7671945b84e18774483dc7079f559845))
* **core:** Password reset should pass in the correct values to external hooks ([#5842](https://github.com/n8n-io/n8n/issues/5842)) ([3bf267c](https://github.com/n8n-io/n8n/commit/3bf267c14757fa67dcfa0edf0b4db74ab1b7415c))
* **core:** Prevent augmentObject from creating infinitely deep proxies ([#5893](https://github.com/n8n-io/n8n/issues/5893)) ([6906b00](https://github.com/n8n-io/n8n/commit/6906b00b0e734dbe59d1a3a91f07ec1007166b72)), closes [#5848](https://github.com/n8n-io/n8n/issues/5848)
* **core:** Use table-prefixes in queries in import commands ([#5887](https://github.com/n8n-io/n8n/issues/5887)) ([de58fb9](https://github.com/n8n-io/n8n/commit/de58fb9860d37a39a1e8963e304b8fc87f234bf6))
* **editor:** Fix focused state in Code node editor ([#5869](https://github.com/n8n-io/n8n/issues/5869)) ([3be37e2](https://github.com/n8n-io/n8n/commit/3be37e25a52983b43b4eed3847922e99f2bf07bc))
* **editor:** Fix loading executions in long execution list ([#5843](https://github.com/n8n-io/n8n/issues/5843)) ([d5d9f58](https://github.com/n8n-io/n8n/commit/d5d9f58f1777040c63a2a0aa3c0d7bf632dc7b26))
* **editor:** Show correct status on canceled executions ([#5813](https://github.com/n8n-io/n8n/issues/5813)) ([00181cd](https://github.com/n8n-io/n8n/commit/00181cd803f5a0cca50b5fc1ab84d0a26dd618ae))
* **Gmail Node:** Gmail luxon object support, fix for timestamp ([695fabb](https://github.com/n8n-io/n8n/commit/695fabb28465d01caa85aefb1e873f88720ce304))
* **HTTP Request Node:** Detect mime-type from streaming responses ([#5896](https://github.com/n8n-io/n8n/issues/5896)) ([0be1292](https://github.com/n8n-io/n8n/commit/0be129254e96c822dceddbfffaf36e0e6b2ef5e8))
* **HubSpot Trigger Node:** Developer API key is required for webhooks ([918c79c](https://github.com/n8n-io/n8n/commit/918c79c137f781764f11ad3a33ead337efce681a))
* **Set Node:** Convert string to number ([72eea0d](https://github.com/n8n-io/n8n/commit/72eea0dfb9e679bde95996d99684e23d081db5a7))



# [0.222.0](https://github.com/n8n-io/n8n/compare/n8n@0.221.2...n8n@0.222.0) (2023-03-30)


### Bug Fixes

* **core:** Assign properties.success earlier to set executionStatus correctly ([#5773](https://github.com/n8n-io/n8n/issues/5773)) ([d33a1ac](https://github.com/n8n-io/n8n/commit/d33a1ac1e9a13985ff84f9271f75ebf368339b6d))
* **core:** Do not mark duplicates as circular references in `jsonStringify` ([#5789](https://github.com/n8n-io/n8n/issues/5789)) ([f5183c6](https://github.com/n8n-io/n8n/commit/f5183c640109fb4c9552d6b2786f8ebc0e35ca4c))
* **core:** Do not user `util.types.isProxy` for tracking of augmented objects ([#5836](https://github.com/n8n-io/n8n/issues/5836)) ([3e413f2](https://github.com/n8n-io/n8n/commit/3e413f2f80d6fa349dc6f6ea1b49027ae163df80))
* **core:** Ensure that all non-lazy-loaded community nodes get post-processed correctly ([#5782](https://github.com/n8n-io/n8n/issues/5782)) ([30aeeb7](https://github.com/n8n-io/n8n/commit/30aeeb70b43ff3916ad79abbe49512a27e50d01d))
* **core:** Force-upgrade `decode-uri-component` to address CVE-2022-38900 ([#5734](https://github.com/n8n-io/n8n/issues/5734)) ([8dd7f6e](https://github.com/n8n-io/n8n/commit/8dd7f6e1d4ac29b450a0af17d545ffd17038b005))
* **core:** Force-upgrade `http-cache-semantics` to address CVE-2022-25881 ([#5733](https://github.com/n8n-io/n8n/issues/5733)) ([f7401fb](https://github.com/n8n-io/n8n/commit/f7401fb6133b9bf18f3825304c478d767e69fe27))
* **core:** Handle Date and RegExp correctly in jsonStringify ([#5812](https://github.com/n8n-io/n8n/issues/5812)) ([753cfb8](https://github.com/n8n-io/n8n/commit/753cfb8b08ff68cc30e6e30959fd0900a44dae21))
* **core:** Handle Date and RegExp objects in AugmentObject ([#5809](https://github.com/n8n-io/n8n/issues/5809)) ([e6d4e72](https://github.com/n8n-io/n8n/commit/e6d4e729a063cdbbf648c2815c3e55ddddef2b58))
* **core:** Improve axios error handling in nodes ([#5699](https://github.com/n8n-io/n8n/issues/5699)) ([33d9784](https://github.com/n8n-io/n8n/commit/33d97843194c1cddfd27356c279c0f7a8c2674d3))
* **core:** Improve community nodes loading ([#5608](https://github.com/n8n-io/n8n/issues/5608)) ([161de11](https://github.com/n8n-io/n8n/commit/161de110cedf2d5d8bc345349d4364ea202e2abd))
* **core:** Initialize queue in the webhook server as well ([#5766](https://github.com/n8n-io/n8n/issues/5766)) ([e67ad29](https://github.com/n8n-io/n8n/commit/e67ad2962589b445592641a588024c02b4d99d3f))
* **core:** Persist CurrentAuthenticationMethod setting change ([#5762](https://github.com/n8n-io/n8n/issues/5762)) ([4498c60](https://github.com/n8n-io/n8n/commit/4498c6013dc5b4646b1e3fdba3adef42bfc87952))
* **core:** Remove circular refs from Code and push msg ([#5741](https://github.com/n8n-io/n8n/issues/5741)) ([b6d8a0f](https://github.com/n8n-io/n8n/commit/b6d8a0f98526bfc98a3d9a722dafce4a53e715ec))
* **core:** Require Auth on icons and nodes/credentials types static files ([#5745](https://github.com/n8n-io/n8n/issues/5745)) ([5dda3f2](https://github.com/n8n-io/n8n/commit/5dda3f2c61b107ec24557c4bf7de284234e406ab))
* **core:** Return SAML service provider urls with config ([#5759](https://github.com/n8n-io/n8n/issues/5759)) ([ac18c0b](https://github.com/n8n-io/n8n/commit/ac18c0b9ebb3a5a736fa72985ce5ae2cdab3b270))
* **core:** Service account private key as a password field ([2b28470](https://github.com/n8n-io/n8n/commit/2b28470fb98a5810ce0d20fe995e2864230005d3))
* **core:** Upgrade `luxon` to address CVE-2023-22467 ([#5731](https://github.com/n8n-io/n8n/issues/5731)) ([469ce32](https://github.com/n8n-io/n8n/commit/469ce32957ac5e4d342db17a2f680ca65c21d44f))
* **core:** Upgrade `simple-git` to address CVE-2022-25912 ([#5730](https://github.com/n8n-io/n8n/issues/5730)) ([4a4e2be](https://github.com/n8n-io/n8n/commit/4a4e2be96c0ce096d100e08823aa6b256719c267))
* **core:** Upgrade `sqlite3` to address CVE-2022-43441 ([#5732](https://github.com/n8n-io/n8n/issues/5732)) ([fd81c74](https://github.com/n8n-io/n8n/commit/fd81c742519882b04f98d25ca41b3fac16dbea8b))
* **core:** Upgrade convict to address CVE-2023-0163 ([#5729](https://github.com/n8n-io/n8n/issues/5729)) ([564bc03](https://github.com/n8n-io/n8n/commit/564bc03d3fab59e4fe7fa904d5deeeb16da85af9))
* **core:** Waiting workflows not stopping ([#5811](https://github.com/n8n-io/n8n/issues/5811)) ([8f50bb6](https://github.com/n8n-io/n8n/commit/8f50bb6ed13688d8a81a171c1f1fb9e85847f138))
* **editor:** Fix connection lost hover text not showing ([#5828](https://github.com/n8n-io/n8n/issues/5828)) ([a2f4a05](https://github.com/n8n-io/n8n/commit/a2f4a05af7f20e007ef16357d71af6a0dbade55c))
* **editor:** Fix issue preventing execution preview loading when in an iframe ([#5817](https://github.com/n8n-io/n8n/issues/5817)) ([d19a973](https://github.com/n8n-io/n8n/commit/d19a9732b7da188017e2141b3deed7ea004c04a6))
* **editor:** Use credentials when fetching node and credential types ([#5760](https://github.com/n8n-io/n8n/issues/5760)) ([d3a34ab](https://github.com/n8n-io/n8n/commit/d3a34ab71bd7fc494fb90cda1aa9827a55c5ed69))
* **Google Sheets Node:** Fix insertOrUpdate cell update with object ([1797cda](https://github.com/n8n-io/n8n/commit/1797cdab5b9e7f23c9f62ce7c6c34c1c2c26b07e))
* **HTTP Request Node:** Add streaming to binary response  ([#5701](https://github.com/n8n-io/n8n/issues/5701)) ([199a91b](https://github.com/n8n-io/n8n/commit/199a91b3981d40b7181f00702c938b9fa58d1ece)), closes [#5663](https://github.com/n8n-io/n8n/issues/5663)
* **HTTP Request Node:** Fix AWS credentials to automatically deconstruct the url ([#5751](https://github.com/n8n-io/n8n/issues/5751)) ([d30b892](https://github.com/n8n-io/n8n/commit/d30b89239587562974cc87ae2e29fe57acddf79e))
* **HTTP Request Node:** Fix AWS credentials to stop removing url params for STS ([#5790](https://github.com/n8n-io/n8n/issues/5790)) ([2c25959](https://github.com/n8n-io/n8n/commit/2c25959e595a48d9ae55c462bd47e014d8c43598))
* **Split In Batches Node:** Roll back changes in v1 and create v2 ([#5747](https://github.com/n8n-io/n8n/issues/5747)) ([135b0d3](https://github.com/n8n-io/n8n/commit/135b0d3e27705b07fb1e9c39a47ac4b70c1bc25d))
* Update Posthog no-capture ([#5693](https://github.com/n8n-io/n8n/issues/5693)) ([a732374](https://github.com/n8n-io/n8n/commit/a732374f24354e0c1f36247f4476e743b0fc78e5))


### Features

* Add test overrides ([#5642](https://github.com/n8n-io/n8n/issues/5642)) ([696e43a](https://github.com/n8n-io/n8n/commit/696e43a919334d982188cc1f86d3e1b76da6a362))
* **core:** Improve ldap/saml toggle and tests ([#5771](https://github.com/n8n-io/n8n/issues/5771)) ([47ee357](https://github.com/n8n-io/n8n/commit/47ee357059bb6d87607165d3c24ce0c99cf8bfc9))
* **core:** Limit user invites when SAML is enabled ([#5761](https://github.com/n8n-io/n8n/issues/5761)) ([57748b7](https://github.com/n8n-io/n8n/commit/57748b71e5cd1399ccaedb9a115b821b34cf55e5))
* **core:** Make OAuth2 error handling consistent with success handling ([#5555](https://github.com/n8n-io/n8n/issues/5555)) ([40aacf9](https://github.com/n8n-io/n8n/commit/40aacf9279c00c4e3c27669fc38a0ca196a788a4))
* **editor:** Fix ResourceLocator dropdown style ([#5714](https://github.com/n8n-io/n8n/issues/5714)) ([02810a9](https://github.com/n8n-io/n8n/commit/02810a9ba3e792a2ec8966a2ca3bf7394740bf24))
* Execution custom data saving and filtering ([#5496](https://github.com/n8n-io/n8n/issues/5496)) ([d78a41d](https://github.com/n8n-io/n8n/commit/d78a41db5420ff6711c30899aa2d71a85049374c)), closes [#5739](https://github.com/n8n-io/n8n/issues/5739)
* **Filter Node:** New node ([cc9fe7b](https://github.com/n8n-io/n8n/commit/cc9fe7b91ffc4ea72c25e1242e0e477112cb283e))



## [0.221.2](https://github.com/n8n-io/n8n/compare/n8n@0.221.1...n8n@0.221.2) (2023-03-24)


### Bug Fixes

* **core:** Assign properties.success earlier to set executionStatus correctly ([6c7772a](https://github.com/n8n-io/n8n/commit/6c7772a0b3276ffe9e5ab8029e17a0ed743ee5a7))



## [0.221.1](https://github.com/n8n-io/n8n/compare/n8n@0.221.0...n8n@0.221.1) (2023-03-23)


### Bug Fixes

* **core:** Initialize queue in the webhook server as well ([163859b](https://github.com/n8n-io/n8n/commit/163859b87a19f3795e2689ce8eba2e2ce6766684))



# [0.221.0](https://github.com/n8n-io/n8n/compare/n8n@0.220.0...n8n@0.221.0) (2023-03-23)


### Bug Fixes

* **core:** Fix calling error workflows in main mode recovery ([#5698](https://github.com/n8n-io/n8n/issues/5698)) ([e0ea97a](https://github.com/n8n-io/n8n/commit/e0ea97af8d7aaa014680f5f9d5702d1cafd49757))
* **core:** Fix telemetry execution status for manual workflows executions ([#5712](https://github.com/n8n-io/n8n/issues/5712)) ([a28396e](https://github.com/n8n-io/n8n/commit/a28396ee91bfbccc6596812606c237a8e2c34088))
* **core:** Return saml attributes after connection test ([#5717](https://github.com/n8n-io/n8n/issues/5717)) ([be172cb](https://github.com/n8n-io/n8n/commit/be172cb720c8a44ebd1f0b86dddab321e1e3c9fd))
* **editor:** Disable tooltip for display modes that don't support mapping ([#5715](https://github.com/n8n-io/n8n/issues/5715)) ([fb8755e](https://github.com/n8n-io/n8n/commit/fb8755ea3c720c98f002a6756c39b8fed11482c0))
* **editor:** Fix execution list item selection ([#5606](https://github.com/n8n-io/n8n/issues/5606)) ([7a352ef](https://github.com/n8n-io/n8n/commit/7a352efff944c52062412e53ea2c1a034a25f908))
* **editor:** Fix for large notifications being cut off ([#5705](https://github.com/n8n-io/n8n/issues/5705)) ([c07f838](https://github.com/n8n-io/n8n/commit/c07f838ce60dc33261fe3e1b5e7dd6fe05f1d63b))
* **editor:** Fix redo in code and expression editor ([#5708](https://github.com/n8n-io/n8n/issues/5708)) ([cd7a55b](https://github.com/n8n-io/n8n/commit/cd7a55ba5aeb83d1e540a65b5c6b2c74fd742461))
* **editor:** Fix the canvas node distance when automatically injecting manual trigger ([#5716](https://github.com/n8n-io/n8n/issues/5716)) ([cb2ba97](https://github.com/n8n-io/n8n/commit/cb2ba97f3837b572e237da1256b9f2ee376767a9))
* **HTTP Request Node:** Fix AWS credentials to automatically deconstruct the url ([#5751](https://github.com/n8n-io/n8n/issues/5751)) ([4ac944a](https://github.com/n8n-io/n8n/commit/4ac944af3028b70ae600000300c16de77c1af1d5))
* **Split In Batches Node:** Roll back changes in v1 and create v2 ([#5747](https://github.com/n8n-io/n8n/issues/5747)) ([cefec77](https://github.com/n8n-io/n8n/commit/cefec7739b6da820d64f9476476e1901d4f386bf))


### Features

* **core:** Augment data instead of copying it ([#5487](https://github.com/n8n-io/n8n/issues/5487)) ([0876c38](https://github.com/n8n-io/n8n/commit/0876c38aaeb8355141fecbc14e84cdda0b2c737b))
* **editor:** Move canvas by holding Space or Middle mouse button ([#5719](https://github.com/n8n-io/n8n/issues/5719)) ([19dded1](https://github.com/n8n-io/n8n/commit/19dded18c9a588a30b9ac1fc274dcd967e9b7b6b))
* **editor:** Recommend and pre-select auth type with overrides ([#5684](https://github.com/n8n-io/n8n/issues/5684)) ([f59b591](https://github.com/n8n-io/n8n/commit/f59b591c93ecd7cbd279668abe6494ef2b88c831))
* **editor:** SSO login button ([#5615](https://github.com/n8n-io/n8n/issues/5615)) ([6916628](https://github.com/n8n-io/n8n/commit/6916628a9f11e07cbcdf390f747f396fb0ef9e3c))
* **QuickChart Node:** Add QuickChart node ([#3572](https://github.com/n8n-io/n8n/issues/3572)) ([233f1fa](https://github.com/n8n-io/n8n/commit/233f1fa7ec230e92e868de0247e315aa6a705ead))



## [0.220.1](https://github.com/n8n-io/n8n/compare/n8n@0.220.0...n8n@0.220.1) (2023-03-22)


### Bug Fixes

* **Split In Batches Node:** Roll back changes in v1 and create v2 ([#5747](https://github.com/n8n-io/n8n/issues/5747)) ([6d1c88e](https://github.com/n8n-io/n8n/commit/6d1c88ea8c2e5dc72c6e6edeeeef52dc1fba4075))



# [0.220.0](https://github.com/n8n-io/n8n/compare/n8n@0.219.1...n8n@0.220.0) (2023-03-16)


### Bug Fixes

* **core:** Initialize License and LDAP in the correct order ([#5673](https://github.com/n8n-io/n8n/issues/5673)) ([90afa5e](https://github.com/n8n-io/n8n/commit/90afa5e55f96fbe46417f4be8f764795fb5c2225))
* **editor:** Display correct error message for env access ([#5634](https://github.com/n8n-io/n8n/issues/5634)) ([5f238ea](https://github.com/n8n-io/n8n/commit/5f238ea6413d25704a5865d339401117e81dbbab))
* **editor:** Fix autocomplete for complex expresions ([#5695](https://github.com/n8n-io/n8n/issues/5695)) ([11bf260](https://github.com/n8n-io/n8n/commit/11bf260bf164c6c9dffe71b875fde139c93f905d))
* **editor:** Fix owner set-up checkbox wording ([#5697](https://github.com/n8n-io/n8n/issues/5697)) ([58232be](https://github.com/n8n-io/n8n/commit/58232bec618edd403f18527913c489bfa11f570b))
* **editor:** Properly handle mapping of dragged expression if it contains hyphen ([#5703](https://github.com/n8n-io/n8n/issues/5703)) ([7025efe](https://github.com/n8n-io/n8n/commit/7025efe8654a8a55ff10e2105ddc6ce2dc5a89d6))
* **Metabase Node:** Fix issue with question results not correctly being returned ([#5665](https://github.com/n8n-io/n8n/issues/5665)) ([d1e3c19](https://github.com/n8n-io/n8n/commit/d1e3c192ba9e2dfd852e570e88f6135d42d2ed45))


### Features

* **core:** Improve SAML connection test ([#5680](https://github.com/n8n-io/n8n/issues/5680)) ([ef07528](https://github.com/n8n-io/n8n/commit/ef07528cc21f06ee52f93bafb34ac54a244609f9))
* **editor:** Add basic Datatable and Pagination components ([#5652](https://github.com/n8n-io/n8n/issues/5652)) ([29f2629](https://github.com/n8n-io/n8n/commit/29f2629716e3693372ec9a4572113a3f3721ff5e))
* **editor:** Add support for schema view in the NDV output ([#5688](https://github.com/n8n-io/n8n/issues/5688)) ([541850f](https://github.com/n8n-io/n8n/commit/541850f95f1c42fc16d9aeee3a3fef68a4b77082))
* **editor:** Do not show actions panel for single-action nodes ([#5683](https://github.com/n8n-io/n8n/issues/5683)) ([de1db92](https://github.com/n8n-io/n8n/commit/de1db927cbdc5fc8ef7d697cccbd8603f66391ea))
* **Item Lists Node:** Update actions ([#5648](https://github.com/n8n-io/n8n/issues/5648)) ([332d50c](https://github.com/n8n-io/n8n/commit/332d50c5f1f8ba63b87325799360adecdbaa06bf))
* **OpenAI Node:** Add support for gpt4 on chat completion ([#5692](https://github.com/n8n-io/n8n/issues/5692)) ([ba73fff](https://github.com/n8n-io/n8n/commit/ba73fff27d2972093746acc3f7016c7420e23459))
* **Split In Batches Node:** Make it easy to combine processed data ([#5655](https://github.com/n8n-io/n8n/issues/5655)) ([2f7639e](https://github.com/n8n-io/n8n/commit/2f7639e9e4b10f08c5cb1c4916fc6ae031375cf3))



## [0.215.4](https://github.com/n8n-io/n8n/compare/n8n@0.215.3...n8n@0.215.4) (2023-03-14)


### Bug Fixes

* **core:** Revert `isPending` check on the user entity ([#5571](https://github.com/n8n-io/n8n/issues/5571)) ([6d2c50d](https://github.com/n8n-io/n8n/commit/6d2c50dfed0aeffa2afdb09f5aac80c0e25a6a06))



## [0.214.5](https://github.com/n8n-io/n8n/compare/n8n@0.214.4...n8n@0.214.5) (2023-03-14)


### Bug Fixes

* **core:** Revert `isPending` check on the user entity ([#5571](https://github.com/n8n-io/n8n/issues/5571)) ([b94af03](https://github.com/n8n-io/n8n/commit/b94af0384243d634683212d5199316067956f628))



## [0.219.1](https://github.com/n8n-io/n8n/compare/n8n@0.219.0...n8n@0.219.1) (2023-03-10)


### Bug Fixes

* **HTTP Request Node:** Remove streaming response  ([#5663](https://github.com/n8n-io/n8n/issues/5663)) ([974d57d](https://github.com/n8n-io/n8n/commit/974d57dfed78489d3f22c8c63e0ea624c637bfe0))



# [0.219.0](https://github.com/n8n-io/n8n/compare/n8n@0.218.0...n8n@0.219.0) (2023-03-09)


### Bug Fixes

* **core:** Allow serving icons for custom nodes with npm scoped names ([#5626](https://github.com/n8n-io/n8n/issues/5626)) ([45ccdd3](https://github.com/n8n-io/n8n/commit/45ccdd3bb5d5601ccc60438d96aadb40cb87588b))
* **core:** Rename advancedFilters to advancedExecutionFilters ([#5643](https://github.com/n8n-io/n8n/issues/5643)) ([419969c](https://github.com/n8n-io/n8n/commit/419969c0d761b1ac7870e7821c0398ecfca1f0ce))
* **editor:** Fix ElButton overrides ([#5605](https://github.com/n8n-io/n8n/issues/5605)) ([2eba050](https://github.com/n8n-io/n8n/commit/2eba05046141bd13145f95c6a1ec1e6fb95b37c2))
* **editor:** Only fetch new versions at app launch ([#5647](https://github.com/n8n-io/n8n/issues/5647)) ([5b9c521](https://github.com/n8n-io/n8n/commit/5b9c521d04bc34a9f84be966a4646f23c56ca3da))
* Fetch credentials on workflows view to include in duplicated workflows ([#5532](https://github.com/n8n-io/n8n/issues/5532)) ([493f7a1](https://github.com/n8n-io/n8n/commit/493f7a1c92d77d3c75fc311892e53f43e1fb367f))
* Fix color discrepancies for executions list items ([#5640](https://github.com/n8n-io/n8n/issues/5640)) ([c81656d](https://github.com/n8n-io/n8n/commit/c81656d149764dc398b93d3eb8626a402eddb0ef))
* **OpenAI Node:** Fix issue with expressions not working with chat complete ([#5609](https://github.com/n8n-io/n8n/issues/5609)) ([e949db3](https://github.com/n8n-io/n8n/commit/e949db352526033394083476077519598dd8061c))
* **OpenAI Node:** Simplify code ([#5618](https://github.com/n8n-io/n8n/issues/5618)) ([1c65bff](https://github.com/n8n-io/n8n/commit/1c65bff31d86ea76ff5fca10341e71389d4de7b5))


### Features

* **Cal Trigger Node:** Update to support v2 webhooks ([#5331](https://github.com/n8n-io/n8n/issues/5331)) ([2889e53](https://github.com/n8n-io/n8n/commit/2889e53b3767f2a61ee7fb3ea9fe1db7c65aaf70))
* **core:** Add advancedFilters feature flag ([#5638](https://github.com/n8n-io/n8n/issues/5638)) ([0b5ef09](https://github.com/n8n-io/n8n/commit/0b5ef09e7cbd0c80a4b79311976b5c06c2be8747))
* **core:** Add SAML post and test endpoints ([#5595](https://github.com/n8n-io/n8n/issues/5595)) ([523fa71](https://github.com/n8n-io/n8n/commit/523fa71705c0408c6c60c7cb5135323e3488e8c9))
* **core:** Add SAML XML validation ([#5600](https://github.com/n8n-io/n8n/issues/5600)) ([ca66ec8](https://github.com/n8n-io/n8n/commit/ca66ec8f4d5ab0e427390b1f1874fb668bc53479))
* **core:** Limit user changes when saml is enabled ([#5577](https://github.com/n8n-io/n8n/issues/5577)) ([b517959](https://github.com/n8n-io/n8n/commit/b5179597f3ec4ae468b2eb91969fa56322088e6f))
* **core:** Refactor and add SAML preferences for service provider instance ([#5637](https://github.com/n8n-io/n8n/issues/5637)) ([6f27b44](https://github.com/n8n-io/n8n/commit/6f27b445ca2307b94ffc7d4eeb24e76d63516a19))
* **editor:** Do not automatically add manual trigger on node plus ([#5644](https://github.com/n8n-io/n8n/issues/5644)) ([ac2f89a](https://github.com/n8n-io/n8n/commit/ac2f89a18a4c25ef1b39bcacc624884de9197fdf))
* **editor:** Redirect users to canvas if they don't have any workflows ([#5629](https://github.com/n8n-io/n8n/issues/5629)) ([354edf6](https://github.com/n8n-io/n8n/commit/354edf6886fa3cc5a59d317dcab59cc75e62dc2d))
* **HTTP Request Node:** Move from Binary Buffer to Binary streaming ([#5610](https://github.com/n8n-io/n8n/issues/5610)) ([ce0d9d2](https://github.com/n8n-io/n8n/commit/ce0d9d2bede7d87b97e18c45b63ea31ecf592255))
* **Mattermost Node:** Add self signed certificate support ([#5630](https://github.com/n8n-io/n8n/issues/5630)) ([01a2160](https://github.com/n8n-io/n8n/commit/01a2160b3b8d36509f4b2871249a3f45358cf692))
* **Microsoft SQL Node:** Add support for self signed certificates ([#5160](https://github.com/n8n-io/n8n/issues/5160)) ([971d5ae](https://github.com/n8n-io/n8n/commit/971d5ae8f5d2bfe319fc700fee2bcf597ea4c07e))
* **Mindee Node:** Add support for v4 API ([#5559](https://github.com/n8n-io/n8n/issues/5559)) ([e56fbfe](https://github.com/n8n-io/n8n/commit/e56fbfef3ebb50706f24ab07505a0031f361d9b1))
* **Slack Node:** Move from Binary Buffer to Binary streaming ([#5612](https://github.com/n8n-io/n8n/issues/5612)) ([9420b0f](https://github.com/n8n-io/n8n/commit/9420b0fdf8ccccb95780c8c97e2b5d14cc4d513e))



## [0.217.1](https://github.com/n8n-io/n8n/compare/n8n@0.217.0...n8n@0.217.1) (2023-02-24)


### Bug Fixes

* **core:** Revert `isPending` check on the user entity ([#5571](https://github.com/n8n-io/n8n/issues/5571)) ([5282fd2](https://github.com/n8n-io/n8n/commit/5282fd266c26e7053ceb887addceed26b741f995))



# [0.218.0](https://github.com/n8n-io/n8n/compare/n8n@0.217.2...n8n@0.218.0) (2023-03-02)


### Bug Fixes

* **core:** Fix execution pruning queries ([#5562](https://github.com/n8n-io/n8n/issues/5562)) ([88de661](https://github.com/n8n-io/n8n/commit/88de6613bda2d4f133410b05c5c2a8d2f1ba838f))
* **core:** Fix Filtering of Workflow by Tags ([#5570](https://github.com/n8n-io/n8n/issues/5570)) ([ea2035b](https://github.com/n8n-io/n8n/commit/ea2035b5102853d2aa7e5e01d70e06acf4abd3d8))
* **core:** Revert `isPending` check on the user entity ([#5571](https://github.com/n8n-io/n8n/issues/5571)) ([a19ec6a](https://github.com/n8n-io/n8n/commit/a19ec6ac94ac2ed6ab96bf7fe2216cdd2324228b))
* Fix issues with nodes missing in nodes panel ([#5599](https://github.com/n8n-io/n8n/issues/5599)) ([5040fea](https://github.com/n8n-io/n8n/commit/5040fea93ecc36017d25f237fe9b3e23bc9d623d))
* Fix mapping paths when appending to empty expression ([#5591](https://github.com/n8n-io/n8n/issues/5591)) ([1f7b478](https://github.com/n8n-io/n8n/commit/1f7b478920ee2b8b4f6affcfd0b42f79b2cd8cd1))
* **Item Lists Node:** Tweak item list summarize field naming  ([#5572](https://github.com/n8n-io/n8n/issues/5572)) ([aa2beaa](https://github.com/n8n-io/n8n/commit/aa2beaa80076fc06360828e466a3dc05e7caddbe))
* Prevent executions from displaying as running forever ([#5563](https://github.com/n8n-io/n8n/issues/5563)) ([46d9ac6](https://github.com/n8n-io/n8n/commit/46d9ac6c6f55a505716c8951f93b149713bcbe35))
* Show Execute Workflow node in nodes panel ([#5583](https://github.com/n8n-io/n8n/issues/5583)) ([d6d1c07](https://github.com/n8n-io/n8n/commit/d6d1c07a53bb903b19c49ea11b9d36993fde7c33))
* Show RabbitMQ node in nodes panel ([#5598](https://github.com/n8n-io/n8n/issues/5598)) ([4f5013f](https://github.com/n8n-io/n8n/commit/4f5013ff53294579fb9e47f90ae08e9a6bc76b75))
* Stop showing mapping hint after mapping ([#5586](https://github.com/n8n-io/n8n/issues/5586)) ([eac4275](https://github.com/n8n-io/n8n/commit/eac4275a7ebfa6ccc6258261b1b3ac36c9df9d88))


### Features

* Add distribution test tracking ([#5588](https://github.com/n8n-io/n8n/issues/5588)) ([91bd014](https://github.com/n8n-io/n8n/commit/91bd0146f35ba3f38c862cac9c5ad48ff7cd38e8))
* Add events to enable onboarding checklist ([#5536](https://github.com/n8n-io/n8n/issues/5536)) ([20c4919](https://github.com/n8n-io/n8n/commit/20c49195131399aa6ab0c6938eebb5e2733c6710))
* **core:** Add SAML login setup ([#5515](https://github.com/n8n-io/n8n/issues/5515)) ([40a934b](https://github.com/n8n-io/n8n/commit/40a934bbb4f6eed80aa5c1de6814c0e0eea65ebd))
* **core:** Add SAML settings and consolidate LDAP under SSO ([#5574](https://github.com/n8n-io/n8n/issues/5574)) ([31cc8de](https://github.com/n8n-io/n8n/commit/31cc8de8297454cad4307e008b3b915475c0a889))
* **editor:** Add missing documentation to autocomplete items for inline code editor ([#5560](https://github.com/n8n-io/n8n/issues/5560)) ([ae63440](https://github.com/n8n-io/n8n/commit/ae634407a47de33d77cb81ae7ce11362e8485fd4))
* **editor:** Show parameter hint on multilines ([#5014](https://github.com/n8n-io/n8n/issues/5014)) ([1942fd8](https://github.com/n8n-io/n8n/commit/1942fd82323183fb31af671ccb8d22f6a4798d7f))
* **Jira Software Node:** Support binary streaming for very large binary files ([#5589](https://github.com/n8n-io/n8n/issues/5589)) ([f61d779](https://github.com/n8n-io/n8n/commit/f61d779667f25a411b51ee61ddd3fe4698f05934))
* **OpenAI Node:** Add support for ChatGPT ([#5596](https://github.com/n8n-io/n8n/issues/5596)) ([06c5ecb](https://github.com/n8n-io/n8n/commit/06c5ecbdf3031a7773e698294ae701a7e501ef50))
* **Telegram Node:** Add Parse Mode to Send Document operation ([#5554](https://github.com/n8n-io/n8n/issues/5554)) ([f3c943e](https://github.com/n8n-io/n8n/commit/f3c943ef8191bd16e16a61ffbed6b1caca0d75a5))



## [0.217.2](https://github.com/n8n-io/n8n/compare/n8n@0.217.1...n8n@0.217.2) (2023-02-27)


### Bug Fixes

* **core:** Fix execution pruning queries ([#5562](https://github.com/n8n-io/n8n/issues/5562)) ([2137ae2](https://github.com/n8n-io/n8n/commit/2137ae23d789af765a7555028e9651029f88cadc))
* **core:** Fix Filtering of Workflow by Tags ([#5570](https://github.com/n8n-io/n8n/issues/5570)) ([51eedac](https://github.com/n8n-io/n8n/commit/51eedaccd427ec11b12fbf43d9dd3f0ebe9633d2))
* **core:** Revert `isPending` check on the user entity ([#5571](https://github.com/n8n-io/n8n/issues/5571)) ([43eec66](https://github.com/n8n-io/n8n/commit/43eec66828b2e03418402742c9695e08b1165bdd))



## [0.217.1](https://github.com/n8n-io/n8n/compare/n8n@0.217.0...n8n@0.217.1) (2023-02-24)


### Bug Fixes

* Prevent executions from displaying as running forever ([#5563](https://github.com/n8n-io/n8n/issues/5563)) ([b30db10](https://github.com/n8n-io/n8n/commit/b30db10d898fa791d99d13192ef411cace4f7c05))



# [0.217.0](https://github.com/n8n-io/n8n/compare/n8n@0.216.1...n8n@0.217.0) (2023-02-23)


### Bug Fixes

* **Baserow Node:** Fix issue with get all not correctly using filters ([#5519](https://github.com/n8n-io/n8n/issues/5519)) ([ee21b7a](https://github.com/n8n-io/n8n/commit/ee21b7a1cfed17936eb6bf50221b7f9983dd38e6))
* **Compare Datasets Node:** UI tweaks and fixes ([7ecd5e5](https://github.com/n8n-io/n8n/commit/7ecd5e59eca01ca2b1a01e0a3e3871bd5d322eea))
* **core:** Do not allow arbitrary path traversal in BinaryDataManager ([#5523](https://github.com/n8n-io/n8n/issues/5523)) ([eef2574](https://github.com/n8n-io/n8n/commit/eef257406730a989ec8e7a056c3d4234300fdb25))
* **core:** Do not allow arbitrary path traversal in the credential-translation endpoint ([#5522](https://github.com/n8n-io/n8n/issues/5522)) ([f0f8d59](https://github.com/n8n-io/n8n/commit/f0f8d59fee223c6bc9f8459890ed4a31ef8cb0af))
* **core:** Do not explicitly bypass auth on urls containing `.svg` ([#5525](https://github.com/n8n-io/n8n/issues/5525)) ([f58573d](https://github.com/n8n-io/n8n/commit/f58573dba30eba8fe3d844d1b7b2dbbb8d51b8b5))
* **core:** Do not remove empty output connections arrays in PurgeInvalidWorkflowConnections migration ([#5546](https://github.com/n8n-io/n8n/issues/5546)) ([0fbb3f0](https://github.com/n8n-io/n8n/commit/0fbb3f0f026432f1aea87b106a0c1f732f93c792))
* **core:** Fix execution status filters ([#5533](https://github.com/n8n-io/n8n/issues/5533)) ([17eff4d](https://github.com/n8n-io/n8n/commit/17eff4d7d6692bfdc251bfa16ce7334858642ce5))
* **core:** User update endpoint should only allow updating email, firstName, and lastName ([#5526](https://github.com/n8n-io/n8n/issues/5526)) ([510855d](https://github.com/n8n-io/n8n/commit/510855d9581f07e5081a7bc11377cd6216ba7edf))
* **Discord Node:** Fix wrong error message being displayed ([#5547](https://github.com/n8n-io/n8n/issues/5547)) ([e251439](https://github.com/n8n-io/n8n/commit/e2514393335e555af47c9aca4f81b31608df9cb5))
* **Discourse Node:** Fix issue with credential test not working ([#5520](https://github.com/n8n-io/n8n/issues/5520)) ([b3e1793](https://github.com/n8n-io/n8n/commit/b3e1793ac0f304ea72d565097b6766bc278e1238))
* **editor:** Apply correct IRunExecutionData to finished workflow ([#5552](https://github.com/n8n-io/n8n/issues/5552)) ([e2d7c18](https://github.com/n8n-io/n8n/commit/e2d7c1804f2d5da15d96edeefd50c5b8e2753fd1))
* **editor:** Fix an issue with zoom and canvas nodes connections ([#5548](https://github.com/n8n-io/n8n/issues/5548)) ([4998ab2](https://github.com/n8n-io/n8n/commit/4998ab23508adf9a244885509b2d5c7c9c9c48f0))
* **editor:** Fix unexpected date rendering on front-end ([#5528](https://github.com/n8n-io/n8n/issues/5528)) ([684d717](https://github.com/n8n-io/n8n/commit/684d71752064e25143e09666e539b91b3dcd5f71))
* **editor:** Remove 'crashed' status from filter ([#5524](https://github.com/n8n-io/n8n/issues/5524)) ([7c517cb](https://github.com/n8n-io/n8n/commit/7c517cb5300481908dd653426089a6a9291e79ca))
* fix typo in error messages when a property does not exist ([#4310](https://github.com/n8n-io/n8n/issues/4310)) ([3af3db1](https://github.com/n8n-io/n8n/commit/3af3db160b5798fe948159b6f3dd48ec743512e7))
* Fixes an issue when saving an active workflow without triggers would cause n8n to be stuck ([#5513](https://github.com/n8n-io/n8n/issues/5513)) ([75a094a](https://github.com/n8n-io/n8n/commit/75a094a8c03afc40b7872cd2115d82e69455286e))
* **Google Calendar Node:** Fix incorrect labels for start and end times when getting all events ([#5529](https://github.com/n8n-io/n8n/issues/5529)) ([f965469](https://github.com/n8n-io/n8n/commit/f965469e13a45d3a7b796dfd6be44573bf8b13d0))
* **Postgres Node:** Fix for tables containing field named json ([5d74a2f](https://github.com/n8n-io/n8n/commit/5d74a2f89a31ee1a386a52d0d71858f73d734e31))
* **S3 Node:** Fix issue with get many buckets not outputting data ([#5514](https://github.com/n8n-io/n8n/issues/5514)) ([1c47677](https://github.com/n8n-io/n8n/commit/1c476770a778b7d034924db847a8757c383bd281))


### Features

* Add new event hooks ([#5530](https://github.com/n8n-io/n8n/issues/5530)) ([d47d008](https://github.com/n8n-io/n8n/commit/d47d0086cc2b0af5338598de1fc496b9d825f9a4))
* Add Required path name mapping to multiple nodes ([#5369](https://github.com/n8n-io/n8n/issues/5369)) ([f1589d4](https://github.com/n8n-io/n8n/commit/f1589d4f0f9f7cc7beec12d9f6598f8286484989))
* **core:** Add configurable execution history limit ([#5505](https://github.com/n8n-io/n8n/issues/5505)) ([db70293](https://github.com/n8n-io/n8n/commit/db702932f3f2b14a097e7f4364c06cbb4f001ebc))
* **core:** Add execution runData recovery and status field ([#5112](https://github.com/n8n-io/n8n/issues/5112)) ([d143f3f](https://github.com/n8n-io/n8n/commit/d143f3f2ec9ce42cfa4db2b41dab019b7b42f379))
* **core:** Add saml feature flag ([#5494](https://github.com/n8n-io/n8n/issues/5494)) ([3a9c257](https://github.com/n8n-io/n8n/commit/3a9c257f55a87890c7456601de13f182cec89fde))
* Deprecate Read Binary File node ([#5490](https://github.com/n8n-io/n8n/issues/5490)) ([11b4671](https://github.com/n8n-io/n8n/commit/11b467137e7652c03c0578654b19dbc157b23220))
* **editor:** Unify regular and trigger node creator panels ([#5315](https://github.com/n8n-io/n8n/issues/5315)) ([9a1e7b5](https://github.com/n8n-io/n8n/commit/9a1e7b52f7ce698f1492af15d0139fb015ba5d30))
* Hide sensitive value in Auth Header Credentials and Auth Query Credentials ([#5534](https://github.com/n8n-io/n8n/issues/5534)) ([4a209e1](https://github.com/n8n-io/n8n/commit/4a209e1dd98ea4b43d0a4d9cd688615cd6d4d5dd))
* Support feature flag evaluation server side ([#5511](https://github.com/n8n-io/n8n/issues/5511)) ([26a20ed](https://github.com/n8n-io/n8n/commit/26a20ed47e8f580504b80150d7550ecb9a49be0d))



## [0.216.2](https://github.com/n8n-io/n8n/compare/n8n@0.216.1...n8n@0.216.2) (2023-02-23)


### Bug Fixes

* **core:** Do not remove empty output connections arrays in PurgeInvalidWorkflowConnections migration ([#5546](https://github.com/n8n-io/n8n/issues/5546)) ([ac86abe](https://github.com/n8n-io/n8n/commit/ac86abe2457d9f54fcd23ac0c8d5f39d565bdcdf))



## [0.215.3](https://github.com/n8n-io/n8n/compare/n8n@0.215.2...n8n@0.215.3) (2023-02-23)


### Bug Fixes

* **core:** Do not allow arbitrary path traversal in BinaryDataManager ([#5523](https://github.com/n8n-io/n8n/issues/5523)) ([f7079da](https://github.com/n8n-io/n8n/commit/f7079daecd210a3a2a94e07c4782d15ee2a995e0))
* **core:** Do not allow arbitrary path traversal in the credential-translation endpoint ([#5522](https://github.com/n8n-io/n8n/issues/5522)) ([14d2a88](https://github.com/n8n-io/n8n/commit/14d2a88120c966a6493c3a64a7a2925af0731b8f))
* **core:** Do not explicitly bypass auth on urls containing `.svg` ([#5525](https://github.com/n8n-io/n8n/issues/5525)) ([0b568ee](https://github.com/n8n-io/n8n/commit/0b568ee5c3d3259aaa43f757ded5583bf9d1e221))
* **core:** Do not remove empty output connections arrays in PurgeInvalidWorkflowConnections migration ([#5546](https://github.com/n8n-io/n8n/issues/5546)) ([a31cb05](https://github.com/n8n-io/n8n/commit/a31cb05fecb3c7fcb8f3def33206bb7676358561))
* **core:** User update endpoint should only allow updating email, firstName, and lastName ([#5526](https://github.com/n8n-io/n8n/issues/5526)) ([d530e20](https://github.com/n8n-io/n8n/commit/d530e20669e90e12a2d2895ae31d0018a53b817a))



## [0.214.4](https://github.com/n8n-io/n8n/compare/n8n@0.214.3...n8n@0.214.4) (2023-02-23)


### Bug Fixes

* **core:** Do not allow arbitrary path traversal in BinaryDataManager ([#5523](https://github.com/n8n-io/n8n/issues/5523)) ([df3f23e](https://github.com/n8n-io/n8n/commit/df3f23e2b8103a15632521e4ba6cf332693acf81))
* **core:** Do not allow arbitrary path traversal in the credential-translation endpoint ([#5522](https://github.com/n8n-io/n8n/issues/5522)) ([397e42d](https://github.com/n8n-io/n8n/commit/397e42d63e80577a0b897873a1d2f19533e27da7))
* **core:** Do not explicitly bypass auth on urls containing `.svg` ([#5525](https://github.com/n8n-io/n8n/issues/5525)) ([a8ca2b1](https://github.com/n8n-io/n8n/commit/a8ca2b1aea687256c7d7d3525a2c50659935d7b8))
* **core:** Do not remove empty output connections arrays in PurgeInvalidWorkflowConnections migration ([#5546](https://github.com/n8n-io/n8n/issues/5546)) ([e6a554f](https://github.com/n8n-io/n8n/commit/e6a554f884d0d8d1e5c3890745986ecc179846d5))
* **core:** User update endpoint should only allow updating email, firstName, and lastName ([#5526](https://github.com/n8n-io/n8n/issues/5526)) ([d622827](https://github.com/n8n-io/n8n/commit/d6228276a26d9dc1bf2b2c5452bc0644b6df0c63))



## [0.216.1](https://github.com/n8n-io/n8n/compare/n8n@0.216.0...n8n@0.216.1) (2023-02-21)


### Bug Fixes

* **core:** Do not allow arbitrary path traversal in BinaryDataManager ([#5523](https://github.com/n8n-io/n8n/issues/5523)) ([40b9784](https://github.com/n8n-io/n8n/commit/40b97846483fe7c58229c156acb66f43a5a79dc3))
* **core:** Do not allow arbitrary path traversal in the credential-translation endpoint ([#5522](https://github.com/n8n-io/n8n/issues/5522)) ([fb07d77](https://github.com/n8n-io/n8n/commit/fb07d77106bb4933758c63bbfb87f591bf4a27dd))
* **core:** Do not explicitly bypass auth on urls containing `.svg` ([#5525](https://github.com/n8n-io/n8n/issues/5525)) ([27adea7](https://github.com/n8n-io/n8n/commit/27adea70459329fc0dddabee69e10c9d1453835f))
* **core:** User update endpoint should only allow updating email, firstName, and lastName ([#5526](https://github.com/n8n-io/n8n/issues/5526)) ([5599221](https://github.com/n8n-io/n8n/commit/5599221007cb09cb81f0623874fafc6cd481384c))



# [0.216.0](https://github.com/n8n-io/n8n/compare/n8n@0.215.2...n8n@0.216.0) (2023-02-16)


### Bug Fixes

* **Bubble Node:** Fix pagination issue when returning all objects ([#5483](https://github.com/n8n-io/n8n/issues/5483)) ([1a20fd9](https://github.com/n8n-io/n8n/commit/1a20fd9f46495e32508d74dbb9ccaaa0f6194a07))
* **core:** Fix data transformation function that are reported not to work properly ([#5338](https://github.com/n8n-io/n8n/issues/5338)) ([0cf45bc](https://github.com/n8n-io/n8n/commit/0cf45bc4c862c7544e69af4981d4607bf0b530e3))
* **core:** Remove unnecessary info from `GET /workflows` response ([#5311](https://github.com/n8n-io/n8n/issues/5311)) ([a2c6ea9](https://github.com/n8n-io/n8n/commit/a2c6ea9e110e51debf137707b52eb7fedbc0032b))
* **HTTP Request Node:** Ignore empty body for auto detect json ([#5215](https://github.com/n8n-io/n8n/issues/5215)) ([af70337](https://github.com/n8n-io/n8n/commit/af703371fc96dcfdd8f418201d3880f124cfcfc4))


### Features

* Add workflow and credential sharing access e2e tests ([#5463](https://github.com/n8n-io/n8n/issues/5463)) ([246189f](https://github.com/n8n-io/n8n/commit/246189f6dae2ce96dabd900ce0a192de731cc6aa))
* **editor:** Add correct credential owner contact details for readonly credentials ([#5208](https://github.com/n8n-io/n8n/issues/5208)) ([36108f8](https://github.com/n8n-io/n8n/commit/36108f82a1c1657c3959225d0635255668bf0af6))
* **editor:** Add most important native props and methods to autocomplete ([#5486](https://github.com/n8n-io/n8n/issues/5486)) ([6592d14](https://github.com/n8n-io/n8n/commit/6592d144d1fb680b34240ce57a6615b06de5cde5))
* **editor:** Update to personalization survey v4 ([#5474](https://github.com/n8n-io/n8n/issues/5474)) ([6265f3a](https://github.com/n8n-io/n8n/commit/6265f3a27a076f6c3c24d0fb323e44c471d85b23))
* **Github Node:** Use resource locator component ([#5489](https://github.com/n8n-io/n8n/issues/5489)) ([00ac4c3](https://github.com/n8n-io/n8n/commit/00ac4c308a4d96a0f93401402dd92bbbd087f082))
* **Github Trigger Node:** Use resource locator component ([#5253](https://github.com/n8n-io/n8n/issues/5253)) ([a3d8fac](https://github.com/n8n-io/n8n/commit/a3d8fac73a8a93d6b7f769e1386276e34066a1b7))
* **Notion Node:** Add icon support for page and database page creation ([#5468](https://github.com/n8n-io/n8n/issues/5468)) ([71cba06](https://github.com/n8n-io/n8n/commit/71cba06b7c1ee8ed42a4dacc2d8114df119339dc))
* **Slack Node:** Add support for manually inputting a channel name ([#5488](https://github.com/n8n-io/n8n/issues/5488)) ([7954ed3](https://github.com/n8n-io/n8n/commit/7954ed3cfbd4d8d0611c0cc51385b49cc80282a6))
* Update telemetry api endpoints ([#5482](https://github.com/n8n-io/n8n/issues/5482)) ([3de49e8](https://github.com/n8n-io/n8n/commit/3de49e8f7894e628b722e2a0c62e8739b1de6be9))



## [0.215.2](https://github.com/n8n-io/n8n/compare/n8n@0.215.1...n8n@0.215.2) (2023-02-14)


### Bug Fixes

* **core:** Fix the issue with test webhooks getting removed incorrectly ([#5466](https://github.com/n8n-io/n8n/issues/5466)) ([4dc458e](https://github.com/n8n-io/n8n/commit/4dc458eca5587cf7765bed6fd384d47a31e66e2c)), closes [/github.com/n8n-io/n8n/pull/5443/files#diff-b386248ff00977749c873ed85821c241b773e9740d7e7adf94e05b73b350ed74L152](https://github.com//github.com/n8n-io/n8n/pull/5443/files/issues/diff-b386248ff00977749c873ed85821c241b773e9740d7e7adf94e05b73b350ed74L152)



## [0.215.1](https://github.com/n8n-io/n8n/compare/n8n@0.215.0...n8n@0.215.1) (2023-02-11)


### Bug Fixes

* **core:** Fix issue that worker and webhook service close directly ([#5461](https://github.com/n8n-io/n8n/issues/5461)) ([3396556](https://github.com/n8n-io/n8n/commit/339655611fcf05ebdf9be7c452bc1164333f122e))
* **core:** Handle versioned custom nodes correctly ([#5313](https://github.com/n8n-io/n8n/issues/5313)) ([59f5c42](https://github.com/n8n-io/n8n/commit/59f5c4221efd6f8733bfb5ab41a0834332e9b9e4))



# [0.215.0](https://github.com/n8n-io/n8n/compare/n8n@0.214.3...n8n@0.215.0) (2023-02-10)


### Bug Fixes

* **ActiveCampaign Node:** Fix additional fields not being sent when updating account contacts ([#5216](https://github.com/n8n-io/n8n/issues/5216)) ([333a817](https://github.com/n8n-io/n8n/commit/333a817a8ef202d4133f2796b066e6a8ec414719))
* **core:** Disable transactions on sqlite migrations that use `PRAGMA foreign_keys` ([#5392](https://github.com/n8n-io/n8n/issues/5392)) ([3a435f7](https://github.com/n8n-io/n8n/commit/3a435f7057ac4e48945bd1b3a4efea0397f026a0))
* **core:** Expression extension failing with optional chaining ([#5370](https://github.com/n8n-io/n8n/issues/5370)) ([c7b58e0](https://github.com/n8n-io/n8n/commit/c7b58e0ed19869a4f47c666cc895ed72fe20e8e4))
* **core:** Fix import command for workflows with old format(pre UM) ([#5403](https://github.com/n8n-io/n8n/issues/5403)) ([fdf47a9](https://github.com/n8n-io/n8n/commit/fdf47a96dee8883b811249e1e427b764cab15004))
* **core:** Stop copying icons to cache ([#5419](https://github.com/n8n-io/n8n/issues/5419)) ([f23fb92](https://github.com/n8n-io/n8n/commit/f23fb9269660721aadd34cbb5bb958d7aaf0bcb2))
* **editor:** Prevent creation of input connections for nodes without input slot ([#5425](https://github.com/n8n-io/n8n/issues/5425)) ([018f8a3](https://github.com/n8n-io/n8n/commit/018f8a3510b280b08d95037f9b6b870748170f3e))
* Error workflow now correctly checks for subworkflow permissions ([#5390](https://github.com/n8n-io/n8n/issues/5390)) ([c8245b9](https://github.com/n8n-io/n8n/commit/c8245b9f872fd2c85ecaaa0da426b3ef9cb03113))
* **Linear Node:** Fix issue with Issue States not loading correctly ([#5435](https://github.com/n8n-io/n8n/issues/5435)) ([57a2b9c](https://github.com/n8n-io/n8n/commit/57a2b9cceb52cbed905459e6ae92007e00a335cc))
* MySQL migration parses database contents if necessary (fix for MariaDB) ([#5441](https://github.com/n8n-io/n8n/issues/5441)) ([2eb72a6](https://github.com/n8n-io/n8n/commit/2eb72a6c9f447f77f78f6d0ab392ebec5515f58c))


### Features

* Change desktop UM experience ([#5312](https://github.com/n8n-io/n8n/issues/5312)) ([5e3e70b](https://github.com/n8n-io/n8n/commit/5e3e70b83bf905c39f23a213f953bc42d7eed357))
* **core:** Add support for WebSockets as an alternative to Server-Sent Events ([#5443](https://github.com/n8n-io/n8n/issues/5443)) ([538984d](https://github.com/n8n-io/n8n/commit/538984dc2f95fe2089f99deefcee3352e4ccd144))
* **Edit Image Node:** Allow WebP as an image format ([#5420](https://github.com/n8n-io/n8n/issues/5420)) ([94f2b2a](https://github.com/n8n-io/n8n/commit/94f2b2a26fca3987715e49352dd3e6f75b8bd6e2))
* **editor:** Add `Object` global completions ([#5407](https://github.com/n8n-io/n8n/issues/5407)) ([d7b3923](https://github.com/n8n-io/n8n/commit/d7b3923c2f5e02680170b132ba0e7cc59cb67cf6))
* **editor:** Bring completions to HTML editor ([#5382](https://github.com/n8n-io/n8n/issues/5382)) ([a07de04](https://github.com/n8n-io/n8n/commit/a07de049a2105e1c2f749958a281cedbf918c39a))
* **HubSpot Trigger Node:** Add conversation events ([#5408](https://github.com/n8n-io/n8n/issues/5408)) ([aeaa663](https://github.com/n8n-io/n8n/commit/aeaa6636201f0ad98603d1abd602bdf6072e8a11))



## [0.214.3](https://github.com/n8n-io/n8n/compare/n8n@0.214.2...n8n@0.214.3) (2023-02-09)

* **editor:** Prevent creation of input connections for nodes without input slot ([#5425](https://github.com/n8n-io/n8n/issues/5425)) ([b57ec1d](https://github.com/n8n-io/n8n/commit/b57ec1d6abbae9e23ae5f473d70674aa14701bce))


## [0.214.2](https://github.com/n8n-io/n8n/compare/n8n@0.214.1...n8n@0.214.2) (2023-02-06)


### Bug Fixes


* **editor:** Correctly show OAuth reconnect button ([#5384](https://github.com/n8n-io/n8n/issues/5384)) ([6482688](https://github.com/n8n-io/n8n/commit/6482688ee04621744451c67f6d6e3292e925bb8d))
* **editor:** Fix resolvable highlighting for HTML editor ([#5379](https://github.com/n8n-io/n8n/issues/5379)) ([31130d5](https://github.com/n8n-io/n8n/commit/31130d5257f253d9be21fe62d668231e27ecbd52))


## [0.214.1](https://github.com/n8n-io/n8n/compare/n8n@0.214.0...n8n@0.214.1) (2023-02-06)


### Bug Fixes

* **editor:** Fix mapping to empty expression input ([#5367](https://github.com/n8n-io/n8n/issues/5367)) ([e4458b4](https://github.com/n8n-io/n8n/commit/e4458b48e005667ae903ee6965e1a299546267f0))
* **editor:** Fix merge node connectors ([#5364](https://github.com/n8n-io/n8n/issues/5364)) ([20356ba](https://github.com/n8n-io/n8n/commit/20356ba8c80196f9562e073c1a55d55a4d6c37b0))
* **editor:** Fix multiple-output endpoints success style after connection is detached ([#5366](https://github.com/n8n-io/n8n/issues/5366)) ([9b628dd](https://github.com/n8n-io/n8n/commit/9b628ddc343f0a40c7ddaab93d5258ac949a4ea2))


### Features

* **Slack Node:** Revamp the node with more functionalities in a new version ([#4587](https://github.com/n8n-io/n8n/issues/4587)) ([4df6942](https://github.com/n8n-io/n8n/commit/4df69428f1e1e440aadddddb019cf559fd824a28))



# [0.214.0](https://github.com/n8n-io/n8n/compare/n8n@0.213.0...n8n@0.214.0) (2023-02-03)


### Bug Fixes

* Add paired item to the most used nodes ([#5220](https://github.com/n8n-io/n8n/issues/5220)) ([409a9ea](https://github.com/n8n-io/n8n/commit/409a9ea3573ded3156142c2662a501d7d6f5e475))
* **core:** Fix oauth2 client credentials not always working ([#5327](https://github.com/n8n-io/n8n/issues/5327)) ([ec7575b](https://github.com/n8n-io/n8n/commit/ec7575b0321edf6e21e5ba5fb4094e9a36e65571))
* **core:** Fix populating of node custom api call options ([#5347](https://github.com/n8n-io/n8n/issues/5347)) ([6985500](https://github.com/n8n-io/n8n/commit/6985500a7d14e21b629de0ee9e3006622e3774bc))
* **core:** Fix value resolution in declarative node design ([#5217](https://github.com/n8n-io/n8n/issues/5217)) ([b27a60b](https://github.com/n8n-io/n8n/commit/b27a60b66568c1cce00f38eec2dd1b6425a5a9c6))
* **core:** Prevent shared user details being saved alongside execution data ([#5334](https://github.com/n8n-io/n8n/issues/5334)) ([6ca49f9](https://github.com/n8n-io/n8n/commit/6ca49f9d5474d37281681ea571fa74e43828ca84))
* **core:** Revert custom API option injecting ([#5345](https://github.com/n8n-io/n8n/issues/5345)) ([6160741](https://github.com/n8n-io/n8n/commit/616074158c10a1928299d7213c58eeb076a664e1)), closes [#5303](https://github.com/n8n-io/n8n/issues/5303)
* **editor:** Add SMTP info translation link slot ([#5288](https://github.com/n8n-io/n8n/issues/5288)) ([c93664a](https://github.com/n8n-io/n8n/commit/c93664a57c6f252044264b09876e9b474740f6e8))
* **editor:** Change executions title to match menu ([#5349](https://github.com/n8n-io/n8n/issues/5349)) ([338b354](https://github.com/n8n-io/n8n/commit/338b354ef1600903833c9939a8618d1989534e0b))
* **editor:** Fix `json` field completions while typing ([#5309](https://github.com/n8n-io/n8n/issues/5309)) ([07b941a](https://github.com/n8n-io/n8n/commit/07b941a043f8aac761af63fd5327f45cbff7d275))
* **editor:** Handling router errors when navigation is canceled by user ([#5271](https://github.com/n8n-io/n8n/issues/5271)) ([911d656](https://github.com/n8n-io/n8n/commit/911d656f995a9a7f50db7e97ae25fcc3230ae4a5))
* **editor:** Set max width for executions list ([#5302](https://github.com/n8n-io/n8n/issues/5302)) ([52dea08](https://github.com/n8n-io/n8n/commit/52dea08003d314841d261533391e05d688dd1fe4))
* **editor:** Stop unsaved changes popup display when navigating away from an untouched workflow ([#5259](https://github.com/n8n-io/n8n/issues/5259)) ([6a93aed](https://github.com/n8n-io/n8n/commit/6a93aed3a2c428633fdf922df73203d3d41a7bb6))
* **editor:** Workflow executions view is broken ([#5341](https://github.com/n8n-io/n8n/issues/5341)) ([50cb757](https://github.com/n8n-io/n8n/commit/50cb75706b73c7349e48956a2e8556b0a2de1e24))
* **Invoice Ninja Node:** Fix line items not being correctly set for quotes and invoices ([#5304](https://github.com/n8n-io/n8n/issues/5304)) ([3b5e1d1](https://github.com/n8n-io/n8n/commit/3b5e1d127fe049934a0a32310ed408cd129b2d7d))
* **Linear Node:** Fix pagination issue for get all issues ([#5324](https://github.com/n8n-io/n8n/issues/5324)) ([f9ecc34](https://github.com/n8n-io/n8n/commit/f9ecc34b10544e787f7034e89068aa6c9356fa04))
* **Mailchimp Trigger Node:** Fix webhook recreation ([#5328](https://github.com/n8n-io/n8n/issues/5328)) ([8f5f1c3](https://github.com/n8n-io/n8n/commit/8f5f1c3aa520576215e16a8cc1a8beadae5f142a))
* Prevent unnecessarily touching updatedAt when n8n starts ([#5340](https://github.com/n8n-io/n8n/issues/5340)) ([b5154d9](https://github.com/n8n-io/n8n/commit/b5154d9be5e3adccbdcbb0ad748ed869ba75d4cc))
* **Schedule Trigger Node:** Change scheduler behaviour for intervals days and hours ([#5133](https://github.com/n8n-io/n8n/issues/5133)) ([78bbe2b](https://github.com/n8n-io/n8n/commit/78bbe2ba27990127b1b6a6333361f35e2d3e7a65))
* **Set Node:** Fix behaviour when selecting continueOnFail & PairedItem ([#5257](https://github.com/n8n-io/n8n/issues/5257)) ([a8637a0](https://github.com/n8n-io/n8n/commit/a8637a0bc6ac19859ce1ff468d0404ac73bc70bb))


### Features

* **core:** Export OpenAPI spec for external tools ([#5294](https://github.com/n8n-io/n8n/issues/5294)) ([5cb7e50](https://github.com/n8n-io/n8n/commit/5cb7e5007de7374f8ee6e6fbe1c5a8138af2d065))
* **core:** Fix populating of node custom api call options ([#5303](https://github.com/n8n-io/n8n/issues/5303)) ([e58bc41](https://github.com/n8n-io/n8n/commit/e58bc41d241b3f4a1701191f69e5eadad969bc5f))
* **core:** Set custom Cache-Control headers for static assets ([#5322](https://github.com/n8n-io/n8n/issues/5322)) ([ee210e8](https://github.com/n8n-io/n8n/commit/ee210e8507ce06f7052328f28ba14451f51b3db4))
* **core:** Simplify pagination in declarative node design ([#5161](https://github.com/n8n-io/n8n/issues/5161)) ([87ceb6f](https://github.com/n8n-io/n8n/commit/87ceb6f4b8ed1838b874639f176b421e0292b576))
* **editor:** Add mapping support for data paths ([#5191](https://github.com/n8n-io/n8n/issues/5191)) ([6092f6c](https://github.com/n8n-io/n8n/commit/6092f6c41ee28f3482675b940b1fdc600ae29971))
* **editor:** Adjust HTML editor component for use in params ([#5285](https://github.com/n8n-io/n8n/issues/5285)) ([8b09e98](https://github.com/n8n-io/n8n/commit/8b09e986542f00675197bc8e003c332e8926779f))
* **editor:** Append expressions in fixed values when mapping to string/json inputs ([#5300](https://github.com/n8n-io/n8n/issues/5300)) ([88c7ef2](https://github.com/n8n-io/n8n/commit/88c7ef29c84e0e9cfce32b97b8921bd5af38db02))
* **editor:** Completions for extensions in expression editor ([#5130](https://github.com/n8n-io/n8n/issues/5130)) ([6d811f0](https://github.com/n8n-io/n8n/commit/6d811f0d9f503905ed74938f97f193c7c3d8e7a2))
* **editor:** Continue to show mapping tooltip after dismiss ([#5289](https://github.com/n8n-io/n8n/issues/5289)) ([c6bc57b](https://github.com/n8n-io/n8n/commit/c6bc57b4cb1f7b647f167a7c18f6c6397e5d1c95))
* **editor:** Roll out schema view ([#5310](https://github.com/n8n-io/n8n/issues/5310)) ([2b1f151](https://github.com/n8n-io/n8n/commit/2b1f15150f5d069629ed34522be26f5503756614))
* **FTP Node:** Stream binary data for uploads and downloads ([#5296](https://github.com/n8n-io/n8n/issues/5296)) ([448c295](https://github.com/n8n-io/n8n/commit/448c295314b4e4842ff0352e03ba1f12025f47c9))
* **Notion Node:** Add image block ([#5237](https://github.com/n8n-io/n8n/issues/5237)) ([36b1e6e](https://github.com/n8n-io/n8n/commit/36b1e6ef1572aec4d905b29a999e4d5f4c72e826))
* **OpenAI Node:** Add frequency-penalty and presence-penalty ([#5137](https://github.com/n8n-io/n8n/issues/5137)) ([04c058a](https://github.com/n8n-io/n8n/commit/04c058a34e7c306141592691fa646ef6480bbc03))
* **Salesforce Node:** Add HasOptedOutOfEmail field to lead resource ([#5235](https://github.com/n8n-io/n8n/issues/5235)) ([59f290f](https://github.com/n8n-io/n8n/commit/59f290fe854767c6bf5c01ce9a0fb537297d82b2))
* **SSH Node:** Stream binary data for uploads and downloads ([#5305](https://github.com/n8n-io/n8n/issues/5305)) ([6f7421f](https://github.com/n8n-io/n8n/commit/6f7421f970b12e870c7d84b0f559b06678e3d42a))
* **Write Binary File Node:** Stream binary data for writes ([#5306](https://github.com/n8n-io/n8n/issues/5306)) ([d87ff13](https://github.com/n8n-io/n8n/commit/d87ff130a44d4542d1b068ed50c37071a14496b8))
* **YouTube Node:** Switch upload operation over to streaming and resumable uploads api ([#5320](https://github.com/n8n-io/n8n/issues/5320)) ([3bb1690](https://github.com/n8n-io/n8n/commit/3bb16900867b3994585eb2a62310e617f123c257))



# [0.213.0](https://github.com/n8n-io/n8n/compare/n8n@0.212.1...n8n@0.213.0) (2023-01-27)


### Bug Fixes

* **core:** Do not crash express app on unhandled rejected promises ([#5252](https://github.com/n8n-io/n8n/issues/5252)) ([7e229a3](https://github.com/n8n-io/n8n/commit/7e229a3d38990022172d4df98afd3dc31dca6e63))
* **core:** Handle missing binary metadata in download urls ([#5242](https://github.com/n8n-io/n8n/issues/5242)) ([21579a8](https://github.com/n8n-io/n8n/commit/21579a8a2af53f3fb4174afc2013cfad43511a31))
* **core:** Upsert credentials and workflows in the import: commands ([#5231](https://github.com/n8n-io/n8n/issues/5231)) ([259296c](https://github.com/n8n-io/n8n/commit/259296c5c940bd5dcebec5ad3c9acc99a7923b8f))
* **core:** Validate numeric IDs in the public API ([#5251](https://github.com/n8n-io/n8n/issues/5251)) ([68e4083](https://github.com/n8n-io/n8n/commit/68e4083bbdb8200966dc9e702bed9ca5cbc1cdf4))
* **editor:** Do not request workflow data twice when opening a workflow ([#5246](https://github.com/n8n-io/n8n/issues/5246)) ([901e94d](https://github.com/n8n-io/n8n/commit/901e94dc01c4b352301053990f197eda48c30b41))
* **editor:** Execution list micro optimization ([#5244](https://github.com/n8n-io/n8n/issues/5244)) ([a1710fb](https://github.com/n8n-io/n8n/commit/a1710fbd272a0f3980a8f323bbccf58806e9b900))
* **editor:** Fix node authentication options ordering and hiding options based on node version ([#5268](https://github.com/n8n-io/n8n/issues/5268)) ([7d74181](https://github.com/n8n-io/n8n/commit/7d7418140eb03da6014ff8ac51668fc427d10c33))
* **editor:** Fix save modal appearing after duplicating a workflow ([#5247](https://github.com/n8n-io/n8n/issues/5247)) ([c711c53](https://github.com/n8n-io/n8n/commit/c711c53ad6b044b8f90a237d6d8d1ce631359dc3))
* **editor:** Prevent workflow execution list infinite no network error ([#5230](https://github.com/n8n-io/n8n/issues/5230)) ([0d33329](https://github.com/n8n-io/n8n/commit/0d33329bc87b705760fdc70ccb39374cbd71f6f6))
* Extension being too eager and making calls when it shouldn't ([#5232](https://github.com/n8n-io/n8n/issues/5232)) ([09bdd96](https://github.com/n8n-io/n8n/commit/09bdd96d290166cced6faf5da4dda83d6d270aa3))
* **Google Drive Node:** Use the correct mimetype on converted downloads ([#5240](https://github.com/n8n-io/n8n/issues/5240)) ([58d0890](https://github.com/n8n-io/n8n/commit/58d0890dc319c918183fd81999dc87ea9c4732fd))
* **HelpScout Node:** Fix tag search not working when getting all conversations ([#5239](https://github.com/n8n-io/n8n/issues/5239)) ([6d36782](https://github.com/n8n-io/n8n/commit/6d36782463cda1d211270ecf9bd1a8cccca22cdc))
* **Notion (Beta) Node:** Fix create database page with multiple relation IDs not working ([#5260](https://github.com/n8n-io/n8n/issues/5260)) ([8ce85e3](https://github.com/n8n-io/n8n/commit/8ce85e37592da061164db18af52852e8ed1d2046))


### Features

* **core:** Add LDAP support ([#3835](https://github.com/n8n-io/n8n/issues/3835)) ([0c70a40](https://github.com/n8n-io/n8n/commit/0c70a4031702d3c770968d5679d2900def7225a8))
* **editor:** Adjust Google sign-in button to adhere to the guidelines ([#5248](https://github.com/n8n-io/n8n/issues/5248)) ([73cbddc](https://github.com/n8n-io/n8n/commit/73cbddcb2dc046f1795740a5dd2258577df4d049))
* **editor:** Simplify NDV by moving authentication details to credentials modal ([#5067](https://github.com/n8n-io/n8n/issues/5067)) ([b321c5e](https://github.com/n8n-io/n8n/commit/b321c5e4ec5aefa605991861db68efc860e0f122))
* **GitLab Node:** Add file operations (create, delete, edit, get, list) ([#5167](https://github.com/n8n-io/n8n/issues/5167)) ([cedf2e0](https://github.com/n8n-io/n8n/commit/cedf2e012c7309cd225f9810d30315c851bcab3a))
* HTML node ([#5107](https://github.com/n8n-io/n8n/issues/5107)) ([74e6f5d](https://github.com/n8n-io/n8n/commit/74e6f5d190d010831fc2ef98afdd9dff3dc93b3c))
* Improve workflow list performance using RecycleScroller and on-demand sharing data loading ([#5181](https://github.com/n8n-io/n8n/issues/5181)) ([874c735](https://github.com/n8n-io/n8n/commit/874c735d0af81c3c81cf82fb9bdf1232608d6400)), closes [#5125](https://github.com/n8n-io/n8n/issues/5125)
* **Jira Software Node:** Use resource locator component ([#5090](https://github.com/n8n-io/n8n/issues/5090)) ([237b1d8](https://github.com/n8n-io/n8n/commit/237b1d8614ffd19215eaee6a0cb9422a16cf0a5c))
* **Send Email Node:** Overhaul ([832fb87](https://github.com/n8n-io/n8n/commit/832fb87954d480ed46913c8b0f8067c96db28aab))



## [0.212.1](https://github.com/n8n-io/n8n/compare/n8n@0.212.0...n8n@0.212.1) (2023-01-23)

### Bug Fixes

- Add schema to postgres migrations (hotfix) ([#5218](https://github.com/n8n-io/n8n/issues/5218)) ([c5245dd](https://github.com/n8n-io/n8n/commit/c5245dd387f8829210a922223e46df7f275e79ca))
- **core:** Fix execute-once incoming data handling ([#5211](https://github.com/n8n-io/n8n/issues/5211)) ([3ea83d8](https://github.com/n8n-io/n8n/commit/3ea83d872ee2f8326fc9cb898fdb05bbe3b827bf))
- **core:** Fix expression extension misdetection ([#5219](https://github.com/n8n-io/n8n/issues/5219)) ([0b123ce](https://github.com/n8n-io/n8n/commit/0b123ce05e14a996f74ed4fe16008edca836d099))
- **core:** Fix onWorkflowPostExecute not being called ([#5224](https://github.com/n8n-io/n8n/issues/5224)) ([4f89fb4](https://github.com/n8n-io/n8n/commit/4f89fb4d4d663a0a39081ceda9d6e88e6c605859))
- **core:** Fix url in error handelling for the error Trigger ([#5201](https://github.com/n8n-io/n8n/issues/5201)) ([6e39175](https://github.com/n8n-io/n8n/commit/6e391755e47efc8a10529b24dee5e90c466b20b9))
- **core:** Make pindata with webhook responding on last node manual-only ([#5223](https://github.com/n8n-io/n8n/issues/5223)) ([fcbf4fd](https://github.com/n8n-io/n8n/commit/fcbf4fd587c0c8721f58b09edc68fe140acaf9f6))
- **editor:** Making parameter input components label configurable ([#5195](https://github.com/n8n-io/n8n/issues/5195)) ([9ce526e](https://github.com/n8n-io/n8n/commit/9ce526e784a6e61ed0f5b0a9ddb9d4ea21584ab2))
- **editor:** Remove infinite loading in not found workflow level execution ([#5174](https://github.com/n8n-io/n8n/issues/5174)) ([96dddf1](https://github.com/n8n-io/n8n/commit/96dddf12e1561935fa191e55baa950c207796e83))
- **Linear Node:** Fix issue with single item not being returned ([#5193](https://github.com/n8n-io/n8n/issues/5193)) ([e810966](https://github.com/n8n-io/n8n/commit/e810966a3b00e7a581120df2b22d71026e9ba4cb))
- **Notion (Beta) Node:** Fix create database page fails if relation param is empty/undefined ([#5182](https://github.com/n8n-io/n8n/issues/5182)) ([11da863](https://github.com/n8n-io/n8n/commit/11da863a2104259248b67edfff7bee3e18b3789a))

### Features

- **Google Analytics Node:** Overhaul for google analytics node ([736e700](https://github.com/n8n-io/n8n/commit/736e700902d333df55abff86c15c688de15c9bde))

# [0.212.0](https://github.com/n8n-io/n8n/compare/n8n@0.211.2...n8n@0.212.0) (2023-01-19)

### Bug Fixes

- **core:** Revert rule @typescript-eslint/prefer-nullish-coalescing ([e667df7](https://github.com/n8n-io/n8n/commit/e667df783c8c396fc40ff14de704b1e0def4a699))
- **editor:** Allow special chars in node selector completion ([#5196](https://github.com/n8n-io/n8n/issues/5196)) ([b718464](https://github.com/n8n-io/n8n/commit/b718464b1f28e52ffb0b12e4b927d8fe3678d02a))
- **GitLab Node:** Update credential test endpoint ([#5166](https://github.com/n8n-io/n8n/issues/5166)) ([e275306](https://github.com/n8n-io/n8n/commit/e275306c64a410c154e586532e35d25a583f75b4))
- **Gmail Trigger Node:** Filter by labels not working ([#5173](https://github.com/n8n-io/n8n/issues/5173)) ([026f3a5](https://github.com/n8n-io/n8n/commit/026f3a532d30dcf79b76c9f9cff709e6af0eb9ee))
- **HTTP Request Node:** Bug - node requires string instead of json ([8f49f49](https://github.com/n8n-io/n8n/commit/8f49f494ae66ce933f0fce3c3b43ce99baa1b728))
- **HTTP Request Node:** Response format to text is ignored for JSON responses ([8dbe615](https://github.com/n8n-io/n8n/commit/8dbe6159d04c963e7858d31d64721ddc0911ea36))

### Features

- **core:** Add Prometheus metrics for n8n events and api invocations (experimental) ([#5177](https://github.com/n8n-io/n8n/issues/5177)) ([9b032d6](https://github.com/n8n-io/n8n/commit/9b032d68bc8a7a45aae73e9442315e872902d50a)), closes [#5187](https://github.com/n8n-io/n8n/issues/5187)
- **Item Lists Node:** Table tranformation ([5426690](https://github.com/n8n-io/n8n/commit/5426690791ead70085681ef31f229fbe15c7d656))

## [0.211.2](https://github.com/n8n-io/n8n/compare/n8n@0.211.1...n8n@0.211.2) (2023-01-17)

### Bug Fixes

- **core:** Restore community nodes installation ([#5180](https://github.com/n8n-io/n8n/issues/5180)) ([c0268f5](https://github.com/n8n-io/n8n/commit/c0268f572fed4953354123da90f780612c7651ee))

### Features

- (Google Sheets Trigger Node): Trigger for Google Sheets ([e839a81](https://github.com/n8n-io/n8n/commit/e839a81cc5f31eb622915749f9e598f248e407d7))

## [0.211.1](https://github.com/n8n-io/n8n/compare/n8n@0.211.0...n8n@0.211.1) (2023-01-16)

### Bug Fixes

- Build `cli` to fix Postgres and MySQL test runs ([#5171](https://github.com/n8n-io/n8n/issues/5171)) ([a0c5232](https://github.com/n8n-io/n8n/commit/a0c5232aa53b13e581b5da4b6f984f5d7893fe33))
- Extend date functions clobbering plus/minus ([#5170](https://github.com/n8n-io/n8n/issues/5170)) ([f634f0d](https://github.com/n8n-io/n8n/commit/f634f0dc59389a8c7ecd4154d2cf9af495b129aa))
- Extension deep compare not quite working for some primitives ([#5172](https://github.com/n8n-io/n8n/issues/5172)) ([98017dc](https://github.com/n8n-io/n8n/commit/98017dc36f3e2fc3d2a5178fb7259205504e5582))
- Upgrade `jsonwebtoken` to address CVE-2022-23540 ([#5116](https://github.com/n8n-io/n8n/issues/5116)) ([97969fc](https://github.com/n8n-io/n8n/commit/97969fc81581379d2a3c49d839206cc9b9e05d9d))

### Features

- **editor:** Supress validation errors for freshly added nodes ([#5149](https://github.com/n8n-io/n8n/issues/5149)) ([582865c](https://github.com/n8n-io/n8n/commit/582865c7e9eff99eabb36636ca7af2d2b2e76af8))
- **Google Ads Node:** Update api version to v11 ([#4427](https://github.com/n8n-io/n8n/issues/4427)) ([dfff982](https://github.com/n8n-io/n8n/commit/dfff982662b7cee5c0203764a59d2355a02a9030))
- **Google Drive Trigger Node:** Use resource locator component ([#5148](https://github.com/n8n-io/n8n/issues/5148)) ([9958c32](https://github.com/n8n-io/n8n/commit/9958c324dbf88f25efd34433ce51af9e3aa44ae3))

# [0.211.0](https://github.com/n8n-io/n8n/compare/n8n@0.210.2...n8n@0.211.0) (2023-01-13)

### Bug Fixes

- **core:** Fixes event msg confirmations if no subscribers present ([#5118](https://github.com/n8n-io/n8n/issues/5118)) ([62d06b1](https://github.com/n8n-io/n8n/commit/62d06b1e6edb8a8a6dfb4c57de6ef3e095e6301c))
- **core:** Remove threads pkg, rewrite log writer worker ([#5134](https://github.com/n8n-io/n8n/issues/5134)) ([e845eb3](https://github.com/n8n-io/n8n/commit/e845eb33f9d0881ae5c8a26d4eab4f2109373ff5))
- **core:** Throw error in UI on expression referencing missing node but do not fail execution ([#5158](https://github.com/n8n-io/n8n/issues/5158)) ([c9e158e](https://github.com/n8n-io/n8n/commit/c9e158e45848ee94b04f49694a552f9f272a97dd))
- DB revert command shouldn't run full migrations before each revert ([#5131](https://github.com/n8n-io/n8n/issues/5131)) ([a9fb393](https://github.com/n8n-io/n8n/commit/a9fb393e1a260a2dc26ef0f759f541fcde1c722f))
- **editor:** Disable data pinning on multiple output node types ([#5111](https://github.com/n8n-io/n8n/issues/5111)) ([56951e8](https://github.com/n8n-io/n8n/commit/56951e83c0fb03a24ddb4cd0b1705e22165b8692))
- **editor:** Do not overwrite window.onerror in production ([#5135](https://github.com/n8n-io/n8n/issues/5135)) ([0dbba6d](https://github.com/n8n-io/n8n/commit/0dbba6d57f34b67935867bd81359fb833654fce1))
- **editor:** Execution page bug fixes ([#5122](https://github.com/n8n-io/n8n/issues/5122)) ([665eaef](https://github.com/n8n-io/n8n/commit/665eaef925d2e311377ecb09859f69f5fddc54b5))
- **editor:** Fixes event bus test ([#5119](https://github.com/n8n-io/n8n/issues/5119)) ([871a1d7](https://github.com/n8n-io/n8n/commit/871a1d7dad839b080df3a27fb68ea90033562f3f))
- **editor:** Hide data pinning discoverability tooltip in execution view ([#5145](https://github.com/n8n-io/n8n/issues/5145)) ([d10ca53](https://github.com/n8n-io/n8n/commit/d10ca530cff1580c20670dd68dfd7937e1a78d74))
- **editor:** Mapping tooltip dismiss ([#5128](https://github.com/n8n-io/n8n/issues/5128)) ([6deb551](https://github.com/n8n-io/n8n/commit/6deb55126e9f493de4717018a3587088f1d5ab41))
- **editor:** Recover from unsaved finished execution ([#5121](https://github.com/n8n-io/n8n/issues/5121)) ([af55ecd](https://github.com/n8n-io/n8n/commit/af55ecd64b1d4948fc08d7d32900fa9d57ef299b))
- **editor:** Setting NDV session ID ([#5144](https://github.com/n8n-io/n8n/issues/5144)) ([c724de6](https://github.com/n8n-io/n8n/commit/c724de6be2e33fe824c42c0ab8242caa9f1133f3))
- First/last being extended on proxy objects ([#5140](https://github.com/n8n-io/n8n/issues/5140)) ([9dca984](https://github.com/n8n-io/n8n/commit/9dca984c0ce68dd9c1ab14a6454c356dddf8287f))
- Handle memory issues gracefully ([#5147](https://github.com/n8n-io/n8n/issues/5147)) ([1445424](https://github.com/n8n-io/n8n/commit/14454243e7e0b40fc766cdb05c6b34756fb59109))
- **PayPal Trigger Node:** Omit verification on sandbox env ([#5150](https://github.com/n8n-io/n8n/issues/5150)) ([e140ecb](https://github.com/n8n-io/n8n/commit/e140ecbc2c6a07b96df3d048eb138dd34b25d2ce))
- Report app startup and DB migration errors to Sentry ([#5127](https://github.com/n8n-io/n8n/issues/5127)) ([a573db2](https://github.com/n8n-io/n8n/commit/a573db2ef78024a4254ff0f468dc47b12148aa28))
- Run every DB migration inside a transaction ([#5129](https://github.com/n8n-io/n8n/issues/5129)) ([62cce2e](https://github.com/n8n-io/n8n/commit/62cce2e518451f6057e316208828539f26868c18))
- Upgrade `class-validator` to address CVE-2019-18413 ([#5139](https://github.com/n8n-io/n8n/issues/5139)) ([14a61f6](https://github.com/n8n-io/n8n/commit/14a61f6ab1f0289e1b96480e3d557d14dd8178d8))
- **Zoom Node:** Add notice about deprecation of Zoom JWT app support ([#5156](https://github.com/n8n-io/n8n/issues/5156)) ([146bc3b](https://github.com/n8n-io/n8n/commit/146bc3bff503be70abaad94418535f23ff8fc511))

### Features

- Add demo experiment to help users activate ([#5141](https://github.com/n8n-io/n8n/issues/5141)) ([c2eb519](https://github.com/n8n-io/n8n/commit/c2eb519398067e799e73b6c3059f57f3deca172a))
- **editor:** Executions page ([#4997](https://github.com/n8n-io/n8n/issues/4997)) ([819c4ad](https://github.com/n8n-io/n8n/commit/819c4adb3cd79c1743debd97c21fc60a2a703534))
- **editor:** Remove prevent-ndv-auto-open feature flag ([#5114](https://github.com/n8n-io/n8n/issues/5114)) ([ab4785a](https://github.com/n8n-io/n8n/commit/ab4785ab31da061df13a6b37fe8790ddc30e3ed0))
- **editor:** Update callout component design ([#5126](https://github.com/n8n-io/n8n/issues/5126)) ([d2d481f](https://github.com/n8n-io/n8n/commit/d2d481f12e1777a60ee5411c8cdac50b1dfc3ee3))
- Expression extension framework ([#4372](https://github.com/n8n-io/n8n/issues/4372)) ([3d05acf](https://github.com/n8n-io/n8n/commit/3d05acf3130cce2c5b5155d91faa22b707ce2373)), closes [#4045](https://github.com/n8n-io/n8n/issues/4045) [#4044](https://github.com/n8n-io/n8n/issues/4044) [#4046](https://github.com/n8n-io/n8n/issues/4046)

## [0.210.2](https://github.com/n8n-io/n8n/compare/n8n@0.210.1...n8n@0.210.2) (2023-01-09)

### Bug Fixes

- **core:** Fix crash of manual workflow executions for unsaved workflows ([#5106](https://github.com/n8n-io/n8n/issues/5106)) ([a43e3e4](https://github.com/n8n-io/n8n/commit/a43e3e4112f1b9ef68ed963c41142fd591916d69))
- **editor:** Omit `pairedItem` from proxy completions ([#5098](https://github.com/n8n-io/n8n/issues/5098)) ([320e646](https://github.com/n8n-io/n8n/commit/320e646380395af00b8b73445af045f9b6315dc4))
- **editor:** Prevent refresh on submit in credential edit modal ([#5091](https://github.com/n8n-io/n8n/issues/5091)) ([9e7a9bf](https://github.com/n8n-io/n8n/commit/9e7a9bfe2096b880e265700437b76e51d9be545f))
- **Google Sheets Node:** Fix for auto-range detection ([77031a2](https://github.com/n8n-io/n8n/commit/77031a295059938c9bf1fdf549b7ffcb6746db17))
- **Read Binary File Node:** Do not crash the execution when the source file does not exist ([#5100](https://github.com/n8n-io/n8n/issues/5100)) ([c97f3ca](https://github.com/n8n-io/n8n/commit/c97f3cad596e26ff7dbd0e51fc5cfeb508d2c198))
- Remove anonymous ID from tracking calls ([#5099](https://github.com/n8n-io/n8n/issues/5099)) ([6d0f2bf](https://github.com/n8n-io/n8n/commit/6d0f2bff7f45ab27d76c34e5d4062df5d711331c))
- Stop OOM crashes in Execution Data pruning ([#5095](https://github.com/n8n-io/n8n/issues/5095)) ([c4df204](https://github.com/n8n-io/n8n/commit/c4df2049a8f8c5e9cbc69f634b0a5747e0677376))
- Update links for user management and SMTP help ([#5109](https://github.com/n8n-io/n8n/issues/5109)) ([47e32e4](https://github.com/n8n-io/n8n/commit/47e32e42682b2d6791157fdb11e5513381bd7452))

### Features

- **editor:** Introduce proxy completions to expressions ([#5075](https://github.com/n8n-io/n8n/issues/5075)) ([f4140d0](https://github.com/n8n-io/n8n/commit/f4140d011fa3b748a89122cd41c9628dd5313efd))

## [0.210.1](https://github.com/n8n-io/n8n/compare/n8n@0.210.0...n8n@0.210.1) (2023-01-05)

### Bug Fixes

- **Google Sheets Node:** Append or Update fails for numeric values ([b5e70d4](https://github.com/n8n-io/n8n/commit/b5e70d45bf5155bafe258dcf04609e6f71c5356d))
- Fix external hooks ([#5094](https://github.com/n8n-io/n8n/issues/5094)) ([d77523b](https://github.com/n8n-io/n8n/commit/d77523bd31884c4493079ee0b0dea8c66e642a95))

### Features

- Add user management invite links without SMTP set up ([#5084](https://github.com/n8n-io/n8n/issues/5084)) ([2327563](https://github.com/n8n-io/n8n/commit/2327563c441634bc6c127f2fe58792657fa7d114)), closes [#5079](https://github.com/n8n-io/n8n/issues/5079) [#5085](https://github.com/n8n-io/n8n/issues/5085)

# [0.210.0](https://github.com/n8n-io/n8n/compare/n8n@0.209.4...n8n@0.210.0) (2023-01-05)

### Bug Fixes

- Apply credential overwrites recursively ([#5072](https://github.com/n8n-io/n8n/issues/5072)) ([5d746c4](https://github.com/n8n-io/n8n/commit/5d746c4a8341e2538caa140bedfa269a5babb8db))
- **core:** Fix full manual execution for error trigger as starter of 2+ node workflow ([#5055](https://github.com/n8n-io/n8n/issues/5055)) ([a7868ae](https://github.com/n8n-io/n8n/commit/a7868ae77d070226a7c52de5a445b03e1455fbc7))
- **core:** Fix OAuth credential creation via API ([#5064](https://github.com/n8n-io/n8n/issues/5064)) ([93da026](https://github.com/n8n-io/n8n/commit/93da026c0d2a6f3738d9e1a3b450ad802ff15826))
- **core:** Fixes issue with workflow lastUpdated field ([#5015](https://github.com/n8n-io/n8n/issues/5015)) ([59004fe](https://github.com/n8n-io/n8n/commit/59004fe7bb1e821444a029c2fd3fb3f0e6a59733))
- **editor:** Clear node creator and scrim on workspace reset ([#5066](https://github.com/n8n-io/n8n/issues/5066)) ([43304b0](https://github.com/n8n-io/n8n/commit/43304b069168ef4ca6bb345eebf01d5f9ff9cb0f))
- **editor:** Fix an infinite loop while loading executions that are not on the current executions list ([#5071](https://github.com/n8n-io/n8n/issues/5071)) ([8cf3c86](https://github.com/n8n-io/n8n/commit/8cf3c868609447df20876d5ef5f25575bbe9da9b))
- **editor:** Make node title non-editable in executions view ([#5046](https://github.com/n8n-io/n8n/issues/5046)) ([2f40a7f](https://github.com/n8n-io/n8n/commit/2f40a7f98a4cea990d6c57cba8efa6fbd9c622e3))
- **editor:** Prevent scrim on executable triggers ([#5068](https://github.com/n8n-io/n8n/issues/5068)) ([e1f9349](https://github.com/n8n-io/n8n/commit/e1f9349c192fef03f31c5d09a1a9d38b50a6fe99))
- **editor:** Support tabbing away from inline expression editor ([#5056](https://github.com/n8n-io/n8n/issues/5056)) ([a2ab78f](https://github.com/n8n-io/n8n/commit/a2ab78f9274427c57db1c59d80d1ef6474879a6a))
- Fix executions bulk deletion ([#5074](https://github.com/n8n-io/n8n/issues/5074)) ([3754c5c](https://github.com/n8n-io/n8n/commit/3754c5c734814ed310eb08a6b69a38c632246696))
- **Google Sheets Node:** Fix exception when no Values to Send are set ([f1184cc](https://github.com/n8n-io/n8n/commit/f1184ccab5dd7f0f7a80a5f39cf4f7bdb387f7ae))
- **Respond to Webhook Node:** Fix issue that content-type header gets overwritten ([#5088](https://github.com/n8n-io/n8n/issues/5088)) ([7954025](https://github.com/n8n-io/n8n/commit/7954025eb2091d70479585fa90efbf9af4db2ae0))
- **Slack Node:** Add missing channels:read OAuth2 scope ([#5092](https://github.com/n8n-io/n8n/issues/5092)) ([62b2fc3](https://github.com/n8n-io/n8n/commit/62b2fc37c343b09e0e9caae49de11bee2e9dbd9b))

### Features

- Add global event bus ([#4860](https://github.com/n8n-io/n8n/issues/4860)) ([b67f803](https://github.com/n8n-io/n8n/commit/b67f803cbee04dd94caee2e80f12a3af810a3984))
- **Compare Datasets Node:** Fuzzy compare option ([9615253](https://github.com/n8n-io/n8n/commit/9615253155bec6b57344d790681c8a598fbc21c0))
- **core:** Add compatibility to redis > 6 ACLs system using username in queue-mode ([#5048](https://github.com/n8n-io/n8n/issues/5048)) ([0ec66bf](https://github.com/n8n-io/n8n/commit/0ec66bfb421c4eb3c6e92144c7563d8d3ea4ac69))
- **core:** Security audit ([#5034](https://github.com/n8n-io/n8n/issues/5034)) ([d548161](https://github.com/n8n-io/n8n/commit/d5481616326b304a76937b104d24326a93f6f565))
- **editor:** Add SSO fakedoor feature ([#5076](https://github.com/n8n-io/n8n/issues/5076)) ([8e8df6d](https://github.com/n8n-io/n8n/commit/8e8df6d6116bb22f372bf4b50511860cacb0e2e0))

### Performance Improvements

- Lazy-load public-api dependencies to reduce baseline memory usage ([#5049](https://github.com/n8n-io/n8n/issues/5049)) ([a455cce](https://github.com/n8n-io/n8n/commit/a455cce7e6cc511360a9d6f9113b5a6d18e06dba))
- Lazy-load queue-mode and analytics dependencies ([#5061](https://github.com/n8n-io/n8n/issues/5061)) ([b828cb3](https://github.com/n8n-io/n8n/commit/b828cb31d621f20b6c9612a2ac79f48e6337e528))

## [0.209.4](https://github.com/n8n-io/n8n/compare/n8n@0.209.3...n8n@0.209.4) (2022-12-28)

### Bug Fixes

- **editor:** Add sticky note without manual trigger ([#5039](https://github.com/n8n-io/n8n/issues/5039)) ([18140e0](https://github.com/n8n-io/n8n/commit/18140e059bd95d51ad24a4ef4d6e6c72ce3137f3))
- **editor:** Display default missing value in table view as `undefined` ([#5038](https://github.com/n8n-io/n8n/issues/5038)) ([33d7a13](https://github.com/n8n-io/n8n/commit/33d7a13e73dffc72b1a9aa4cf603e7758c65e40c))
- **editor:** Fix displaying of some trigger nodes in the creator panel ([#5040](https://github.com/n8n-io/n8n/issues/5040)) ([4daf905](https://github.com/n8n-io/n8n/commit/4daf905ce264f6f76045a508e2f9ed849f2b1f5e))
- **editor:** Fix trigger node type identification on add to canvas ([#5043](https://github.com/n8n-io/n8n/issues/5043)) ([2aba0c6](https://github.com/n8n-io/n8n/commit/2aba0c6d47d6d87038db6877a29e15ed079d712b))
- **editor:** Usage and plans page on Desktop ([#5045](https://github.com/n8n-io/n8n/issues/5045)) ([26e2321](https://github.com/n8n-io/n8n/commit/26e2321a710d7b42559492a6605cef3a248d918e))

### Features

- **editor:** Switch to expression on `=` input ([#5044](https://github.com/n8n-io/n8n/issues/5044)) ([16bd761](https://github.com/n8n-io/n8n/commit/16bd7610fc337fa5ba9b0088b91396bb13570bcb))

## [0.209.3](https://github.com/n8n-io/n8n/compare/n8n@0.209.2...n8n@0.209.3) (2022-12-27)

### Bug Fixes

- **core:** Do not send credentials to browser console ([#5031](https://github.com/n8n-io/n8n/issues/5031)) ([afc5297](https://github.com/n8n-io/n8n/commit/afc529799d5049e1ccaf249d191dce7ff237ee96))
- **core:** Non owner should be permitted to use their own credentials ([#5036](https://github.com/n8n-io/n8n/issues/5036)) ([6efbac3](https://github.com/n8n-io/n8n/commit/6efbac307fb7b0e8436ad1dbd8662b8d1a2167f6))
- **editor:** Fix for loading executions that are not on the current executions list ([#5035](https://github.com/n8n-io/n8n/issues/5035)) ([d0865e2](https://github.com/n8n-io/n8n/commit/d0865e28ffe78ce5ec201dab12b634cbdafcb4e8))
- **editor:** Transparentize tertiary button on Usage page ([#5033](https://github.com/n8n-io/n8n/issues/5033)) ([d6bc760](https://github.com/n8n-io/n8n/commit/d6bc760ab4b003d6233df8428f373b4c8f760a7c))
- **editor:** Update credential owner warning when sharing ([#5029](https://github.com/n8n-io/n8n/issues/5029)) ([a8f4efa](https://github.com/n8n-io/n8n/commit/a8f4efaf3ebc349c6ee073200e19ac57eb961ce9))

### Features

- **core:** Implement webhook-only manual execution ([#4960](https://github.com/n8n-io/n8n/issues/4960)) ([d113977](https://github.com/n8n-io/n8n/commit/d113977b10ffe1db879e7fa0807da8147e52ca5d))
- **editor:** Improve UX for brace completion from selection ([#5024](https://github.com/n8n-io/n8n/issues/5024)) ([52077e2](https://github.com/n8n-io/n8n/commit/52077e2c45fca3d5830a39ca3416b073f783fbf5))

## [0.209.2](https://github.com/n8n-io/n8n/compare/n8n@0.209.1...n8n@0.209.2) (2022-12-23)

### Bug Fixes

- **editor:** Ensure full tree on expression editor parse ([#5027](https://github.com/n8n-io/n8n/issues/5027)) ([47854eb](https://github.com/n8n-io/n8n/commit/47854ebc36c115110bd3cc65b3f1fd95a89fdb9d))
- Fix automatic credential selection when credentials are shared ([#5020](https://github.com/n8n-io/n8n/issues/5020)) ([6a8448d](https://github.com/n8n-io/n8n/commit/6a8448da5fceae393a31f222981a33263de72c1a))

### Performance Improvements

- Improve workflows list performance ([#5021](https://github.com/n8n-io/n8n/issues/5021)) ([bb0eeda](https://github.com/n8n-io/n8n/commit/bb0eedada9afcae589c968ffcb583fae7b6e1959))

## [0.209.1](https://github.com/n8n-io/n8n/compare/n8n@0.209.0...n8n@0.209.1) (2022-12-22)

### Bug Fixes

- **AWS DynamoDB Node:** Fix issue pagination and simplify issue [#4956](https://github.com/n8n-io/n8n/issues/4956) [#4957](https://github.com/n8n-io/n8n/issues/4957) ([#4959](https://github.com/n8n-io/n8n/issues/4959)) ([a43ea17](https://github.com/n8n-io/n8n/commit/a43ea177ebcc983ccc440662f397bf8b1698b4df))
- DynamoDB node type issues ([#5002](https://github.com/n8n-io/n8n/issues/5002)) ([9568b74](https://github.com/n8n-io/n8n/commit/9568b747c74cd72fb7629e95a7555878b4ac4afb))
- **editor:** Fix for executions preview scroll load and wrong execution displayed ([#4994](https://github.com/n8n-io/n8n/issues/4994)) ([bd0c2af](https://github.com/n8n-io/n8n/commit/bd0c2afaac37194efec8872f9fdb0a37a3f74c40))
- **editor:** Force parse on long expressions ([#5009](https://github.com/n8n-io/n8n/issues/5009)) ([22fcc8f](https://github.com/n8n-io/n8n/commit/22fcc8f2be64fb381a64f12485d81b598ef406e5))
- Issue with credentials and workflows not being matched correctly due to incorrect typing ([#5011](https://github.com/n8n-io/n8n/issues/5011)) ([746e848](https://github.com/n8n-io/n8n/commit/746e8487d250d77d91dabd8463f869a3e96d0fc2))
- Restore missing tags in workflow retrieve ([#5004](https://github.com/n8n-io/n8n/issues/5004)) ([87d8865](https://github.com/n8n-io/n8n/commit/87d8865ad38e1e5b4a3bca7d807536975116ba82))
- Show trigger actions again in nodes panel ([#5016](https://github.com/n8n-io/n8n/issues/5016)) ([e7cb190](https://github.com/n8n-io/n8n/commit/e7cb1907cdf90e9497c24f39f3e9b53e5470762c)), closes [#4976](https://github.com/n8n-io/n8n/issues/4976)

# [0.209.0](https://github.com/n8n-io/n8n/compare/n8n@0.208.1...n8n@0.209.0) (2022-12-21)

### Bug Fixes

- **editor:** Correctly display trigger nodes without actions and with related regular node in the "On App Events" category ([#4976](https://github.com/n8n-io/n8n/issues/4976)) ([445463a](https://github.com/n8n-io/n8n/commit/445463a605f5f327f897b23a9b4504939358d0df))
- Fix stickies resize ([#4986](https://github.com/n8n-io/n8n/issues/4986)) ([82f7635](https://github.com/n8n-io/n8n/commit/82f763589b21815e5ba91c10a4676d25f843eddd))
- Hide trigger tooltip for nodes with static test output ([#4970](https://github.com/n8n-io/n8n/issues/4970)) ([5b11dc3](https://github.com/n8n-io/n8n/commit/5b11dc3ff9ff75eb7c65721e0d6c03707039e7ff))
- Keep expression when dropping mapped value ([#4981](https://github.com/n8n-io/n8n/issues/4981)) ([87c7643](https://github.com/n8n-io/n8n/commit/87c76434a294f10474711ba3f023f2f4ca47f14d))
- Prevent keyboard shortcuts in expression editor modal ([#4984](https://github.com/n8n-io/n8n/issues/4984)) ([29364ea](https://github.com/n8n-io/n8n/commit/29364ea7026e5e2a288b1866956f01e380ff05a0))
- Redirect home to workflows always ([#4968](https://github.com/n8n-io/n8n/issues/4968)) ([90bfdfd](https://github.com/n8n-io/n8n/commit/90bfdfd577c02aee520545cf8758019042cdf99c))
- Update mapping gifs ([#4982](https://github.com/n8n-io/n8n/issues/4982)) ([9d00b47](https://github.com/n8n-io/n8n/commit/9d00b4748b39f5c2b08721c5ee73e47b43230b9d))
- Upgrade amqplib to address CVE-2022-0686 ([#4972](https://github.com/n8n-io/n8n/issues/4972)) ([570ed3b](https://github.com/n8n-io/n8n/commit/570ed3b52191cf3a162fcdaaabc8ab15fb0ef08c))
- View option for binary-data shouldn't download the file on Chrome/Edge ([#4995](https://github.com/n8n-io/n8n/issues/4995)) ([e225c31](https://github.com/n8n-io/n8n/commit/e225c3190ea4cb5f68f642aab455ed0044fdecf9))

### Features

- **editor:** Add usage and plan pages ([#4819](https://github.com/n8n-io/n8n/issues/4819)) ([0da338f](https://github.com/n8n-io/n8n/commit/0da338f9b5f850b25e97383ae1f4cec8d0e4c17b)), closes [#4793](https://github.com/n8n-io/n8n/issues/4793) [#4842](https://github.com/n8n-io/n8n/issues/4842) [#4866](https://github.com/n8n-io/n8n/issues/4866) [#4875](https://github.com/n8n-io/n8n/issues/4875) [#4958](https://github.com/n8n-io/n8n/issues/4958) [#4979](https://github.com/n8n-io/n8n/issues/4979)
- Update mapping pill for table/json views ([#4965](https://github.com/n8n-io/n8n/issues/4965)) ([343f53b](https://github.com/n8n-io/n8n/commit/343f53bf5393e86eb850d07de85b762476294656))

## [0.208.1](https://github.com/n8n-io/n8n/compare/n8n@0.208.0...n8n@0.208.1) (2022-12-19)

### Bug Fixes

- Always retain original errors in the error chain on NodeOperationError ([#4951](https://github.com/n8n-io/n8n/issues/4951)) ([231257d](https://github.com/n8n-io/n8n/commit/231257d0817df711cf900703fd686efb8307eeb2))
- BinaryDataManager should store metadata when saving from buffer as well ([#4964](https://github.com/n8n-io/n8n/issues/4964)) ([5cbb5f4](https://github.com/n8n-io/n8n/commit/5cbb5f4bc8e09755e29bcc08715129d61c3fd1b6))
- **editor:** Fix for wrong execution data displayed in executions preview ([#4966](https://github.com/n8n-io/n8n/issues/4966)) ([bfc8e68](https://github.com/n8n-io/n8n/commit/bfc8e68b37f77bd1a8259ca8162269451aca4f28))
- Pick up credential test functions from versioned nodes as well ([#4962](https://github.com/n8n-io/n8n/issues/4962)) ([2797c08](https://github.com/n8n-io/n8n/commit/2797c085e51548a29b83dd6ce057ac71bde9ed0c))

# [0.208.0](https://github.com/n8n-io/n8n/compare/n8n@0.207.1...n8n@0.208.0) (2022-12-16)

### Bug Fixes

- **core:** Fix for Google and Microsoft generic OAuth2 credentials ([efa4c56](https://github.com/n8n-io/n8n/commit/efa4c567579d88f9ce764c535dfb41e7391a1286))
- **core:** Fix HTTP Digest Auth for responses without an opaque parameter ([#4806](https://github.com/n8n-io/n8n/issues/4806)) ([6fac502](https://github.com/n8n-io/n8n/commit/6fac502f9ec288d7df2263e6f5a28b3a1fa84595))
- **Disqus Node:** Fix thread parameter for "Get All Threads" operation ([#4912](https://github.com/n8n-io/n8n/issues/4912)) ([a04f838](https://github.com/n8n-io/n8n/commit/a04f838117076424084d858494103638fc201996))
- Do not crash the server when Telemetry is blocked via DNS ([#4947](https://github.com/n8n-io/n8n/issues/4947)) ([6127c95](https://github.com/n8n-io/n8n/commit/6127c958f5ed786ee93f8fedb3344d6792158723))
- **editor:** Allow mapping onto expression editor with selection range ([#4945](https://github.com/n8n-io/n8n/issues/4945)) ([6b83972](https://github.com/n8n-io/n8n/commit/6b83972f6e18e03874eb11180488505b83a0111a))
- **editor:** Do not show actions dialog for actionless triggers when selected via keyboard ([#4911](https://github.com/n8n-io/n8n/issues/4911)) ([74100d3](https://github.com/n8n-io/n8n/commit/74100d3d5b12f70e78e04e8c87541f3adf6decdb))
- **editor:** Fix an issue where some node actions wouldn't select default params correctly ([#4946](https://github.com/n8n-io/n8n/issues/4946)) ([626879b](https://github.com/n8n-io/n8n/commit/626879b3a2f8f4fb6b1c365297d752f456a47610))
- **editor:** Fix typo in retry-button option "Retry with original workflow" ([#4528](https://github.com/n8n-io/n8n/issues/4528)) ([76a3f13](https://github.com/n8n-io/n8n/commit/76a3f1345877599d46691f37878e3fc3fa062243))
- Update permission for showing workflow caller policy ([#4916](https://github.com/n8n-io/n8n/issues/4916)) ([f73267f](https://github.com/n8n-io/n8n/commit/f73267ffa5b4a265ab6be52e887747487cae10c5))

### Features

- Add workflow sharing telemetry ([#4906](https://github.com/n8n-io/n8n/issues/4906)) ([ac066fc](https://github.com/n8n-io/n8n/commit/ac066fc9f3a2c1abeb327dacd7b98ae3a47e2371))
- **core:** Allow for hiding usage page via environment ([#4899](https://github.com/n8n-io/n8n/issues/4899)) ([0f40ca3](https://github.com/n8n-io/n8n/commit/0f40ca39ba64156df186bbf27433ab17edbfa1a6))
- **editor:** Inline expression editor ([#4814](https://github.com/n8n-io/n8n/issues/4814)) ([a125989](https://github.com/n8n-io/n8n/commit/a1259898c01406ebd7f8d0182a6c66fd8b0c7734)), closes [#4836](https://github.com/n8n-io/n8n/issues/4836) [#4846](https://github.com/n8n-io/n8n/issues/4846)
- **editor:** Update user management setup message when sharing is disabled ([#4928](https://github.com/n8n-io/n8n/issues/4928)) ([fbcbef2](https://github.com/n8n-io/n8n/commit/fbcbef20e7b193d6c69334a1da3c0d16936c5ec4))
- Hide credentials password values ([#4868](https://github.com/n8n-io/n8n/issues/4868)) ([fe0f982](https://github.com/n8n-io/n8n/commit/fe0f9824377026a1660d6fda63da79b6cc31ea4b))
- **OpenAI Node:** Add a node to work with OpenAI ([#4932](https://github.com/n8n-io/n8n/issues/4932)) ([7a984bb](https://github.com/n8n-io/n8n/commit/7a984bb6b74381fecb43755c1421be9d80b3ed44))
- **Send Email Node:** Add replyTo support ([#4941](https://github.com/n8n-io/n8n/issues/4941)) ([3140942](https://github.com/n8n-io/n8n/commit/31409420c2367c75cd8eaaf82d5b81f467efc8bb))
- Set all resources view as default subview ([#4919](https://github.com/n8n-io/n8n/issues/4919)) ([bcde07e](https://github.com/n8n-io/n8n/commit/bcde07e03288729ed185d1508cd73efebd82dec0))
- Update workflow overwriting message ([#4917](https://github.com/n8n-io/n8n/issues/4917)) ([2964458](https://github.com/n8n-io/n8n/commit/2964458191a02046a1806bd413e67ebf1308c2f8))

## [0.207.1](https://github.com/n8n-io/n8n/compare/n8n@0.207.0...n8n@0.207.1) (2022-12-13)

### Bug Fixes

- **editor:** Fix undo on Windows and Linux ([#4898](https://github.com/n8n-io/n8n/issues/4898)) ([3fc2d7c](https://github.com/n8n-io/n8n/commit/3fc2d7cc5af54f826a8f0c27cb7860448f92bb77))
- **editor:** Schema view render empty data ([#4902](https://github.com/n8n-io/n8n/issues/4902)) ([0b6d470](https://github.com/n8n-io/n8n/commit/0b6d47086a27117ceb0a1da107e5fcfbe11e0cd4))
- Ensure parent directory exists before copying over the icons to generated static directory ([#4865](https://github.com/n8n-io/n8n/issues/4865)) ([91e9a88](https://github.com/n8n-io/n8n/commit/91e9a88e3a83530e1dce2e72b8796da24775dcf2))

# [0.207.0](https://github.com/n8n-io/n8n/compare/n8n@0.206.1...n8n@0.207.0) (2022-12-12)

### Bug Fixes

- **core:** Remove `nodeGetter` checks ([#4883](https://github.com/n8n-io/n8n/issues/4883)) ([07b2f76](https://github.com/n8n-io/n8n/commit/07b2f7678cc409840328da8f2e0b6f064fab10d8))
- **editor:** Avoid adding manual trigger node when webhook node is added ([#4887](https://github.com/n8n-io/n8n/issues/4887)) ([b689d2d](https://github.com/n8n-io/n8n/commit/b689d2d7c28eb90c8979aba5bbc2f75867289505))
- **editor:** Fix credential sharing issues handler when no matching id or name ([#4879](https://github.com/n8n-io/n8n/issues/4879)) ([1cce8ea](https://github.com/n8n-io/n8n/commit/1cce8eaf16a4394b4241572641427011287a7dc2))
- **editor:** Fix for broken tab navigation ([#4881](https://github.com/n8n-io/n8n/issues/4881)) ([983c544](https://github.com/n8n-io/n8n/commit/983c5447c512651db96fbc57f2934c019dd3bf20))
- **editor:** Schema view shows checkbox in case of empty data ([#4889](https://github.com/n8n-io/n8n/issues/4889)) ([b0c158c](https://github.com/n8n-io/n8n/commit/b0c158c64fa7df7da7fefb6ee24223ce650318b2))
- Increase workflow reactivation max timeout to 1 day ([#4869](https://github.com/n8n-io/n8n/issues/4869)) ([593354b](https://github.com/n8n-io/n8n/commit/593354b6d89b577182873ef621c2c86c5415ef48))
- Issue listing executions with Postgres ([#4856](https://github.com/n8n-io/n8n/issues/4856)) ([5156328](https://github.com/n8n-io/n8n/commit/5156328c34f384e292e9cfaebe72ad0666b02af6))
- **Move Binary Data Node:** Stringify objects before encoding them in MoveBinaryData ([#4882](https://github.com/n8n-io/n8n/issues/4882)) ([3b969d2](https://github.com/n8n-io/n8n/commit/3b969d2cd11e2bff3402cdc5e8825b105b453630))
- Remove foreign credentials when copying nodes or duplicating workflow ([#4880](https://github.com/n8n-io/n8n/issues/4880)) ([7d2e2ee](https://github.com/n8n-io/n8n/commit/7d2e2ee0f74fbe98c0e69ec1383e13af8b8cc035))
- **Split In Batches Node:** Fix issue with pairedItem ([#4873](https://github.com/n8n-io/n8n/issues/4873)) ([38d7300](https://github.com/n8n-io/n8n/commit/38d7300d2a8168643a75f0c4fff108949f25ca15))
- Stop returning `UNKNOWN ERROR` in the response if an actual error message is available ([#4859](https://github.com/n8n-io/n8n/issues/4859)) ([4cb4c5e](https://github.com/n8n-io/n8n/commit/4cb4c5e8188fd930312e3bf720472af35731a968))
- Update duplicate action ([#4858](https://github.com/n8n-io/n8n/issues/4858)) ([19e0e96](https://github.com/n8n-io/n8n/commit/19e0e962710070d4517b20b8c8b2b57392f2100a))
- Upgrade sse-channel to mitigate CVE-2019-10744 ([#4835](https://github.com/n8n-io/n8n/issues/4835)) ([7e1a13f](https://github.com/n8n-io/n8n/commit/7e1a13f9b2cc110343f3dc1f26c9a0703eeee588))

### Features

- Add sharing permissions info for workflow sharees ([#4892](https://github.com/n8n-io/n8n/issues/4892)) ([c013245](https://github.com/n8n-io/n8n/commit/c013245db726bf7e2a880ac538631c53450a6471))
- **editor:** Add undo/redo support for canvas actions ([#4787](https://github.com/n8n-io/n8n/issues/4787)) ([b2aba48](https://github.com/n8n-io/n8n/commit/b2aba48dfe441225c36ba1626aa6f8eb4f1a8173))
- **editor:** Node creator actions ([#4696](https://github.com/n8n-io/n8n/issues/4696)) ([79fe57d](https://github.com/n8n-io/n8n/commit/79fe57dad8093b27651ce82164d6e7a0f08f9e43))
- Handle sharing features when user skips owner setup ([#4850](https://github.com/n8n-io/n8n/issues/4850)) ([6f1b78d](https://github.com/n8n-io/n8n/commit/6f1b78df9877666212d9b01818155e30c2caba0f))
- Update credential test error message for sharees ([#4864](https://github.com/n8n-io/n8n/issues/4864)) ([4765d76](https://github.com/n8n-io/n8n/commit/4765d767e361608a6349d08f7116dedc2a0e7e35))

## [0.206.1](https://github.com/n8n-io/n8n/compare/n8n@0.206.0...n8n@0.206.1) (2022-12-07)

### Bug Fixes

- **core:** Make expression resolution improvements ([#4829](https://github.com/n8n-io/n8n/issues/4829)) ([0bd13c7](https://github.com/n8n-io/n8n/commit/0bd13c71739c4fb34feab4f7a169ee89bc77eee8))
- **editor:** Schema unit test stub fontawesome icon ([#4840](https://github.com/n8n-io/n8n/issues/4840)) ([1e4ca1f](https://github.com/n8n-io/n8n/commit/1e4ca1f0d0c89386470db7f6ce265a1339c79562))
- Remove unnecessary console message ([#4848](https://github.com/n8n-io/n8n/issues/4848)) ([2ad62bc](https://github.com/n8n-io/n8n/commit/2ad62bcd442c4595daef4d02119122d9c37ab43d))

# [0.206.0](https://github.com/n8n-io/n8n/compare/n8n@0.205.0...n8n@0.206.0) (2022-12-06)

### Bug Fixes

- **Code Node:** Restore `pairedItem` to required n8n item keys ([#4821](https://github.com/n8n-io/n8n/issues/4821)) ([915f144](https://github.com/n8n-io/n8n/commit/915f1445c26d834e3d43602f901a198931a107e1))
- **core:** Fix linter error ([#4808](https://github.com/n8n-io/n8n/issues/4808)) ([3bb3809](https://github.com/n8n-io/n8n/commit/3bb3809eecd1b660c0d05c26164b9ccc90a37008))
- **core:** Fix partial execution with pinned data on child node run ([#4764](https://github.com/n8n-io/n8n/issues/4764)) ([5d75e6c](https://github.com/n8n-io/n8n/commit/5d75e6ceb3bf7d88229b4e71dda3250086aceb05))
- **core:** OAuth2 scopes does not save ([7aefed4](https://github.com/n8n-io/n8n/commit/7aefed46dcdb5d795fe9755c9fc64f445136bc17))
- Enable source-maps on WorkflowRunnerProcess in `own` mode ([#4832](https://github.com/n8n-io/n8n/issues/4832)) ([9485e2f](https://github.com/n8n-io/n8n/commit/9485e2f12a4131ec24f504591290246e24f1cd09))
- **Execute Workflow Node:** Update Execute Workflow node info notice text ([#4809](https://github.com/n8n-io/n8n/issues/4809)) ([9e7a156](https://github.com/n8n-io/n8n/commit/9e7a156532293956e74103c66babd6c967bb062c))
- **Gmail Trigger Node:** Trigger node missing some emails ([67aad63](https://github.com/n8n-io/n8n/commit/67aad6334358dfecd5ba3a6e8f085fca73bd40ad))
- Handle error when workflow does not exist or is inaccessible ([#4831](https://github.com/n8n-io/n8n/issues/4831)) ([b71295e](https://github.com/n8n-io/n8n/commit/b71295e4de658fb134b67eaa0b630704f858ce7e))
- **Local File Trigger Node:** Fix issue that causes a crash if the ignore field is empty ([#4824](https://github.com/n8n-io/n8n/issues/4824)) ([#4825](https://github.com/n8n-io/n8n/issues/4825)) ([c311424](https://github.com/n8n-io/n8n/commit/c3114241fdd399555666d2f5890815b6196ce1bf))
- Make `nodes.exclude` and `nodes.include` work with lazy-loaded nodes ([#4833](https://github.com/n8n-io/n8n/issues/4833)) ([85241fd](https://github.com/n8n-io/n8n/commit/85241fd230675691828c8d711f86aabb7e48dabe))

### Features

- Add message for readonly nodes. Improve foreign credentials handling ([#4759](https://github.com/n8n-io/n8n/issues/4759)) ([eb112ff](https://github.com/n8n-io/n8n/commit/eb112ffd23cec04f290d515917c227b628db2834))
- Add prompt to overwrite changes when concurrent editing occurs ([#4817](https://github.com/n8n-io/n8n/issues/4817)) ([af6ac42](https://github.com/n8n-io/n8n/commit/af6ac42aa3ec6805a2a18b920128beafcb9a3cdc))
- **core:** Workflow Execution Statistics ([#4200](https://github.com/n8n-io/n8n/issues/4200)) ([1722c6b](https://github.com/n8n-io/n8n/commit/1722c6b0c5dde87d3389c328b611cbb611b2853e))
- **editor:** Alert design system component ([#4834](https://github.com/n8n-io/n8n/issues/4834)) ([9dbb3ea](https://github.com/n8n-io/n8n/commit/9dbb3ea182cba890781a89fe28eda2c7b50dbc65))
- **editor:** Schema view ([#4615](https://github.com/n8n-io/n8n/issues/4615)) ([4528f34](https://github.com/n8n-io/n8n/commit/4528f34462396b5faf550c5a58c4dd9163bdbc40))
- Fix checkbox line height and make checkbox label clickable ([#4818](https://github.com/n8n-io/n8n/issues/4818)) ([1b7952a](https://github.com/n8n-io/n8n/commit/1b7952a516a5c5dfe1f79e25f811fc044a5e4962))
- **KoBoToolbox Node:** Add support for Media file API ([#4578](https://github.com/n8n-io/n8n/issues/4578)) ([37e580e](https://github.com/n8n-io/n8n/commit/37e580eb0628a651ecbc8faa3ad447cd0177d7cf))

# [0.205.0](https://github.com/n8n-io/n8n/compare/n8n@0.204.0...n8n@0.205.0) (2022-12-02)

### Bug Fixes

- **AWS SNS Node:** Pagination Issue ([d96d161](https://github.com/n8n-io/n8n/commit/d96d1610ba921ba71e90677d379b025741c7c9c8))
- **core:** Ensure executions list is properly filtered for all users ([#4765](https://github.com/n8n-io/n8n/issues/4765)) ([ddf787c](https://github.com/n8n-io/n8n/commit/ddf787c087e523871891fd363f810075943b5e7b))
- **core:** Fix `$items().length` in Execute Once mode ([#4755](https://github.com/n8n-io/n8n/issues/4755)) ([3d67df4](https://github.com/n8n-io/n8n/commit/3d67df490cad944704cd7da85c622feb418a2ea8))
- **core:** Mark binary data to be deleted when pruning executions ([#4713](https://github.com/n8n-io/n8n/issues/4713)) ([78c66f1](https://github.com/n8n-io/n8n/commit/78c66f16d6c4677a63be18d823866ad3d1414843))
- **core:** OAuth2 scope saved to DB fix ([7cb5dc2](https://github.com/n8n-io/n8n/commit/7cb5dc2aa5d15c574b0e07d0d7fa23dd9a9996ea))
- Credential overwrites should take precedence over credential default values ([#4782](https://github.com/n8n-io/n8n/issues/4782)) ([2ce6291](https://github.com/n8n-io/n8n/commit/2ce62917da514714b7198cab63dcfc0b1ebc0473))
- **editor:** Fix slots rendering of NodeCreator's NoResults component ([#4721](https://github.com/n8n-io/n8n/issues/4721)) ([d8c2dff](https://github.com/n8n-io/n8n/commit/d8c2dffc37155eb013a12d21cab6504264d16b8e))
- **editor:** JSON view values can be mapped like keys ([#4702](https://github.com/n8n-io/n8n/issues/4702)) ([6d4e959](https://github.com/n8n-io/n8n/commit/6d4e9598846c9c2eb128ce039d4aeae080178627))
- **Google Sheets Node:** Fix exception if no matching rows are found ([579f9c4](https://github.com/n8n-io/n8n/commit/579f9c4d4e5907a4ffba9a7ec6bcbb5d2faaefb9))
- **Google Sheets Node:** Fix for append operation if no empty rows in sheet ([741c7da](https://github.com/n8n-io/n8n/commit/741c7da8b1a3f2824613d2a4c4880423c8be91cb))
- Lazy load nodes for credentials testing ([#4760](https://github.com/n8n-io/n8n/issues/4760)) ([0a7a2f3](https://github.com/n8n-io/n8n/commit/0a7a2f3e4179c6bd186547dd43a5c43400c18ff8))
- **Microsoft Outlook Node:** Fix binary attachment upload ([#4766](https://github.com/n8n-io/n8n/issues/4766)) ([528439c](https://github.com/n8n-io/n8n/commit/528439cb4d5ff3f61dddf75dea6377f508429155))
- **Pipedrive Node:** Resolve properties not working ([c853b80](https://github.com/n8n-io/n8n/commit/c853b8078e66a671df448106956a0929c5b19b0a))
- Remove background for resource ownership selector ([#4748](https://github.com/n8n-io/n8n/issues/4748)) ([30214f2](https://github.com/n8n-io/n8n/commit/30214f2bc20da18e16924e4047891a6ea8586593))
- Update padding for resource filters dropdown ([#4751](https://github.com/n8n-io/n8n/issues/4751)) ([aff8cd9](https://github.com/n8n-io/n8n/commit/aff8cd9a2b376a429450661f108cdf8eb6e6d082))
- Update size of select components in filters dropdown ([#4747](https://github.com/n8n-io/n8n/issues/4747)) ([d6d442d](https://github.com/n8n-io/n8n/commit/d6d442d45882423661631ee40b732ed78543abfc))
- Update workflow save button type and design and share button type ([#4752](https://github.com/n8n-io/n8n/issues/4752)) ([b89301e](https://github.com/n8n-io/n8n/commit/b89301ec36fdbdc2a1d7c8996526b55930c20335))

### Features

- **editor:** Overhaul expression editor modal ([#4631](https://github.com/n8n-io/n8n/issues/4631)) ([59771c8](https://github.com/n8n-io/n8n/commit/59771c80ea6ccd1b0da4946f6d017e02b8016609))
- **Facebook Graph API Node:** Update to support api version 15 ([#4791](https://github.com/n8n-io/n8n/issues/4791)) ([2a85af1](https://github.com/n8n-io/n8n/commit/2a85af1bdb7098463085f1e5c96b25f820e19e15))
- **Google Calendar Node:** Use resource locator component for calendar parameters ([#4410](https://github.com/n8n-io/n8n/issues/4410)) ([b319671](https://github.com/n8n-io/n8n/commit/b319671fd0f0488488788b472af140014bd7cc99))
- **Postmark Trigger Node:** Update credentials so they can be used with the HTTP Request Node ([#4790](https://github.com/n8n-io/n8n/issues/4790)) ([0c759dc](https://github.com/n8n-io/n8n/commit/0c759dc548c058372fde5d117ea34489f7a6a2d9))
- **Todoist Node:** Update to use latest api version ([#4650](https://github.com/n8n-io/n8n/issues/4650)) ([09a48c5](https://github.com/n8n-io/n8n/commit/09a48c51b64aaf31888e98b7f2711140e9818bed))

# [0.204.0](https://github.com/n8n-io/n8n/compare/n8n@0.203.1...n8n@0.204.0) (2022-11-24)

### Bug Fixes

- **core:** Fix `$items().length` behavior in `executeOnce` mode ([#4694](https://github.com/n8n-io/n8n/issues/4694)) ([b87c122](https://github.com/n8n-io/n8n/commit/b87c12285fa2b339e726f81e271715e258b6a075))
- **core:** Fix for unused imports ([a6df51b](https://github.com/n8n-io/n8n/commit/a6df51b6e83fa25dad962ab212123edb3c055cac))
- **core:** Use CredentialsOverwrites when testing credentials ([#4675](https://github.com/n8n-io/n8n/issues/4675)) ([772ec78](https://github.com/n8n-io/n8n/commit/772ec78349b5b6877bf681f3262951e3a4e34fe4))
- Disable workflow locking due to issues ([#4708](https://github.com/n8n-io/n8n/issues/4708)) ([ee6ac5d](https://github.com/n8n-io/n8n/commit/ee6ac5d3417a2f308a7f4a3cda18c01fcec57faf))
- **editor:** Fix for missing node connections in dev environment ([#4707](https://github.com/n8n-io/n8n/issues/4707)) ([b18ae18](https://github.com/n8n-io/n8n/commit/b18ae18a6b10fb125f3eed73103e33e3519cd82c))
- **editor:** Fix missing resource locator component ([#4649](https://github.com/n8n-io/n8n/issues/4649)) ([44182f2](https://github.com/n8n-io/n8n/commit/44182f23a5e62c53209b3fa19edd1727586551ff))
- **editor:** Prevent node-creator tabs from showing when toggled by CanvasAddButton ([#4661](https://github.com/n8n-io/n8n/issues/4661)) ([60746dc](https://github.com/n8n-io/n8n/commit/60746dc92ee1b6c33015e2a6a0d34bc981aa1dd5))
- **editor:** Table view column limit tooltip ([#4655](https://github.com/n8n-io/n8n/issues/4655)) ([3ac9ba3](https://github.com/n8n-io/n8n/commit/3ac9ba3491c0dc1de283bc4285a243e02747f971))
- Fix broken n8n-info-tip slots ([#4665](https://github.com/n8n-io/n8n/issues/4665)) ([6c99223](https://github.com/n8n-io/n8n/commit/6c992233a053db1ea235f785a52a754c1e694555))
- **IF Node:** Fix "Is Empty" and "Is Not Empty" operation fails for date objects ([#4670](https://github.com/n8n-io/n8n/issues/4670)) ([753f4c9](https://github.com/n8n-io/n8n/commit/753f4c9a7d34c8d3329d4dc024fcf272f6f47ff3))
- Remove redundant await in node's api request functions without try/catch ([#4639](https://github.com/n8n-io/n8n/issues/4639)) ([67983e8](https://github.com/n8n-io/n8n/commit/67983e8f945397d3fb0be55fdeb47609be92b2cb))
- **Schedule Trigger Node:** Fixes inconsitent behavior with cron and weekly intervals ([#4558](https://github.com/n8n-io/n8n/issues/4558)) ([2fb8ed8](https://github.com/n8n-io/n8n/commit/2fb8ed825b18118fc0783e95d1551ee2ce8c3a38))
- Workflow activation should not crash if one of the credential is invalid ([#4671](https://github.com/n8n-io/n8n/issues/4671)) ([c0e13c2](https://github.com/n8n-io/n8n/commit/c0e13c2a8f9374e9c65aae3ce4102e37c993cf74))

### Features

- Add credentials E2E test suite and page object ([#4596](https://github.com/n8n-io/n8n/issues/4596)) ([b5b44d1](https://github.com/n8n-io/n8n/commit/b5b44d1b598e67ef7e735d7cdfb5233ca72caca6))
- Add save confirmation modal when leaving sharing modal ([#4683](https://github.com/n8n-io/n8n/issues/4683)) ([173badc](https://github.com/n8n-io/n8n/commit/173badc4e099ebb818686dc5a25c2192c138bcd9))
- Add share button to workflows list ([#4681](https://github.com/n8n-io/n8n/issues/4681)) ([a356d7b](https://github.com/n8n-io/n8n/commit/a356d7bdbadd5a4c69c61c5a5a30e75e9765e3d2))
- **core:** Add license support to n8n ([#4566](https://github.com/n8n-io/n8n/issues/4566)) ([30e5d3d](https://github.com/n8n-io/n8n/commit/30e5d3d04c3457780875cc36637c8c1ea14ec783))
- **core:** Lazy-load nodes and credentials to reduce baseline memory usage ([#4577](https://github.com/n8n-io/n8n/issues/4577)) ([b6c57e1](https://github.com/n8n-io/n8n/commit/b6c57e19fc5683dd7fb9eabb60ec4e89359c59eb))
- **editor:** Add workflows list status filter ([#4690](https://github.com/n8n-io/n8n/issues/4690)) ([5364e7f](https://github.com/n8n-io/n8n/commit/5364e7fc9250421b799adc28b3e47dc75819ec7d))
- Show delete button based on workflow permissions ([#4686](https://github.com/n8n-io/n8n/issues/4686)) ([4f64e26](https://github.com/n8n-io/n8n/commit/4f64e26a83c7e62c98d93c38bf3dcb6cdfaadb58))
- Show toast when saving workflow sharing settings ([#4684](https://github.com/n8n-io/n8n/issues/4684)) ([6f8d0de](https://github.com/n8n-io/n8n/commit/6f8d0de55dc9c3c1cdb17329a8560ee8453c639a))
- Switch owner subview to all subview if has shared resources ([#4672](https://github.com/n8n-io/n8n/issues/4672)) ([e3e17e5](https://github.com/n8n-io/n8n/commit/e3e17e5dac685b1230e39bbef247312419b71f9b))
- Use longer stack-traces when error-reporting is enabled ([#4674](https://github.com/n8n-io/n8n/issues/4674)) ([de5b0b0](https://github.com/n8n-io/n8n/commit/de5b0b03fedede680f5a6e0f4dc73770b888bf46))

### Performance Improvements

- **Code Node:** Improve n8n item key validation performance ([#4669](https://github.com/n8n-io/n8n/issues/4669)) ([740513b](https://github.com/n8n-io/n8n/commit/740513b42440b8760cd488659e92abe9951462b0))

## [0.203.1](https://github.com/n8n-io/n8n/compare/n8n@0.203.0...n8n@0.203.1) (2022-11-18)

### Bug Fixes

- **Google Sheets Node:** Versioning fix ([4e66672](https://github.com/n8n-io/n8n/commit/4e66672df225e67297981b7ee3408e5849db418a))

# [0.203.0](https://github.com/n8n-io/n8n/compare/n8n@0.202.1...n8n@0.203.0) (2022-11-17)

### Bug Fixes

- Add back mapping hint when parameter is focused ([#4634](https://github.com/n8n-io/n8n/issues/4634)) ([b35172e](https://github.com/n8n-io/n8n/commit/b35172e442a131f76c2d902d451356ab937bba48))
- **core:** Deduplicate error handling in nodes ([#4319](https://github.com/n8n-io/n8n/issues/4319)) ([c7133ec](https://github.com/n8n-io/n8n/commit/c7133ecd3fe6f022a537b6edb4c006d6786efad2))
- **editor:** Add 'Stop execution' button to execution preview ([#4632](https://github.com/n8n-io/n8n/issues/4632)) ([be7672a](https://github.com/n8n-io/n8n/commit/be7672a177bfcf997ec241af7c628a90312849b1))
- **editor:** Curb direct item access linting ([#4591](https://github.com/n8n-io/n8n/issues/4591)) ([271cd06](https://github.com/n8n-io/n8n/commit/271cd06a6ac6274a83a6a71fe76072281edf3724))
- **editor:** Fix expression editor variable selector filter ([#4590](https://github.com/n8n-io/n8n/issues/4590)) ([69b332b](https://github.com/n8n-io/n8n/commit/69b332b0e3321d3d1c635e53ec134d15b7e54bb9))
- **editor:** Fix for execution retry dropdown not closing ([#4575](https://github.com/n8n-io/n8n/issues/4575)) ([e0ec5a6](https://github.com/n8n-io/n8n/commit/e0ec5a6aa932db281aafe07be65aa86719e41b09))
- **editor:** Fix for logging error on user logout ([#4633](https://github.com/n8n-io/n8n/issues/4633)) ([7483e14](https://github.com/n8n-io/n8n/commit/7483e147fc552d981d03d0e96112725335c64002))
- **editor:** Fix zero treated as missing value in resource locator ([#4612](https://github.com/n8n-io/n8n/issues/4612)) ([b0bbcf6](https://github.com/n8n-io/n8n/commit/b0bbcf6028dcf3b9e25dacb1aee06a79f45f9e04))
- **editor:** Hide pin data in production executions ([#4595](https://github.com/n8n-io/n8n/issues/4595)) ([edebad1](https://github.com/n8n-io/n8n/commit/edebad1a89f1dd239c833c166a6e7f845d6df035))
- **editor:** Skip optional chaining operators in Code Node editor linting ([#4592](https://github.com/n8n-io/n8n/issues/4592)) ([ccacd42](https://github.com/n8n-io/n8n/commit/ccacd42b3706267b704f370f1044eb1ca7f5286c))
- **editor:** Update to 'Expression/Fixed' toggle - Keep expression when switching to Fixed ([#4599](https://github.com/n8n-io/n8n/issues/4599)) ([6eee155](https://github.com/n8n-io/n8n/commit/6eee155ecb91c680c5a9d4f23502da35ab249a9d))
- Fix foreign credentials being shown for new nodes ([#4622](https://github.com/n8n-io/n8n/issues/4622)) ([dea67ca](https://github.com/n8n-io/n8n/commit/dea67ca6b7eee02fd5ea24c48224c65e937e97f2))
- Fix user redirect to signin bug ([#4623](https://github.com/n8n-io/n8n/issues/4623)) ([402b75a](https://github.com/n8n-io/n8n/commit/402b75ac280cf74df30aaf758f1c0a15762ad996))
- Store copy of workflow in workflowsById to prevent node data bugs ([#4637](https://github.com/n8n-io/n8n/issues/4637)) ([9cadaea](https://github.com/n8n-io/n8n/commit/9cadaea3a44b8b983a2c8c1e78271ffcd114ef4d))

### Features

- Add duplicate workflow error handler ([#4616](https://github.com/n8n-io/n8n/issues/4616)) ([f7a9ef9](https://github.com/n8n-io/n8n/commit/f7a9ef91166df1a71db1f7827cb43ffd687839d4))
- Add workflow data reset action ([#4618](https://github.com/n8n-io/n8n/issues/4618)) ([0daa36c](https://github.com/n8n-io/n8n/commit/0daa36c1978c6722d178e16c6f756b7205068c09))
- **Compare Datasets Node:** Node tweaks ([423ee81](https://github.com/n8n-io/n8n/commit/423ee81e33b88c5ed6152b75b69219c3e4ff16c8))
- **core:** Add credential runtime checks and prevent tampering in manual run ([#4481](https://github.com/n8n-io/n8n/issues/4481)) ([d35d63a](https://github.com/n8n-io/n8n/commit/d35d63a855522c781b38238e107a6aaa211764c6))
- **Google Sheets Node:** Overhaul of node ([d96d6f1](https://github.com/n8n-io/n8n/commit/d96d6f11dbe2f1c75ff572baa4906fb628a2eb5c))
- **Notion (Beta) Node:** Use resource locator component for database and page parameters ([#4340](https://github.com/n8n-io/n8n/issues/4340)) ([277b6b7](https://github.com/n8n-io/n8n/commit/277b6b73c37187f524474364c3b58adbc15486e0))

## [0.202.1](https://github.com/n8n-io/n8n/compare/n8n@0.202.0...n8n@0.202.1) (2022-11-10)

### Bug Fixes

- Disable some error tracking ([#4579](https://github.com/n8n-io/n8n/issues/4579)) ([b2201d0](https://github.com/n8n-io/n8n/commit/b2201d0c77cf024e39f6569e7806871d38408201))

# [0.202.0](https://github.com/n8n-io/n8n/compare/n8n@0.201.0...n8n@0.202.0) (2022-11-10)

### Bug Fixes

- **API:** Do not use names for typeorm connections ([#4532](https://github.com/n8n-io/n8n/issues/4532)) ([f5c2080](https://github.com/n8n-io/n8n/commit/f5c20803d782d06ffc42dabd0a11467d44bd1888))
- **core:** Fix manual execution of pinned trigger on main mode ([#4535](https://github.com/n8n-io/n8n/issues/4535)) ([5d73b6e](https://github.com/n8n-io/n8n/commit/5d73b6e48aef2b0b386369b7d1f208845f912da5))
- **core:** Streamline multiple pinned triggers behavior ([#4569](https://github.com/n8n-io/n8n/issues/4569)) ([953457a](https://github.com/n8n-io/n8n/commit/953457ad8676501f9c92eb1f7bb68521a975975c))
- **editor:** Curb arg linting for `$input.first()` and `$input.last()` ([#4526](https://github.com/n8n-io/n8n/issues/4526)) ([0edd4bc](https://github.com/n8n-io/n8n/commit/0edd4bcc8783de0da591ad147700c450e01ba919))
- **editor:** Fix duplicate bug when new workflow is open ([#4559](https://github.com/n8n-io/n8n/issues/4559)) ([536c834](https://github.com/n8n-io/n8n/commit/536c834313b73bf36f9c9cc291dca4e4b4b860be))
- **editor:** Fix for incorrect execution saving indicator in executions view ([#4547](https://github.com/n8n-io/n8n/issues/4547)) ([0117191](https://github.com/n8n-io/n8n/commit/01171912e7587933792e5cd1cd605a6ec3b0b1be))
- **editor:** Fix for oauth authorization ([#4572](https://github.com/n8n-io/n8n/issues/4572)) ([d06197d](https://github.com/n8n-io/n8n/commit/d06197d879707c6a9826ae192682262c4f6c02ed))
- **editor:** Fix workflow activation from the Workflows view ([#4549](https://github.com/n8n-io/n8n/issues/4549)) ([d2bec63](https://github.com/n8n-io/n8n/commit/d2bec63cecbc39f1881a883d36b6a2c3ea1568a9))
- **editor:** Fix workflow back button navigation ([#4546](https://github.com/n8n-io/n8n/issues/4546)) ([825637f](https://github.com/n8n-io/n8n/commit/825637f02a5d1bc9f00cb68f19221dd7d0e055cb))
- **editor:** Prevent adding of the start node when importing workflow in the demo mode ([#4564](https://github.com/n8n-io/n8n/issues/4564)) ([49748f2](https://github.com/n8n-io/n8n/commit/49748f27a2bfbb0356ba2c30c35d34a3ad9d8063))
- **editor:** Show string numbers and null properly in JSON view ([#4513](https://github.com/n8n-io/n8n/issues/4513)) ([f6b85f4](https://github.com/n8n-io/n8n/commit/f6b85f4a69adbad10854ff77015d0d2ee69cfeac))
- **editor:** Switch `CodeNodeEditor` linter parser to `esprima-next` ([#4524](https://github.com/n8n-io/n8n/issues/4524)) ([5e0ded4](https://github.com/n8n-io/n8n/commit/5e0ded4a84a3da1fc4cd32d135cb4eb30dbd9b35))
- **editor:** Tweak dragged mapping state ([#4550](https://github.com/n8n-io/n8n/issues/4550)) ([b3cd62d](https://github.com/n8n-io/n8n/commit/b3cd62d866eeb734de253f656ee2b67c147a10c1))
- **editor:** Update workflow buttons spacings ([#4534](https://github.com/n8n-io/n8n/issues/4534)) ([88baaa0](https://github.com/n8n-io/n8n/commit/88baaa0eb15f3d1cff22ed5994b0cd39bddf5b7b))
- **editor:** Use base path in workflow preview component URL ([#4560](https://github.com/n8n-io/n8n/issues/4560)) ([db163b7](https://github.com/n8n-io/n8n/commit/db163b71b90d073cc963f63d5455b3a84f236917))
- **HTTP Request Node:** Show error cause in the output ([#4538](https://github.com/n8n-io/n8n/issues/4538)) ([c239eea](https://github.com/n8n-io/n8n/commit/c239eea1b9fc7c7397db8135528ac0d136be1c84))
- **HTTP Request Node:** Use the data in "Put Output in Field" field ([#4487](https://github.com/n8n-io/n8n/issues/4487)) ([39d4bb2](https://github.com/n8n-io/n8n/commit/39d4bb2639794eeb9c2e998daaac3accad1802b4))
- **HubSpot Node:** Add notice to HubSpot credentials about API Key Sunset ([#4570](https://github.com/n8n-io/n8n/issues/4570)) ([9b5db8d](https://github.com/n8n-io/n8n/commit/9b5db8d7be501ff06e49fd25ce9e0f3e9aa8fbea))
- **Notion Trigger (Beta) Node:** Fix Notion trigger polling strategy ([3b34050](https://github.com/n8n-io/n8n/commit/3b3405089d9194515192f10ab4085e1493bb86b5))
- **Raindrop Node:** Update access token URL ([#4542](https://github.com/n8n-io/n8n/issues/4542)) ([740df0c](https://github.com/n8n-io/n8n/commit/740df0c1e5e578269fcaa0ce767c5894c6a852d4))
- **SendInBlue Trigger Node:** Fix typo in credential name ([#4357](https://github.com/n8n-io/n8n/issues/4357)) ([5d852f9](https://github.com/n8n-io/n8n/commit/5d852f9230a73c04b5242803949117cce8bffeed))
- Update E2E testing env variables ([#4556](https://github.com/n8n-io/n8n/issues/4556)) ([f9d9f88](https://github.com/n8n-io/n8n/commit/f9d9f88f8a9d217101c2f5c67f3d3db6aa6b9b92))

### Features

- Add cypress e2e tests for signup and signin ([#3490](https://github.com/n8n-io/n8n/issues/3490)) ([7764486](https://github.com/n8n-io/n8n/commit/77644860c0fcd3d78732097ebf5d0b0457da7d57))
- **API:** Report unhandled app crashes to Sentry ([#4548](https://github.com/n8n-io/n8n/issues/4548)) ([2425c10](https://github.com/n8n-io/n8n/commit/2425c10b2b5ec65bfb05d3f6443a139ec71c6a9a))
- **API:** Set up error tracking using Sentry ([#4394](https://github.com/n8n-io/n8n/issues/4394)) ([41cb0ee](https://github.com/n8n-io/n8n/commit/41cb0eec6e634f3f346644f885f8a6064e77cc7b))
- **core:** Add ownership, sharing and credential details to `GET /workflows` ([#4510](https://github.com/n8n-io/n8n/issues/4510)) ([026fb50](https://github.com/n8n-io/n8n/commit/026fb50512d6a31bf483646ec68276fb6f39abfe))
- **editor:** Add support for notice credentials properties ([#4557](https://github.com/n8n-io/n8n/issues/4557)) ([de96def](https://github.com/n8n-io/n8n/commit/de96def372d63df27c3433bca4fae6f75c874e8e))
- Switch from npm to pnpm ([#4429](https://github.com/n8n-io/n8n/issues/4429)) ([7367773](https://github.com/n8n-io/n8n/commit/736777385c54d5b20174c9c1fda38bb31fbf14b4))

# [0.201.0](https://github.com/n8n-io/n8n/compare/n8n@0.200.1...n8n@0.201.0) (2022-11-02)

### Bug Fixes

- **core:** Fix workflow hasing for MySQL ([#4491](https://github.com/n8n-io/n8n/issues/4491)) ([2b5613e](https://github.com/n8n-io/n8n/commit/2b5613ed68ecc6991ec68ca21807cbc1e976aa22))
- **core:** Make `deepCopy` backward compatible ([#4505](https://github.com/n8n-io/n8n/issues/4505)) ([b282c7e](https://github.com/n8n-io/n8n/commit/b282c7e5d98c94b13a861167fef8af204267c5bd)), closes [#4508](https://github.com/n8n-io/n8n/issues/4508)
- displayOptions not getting value of RLC ([#4460](https://github.com/n8n-io/n8n/issues/4460)) ([3a1fa09](https://github.com/n8n-io/n8n/commit/3a1fa09108a115609e2dbbf257603ef5d7fc91d2))
- **editor:** Disable settings link in executions view for unsaved workflows ([#4493](https://github.com/n8n-io/n8n/issues/4493)) ([dcec5e9](https://github.com/n8n-io/n8n/commit/dcec5e9e8231609a9461acb196ab157ab6fabcd2))
- **editor:** Fix an issue with not being able to save some of the forms ([#4499](https://github.com/n8n-io/n8n/issues/4499)) ([1e445fc](https://github.com/n8n-io/n8n/commit/1e445fc1a38dd7541ee6fcc4b535180fa3844799))
- **editor:** Fix interim updates on executions view ([#4497](https://github.com/n8n-io/n8n/issues/4497)) ([cf034c0](https://github.com/n8n-io/n8n/commit/cf034c015fee7bc6eead0e4901bafef3a08fe88b))
- **editor:** Gix node creator search when there's active subcategory ([#4494](https://github.com/n8n-io/n8n/issues/4494)) ([f244975](https://github.com/n8n-io/n8n/commit/f24497589f9bff176ea8df3196e9aaaaef7dfb51))
- **editor:** : Limit columns in table view to prevent unresponsive UI when opening NDV ([#4480](https://github.com/n8n-io/n8n/issues/4480)) ([41e6489](https://github.com/n8n-io/n8n/commit/41e6489b75414c7fe55531223aa23f0817401539))

### Features

- **core:** Reimplement blocking workflow updates on interim changes ([#4446](https://github.com/n8n-io/n8n/issues/4446)) ([46905fd](https://github.com/n8n-io/n8n/commit/46905fd2cbcdbff7cf8056e010524fc0b74b7d53))
- **editor:** Block UI in NDV when workflow is listening to events ([#4390](https://github.com/n8n-io/n8n/issues/4390)) ([6c2c621](https://github.com/n8n-io/n8n/commit/6c2c621f1debcef73ca789204a651c3f5f23628e))
- **Venafi TLS Protect Cloud Node:** Make issuing template depend on application ([#4476](https://github.com/n8n-io/n8n/issues/4476)) ([d1d1288](https://github.com/n8n-io/n8n/commit/d1d1288ba91a6ebe9667f1c026e4575407fb5a70))

### Performance Improvements

- **editor:** Improve array intersection utility function ([#4503](https://github.com/n8n-io/n8n/issues/4503)) ([b0df810](https://github.com/n8n-io/n8n/commit/b0df8107458e3f6cbfccfc21a717e4085c4ab3d5))

## [0.200.1](https://github.com/n8n-io/n8n/compare/n8n@0.200.0...n8n@0.200.1) (2022-10-28)

### Bug Fixes

- **API:** Do not reset the auth cookie on every request to `GET /login` ([#4459](https://github.com/n8n-io/n8n/issues/4459)) ([c66929f](https://github.com/n8n-io/n8n/commit/c66929f53d87035160ad099873d73cea3fff4d2a))
- **AWS SNS Trigger Node:** Add missing jsonParse import ([#4463](https://github.com/n8n-io/n8n/issues/4463)) ([e6ec134](https://github.com/n8n-io/n8n/commit/e6ec134cf37ac21b26d10162b3d49da7dad85a1a))
- **core:** Updating deepCopy to avoid max callstack with circular deps ([#4468](https://github.com/n8n-io/n8n/issues/4468)) ([ca60b0e](https://github.com/n8n-io/n8n/commit/ca60b0e203d950605506eb7687a10b5c87b4492f))
- **editor:** Fix for executions view auto-refresh and new workflow saving ([#4462](https://github.com/n8n-io/n8n/issues/4462)) ([dbac795](https://github.com/n8n-io/n8n/commit/dbac7955f94007a8b305400ae28ccf1e5c040261))
- **editor:** Redirect old path /workflow ([#4469](https://github.com/n8n-io/n8n/issues/4469)) ([7620d93](https://github.com/n8n-io/n8n/commit/7620d93eda525c528823c20e83883ad10020bd76))
- **editor:** Remove filter that prevented showing running executions ([#4470](https://github.com/n8n-io/n8n/issues/4470)) ([658e886](https://github.com/n8n-io/n8n/commit/658e886861acb5897e9e87cf4d66cee9b6a6003a))

# [0.200.0](https://github.com/n8n-io/n8n/compare/n8n@0.199.0...n8n@0.200.0) (2022-10-27)

### Bug Fixes

- **API:** Validate excecutions and workflow filter parameters ([#4424](https://github.com/n8n-io/n8n/issues/4424)) ([dd3c596](https://github.com/n8n-io/n8n/commit/dd3c59677bbdcb49332975fd84d9e88852f76c8d))
- **core:** Amend typing for `jsonParse()` options ([#4423](https://github.com/n8n-io/n8n/issues/4423)) ([1732324](https://github.com/n8n-io/n8n/commit/1732324965cce2030d0198f7b7e7091edfad6727))
- **core:** Fix `predefinedCredentialType` in node graph item ([#4379](https://github.com/n8n-io/n8n/issues/4379)) ([77233f2](https://github.com/n8n-io/n8n/commit/77233f23701fa456a7d0170dc0b8118afa71a8c5))
- **core:** Fix canvas node execution skipping parent nodes ([#4438](https://github.com/n8n-io/n8n/issues/4438)) ([3a9684d](https://github.com/n8n-io/n8n/commit/3a9684df9f26464b3e1f9924871304f136de61fd))
- **core:** Fix single-node execution failing in `main` mode ([#4421](https://github.com/n8n-io/n8n/issues/4421)) ([5745027](https://github.com/n8n-io/n8n/commit/5745027cee9d3cb92dfc9d9025a0645f50185752))
- **core:** Set JWT authentication token sameSite policy to lax ([#4425](https://github.com/n8n-io/n8n/issues/4425)) ([1f4eaeb](https://github.com/n8n-io/n8n/commit/1f4eaeb3ae33ad88a4b07e664e2f8f8f1235bc6f))
- **core:** Update to imports in helpers ([91bd3c6](https://github.com/n8n-io/n8n/commit/91bd3c6567401dedb0216a07ab31310e451ff1e7))
- **editor:** Curb item method linting in single-item mode in `CodeNodeEditor` linter ([#4455](https://github.com/n8n-io/n8n/issues/4455)) ([b226aed](https://github.com/n8n-io/n8n/commit/b226aed9bb60981e1a69b799f3b57ba56b7bbaa1))
- **editor:** Stop rendering expressions as html ([#4420](https://github.com/n8n-io/n8n/issues/4420)) ([779b0d5](https://github.com/n8n-io/n8n/commit/779b0d58f741b9e8eea978f1651701e586d722c4))
- **Email Trigger (IMAP) Node:** Backport V2 mark-seen-after-processing to V1 ([#4435](https://github.com/n8n-io/n8n/issues/4435)) ([b296fb0](https://github.com/n8n-io/n8n/commit/b296fb06f3222ad56c9d8267f8b8283097fde113))
- **Email Trigger (IMAP) Node:** Improve connection handling and credentials ([#4393](https://github.com/n8n-io/n8n/issues/4393)) ([1a37f00](https://github.com/n8n-io/n8n/commit/1a37f0003f5d7029bc36ba91d51235e96e8719cc))
- **HTTP Request Node:** Fix sending previously selected credentials ([#4457](https://github.com/n8n-io/n8n/issues/4457)) ([44ad249](https://github.com/n8n-io/n8n/commit/44ad249827d47e0cc9584edcb2e2bcf7b088f026))
- **InvoiceNinja Node:** Added support for v5 ([2f4649c](https://github.com/n8n-io/n8n/commit/2f4649cdf44e15b41b40879f27ffe39406a53b1b))
- **TheHive Node:** Fix node issues ([ca9eca9](https://github.com/n8n-io/n8n/commit/ca9eca9ae9e168886502649458ccdb67d1261c09))

### Features

- **Airtable Trigger Node:** Use resource locator component for base and table parameters ([#4391](https://github.com/n8n-io/n8n/issues/4391)) ([227212c](https://github.com/n8n-io/n8n/commit/227212c928535f302879e9be6b585faa41c95b80))
- **core, editor:** Introduce workflow caller policy ([#4368](https://github.com/n8n-io/n8n/issues/4368)) ([e8935de](https://github.com/n8n-io/n8n/commit/e8935de3b2dbbf25df139c59fbdd298528397eca))
- **core:** Block workflow update on interim change ([#4397](https://github.com/n8n-io/n8n/issues/4397)) ([cddd012](https://github.com/n8n-io/n8n/commit/cddd012a2fa834ca6b3d85296caadcf3b8cc7bb5))
- **editor:** Add readonly state for nodes ([#4299](https://github.com/n8n-io/n8n/issues/4299)) ([408bd96](https://github.com/n8n-io/n8n/commit/408bd968152ad8bbafda7037f6eb8f5550d04c77))
- **editor:** Implement executions preview via the new executions tab in node view ([#4311](https://github.com/n8n-io/n8n/issues/4311)) ([d833345](https://github.com/n8n-io/n8n/commit/d833345092baf3c12828a5a7680c9fb8555d2c57))
- **editor:** Improve nodes panel search ([#4399](https://github.com/n8n-io/n8n/issues/4399)) ([f6733cf](https://github.com/n8n-io/n8n/commit/f6733cff9d88d9b3298f6afc2c59c0dea59c6464))
- **HTTP Request Node:** Add option for raw json header & query ([#4408](https://github.com/n8n-io/n8n/issues/4408)) ([8f25da5](https://github.com/n8n-io/n8n/commit/8f25da52b1c2d228018df8186985a2b067bd2123))
- **Write Binary File Node:** Add option to append to a file ([#4386](https://github.com/n8n-io/n8n/issues/4386)) ([4b13b33](https://github.com/n8n-io/n8n/commit/4b13b3398dce5338f46c80867d6e4c8c685f6c22))

# [0.199.0](https://github.com/n8n-io/n8n/compare/n8n@0.198.2...n8n@0.199.0) (2022-10-21)

### Bug Fixes

- **CompareDatasets Node:** Removed quotes from branch names ([263794c](https://github.com/n8n-io/n8n/commit/263794ce4038720181b147f8468dc07db33ec3ee))
- **editor:** Fix bottom menu hover bug ([#4349](https://github.com/n8n-io/n8n/issues/4349)) ([353a28b](https://github.com/n8n-io/n8n/commit/353a28bfe75ef75983df965cedfea2053c3cccfa))
- **editor:** Fix pairedItem telemetry error reporting ([b67e41b](https://github.com/n8n-io/n8n/commit/b67e41b45ee43a215a476adbf0c0b7bf6121e5d5))
- **editor:** Fix performance issues when opening node or editing code node with a lot of data ([#4388](https://github.com/n8n-io/n8n/issues/4388)) ([356a42a](https://github.com/n8n-io/n8n/commit/356a42a18752eaf7b70ee2e0c41ef6f248cd10b8))
- **editor:** Fix workflow not stopping on clicking stop button ([#4382](https://github.com/n8n-io/n8n/issues/4382)) ([50c18a7](https://github.com/n8n-io/n8n/commit/50c18a789a79b23a95830bdfd376ed6461d852d5))
- **editor:** Prevent text highlight on FireFox when mapping data ([#4347](https://github.com/n8n-io/n8n/issues/4347)) ([e1e2c94](https://github.com/n8n-io/n8n/commit/e1e2c943316a29bda989f3d96a7a40e3f57e3bab))
- **editor:** Remove wrong linting from Code node editor ([#4384](https://github.com/n8n-io/n8n/issues/4384)) ([77d041b](https://github.com/n8n-io/n8n/commit/77d041ba783a536b0572ef68ab4eeac8118c8ba8))
- **editor:** Replace cron node with schedule node ([#4371](https://github.com/n8n-io/n8n/issues/4371)) ([161cca9](https://github.com/n8n-io/n8n/commit/161cca9494eb115d4707a9fc3d273ba732b9da76))
- **editor:** Show null value in table view ([#4346](https://github.com/n8n-io/n8n/issues/4346)) ([bb4e08c](https://github.com/n8n-io/n8n/commit/bb4e08c0766487b150fad4ec3ee301d765d413d3))
- **Elasticsearch Node:** Fix pagination issue ([a02e92d](https://github.com/n8n-io/n8n/commit/a02e92d664b2896ee1abd30c761e25e96f4f44e3))
- **Google Drive Node:** Fix drive hint typo in resource locator ([#4387](https://github.com/n8n-io/n8n/issues/4387)) ([4ce0fed](https://github.com/n8n-io/n8n/commit/4ce0fed0ab2d464d9fa4051fed070f86a64fef57))
- **HTTP Request Node:** Avoid error when response doesn't include content-type ([#4365](https://github.com/n8n-io/n8n/issues/4365)) ([61b9909](https://github.com/n8n-io/n8n/commit/61b9909ac3925d51eb767542b70c82e57905b392))
- **n8n Node:** Fix resource locator not returning all items ([#4248](https://github.com/n8n-io/n8n/issues/4248)) ([ed4dcbb](https://github.com/n8n-io/n8n/commit/ed4dcbb5ddf3ded5ec9faa16badc128a0fcecf26))
- **Shedule Node:** Fixes multiple intervals, fixes week interval ([#4376](https://github.com/n8n-io/n8n/issues/4376)) ([971c2c0](https://github.com/n8n-io/n8n/commit/971c2c0aed0a2402fa6eb6217ddc914d1fade68b))

### Features

- **Compare Node:** New node to compare two inputs ([638d6f6](https://github.com/n8n-io/n8n/commit/638d6f60d3f1abd7f647cfe2964259a889e6cd1a))
- **core:** Block workflow update on interim change ([#4374](https://github.com/n8n-io/n8n/issues/4374)) ([e83b9bd](https://github.com/n8n-io/n8n/commit/e83b9bd98395fcdb1238f9226c08cf88a259654c))
- **core:** Enable sending client credentials in body ([#4377](https://github.com/n8n-io/n8n/issues/4377)) ([7fcd821](https://github.com/n8n-io/n8n/commit/7fcd821cadca942bd1321229f9f0f76fe663dc34))
- **editor, core, cli:** Implement new workflow experience ([#4358](https://github.com/n8n-io/n8n/issues/4358)) ([dae01f3](https://github.com/n8n-io/n8n/commit/dae01f3abef57fcb62af1e2e15d807d612ab4252))
- **editor:** Add automatic credential selection for new nodes ([#2746](https://github.com/n8n-io/n8n/issues/2746)) ([d31fbbb](https://github.com/n8n-io/n8n/commit/d31fbbba27895c5ab1ccdbf6d8c94b5b7b00893e))
- **editor:** Create new workflows page ([#4267](https://github.com/n8n-io/n8n/issues/4267)) ([be7aac3](https://github.com/n8n-io/n8n/commit/be7aac32797a2e4b3ffcd696ed700e5479692cbd))
- **editor:** Switch initial route based on feature flag ([#4383](https://github.com/n8n-io/n8n/issues/4383)) ([6d25eed](https://github.com/n8n-io/n8n/commit/6d25eed0500956ffe14022e396b5e9e628d80176))
- **Hubspot Node:** Enable hubspot credentials for http predefined types ([#3686](https://github.com/n8n-io/n8n/issues/3686)) ([b5c40e6](https://github.com/n8n-io/n8n/commit/b5c40e6294f876f18bc37a4d2e962832ee2f40a5))
- **Node:** Add the Scheduler Node ([#4223](https://github.com/n8n-io/n8n/issues/4223)) ([128c3b8](https://github.com/n8n-io/n8n/commit/128c3b83dfff3a3c21b2169da010698a3f4d20de))
- **Rundeck Node:** Update credential with test and make useable in HTTP Request node ([#3879](https://github.com/n8n-io/n8n/issues/3879)) ([fc87650](https://github.com/n8n-io/n8n/commit/fc876501809f5af0c7456867eae99f64b9ed653e))

### Performance Improvements

- update deepCopy ([#4364](https://github.com/n8n-io/n8n/issues/4364)) ([1aa21ed](https://github.com/n8n-io/n8n/commit/1aa21ed3df28684bad1696fd7f9349295d5b6219))

## [0.198.2](https://github.com/n8n-io/n8n/compare/n8n@0.198.1...n8n@0.198.2) (2022-10-14)

### Bug Fixes

- **editor:** Fix bug where one cannot scroll down parameters ([#4348](https://github.com/n8n-io/n8n/issues/4348)) ([7a76c2a](https://github.com/n8n-io/n8n/commit/7a76c2a35dac65048ab123932a54bc420e1d5a5c))

## [0.198.1](https://github.com/n8n-io/n8n/compare/n8n@0.198.0...n8n@0.198.1) (2022-10-14)

### Bug Fixes

- **editor:** Change start position of the start node ([#4345](https://github.com/n8n-io/n8n/issues/4345)) ([719a827](https://github.com/n8n-io/n8n/commit/719a82743b61d54bb101766f870538829321380c))
- **editor:** Align JSON view properties and their values ([#4343](https://github.com/n8n-io/n8n/issues/4343)) ([594a161](https://github.com/n8n-io/n8n/commit/594a16161ea80f9de7056d0fbce887f39ca74abb))
- **editor:** Fix `BASE_PATH` for Vite dev mode ([#4342](https://github.com/n8n-io/n8n/issues/4342)) ([24288a5](https://github.com/n8n-io/n8n/commit/24288a554d445f4fc12ad278e0736cd1e494f6ea))
- **editor:** Fix data pinning success source ([#4339](https://github.com/n8n-io/n8n/issues/4339)) ([763d2fd](https://github.com/n8n-io/n8n/commit/763d2fd24b0784aa28fc182be8b578537a6fb9a7))

# [0.198.0](https://github.com/n8n-io/n8n/compare/n8n@0.197.1...n8n@0.198.0) (2022-10-14)

### Bug Fixes

- **Box Node:** Fix issue with create folder operation showing extra items ([#4309](https://github.com/n8n-io/n8n/issues/4309)) ([28bea7e](https://github.com/n8n-io/n8n/commit/28bea7e109ac487014d16773414b53ddd5b0a631))
- **core, editor:** Prevent overlapping `runData` and `pinData` ([#4323](https://github.com/n8n-io/n8n/issues/4323)) ([cd74c3e](https://github.com/n8n-io/n8n/commit/cd74c3ebaea57a3894e12774ecb043184538b811))
- **core:** Expression evaluation of process should respect `N8N_BLOCK_ENV_ACCESS_IN_NODE` ([#4338](https://github.com/n8n-io/n8n/issues/4338)) ([5df09bb](https://github.com/n8n-io/n8n/commit/5df09bb31cb4b463007fc829073b66d1dce85fec))
- **editor-ui:** Fix axios baseUrl when hosted under a subfolder ([#4336](https://github.com/n8n-io/n8n/issues/4336)) ([c2e9a03](https://github.com/n8n-io/n8n/commit/c2e9a03ac54443f4fe65651edbce74ad95e8ca7d))
- **editor:** Change horizontal scrollbar rendering in various places ([#4282](https://github.com/n8n-io/n8n/issues/4282)) ([fdbc11a](https://github.com/n8n-io/n8n/commit/fdbc11a288f9fe9aac36017366b5817a05f4fbbf))
- **editor:** Disable trigger node execution pinning toolip for schedule nodes ([#4334](https://github.com/n8n-io/n8n/issues/4334)) ([d4b74bd](https://github.com/n8n-io/n8n/commit/d4b74bd66a4929517c0a66665443bf4059a74932))
- **editor:** Fix for menu collapse lag when loading a credentials page ([#4329](https://github.com/n8n-io/n8n/issues/4329)) ([298c4f2](https://github.com/n8n-io/n8n/commit/298c4f20a9ec5099953f57f3233e51d1c53d159f))
- **G Suite Admin Node:** Fix issue with user update operation failing ([#4317](https://github.com/n8n-io/n8n/issues/4317)) ([3e157f7](https://github.com/n8n-io/n8n/commit/3e157f73a441884dc2015c5cf3cdac6644876a7e))
- **GitLab Trigger Node:** Fix issue with trigger not always activating ([#4303](https://github.com/n8n-io/n8n/issues/4303)) ([2e916b6](https://github.com/n8n-io/n8n/commit/2e916b65644d4b844a4a626a0f0b92c2dd476128))
- **HTTP Request Node:** Fix oauth credentials not working properly for some predefined credentials ([#4277](https://github.com/n8n-io/n8n/issues/4277)) ([aa6c786](https://github.com/n8n-io/n8n/commit/aa6c786041d754bb795e3afd52e76c09541ffb63))
- **KoboToolbox Node:** Fix hook logs not working correctly ([#4286](https://github.com/n8n-io/n8n/issues/4286)) ([ebf4515](https://github.com/n8n-io/n8n/commit/ebf45157e610d1e2527e6180de99105b8aeb0fb8))
- **SeaTable Node:** Fix link items not showing in response ([#4170](https://github.com/n8n-io/n8n/issues/4170)) ([69684fc](https://github.com/n8n-io/n8n/commit/69684fc4f761f970a740b68865304a17257ed20c))
- **Zoom Node:** Fix issue with missing output items ([#4315](https://github.com/n8n-io/n8n/issues/4315)) ([a82fd3f](https://github.com/n8n-io/n8n/commit/a82fd3f33ff81d2b996e2975c5fd95c8abe84467))

- feat(Merge Node)!: Node tweaks n8n-4939 (#4321) ([6a37071](https://github.com/n8n-io/n8n/commit/6a37071350fee9ab861c34f4667709065f03f11a)), closes [#4321](https://github.com/n8n-io/n8n/issues/4321)

### Features

- **Citrix Node:** Add certificate install operation ([#4308](https://github.com/n8n-io/n8n/issues/4308)) ([bbb8c56](https://github.com/n8n-io/n8n/commit/bbb8c56b0e9b2c146ae17d956a09759ecded47f5))
- **Code Node:** Create Code node ([#3965](https://github.com/n8n-io/n8n/issues/3965)) ([1db4fa2](https://github.com/n8n-io/n8n/commit/1db4fa2bf87f02ccced4774eb547646c611cad40)), closes [#3930](https://github.com/n8n-io/n8n/issues/3930) [#4192](https://github.com/n8n-io/n8n/issues/4192) [#4220](https://github.com/n8n-io/n8n/issues/4220)
- **editor:** Update expressions display ([#4171](https://github.com/n8n-io/n8n/issues/4171)) ([6b53849](https://github.com/n8n-io/n8n/commit/6b538494cea62aa8c5b104b244f61e07baa58f18)), closes [#4149](https://github.com/n8n-io/n8n/issues/4149)
- **editor:** Updated n8n-menu component ([#4290](https://github.com/n8n-io/n8n/issues/4290)) ([6af3ba7](https://github.com/n8n-io/n8n/commit/6af3ba75dc90a511395674e9f64e5032e133952b)), closes [#4060](https://github.com/n8n-io/n8n/issues/4060)
- **Kafka Node:** Add key option for messages ([#4210](https://github.com/n8n-io/n8n/issues/4210)) ([1811c54](https://github.com/n8n-io/n8n/commit/1811c54917e5940a3f170761c94096845319db28))
- **MySql Node:** Use resource locator component for table parameter ([#4313](https://github.com/n8n-io/n8n/issues/4313)) ([9a06c6d](https://github.com/n8n-io/n8n/commit/9a06c6df251d5502b9f27320b49458cfb1ee3d57))
- **Venafi TLS Protect Cloud Trigger Node:** Add Venafi TLS Protect Cloud Trigger ([#4288](https://github.com/n8n-io/n8n/issues/4288)) ([7a2e5bd](https://github.com/n8n-io/n8n/commit/7a2e5bde90976d5682f3bd3a6896da920ec3ea37))

### Performance Improvements

- **ci:** Sort CI steps by length ([#4243](https://github.com/n8n-io/n8n/issues/4243)) ([d47ff48](https://github.com/n8n-io/n8n/commit/d47ff48fb633cb93cc1df2be06f9608f4f23c14a))

### BREAKING CHANGES

- The Merge node list of operations was rearranged.

Merge node: 'Combine' operation was added with 'Combine Mode' option, operations 'Merge By Fields', 'Merge By Position' and 'Multiplex' placed under 'Combine Mode' option.
To update -go to the workflows that use the Merge node, select 'Combine' operation and then choose an option from 'Combination Mode' that matches an operation that was previously used. If you want to continue even on error, you can set "Continue on Fail" to true.

## [0.197.1](https://github.com/n8n-io/n8n/compare/n8n@0.197.0...n8n@0.197.1) (2022-10-10)

### Bug Fixes

- **editor:** Fix resource locator width for trigger nodes ([#4302](https://github.com/n8n-io/n8n/issues/4302)) ([845d1f8](https://github.com/n8n-io/n8n/commit/845d1f8bd9763e9b886ac70c7ccbd37ff1c24b43))

# [0.197.0](https://github.com/n8n-io/n8n/compare/n8n@0.196.0...n8n@0.197.0) (2022-10-10)

### Bug Fixes

- **cli:** Cache generated assets in user writable directory instead ([#4275](https://github.com/n8n-io/n8n/issues/4275)) ([e63eee2](https://github.com/n8n-io/n8n/commit/e63eee28e00ae01fe4db92ac1235d7be7f25b76d))
- **core:** Fix excess run for pinned trigger in partial execution ([#4185](https://github.com/n8n-io/n8n/issues/4185)) ([a751fd3](https://github.com/n8n-io/n8n/commit/a751fd3ce762df99490889153d36029ff4cd00da))
- **core:** Fix hooks URLs no longer added to `index.html` ([#4262](https://github.com/n8n-io/n8n/issues/4262)) ([cc2a2e4](https://github.com/n8n-io/n8n/commit/cc2a2e438b0dee703b40dab67b4770dc06c76a7e))
- **editor:** Fix `pairedItem` in combination with pinned data ([#4257](https://github.com/n8n-io/n8n/issues/4257)) ([e30c78f](https://github.com/n8n-io/n8n/commit/e30c78febeac8bfcfbe5f1c4c13122594d8a518e))
- **Github Trigger Node:** Fix issue with trigger not always activating ([#4284](https://github.com/n8n-io/n8n/issues/4284)) ([694f1ba](https://github.com/n8n-io/n8n/commit/694f1ba4f5780b2e9821db52e579883bbc289df4))
- **Microsoft Excel Node:** Fix issue with pagination when getting all items ([#4247](https://github.com/n8n-io/n8n/issues/4247)) ([1067ec0](https://github.com/n8n-io/n8n/commit/1067ec0f5bd8e57650ccd9924e01fc52fbf0c43c))
- **Microsoft ToDo Node:** Fix pagination issue when getting all items ([#4222](https://github.com/n8n-io/n8n/issues/4222)) ([4595b54](https://github.com/n8n-io/n8n/commit/4595b54e562c50c48bdfe8049cb170196713cc8b))

### Features

- **AWS Certificate Manager Node:** Add AWS Certificate Manager node ([#4263](https://github.com/n8n-io/n8n/issues/4263)) ([9b3f30d](https://github.com/n8n-io/n8n/commit/9b3f30d584901e7dc5fa87854e72f438f2557665))
- **AWS Elastic Load Balancer Node:** Add Elastic Load Balancer node ([#4264](https://github.com/n8n-io/n8n/issues/4264)) ([fac6efb](https://github.com/n8n-io/n8n/commit/fac6efbb4158aa713bf5472d27b6fe341db8047d))
- **Citrix ADC Node:** Add Citrix ADC node ([#4274](https://github.com/n8n-io/n8n/issues/4274)) ([7abc7e6](https://github.com/n8n-io/n8n/commit/7abc7e64082b60fa48f99f4b1f41d176fbb6d6ad))
- **Cloudflare Node:** Add Cloudflare node ([#4271](https://github.com/n8n-io/n8n/issues/4271)) ([94a02c6](https://github.com/n8n-io/n8n/commit/94a02c64928205c441af5515739fe8eab7160b33))
- **core:** Improve light versioning support in declarative node design ([#4254](https://github.com/n8n-io/n8n/issues/4254)) ([1b320cd](https://github.com/n8n-io/n8n/commit/1b320cd8c9b1e00257c03f92a175e3c9ab9f8030))
- **Crypto Node:** Add SHA3 support ([#4285](https://github.com/n8n-io/n8n/issues/4285)) ([9407fdd](https://github.com/n8n-io/n8n/commit/9407fddd21295b7bdf2757736b69b046a02e798c))
- **editor:** JSON mapping ([#4270](https://github.com/n8n-io/n8n/issues/4270)) ([19e333e](https://github.com/n8n-io/n8n/commit/19e333e6602648feacd80277e170d8af38ce06c4))
- **Venafi TLS Protect Cloud Node:** Add Venafi TLS Protect Cloud ([#4253](https://github.com/n8n-io/n8n/issues/4253)) ([d36e920](https://github.com/n8n-io/n8n/commit/d36e920997d55957385e4ab4d6734639a4c28648))
- **Venafi TLS Protect Datacenter Node:** Add Venafi TLS Protect Datacenter node ([#4255](https://github.com/n8n-io/n8n/issues/4255)) ([a14110e](https://github.com/n8n-io/n8n/commit/a14110e663caca8e886312a116805c41020ba812))

### Performance Improvements

- **tooling:** Upgrade to TypeScript 4.8 ([#4207](https://github.com/n8n-io/n8n/issues/4207)) ([9089dbe](https://github.com/n8n-io/n8n/commit/9089dbe94220f1789d2cea74608352a070e09bac))

# [0.196.0](https://github.com/n8n-io/n8n/compare/n8n@0.195.5...n8n@0.196.0) (2022-09-30)

### Bug Fixes

- **build:** Add typing for SSE channel ([#4196](https://github.com/n8n-io/n8n/issues/4196)) ([eaf13cd](https://github.com/n8n-io/n8n/commit/eaf13cdf759497816255926ccc4a60f176d36a1a))
- **build:** Fix lint issue to fix build ([#4232](https://github.com/n8n-io/n8n/issues/4232)) ([40795d6](https://github.com/n8n-io/n8n/commit/40795d6adf383ec09290ca2a9da7e6ebeeaffb03))
- **Trello Node:** cardId property not showing up for completed checklist in Trello ([#4186](https://github.com/n8n-io/n8n/issues/4186)) ([05d2275](https://github.com/n8n-io/n8n/commit/05d227571d53a93380aab05444c5de38e448a317))
- **cli:** Add git to all docker images ([#4189](https://github.com/n8n-io/n8n/issues/4189)) ([0b6a958](https://github.com/n8n-io/n8n/commit/0b6a9585d41992f5dcc1a5683adc3f36e43955af))
- **cli:** Disable `X-Powered-By: Express` Header ([#4224](https://github.com/n8n-io/n8n/issues/4224)) ([a8da9c3](https://github.com/n8n-io/n8n/commit/a8da9c31a95dabbbdc4eb67e5157dd5631ff3031))
- **cli:** Disable CORS on SSE connections in production ([#4190](https://github.com/n8n-io/n8n/issues/4190)) ([e6e4f29](https://github.com/n8n-io/n8n/commit/e6e4f297c697c3371743bc1e1b2524235c4aea19))
- **core:** Remove commented out lines ([6ac442a](https://github.com/n8n-io/n8n/commit/6ac442a2accdeb4e51a3333ac6c45c8bfde0608d))
- delete unused dependencies ([#4231](https://github.com/n8n-io/n8n/issues/4231)) ([737cbf9](https://github.com/n8n-io/n8n/commit/737cbf9694296b76bc6c19716ffd6d4dcccf1c18))
- **editor:** Add missing event handler to accordion component ([#4179](https://github.com/n8n-io/n8n/issues/4179)) ([e709cb5](https://github.com/n8n-io/n8n/commit/e709cb5fe28839cf314a511a5a40f374a8ad4647))
- **editor:** Fix storybook setup ([#4234](https://github.com/n8n-io/n8n/issues/4234)) ([43dc8e6](https://github.com/n8n-io/n8n/commit/43dc8e6da1970d7ea4bb67635c8b20354150c87d))
- **editor:** Fix `BASE_URL` replacement on windows ([#4202](https://github.com/n8n-io/n8n/issues/4202)) ([5f0c656](https://github.com/n8n-io/n8n/commit/5f0c65690b8dddd21f5a694d6e74980296c7fbb8))
- **editor:** Fix ParameterInput inputField ref focus ([#4215](https://github.com/n8n-io/n8n/issues/4215)) ([ed40397](https://github.com/n8n-io/n8n/commit/ed403972a929c710180b2ac47fa4057ec47c4a35))
- **editor:** Make lodash aliases work on case-sensitive filesystems ([#4233](https://github.com/n8n-io/n8n/issues/4233)) ([a381729](https://github.com/n8n-io/n8n/commit/a3817291d7795345542b63641e265fe8f29e8750))
- **editor:** Fix copy-pasting workflow into pin data code editor ([#4193](https://github.com/n8n-io/n8n/issues/4193)) ([a4f9f04](https://github.com/n8n-io/n8n/commit/a4f9f041a07bea641c09d517942393c24d5e4a37))
- **editor:** Fix run data footer overflow ([#4175](https://github.com/n8n-io/n8n/issues/4175)) ([20b0e14](https://github.com/n8n-io/n8n/commit/20b0e14f728cd9b77e993ee15e3bd276b102e427))
- **editor:** Fix run data pagination selector not showing ([#4187](https://github.com/n8n-io/n8n/issues/4187)) ([2b3a090](https://github.com/n8n-io/n8n/commit/2b3a0901aa07046dc68cc6ece6c015819835cfd4))
- **editor:** Fix run selector not opening ([#4199](https://github.com/n8n-io/n8n/issues/4199)) ([67513e1](https://github.com/n8n-io/n8n/commit/67513e191d82dfa97a477e38770fe610dd9fca65))
- **editor:** Updating leftover i18n references in NodeView ([#4236](https://github.com/n8n-io/n8n/issues/4236)) ([068c5db](https://github.com/n8n-io/n8n/commit/068c5db1eecd60d650c3646f62eeadfad42df470))
- **editor:** Updating wrong i18n string reference ([#4209](https://github.com/n8n-io/n8n/issues/4209)) ([80e2d65](https://github.com/n8n-io/n8n/commit/80e2d65933101e69dee98ba69e80156f2ad3b7a9))
- **editor:** Fix slow loading times for nodeTypes, node creator vuex reference, and pushConnection in settings views ([#4230](https://github.com/n8n-io/n8n/issues/4230)) ([d3c0d99](https://github.com/n8n-io/n8n/commit/d3c0d998679965f53fb170e0f476f7bd17665645))
- **Merge Node:** Update description in merge node ([47eb531](https://github.com/n8n-io/n8n/commit/47eb531e980b1998fdaaece5cf533dc3903dc796))
- **core:** Fix and harmonize all primaryDocumentation links ([#4191](https://github.com/n8n-io/n8n/issues/4191)) ([6e8e4f5](https://github.com/n8n-io/n8n/commit/6e8e4f5937eb257efcbb4ff37c6b9403a044eecf))
- **core:** Remove --forceExit flag from cli tests ([#4211](https://github.com/n8n-io/n8n/issues/4211)) ([faaeb52](https://github.com/n8n-io/n8n/commit/faaeb52a14a40b30ffe90cddb84c45af55acdf93))
- **Wekan Node:** Fix authentication with new versions of Wekan ([#4088](https://github.com/n8n-io/n8n/issues/4088)) ([764bd35](https://github.com/n8n-io/n8n/commit/764bd3522b72d6188f2425df0710d16c5b34a20b))
- **Wufoo Trigger Node:** Fix form names not being listed correctly ([#4151](https://github.com/n8n-io/n8n/issues/4151)) ([616d62a](https://github.com/n8n-io/n8n/commit/616d62aa8ef64952eb248b162176460a7ac65cc3))

### Features

- **editor:** Add support for unit testing using vitest in editor-ui ([#4184](https://github.com/n8n-io/n8n/issues/4184)) ([bb66e60](https://github.com/n8n-io/n8n/commit/bb66e60afcbf120f3f916339c983b881ea185487))
- **cli:** Optimise serving static assets ([#4182](https://github.com/n8n-io/n8n/issues/4182)) ([8b0ccc0](https://github.com/n8n-io/n8n/commit/8b0ccc017bab28903d57a91602331981e45077d9))
- **core:** Improve paired item and add additional variables ([#3765](https://github.com/n8n-io/n8n/issues/3765)) ([5526057](https://github.com/n8n-io/n8n/commit/5526057efc7d27a1373dc2c46beda2737ed54689))
- **editor:** Update ResourceLocator error text ([#4242](https://github.com/n8n-io/n8n/issues/4242)) ([b0397f0](https://github.com/n8n-io/n8n/commit/b0397f0262f8a921a0552179ca95cba5f03295ce))
- **editor:** Main navigation redesign ([#4144](https://github.com/n8n-io/n8n/issues/4144)) ([3db53a1](https://github.com/n8n-io/n8n/commit/3db53a193418db2554e00d7499457d7f400663e1)), closes [#4060](https://github.com/n8n-io/n8n/issues/4060)
- **HTTP Request Node:** Redesign and add the ability to import cURL commands ([#3860](https://github.com/n8n-io/n8n/issues/3860)) ([f37d6ba](https://github.com/n8n-io/n8n/commit/f37d6ba03bcac82a50b2e9ee60c29d6a1a4be911))
- **editor:** Migrate editor-ui to Vite.js and various DX improvements (N8N-2277) ([#4061](https://github.com/n8n-io/n8n/issues/4061)) ([27e2ce0](https://github.com/n8n-io/n8n/commit/27e2ce047060ca8bfdef43cb7fe50b58c9508375)), closes [#4069](https://github.com/n8n-io/n8n/issues/4069)
- **n8n Api node:** Add core node for consuming the n8n API ([#4076](https://github.com/n8n-io/n8n/issues/4076)) ([929315f](https://github.com/n8n-io/n8n/commit/929315f9e4b56d975783b7d069bdb163218aa7d5))
- **RabbitMQ Trigger Node:** Automatically reconnect on disconnect ([#4019](https://github.com/n8n-io/n8n/issues/4019)) ([23bd71b](https://github.com/n8n-io/n8n/commit/23bd71b82aafb4d894091a115a168a049c5f594c))
- **core:** Share unshared credentials with owner on reset ([#4216](https://github.com/n8n-io/n8n/issues/4216)) ([3b7de6d](https://github.com/n8n-io/n8n/commit/3b7de6db725cffbd5ee9f06aee00029d984fe7b8))
- **Slack Node:** Add operation get many for user resource ([#3150](https://github.com/n8n-io/n8n/issues/3150)) ([2714b4c](https://github.com/n8n-io/n8n/commit/2714b4ced786212906f79c11fae28819aae420e4))
- **WhatsApp Business node:** Add WhatsApp node ([#3659](https://github.com/n8n-io/n8n/issues/3659)) ([f63710a](https://github.com/n8n-io/n8n/commit/f63710a8923bd742f3259822870f3a2f0b7e04aa))

## [0.195.5](https://github.com/n8n-io/n8n/compare/n8n@0.195.4...n8n@0.195.5) (2022-09-23)

### Bug Fixes

- **editor:** Fix extract value logic for expressions ([#4178](https://github.com/n8n-io/n8n/issues/4178)) ([46f9562](https://github.com/n8n-io/n8n/commit/46f95622e38e0327c01927bc41f4ea3c413db466))

## [0.195.4](https://github.com/n8n-io/n8n/compare/n8n@0.195.3...n8n@0.195.4) (2022-09-22)

### Bug Fixes

- **core:** Fix resolve RL values in expressions ([#4173](https://github.com/n8n-io/n8n/issues/4173)) ([469c391](https://github.com/n8n-io/n8n/commit/469c391fee70479d8095a90e6eb525032a0e02a5))

### Features

- **editor-ui:** Resizable main panel ([#3980](https://github.com/n8n-io/n8n/issues/3980)) ([d01f7d4](https://github.com/n8n-io/n8n/commit/d01f7d4d93366054075fdfcadfdff5cf03913472)), closes [#3930](https://github.com/n8n-io/n8n/issues/3930)

## [0.195.3](https://github.com/n8n-io/n8n/compare/n8n@0.195.2...n8n@0.195.3) (2022-09-22)

### Bug Fixes

- **editor:** Fix expressions bug with numbers and booleans ([#4169](https://github.com/n8n-io/n8n/issues/4169)) ([19d08e6](https://github.com/n8n-io/n8n/commit/19d08e641896fa9b1c9edf04505eac213e1de71a))
- **MSSQL Node:** Support tdsVersion option ([89d2d10](https://github.com/n8n-io/n8n/commit/89d2d10c520482f47ddd755e76b0bdf3d45e6008))

## [0.195.2](https://github.com/n8n-io/n8n/compare/n8n@0.195.1...n8n@0.195.2) (2022-09-22)

### Bug Fixes

- **core:** Fix mysql migration ([#4166](https://github.com/n8n-io/n8n/issues/4166)) ([0aeb55d](https://github.com/n8n-io/n8n/commit/0aeb55dcfd6c107c67e4c974e3371e29e188310b))

## [0.195.1](https://github.com/n8n-io/n8n/compare/n8n@0.195.0...n8n@0.195.1) (2022-09-21)

### Bug Fixes

- **core:** Fix postgres migration ([#4164](https://github.com/n8n-io/n8n/issues/4164)) ([2598ec8](https://github.com/n8n-io/n8n/commit/2598ec8a3e7a7d4e444cd4767d5944fa691dd9e1))

# [0.195.0](https://github.com/n8n-io/n8n/compare/n8n@0.194.0...n8n@0.195.0) (2022-09-21)

### Bug Fixes

- **Box Node:** Fix issue with response data not being returned ([#4147](https://github.com/n8n-io/n8n/issues/4147)) ([3cfc5b5](https://github.com/n8n-io/n8n/commit/3cfc5b55abe6aba3b68ae27846cd18e3ec79b518))
- **cli:** Fix issue with n8n crashing when error in poll method ([#4008](https://github.com/n8n-io/n8n/issues/4008)) ([6c41b29](https://github.com/n8n-io/n8n/commit/6c41b29ad2c1fffc5710d06250037e2a278b9b4a))
- **editor:** Fix broken output panel for wait node executions ([#4156](https://github.com/n8n-io/n8n/issues/4156)) ([40ebbea](https://github.com/n8n-io/n8n/commit/40ebbeaefc3a8c0e730468cd8171590dc823106c))
- **core:** Prevent calls to constructor to forbid arbitrary code execution ([#4139](https://github.com/n8n-io/n8n/issues/4139)) ([a8030db](https://github.com/n8n-io/n8n/commit/a8030dbda5b17ee158ac7ef7f586f212698252f7))
- **HTTP Node:** Fix instance crashing when batching enabled ([#3902](https://github.com/n8n-io/n8n/issues/3902)) ([0ab89ad](https://github.com/n8n-io/n8n/commit/0ab89ad5d66c1082ec2464813a9622431fa7f230))
- **public-api:** Create correct OAuth2 credential schema ([#4111](https://github.com/n8n-io/n8n/issues/4111)) ([28ab4f6](https://github.com/n8n-io/n8n/commit/28ab4f66f096eb6ec483e344bffe98b9a81520c6))
- **Xero Node:** fix line amount types being ignored when creating new invoices ([#4146](https://github.com/n8n-io/n8n/issues/4146)) ([3e2e9e6](https://github.com/n8n-io/n8n/commit/3e2e9e6009301006be7c7e96444ff4bbf824358c))

### Features

- **editor:** Add resource locator parameter ([#3932](https://github.com/n8n-io/n8n/issues/3932)) ([ad73f89](https://github.com/n8n-io/n8n/commit/ad73f8995c34a664391dcc467aca55f44f4bde71))
- **cli:** User Management and Credentials sharing ([#3602](https://github.com/n8n-io/n8n/issues/3602)) ([97cd564](https://github.com/n8n-io/n8n/commit/97cd564f7b4c5ba1472e517e0d54897b2cabcc26))

### Performance Improvements

- **ci:** Cache npm dependencies ([#4138](https://github.com/n8n-io/n8n/issues/4138)) ([1bdc102](https://github.com/n8n-io/n8n/commit/1bdc102892e77f2723ffed383874092cf4e07810))

# [0.194.0](https://github.com/n8n-io/n8n/compare/n8n@0.193.5...n8n@0.194.0) (2022-09-15)

### Bug Fixes

- AWS credential testing issue ([#4107](https://github.com/n8n-io/n8n/issues/4107)) ([5130529](https://github.com/n8n-io/n8n/commit/51305290663dc4bc05cdbb075d685673217081f9))
- **cli,core:** Address Dependabot warnings [N8N-4121] ([#3883](https://github.com/n8n-io/n8n/issues/3883)) ([461848f](https://github.com/n8n-io/n8n/commit/461848fcc4a33b0adf9958bebb2557bfa15100d6))
- **cli:** Avoid scanning unnecessary directories on windows ([#4082](https://github.com/n8n-io/n8n/issues/4082)) ([84b56eb](https://github.com/n8n-io/n8n/commit/84b56eb48e727389189c517598aadadd6f2ccf23)), closes [#4007](https://github.com/n8n-io/n8n/issues/4007)
- **cli:** Load nodes and credentials on windows using the correct file-path ([#4084](https://github.com/n8n-io/n8n/issues/4084)) ([b6c1187](https://github.com/n8n-io/n8n/commit/b6c1187922ab6552e303c98341c5732ffa96c55f))
- **cli:** Password reset should trigger internal and external hooks ([#4066](https://github.com/n8n-io/n8n/issues/4066)) ([12507d3](https://github.com/n8n-io/n8n/commit/12507d39d68a2961c6e567b6b7d83759010918b0))
- **cli:** Use absolute paths for loading custom nodes and credentials ([#4099](https://github.com/n8n-io/n8n/issues/4099)) ([43c9f01](https://github.com/n8n-io/n8n/commit/43c9f019bd3e25215134970570c574da663dd3e0)), closes [#4082](https://github.com/n8n-io/n8n/issues/4082)
- **core & Function nodes:** Update function nodes to work with binary-data-mode 'filesystem'. ([#3845](https://github.com/n8n-io/n8n/issues/3845)) ([f6064ef](https://github.com/n8n-io/n8n/commit/f6064ef278bb481a78942af3af9675f29e59045b)), closes [#1](https://github.com/n8n-io/n8n/issues/1)
- **core:** Fix issue with returnJsonArray helper breaking nodes that return no data ([3de0e22](https://github.com/n8n-io/n8n/commit/3de0e228cb78f292ead4d0103040d2c00943deae))
- **core:** Fix node renaming in expressions ([381c09f](https://github.com/n8n-io/n8n/commit/381c09fa47212a12f6c7bc166ac641afd97c9681))
- **core:** Update oauth endpoints to use instance base url ([dd3ba96](https://github.com/n8n-io/n8n/commit/dd3ba963723fbdef7d4239f0890c0776bffd062e))
- **eslint:** Setup eslint to run on every package ([#4050](https://github.com/n8n-io/n8n/issues/4050)) ([69eb979](https://github.com/n8n-io/n8n/commit/69eb97999da0543308285ebc834f3454c2eea727))
- **GoogleBigQuery Node:** Fix empty response when creating records ([#4056](https://github.com/n8n-io/n8n/issues/4056)) ([9f92a4d](https://github.com/n8n-io/n8n/commit/9f92a4d681918cb8d9f0d5b0bd322b93da0ba3ef))
- **Hubspot Node:** Correct canvas name of HubSpot node ([#4054](https://github.com/n8n-io/n8n/issues/4054)) ([e1025e8](https://github.com/n8n-io/n8n/commit/e1025e888c56995d284e0b5889af2e93b57ad3eb))
- Issue with versioned nodes not loading properly ([#4094](https://github.com/n8n-io/n8n/issues/4094)) ([9e1fa4c](https://github.com/n8n-io/n8n/commit/9e1fa4c0459b0bebe725f5e6db84104bcd37690d))
- **MongoDB Node:** Update mongo driver to 4.9.1 ([#4095](https://github.com/n8n-io/n8n/issues/4095)) ([f70e6d2](https://github.com/n8n-io/n8n/commit/f70e6d23455b5b380ffb607100e0090203e31047))
- **node:** Google Cloud Storage linting rules ([36ec81f](https://github.com/n8n-io/n8n/commit/36ec81f62489a7bc3442e46048f92d2ae9de1ce7))
- **public-api:** Fix error updating workflow with property not defined in the schema ([#4089](https://github.com/n8n-io/n8n/issues/4089)) ([f40ae50](https://github.com/n8n-io/n8n/commit/f40ae501b4dca8f00db41d8fc07b496ad06cf10f))
- **typescript:** Use consistent typescript configs ([#4049](https://github.com/n8n-io/n8n/issues/4049)) ([9267e8f](https://github.com/n8n-io/n8n/commit/9267e8fb1283794e7ebc109772e584b0471bef27))
- **workflow:** Remove a few `ts-ignore` and `eslint-disable` ([#3958](https://github.com/n8n-io/n8n/issues/3958)) ([a73ac1d](https://github.com/n8n-io/n8n/commit/a73ac1d94f5081051d1280b7ebc467f22e3d100d))

### Features

- **Adalo Node:** Add Adalo node ([#3102](https://github.com/n8n-io/n8n/issues/3102)) ([9a59d0a](https://github.com/n8n-io/n8n/commit/9a59d0a5d10b83ed4642e59c16310a436fd92a7a))
- **cli:** Load all nodes and credentials code in isolation ([#3906](https://github.com/n8n-io/n8n/issues/3906)) ([b450e97](https://github.com/n8n-io/n8n/commit/b450e977a32944a5289db2553bf12bdef4e1d3b3))
- **core, editor-ui:** Introduce node deprecation ([#4103](https://github.com/n8n-io/n8n/issues/4103)) ([98ed207](https://github.com/n8n-io/n8n/commit/98ed2076072858109f5ed512786af61dff0314d6))
- **editor:** Implement HTML sanitization for Notification and Message components ([#4081](https://github.com/n8n-io/n8n/issues/4081)) ([ea2d18b](https://github.com/n8n-io/n8n/commit/ea2d18b66dba1393a0425b5074884b782f959e5c))
- **editor:** Show input number for multi-input nodes ([#4000](https://github.com/n8n-io/n8n/issues/4000)) ([8c95d6e](https://github.com/n8n-io/n8n/commit/8c95d6ec53b735cc322a3b5f2a5a78002ae8441a))
- **gmail:** Overhaul Gmail node + create gmail trigger ([#3734](https://github.com/n8n-io/n8n/issues/3734)) ([74304db](https://github.com/n8n-io/n8n/commit/74304db4e2ae66b82695244d07c6ff8a9ffe37cf))
- **Google Cloud Storage Node:** Add GCS Node with Bucket and Object operations ([1e963d8](https://github.com/n8n-io/n8n/commit/1e963d8e1ed6956e8af02e70da304211aa725ea1))
- **Merge Node:** Overhaul of merge node ([f1a5697](https://github.com/n8n-io/n8n/commit/f1a569791d5289ced8ac78d97452f6ad5bf8d1b8))
- **typescript:** Setup Typescript incremental builds ([#3876](https://github.com/n8n-io/n8n/issues/3876)) ([799676b](https://github.com/n8n-io/n8n/commit/799676b24d9ba5628dc875de1c0bbcf7e51a51cc))

## [0.193.5](https://github.com/n8n-io/n8n/compare/n8n@0.193.4...n8n@0.193.5) (2022-09-07)

### Bug Fixes

- **editor:** Disable editing in Function nodes in executions view ([#4041](https://github.com/n8n-io/n8n/issues/4041)) ([772836a](https://github.com/n8n-io/n8n/commit/772836abc7d81fce74547dd3644c45eaea9c0a75))
- **editor:** use correct attribute on button to make it full width ([#4048](https://github.com/n8n-io/n8n/issues/4048)) ([b26545d](https://github.com/n8n-io/n8n/commit/b26545d94c9b718e20580e511aab676e98de66dc))
- **editor:** Wrong popup title when "Click To Copy" on OAuth2 Redirect Url credentials ([#4043](https://github.com/n8n-io/n8n/issues/4043)) ([0acac35](https://github.com/n8n-io/n8n/commit/0acac355e1bfff326d3bb575d5b21f0004a0c792))
- **Gmail Node:** Fix node and improve helper so to avoid double wrapping in json key ([#4052](https://github.com/n8n-io/n8n/issues/4052)) ([fbd044b](https://github.com/n8n-io/n8n/commit/fbd044bf874f270c9f9e7cda9aaecdc235ddc677))

## [0.193.4](https://github.com/n8n-io/n8n/compare/n8n@0.193.3...n8n@0.193.4) (2022-09-06)

### Bug Fixes

- **AWS Nodes:** Handle query string and body properly for AWS related requests ([#4039](https://github.com/n8n-io/n8n/issues/4039)) ([103f04e](https://github.com/n8n-io/n8n/commit/103f04e4eba08a1cd888e71073cf24178a2b52ba))
- **AWS Lambda Node:** Fix json data being sent to AWS Lambda as string ([#4029](https://github.com/n8n-io/n8n/issues/4029)) ([c28f69b](https://github.com/n8n-io/n8n/commit/c28f69b276fe46c42dfb62753b565ebae37431f5))
- **Beeminder Node:** Fix request id not being sent when creating a new datapoint ([73c5210](https://github.com/n8n-io/n8n/commit/73c52102949274c4c67ae34c458a6afa9520c150))
- **cli:** Include "auth-excluded" endpoints on the history middleware as well ([#4028](https://github.com/n8n-io/n8n/issues/4028)) ([d554128](https://github.com/n8n-io/n8n/commit/d55412845784fda4d42a1dcaca60515ad10d2aa0))
- **core:** Fix MySQL migration issue with table prefix ([#4013](https://github.com/n8n-io/n8n/issues/4013)) ([fc6484b](https://github.com/n8n-io/n8n/commit/fc6484ba4d48363fd846d5c800a25a207082f58d))
- Correct all the spelling typos ([#3960](https://github.com/n8n-io/n8n/issues/3960)) ([49c85a1](https://github.com/n8n-io/n8n/commit/49c85a1df8417918797c3fe6db46f35f9fe86bdf))
- Fix n8n-square-button import. ([#4024](https://github.com/n8n-io/n8n/issues/4024)) ([bbd967b](https://github.com/n8n-io/n8n/commit/bbd967bbdfb744874eeae5aced7ce122039b59d5))
- **GitHub Node:** Fix binary data not being returned ([#4017](https://github.com/n8n-io/n8n/issues/4017)) ([5753110](https://github.com/n8n-io/n8n/commit/575311040261be2982a3c7107bf1ea8b7b63fbb5))
- **GraphQL Node:** Fix issue with return items ([#4016](https://github.com/n8n-io/n8n/issues/4016)) ([6216132](https://github.com/n8n-io/n8n/commit/6216132ae2f3b908aacf266f4a34143bb8a74f0a))
- **Postgres Node:** Fix ssue with postgres insert and paired item ([#4020](https://github.com/n8n-io/n8n/issues/4020)) ([9314086](https://github.com/n8n-io/n8n/commit/9314086b6a84ce0f24992827ab316dee4709d118))
- **Kafka Trigger Node:** fix kafka trigger not working with default max requests value ([71cae90](https://github.com/n8n-io/n8n/commit/71cae90679d9d6fe4cf0dc898827cc9cd4457873))
- **MonicaCrm Node:** Fix pagination when using return all ([82827d0](https://github.com/n8n-io/n8n/commit/82827d0a12e889b2fdebd422bd1fcb483860599e))
- **Node Gmail:** Fix bug related to paired items ([2746905](https://github.com/n8n-io/n8n/commit/2746905570c2056abf9c388cc28c7d1d7b9f5102))
- **Raindrop Node:** Fix issue refreshing OAuth2 credentials ([3163742](https://github.com/n8n-io/n8n/commit/3163742fd7ae0afa86919e5f473be3d2bd88282b))
- **Shopify Node:** Fix pagination when empty fields are sent ([071ab40](https://github.com/n8n-io/n8n/commit/071ab40c9fa523b8ee47c9428ee6078e43985816))

### Features

- Add possibility to configure stop time for workers ([#4012](https://github.com/n8n-io/n8n/issues/4012)) ([a3791c2](https://github.com/n8n-io/n8n/commit/a3791c22b3f0be16324e1223aa719e6f122a51c1))
- **cli:** Add external hooks for when members are added or deleted ([#3988](https://github.com/n8n-io/n8n/issues/3988)) ([6be9997](https://github.com/n8n-io/n8n/commit/6be999714f62f22ec5d8ab82f91f7fc5a2b55c4d))
- **editor:** Use i18n component instead od v-html for localization ([287533e](https://github.com/n8n-io/n8n/commit/287533e6c819329dc84f2e23a33faed66181d07a))

## [0.193.3](https://github.com/n8n-io/n8n/compare/n8n@0.193.2...n8n@0.193.3) (2022-09-01)

### Bug Fixes

- **cli:** Initialize mailer just if connection can be verified ([#3997](https://github.com/n8n-io/n8n/issues/3997)) ([936cb11](https://github.com/n8n-io/n8n/commit/936cb117895695f9519f0debb3bcac275d98eda8))
- **core:** Fix disabled parent output in partial execution ([#3946](https://github.com/n8n-io/n8n/issues/3946)) ([c8743ff](https://github.com/n8n-io/n8n/commit/c8743ff6cad1563d31d4d39ffa742726830a4f38))
- **nodes:** Remove duplicate wrap of paired item data ([#4001](https://github.com/n8n-io/n8n/issues/4001)) ([54efe20](https://github.com/n8n-io/n8n/commit/54efe20ee4834fbf9306be161b36f115b9eb0834))

### Features

- **nodes:** Add database and non http credentials test ([d82e879](https://github.com/n8n-io/n8n/commit/d82e87979dc0fe47e264b0e7bb46c325157d9603))
- **Mongo DB Node:** Add MongoDB credential testing and two operations ([#3901](https://github.com/n8n-io/n8n/issues/3901)) ([b5511e5](https://github.com/n8n-io/n8n/commit/b5511e5ac7745c6b4a20aa49d2633f2f91bdbb7b))

## [0.193.2](https://github.com/n8n-io/n8n/compare/n8n@0.193.1...n8n@0.193.2) (2022-09-01)

### Bug Fixes

- **docker:** n8n docker image needs su-exec ([#3993](https://github.com/n8n-io/n8n/issues/3993)) ([aec2489](https://github.com/n8n-io/n8n/commit/aec2489aefb8fca522302bdcaa002fa62393b70a))
- **docker:** Revert docker `USER` and `WORKDIR` changes ([#3992](https://github.com/n8n-io/n8n/issues/3992)) ([34a99fd](https://github.com/n8n-io/n8n/commit/34a99fd089a754170ed4f2b9bdc02fc951d7e9bc))
- **core:** Fix OAuth2 issues ([#3391](https://github.com/n8n-io/n8n/pull/3991))

## [0.193.1](https://github.com/n8n-io/n8n/compare/n8n@0.193.0...n8n@0.193.1) (2022-08-31)

### Bug Fixes

- **editor:** Fix bug where col headers don't show ([#3985](https://github.com/n8n-io/n8n/issues/3985)) ([bee3840](https://github.com/n8n-io/n8n/commit/bee38400505b8862a4e1e5bf28b18088ff8ced8f))

# [0.193.0](https://github.com/n8n-io/n8n/compare/n8n@0.192.2...n8n@0.193.0) (2022-08-31)

### Bug Fixes

- **ci:** Setup a separate workflow action to test for pushes on master ([#3951](https://github.com/n8n-io/n8n/issues/3951)) ([1f9bdd0](https://github.com/n8n-io/n8n/commit/1f9bdd09a29a5e0564ddc874814eaf36d9380ee7))
- **core:** Make digest auth work with query params ([087d3f9](https://github.com/n8n-io/n8n/commit/087d3f99f1f5c38db763686c10c6181e20c08307))
- **editor:** Sending data as query on DELETE method ([#3972](https://github.com/n8n-io/n8n/issues/3972)) ([fc2ff35](https://github.com/n8n-io/n8n/commit/fc2ff35c412b1c10471659c91dc0fe11a3363495))
- Fix credentials_entity table migration for mysql ([#3979](https://github.com/n8n-io/n8n/issues/3979)) ([349826e](https://github.com/n8n-io/n8n/commit/349826e87fdb03a9f378422ecfac83d42bb5a376))
- **npm:** Improve .npmignore to reduce the size of the published packages ([#3970](https://github.com/n8n-io/n8n/issues/3970)) ([15d5ac6](https://github.com/n8n-io/n8n/commit/15d5ac6f3c7732374f07726c5697ba341eb9aa70))

### Features

- **design-system,editor-ui:** Upgrade some of the frontend dev dependencies ([#3978](https://github.com/n8n-io/n8n/issues/3978)) ([b428e9f](https://github.com/n8n-io/n8n/commit/b428e9fb9ffb506c97f91d45072e32241a3b07d6))
- **docker:** Reduce the size of alpine docker images ([#3973](https://github.com/n8n-io/n8n/issues/3973)) ([398adb2](https://github.com/n8n-io/n8n/commit/398adb23e8785c92478c4d80c944e60e9278ffdf))
- **editor:** Limit when to show mapping tooltip ([#3976](https://github.com/n8n-io/n8n/issues/3976)) ([8fc9f07](https://github.com/n8n-io/n8n/commit/8fc9f07f39edf8944214200dd787b2d0c9b6caff))
- **HighLevel Node:** Add HighLevel node ([c2e97a8](https://github.com/n8n-io/n8n/commit/c2e97a89f923bbebe0a6d882e86d792fcda3116d))

## [0.192.2](https://github.com/n8n-io/n8n/compare/n8n@0.192.1...n8n@0.192.2) (2022-08-25)

### Bug Fixes

- **editor:** Fix feature flag check when PH is unavailable ([#3944](https://github.com/n8n-io/n8n/issues/3944)) ([93c26da](https://github.com/n8n-io/n8n/commit/93c26dac286e8fa984cb6fb6fecd6167fc4143f3))
- **editor:** fix mapping bug when val is null ([#3942](https://github.com/n8n-io/n8n/issues/3942)) ([a21dbdc](https://github.com/n8n-io/n8n/commit/a21dbdc45b6f434f7ecd8b541bb32d397fd95c89))

## [0.192.1](https://github.com/n8n-io/n8n/compare/n8n@0.192.0...n8n@0.192.1) (2022-08-25)

### Bug Fixes

- **cli:** Account for non-array in pindata migration ([#3938](https://github.com/n8n-io/n8n/issues/3938)) ([f052187](https://github.com/n8n-io/n8n/commit/f0521873e1acf8c6491b75f37be1dd824bb355bc))

# [0.192.0](https://github.com/n8n-io/n8n/compare/n8n@0.191.1...n8n@0.192.0) (2022-08-24)

### Bug Fixes

- **cli:** Account for unparseable string in JSON key migration ([#3927](https://github.com/n8n-io/n8n/issues/3927)) ([ab45898](https://github.com/n8n-io/n8n/commit/ab45898a69dd9354cdb365187dec0d58a1836418))
- **cli:** Fix excessive instantiation type error for flattened execution ([#3921](https://github.com/n8n-io/n8n/issues/3921)) ([1d4f92a](https://github.com/n8n-io/n8n/commit/1d4f92a6575a7af6dbd4f03b61202cb56badf6a1))
- **cli:** Init nodes dir to ensure `npm install` succeeds ([#3934](https://github.com/n8n-io/n8n/issues/3934)) ([2d6eea8](https://github.com/n8n-io/n8n/commit/2d6eea82d324d4560f7445d87647ce0d5e87c678))
- **cli:** tsc build errors should fail turborepo builds as well ([#3923](https://github.com/n8n-io/n8n/issues/3923)) ([f22bd28](https://github.com/n8n-io/n8n/commit/f22bd2805d87c552d92d0da0313bf7f9c498f103))
- **core:** Account for enabled state in first pinned trigger ([#3912](https://github.com/n8n-io/n8n/issues/3912)) ([6bd7a09](https://github.com/n8n-io/n8n/commit/6bd7a09a455b61eae5edad1d93e8a7e00c0c68b3))
- **core:** Fix pinned trigger execution ([#3895](https://github.com/n8n-io/n8n/issues/3895)) ([17799cd](https://github.com/n8n-io/n8n/commit/17799cda46ad764f537d9546346ab4e04e36e681))
- **NextCloud Node:** Fix issue with credential verification and sharing file ([2b4f5c6](https://github.com/n8n-io/n8n/commit/2b4f5c6c785ab6ffc7198f60369886c44dea6ef2))
- **Freshdesk Node:** Fix issue when getAll operation requires non existent options ([329fe95](https://github.com/n8n-io/n8n/commit/329fe9581f63fe44daba5ef79724d9339cb8c813))

### Features

- **cli:** Notify external hooks about user profile and password changes ([#3919](https://github.com/n8n-io/n8n/issues/3919)) ([7d74dda](https://github.com/n8n-io/n8n/commit/7d74ddab29e05a81962fd80469248e8cee8bf9bf))
- **core, editor:** Support `pairedItem` for pinned data ([#3843](https://github.com/n8n-io/n8n/issues/3843)) ([b1e7152](https://github.com/n8n-io/n8n/commit/b1e715299d8a78188fad413392babdea7d044049))
- **core:** Add command to scripts for easy launch n8n with tunnel ([725a567](https://github.com/n8n-io/n8n/commit/725a567f07c08767f58d4ceb88386a9be694bfd2))
- **editor, core:** Integrate PostHog ([#3865](https://github.com/n8n-io/n8n/issues/3865)) ([43e054f](https://github.com/n8n-io/n8n/commit/43e054f5abae87b989ffe391a251961a2bc05542))
- **editor:** Map expressions from input table ([#3864](https://github.com/n8n-io/n8n/issues/3864)) ([ce076dc](https://github.com/n8n-io/n8n/commit/ce076dca48847562067c5149ecdd529fcc014e3f))

## [0.191.1](https://github.com/n8n-io/n8n/compare/n8n@0.191.0...n8n@0.191.1) (2022-08-19)

### Bug Fixes

- **editor:** Fix issue with disappearing connections after rename ([#3899](https://github.com/n8n-io/n8n/issues/3899)) ([ad0c214](https://github.com/n8n-io/n8n/commit/ad0c214f8ec2088ff30f408fe5ec51216468cdff))

# [0.191.0](https://github.com/n8n-io/n8n/compare/n8n@0.190.0...n8n@0.191.0) (2022-08-17)

### Bug Fixes

- **cli:** Fix community nodes tests on Postgres and MySQL ([#3861](https://github.com/n8n-io/n8n/issues/3861)) ([620525e](https://github.com/n8n-io/n8n/commit/620525ea85b7de24c0c5f3d3b57350a0a578d9b4))
- **core:** Fix issue with not displayed child workflow executions ([#3867](https://github.com/n8n-io/n8n/issues/3867)) ([f782bcd](https://github.com/n8n-io/n8n/commit/f782bcd52dbe364d1fca1bd29c9222f434df90ae))
- **editor:** Handling errors when opening settings and executions ([#3877](https://github.com/n8n-io/n8n/issues/3877)) ([762b422](https://github.com/n8n-io/n8n/commit/762b4224888cc5949eced048729fe313ec055f1c))
- **editor:** Improve expression and parameters performance ([#3874](https://github.com/n8n-io/n8n/issues/3874)) ([3608d13](https://github.com/n8n-io/n8n/commit/3608d132c0fbdb193758ba9a9c0f1da725d2313a))
- **public-api:** Fix executions pagination in Postgres and Mysql ([52015a6](https://github.com/n8n-io/n8n/commit/52015a6f033eae5c2ea9ac125a7c947d96ce7463))

### Features

- **cli:** Enable community nodes based on npm availability ([#3871](https://github.com/n8n-io/n8n/issues/3871)) ([936264b](https://github.com/n8n-io/n8n/commit/936264b3c6506cdc25b9ad55a23b314b2582275b))
- **editor:** Added animated tooltips to draggable columns in input panel ([054cc01](https://github.com/n8n-io/n8n/commit/054cc010edfc9f0f5cc72ac94f26afe52a66a192))

# [0.190.0](https://github.com/n8n-io/n8n/compare/n8n@0.189.1...n8n@0.190.0) (2022-08-10)

### Bug Fixes

- **core:** Fix crash caused by parallel test-webhook calls ([#3756](https://github.com/n8n-io/n8n/issues/3756)) ([8fe71db](https://github.com/n8n-io/n8n/commit/8fe71dba4bf568e70ed740ac3413aae77559ca3c))
- **core:** Fix issue that static data did not get saved for poll-triggers ([#3853](https://github.com/n8n-io/n8n/issues/3853)) ([8311abc](https://github.com/n8n-io/n8n/commit/8311abcf9d453f0d253c269e7d1c3842fcf8e256))
- **GitHub Trigger:** Fix typo ([#3859](https://github.com/n8n-io/n8n/issues/3859)) ([7b3d6de](https://github.com/n8n-io/n8n/commit/7b3d6de44eeb6cb066fb378c52fcc5aec60c4fdf))
- **public-api:** fix issue paginating executions ([b9fe707](https://github.com/n8n-io/n8n/commit/b9fe707cbd9df4a33b6040215826375bef238b65))

### Features

- Synchronize default VSCode settings ([#3833](https://github.com/n8n-io/n8n/issues/3833)) ([11461fd](https://github.com/n8n-io/n8n/commit/11461fda5fae10077ea9804b5cc9581074107005))

## [0.189.1](https://github.com/n8n-io/n8n/compare/n8n@0.189.0...n8n@0.189.1) (2022-08-05)

### Bug Fixes

- Fix issue with MySQL/MariaDB migration ([#3832](https://github.com/n8n-io/n8n/issues/3832))

# [0.189.0](https://github.com/n8n-io/n8n/compare/n8n@0.188.0...n8n@0.189.0) (2022-08-03)

### Bug Fixes

- **editor:** Fix label cut off ([#3820](https://github.com/n8n-io/n8n/issues/3820)) ([0f27be4](https://github.com/n8n-io/n8n/commit/0f27be4447662056a2ba13c027280830f7eab09b))
- Fix problem saving workflow when tags disabled ([#3792](https://github.com/n8n-io/n8n/issues/3792)) ([f0dddaa](https://github.com/n8n-io/n8n/commit/f0dddaa2a585715b35e26b16e1003e1683ab9402))

### Features

- **NocoDB Node:** Add support v0.90.0+ ([#3146](https://github.com/n8n-io/n8n/issues/3146)) ([d65a9ed](https://github.com/n8n-io/n8n/commit/d65a9ed118ff16c67b6d69d68108d8b7da1814d9))
- **SendInBlue Node:** Add SendInBlue Regular + Trigger Node ([#3746](https://github.com/n8n-io/n8n/issues/3746)) ([74cedd9](https://github.com/n8n-io/n8n/commit/74cedd94a82f0c053a24b6e925d9e3bcadcebfbc))
- Support community nodes on Windows ([#3823](https://github.com/n8n-io/n8n/issues/3823)) ([e8eda74](https://github.com/n8n-io/n8n/commit/e8eda7470a17deec1f5eab8cded6e74a8e3aee39))

# [0.188.0](https://github.com/n8n-io/n8n/compare/n8n@0.187.2...n8n@0.188.0) (2022-07-27)

### Bug Fixes

- **AWS DynamoDB Node:** Fix expression attribute names ([#3763](https://github.com/n8n-io/n8n/issues/3763)) ([88cb265](https://github.com/n8n-io/n8n/commit/88cb26556c162aa1281dfa6a9fa8eca4cd071e9d))
- **core:** Add windows support to import:credentials --separate ([#3589](https://github.com/n8n-io/n8n/issues/3589)) ([2fb590e](https://github.com/n8n-io/n8n/commit/2fb590e8440ac35567fdbf745b294d79feb8c5a9))
- **editor:** Fix linking buttons color ([#3770](https://github.com/n8n-io/n8n/issues/3770)) ([deb510a](https://github.com/n8n-io/n8n/commit/deb510a8e0057280da43f3b3e72d8acca5829745))
- **editor:** Fix pin data in executions when pinData is null. ([#3787](https://github.com/n8n-io/n8n/issues/3787)) ([30c0f21](https://github.com/n8n-io/n8n/commit/30c0f21b3f37280403848592877cb8658367b85e))
- **editor:** Fix spaces bug ([#3774](https://github.com/n8n-io/n8n/issues/3774)) ([02549e3](https://github.com/n8n-io/n8n/commit/02549e3ba9233a6d9f75fc1f9ff138e2aff7f4b9))
- **editor:** Fix sticky duplication and position bug ([#3755](https://github.com/n8n-io/n8n/issues/3755)) ([92614c8](https://github.com/n8n-io/n8n/commit/92614c81abfdbca51d4901b364467d3505870255))
- **editor:** Restore pindata header colors ([#3758](https://github.com/n8n-io/n8n/issues/3758)) ([1a7318b](https://github.com/n8n-io/n8n/commit/1a7318b4cf6081e5ba743117cf90ef6920625aa0))
- Fix node_type property in all events ([#3759](https://github.com/n8n-io/n8n/issues/3759)) ([1f1a63c](https://github.com/n8n-io/n8n/commit/1f1a63c39adc673259c951af3e5152c5edc34968))
- **Fix Rocketchat Node:** Fix authentication issue ([#3778](https://github.com/n8n-io/n8n/issues/3778)) ([2710061](https://github.com/n8n-io/n8n/commit/271006152386511c19feb54e438fa60966dbf705))
- **Mautic Node:** Fix authentication issue ([#3761](https://github.com/n8n-io/n8n/issues/3761)) ([fe58769](https://github.com/n8n-io/n8n/commit/fe58769b4830f388ad67ae1c32fcaa55aa0b848e))

### Features

- Improvements to pairedItem ([1348349](https://github.com/n8n-io/n8n/commit/13483497484e205975ef71091e3892f757f608e1))
- **Item List Node:** Add operation for creating array from input items ([#3149](https://github.com/n8n-io/n8n/issues/3149)) ([553b14a](https://github.com/n8n-io/n8n/commit/553b14a13c7c9056447ef0b18c9427f26221b44d))
- **Kafka Trigger Node:** Add additional options ([#3600](https://github.com/n8n-io/n8n/issues/3600)) ([3496a39](https://github.com/n8n-io/n8n/commit/3496a39788b654b46485955ba5cce5e5865babc7))
- **Metabase Node:** Add Metabase Node ([#3033](https://github.com/n8n-io/n8n/issues/3033)) ([81b5828](https://github.com/n8n-io/n8n/commit/81b58285588f142c0b1cc148f0092c462eefdd73))

## [0.187.2](https://github.com/n8n-io/n8n/compare/n8n@0.187.1...n8n@0.187.2) (2022-07-21)

### Bug Fixes

- **editor:** Fix console error ([#3751](https://github.com/n8n-io/n8n/issues/3751)) ([3a98028](https://github.com/n8n-io/n8n/commit/3a98028722d634f604a650d891cf6fabf722993d))
- **editor:** Fix login issue for non-admin users ([#3754](https://github.com/n8n-io/n8n/issues/3754)) ([ccd1ed2](https://github.com/n8n-io/n8n/commit/ccd1ed2c4c5153637a7900a79a40b1c4f53e7635))
- **editor:** Fix problems with credentials modal if no node is opened ([#3749](https://github.com/n8n-io/n8n/issues/3749)) ([5efe4a4](https://github.com/n8n-io/n8n/commit/5efe4a4c54211f1d395202c420403be3cc7e4446))
- **NocoDB Node:** Fix authentication issue ([#3750](https://github.com/n8n-io/n8n/issues/3750)) ([e65016c](https://github.com/n8n-io/n8n/commit/e65016c861176a7b17f23c5fbf3c0a3fcc1e5e1d))

## [0.187.1](https://github.com/n8n-io/n8n/compare/n8n@0.187.0...n8n@0.187.1) (2022-07-20)

### Bug Fixes

- **editor:** Fix issue that new nodes did not get automatically displayed in all connected browsers ([#3745](https://github.com/n8n-io/n8n/issues/3745)) ([34a9bee](https://github.com/n8n-io/n8n/commit/34a9beefa5b0f169f38ca48d3444af8f160c85a2))

# [0.187.0](https://github.com/n8n-io/n8n/compare/n8n@0.186.1...n8n@0.187.0) (2022-07-20)

### Bug Fixes

- **api:** Add missing node settings parameters ([#3737](https://github.com/n8n-io/n8n/issues/3737)) ([803e009](https://github.com/n8n-io/n8n/commit/803e0097fada1bf0385ac37965f0cc47bed28948))
- **api:** Validate static data value for resource workflow ([#3736](https://github.com/n8n-io/n8n/issues/3736)) ([7ba9a05](https://github.com/n8n-io/n8n/commit/7ba9a055cdeb2b0713857747a5b722dab65d3678))
- **Baserow Node:** Fix issue that table names are not getting pulled in new version ([#3721](https://github.com/n8n-io/n8n/issues/3721)) ([f65a5db](https://github.com/n8n-io/n8n/commit/f65a5db478da0da65735bdc5bb09774f1d473ec9))
- **editor:** Hide 'Execute previous node' button in readonly mode ([#3714](https://github.com/n8n-io/n8n/issues/3714)) ([7fb81dc](https://github.com/n8n-io/n8n/commit/7fb81dcd8a6c56e6e104be94278c690caf35c846))
- **editor:** Hide tabs if only 1 branch ([#3743](https://github.com/n8n-io/n8n/issues/3743)) ([fb67543](https://github.com/n8n-io/n8n/commit/fb67543b2f10c558abcacc5454d6fa0687ee4702))
- Fix broken links in nodes ([#3716](https://github.com/n8n-io/n8n/issues/3716)) ([c9b7b6d](https://github.com/n8n-io/n8n/commit/c9b7b6d30fe822bddb3d68e1b4757ffe654e918b))

### Features

- Add more credentials tests ([#3668](https://github.com/n8n-io/n8n/issues/3668)) ([683d2df](https://github.com/n8n-io/n8n/commit/683d2dfc98136503971a4beb1692e5ca191d5016))
- Add support for preAuthentication and add Metabase credentials ([#3399](https://github.com/n8n-io/n8n/issues/3399)) ([994c89a](https://github.com/n8n-io/n8n/commit/994c89a6c6ade5b99d6218c9776adc15c286b619))
- **core:** Autofix pairedItem information if inputItems(n) === outputItems(n) ([68fb1c6](https://github.com/n8n-io/n8n/commit/68fb1c64dca99fb603fe6d52fd50c4749a2ca898))
- **editor:** Add data pinning functionality ([#3511](https://github.com/n8n-io/n8n/issues/3511)) ([15693b0](https://github.com/n8n-io/n8n/commit/15693b0056097129a57dfc600807dbc5e1cc07f1)
- **editor:** Add drag and drop data mapping ([#3708](https://github.com/n8n-io/n8n/issues/3708)) ([577c73e](https://github.com/n8n-io/n8n/commit/577c73ee25c5bfc943ef5ed1de550fcb489f4998))
- **ERPNext Node:** Add credential test and add support for unauthorized certs ([#3732](https://github.com/n8n-io/n8n/issues/3732)) ([a02b206](https://github.com/n8n-io/n8n/commit/a02b20617071e1ca398735456cb416d6ab3f34a0)), closes [#3739](https://github.com/n8n-io/n8n/issues/3739)
- **Google Drive Node:** Add move to trash support ([#3693](https://github.com/n8n-io/n8n/issues/3693)) ([7406432](https://github.com/n8n-io/n8n/commit/74064325c892c5b506260e650d3361636b578b1e))
- Make it possible to dynamically load community nodes ([#2849](https://github.com/n8n-io/n8n/issues/2849)) ([c85faff](https://github.com/n8n-io/n8n/commit/c85faff4f1c6ba11c02cf5c14122d2c7341f3ec3)), closes [#3497](https://github.com/n8n-io/n8n/issues/3497) [#3501](https://github.com/n8n-io/n8n/issues/3501) [#3527](https://github.com/n8n-io/n8n/issues/3527) [#3562](https://github.com/n8n-io/n8n/issues/3562)
- **Mindee Node:** Add support for new version ([#3596](https://github.com/n8n-io/n8n/issues/3596)) ([1965407](https://github.com/n8n-io/n8n/commit/1965407030638cc309c99d344121f47805c93799))
- **Notion Node:** Allow to ignore Notion URL properties if empty ([#3564](https://github.com/n8n-io/n8n/issues/3564)) ([6cb9aef](https://github.com/n8n-io/n8n/commit/6cb9aefb0b3e4d17382042371a20e63f23641581))
- **Shopify Node:** Add OAuth support ([#3389](https://github.com/n8n-io/n8n/issues/3389)) ([945e25a](https://github.com/n8n-io/n8n/commit/945e25a77cf9ba33bc3e4b70053319ea86230cf7))

## [0.186.1](https://github.com/n8n-io/n8n/compare/n8n@0.186.0...n8n@0.186.1) (2022-07-14)

### Bug Fixes

- **Airtable Node:** Fix authentication issue ([#3709](https://github.com/n8n-io/n8n/issues/3709)) ([33d8042](https://github.com/n8n-io/n8n/commit/33d804284ae02140749ab94eecfca1699e13afee))

# [0.186.0](https://github.com/n8n-io/n8n/compare/n8n@0.185.0...n8n@0.186.0) (2022-07-13)

### Bug Fixes

- **editor:** Fix error after multiple executions ([#3697](https://github.com/n8n-io/n8n/issues/3697)) ([d200661](https://github.com/n8n-io/n8n/commit/d200661b84c36b3f04d812cf022bb338f9664392))
- **EmailReadImap Node:** Improve handling of network problems ([#3406](https://github.com/n8n-io/n8n/issues/3406)) ([6f5809e](https://github.com/n8n-io/n8n/commit/6f5809edb3f9cac0c29d448300b37ab9b6e74c08))
- **Google Drive Node:** Process all input items with List operation ([#3525](https://github.com/n8n-io/n8n/issues/3525)) ([ece1836](https://github.com/n8n-io/n8n/commit/ece1836c45707d349330f742eb3b83fa1f4eaebb))
- **Telegram Node:** Fix sending binaryData media (photo, document, video etc.) ([#3408](https://github.com/n8n-io/n8n/issues/3408)) ([af45a07](https://github.com/n8n-io/n8n/commit/af45a07f21d8448bad5c12ed702b7aa983017a2b))

### Features

- Add item information to more node errors ([#3681](https://github.com/n8n-io/n8n/issues/3681)) ([2a8043c](https://github.com/n8n-io/n8n/commit/2a8043cd27968b92b1857135d130e3ee54aae779))
- **AWS DynamoDB Node:** Improve error handling + add optional GetAll Scan FilterExpression ([#3318](https://github.com/n8n-io/n8n/issues/3318)) ([732c8fc](https://github.com/n8n-io/n8n/commit/732c8fcf8488fc35839855499f75202436fc4c9a))
- **Customer.io Node:** Add support for tracking API region selection ([#3378](https://github.com/n8n-io/n8n/issues/3378)) ([82a254a](https://github.com/n8n-io/n8n/commit/82a254a8d9295901e42ec999432a7f5b40f38281))
- **Elasticsearch Node:** Add 'Source Excludes' and 'Source Includes' options on 'Document: getAll' operation ([#3660](https://github.com/n8n-io/n8n/issues/3660)) ([8999403](https://github.com/n8n-io/n8n/commit/899940322831612bdf6e59db7f696c34f96cd496))
- **Elasticsearch Node:** Add credential tests, index pipelines and index refresh ([#2420](https://github.com/n8n-io/n8n/issues/2420))
- **Freshworks CRM Node:** Add Search + Lookup functionality ([#3131](https://github.com/n8n-io/n8n/issues/3131)) ([dbc0280](https://github.com/n8n-io/n8n/commit/dbc02803db5351d759b1420e94b14f2c7c8b1bef))
- **Jira Trigger Node:** Add optional query auth for security ([#3172](https://github.com/n8n-io/n8n/issues/3172)) ([25093b6](https://github.com/n8n-io/n8n/commit/25093b64e693a33a76efd1bd12f00ce0d4cc0f3c))
- **Postgres Node:** Improvement handling of large numbers ([#3360](https://github.com/n8n-io/n8n/issues/3360)) ([9f908e7](https://github.com/n8n-io/n8n/commit/9f908e7405d687bf57391e503ad724d58caaac07))
- **Redis Node:** Add push and pop operations ([#3127](https://github.com/n8n-io/n8n/issues/3127)) ([32c68eb](https://github.com/n8n-io/n8n/commit/32c68eb126f8411d1a3261dc8a900c109b99da6f))
- **Rename Node:** Add regex replace ([#2576](https://github.com/n8n-io/n8n/issues/2576)) ([eae9a60](https://github.com/n8n-io/n8n/commit/eae9a60a431bc08fb58016e3249328abb90716b0))
- **SpreadsheetFile Node:** Allow skipping headers when writing spreadsheets ([#3234](https://github.com/n8n-io/n8n/issues/3234)) ([dbfb8d5](https://github.com/n8n-io/n8n/commit/dbfb8d56dc6290837701dea5957d4e73db418892))
- Updated multiple credentials with tests and allow to be used on HTTP Request Node ([#3670](https://github.com/n8n-io/n8n/issues/3670)) ([d5d4dd3](https://github.com/n8n-io/n8n/commit/d5d4dd38450b788ee0ce3ed8ad0eb714c86977d2))

# [0.185.0](https://github.com/n8n-io/n8n/compare/n8n@0.184.0...n8n@0.185.0) (2022-07-05)

### Bug Fixes

- **Hubspot Node:** Fix search endpoints ([#3640](https://github.com/n8n-io/n8n/issues/3640)) ([16b9926](https://github.com/n8n-io/n8n/commit/16b9926cd25abf4a2ae4c9eba494340eab58082f))
- **KoboToolbox Node:** Improve attachment matching logic and GeoJSON Polygon format ([#3535](https://github.com/n8n-io/n8n/issues/3535)) ([637e815](https://github.com/n8n-io/n8n/commit/637e81552f86788058567342cf69e2784e3d6b2f))
- **Odoo Node:** Prevent possible issues with some custom fields ([#3496](https://github.com/n8n-io/n8n/issues/3496)) ([7d968ec](https://github.com/n8n-io/n8n/commit/7d968ec202ceccc6a009ec150747cc927273f841))
- **Sticky Node:** Fix main header hiding ([#3654](https://github.com/n8n-io/n8n/issues/3654)) ([88486bc](https://github.com/n8n-io/n8n/commit/88486bc778786d4a47ef1bb5c743c9fb206aee01))
- **Todoist Node:** Fix multiple item support ([#3614](https://github.com/n8n-io/n8n/issues/3614)) ([7ba85c4](https://github.com/n8n-io/n8n/commit/7ba85c4ab910ed02696078ece12c88f2141cccad))

### Features

- **core:** Add `action` to `INodePropertyOptions` ([#3610](https://github.com/n8n-io/n8n/issues/3610)) ([3c65968](https://github.com/n8n-io/n8n/commit/3c659682e94cdd01fd6f267a468a031b028cf690))
- **DeepL Node:** Add support for longer texts + Credential tests ([#3651](https://github.com/n8n-io/n8n/issues/3651)) ([88d6cfc](https://github.com/n8n-io/n8n/commit/88d6cfc07bfd2be64a39f285d235e22aae8c1522))
- **Facebook Node:** Add support for Facebook Graph API versions 14 ([#3656](https://github.com/n8n-io/n8n/issues/3656)) ([174d063](https://github.com/n8n-io/n8n/commit/174d06383191e6e70ba27bc3e6e46527731c80b5))
- **Google Ads Node:** Add new node ([#3526](https://github.com/n8n-io/n8n/issues/3526)) ([088daf9](https://github.com/n8n-io/n8n/commit/088daf952ea7340a3101362bce18668147b8431f))
- **Jira Node:** Use Jira rendered fields with simplify option ([#3323](https://github.com/n8n-io/n8n/issues/3323)) ([07b6cff](https://github.com/n8n-io/n8n/commit/07b6cffdba55a48bfed629a1faec8cf88bee88bc))
- **Webflow Trigger Node:** Reduce chance of webhook duplication and add credential test ([#3594](https://github.com/n8n-io/n8n/issues/3594)) ([224e008](https://github.com/n8n-io/n8n/commit/224e008fb64dabef99998508eb4385e1b872c5ad))
- **Wordpress Node:** Add post template option ([#3139](https://github.com/n8n-io/n8n/issues/3139)) ([02bc3da](https://github.com/n8n-io/n8n/commit/02bc3da78545de4771edf6fdc68720b0e7d596b9))

# [0.184.0](https://github.com/n8n-io/n8n/compare/n8n@0.183.0...n8n@0.184.0) (2022-06-29)

### Bug Fixes

- **core:** Fix logger error when logging circular json ([#3583](https://github.com/n8n-io/n8n/issues/3583)) ([3cb693d](https://github.com/n8n-io/n8n/commit/3cb693d5d4b8aaf800df70e62c1b2ca2ff208c4d))
- Correct misfix from `node-param-display-name-wrong-for-dynamic-multi-options` ([#3575](https://github.com/n8n-io/n8n/issues/3575)) ([2ccc7fb](https://github.com/n8n-io/n8n/commit/2ccc7fbc9d1df3f044cf42fe1af72bc7352caa9f))
- **Cortex Node:** Fix issue that not all Analyzers got returned ([#3606](https://github.com/n8n-io/n8n/issues/3606)) ([6e595c7](https://github.com/n8n-io/n8n/commit/6e595c72760f47107f67c1fd2bdbe76c31af4a8b))
- **editor:** Display full text of long error messages ([#3561](https://github.com/n8n-io/n8n/issues/3561)) ([8db4405](https://github.com/n8n-io/n8n/commit/8db44057f2101698ef4869fca436862e4dd39fc1))
- **editor:** Fix credentials rendering when the node has no parameters ([#3563](https://github.com/n8n-io/n8n/issues/3563)) ([55bab19](https://github.com/n8n-io/n8n/commit/55bab19eb440ed9d58137f4334a37d5f731afe0f))
- Fix issue with required optional parameters ([#3577](https://github.com/n8n-io/n8n/issues/3577)) ([42d2959](https://github.com/n8n-io/n8n/commit/42d2959f47f33defda4239a4d2fbba6927d98617))
- Fix issue with required optional parameters ([#3597](https://github.com/n8n-io/n8n/issues/3597)) ([848fcfd](https://github.com/n8n-io/n8n/commit/848fcfde5d95d952170e9a3d51b629971a13b832))
- **HTTP Request Node:** Make all OAuth2 credentials work with HTTP Request Node ([#3503](https://github.com/n8n-io/n8n/issues/3503)) ([acdb4d9](https://github.com/n8n-io/n8n/commit/acdb4d92c8ef95646e69694b2451a9111a81c52f))
- **LinkedIn Node:** Fix LinkedIn image preview ([#3528](https://github.com/n8n-io/n8n/issues/3528)) ([32f245d](https://github.com/n8n-io/n8n/commit/32f245da53c186a03172dbb23761a05b5e301532))
- **Salesforce Node:** Fix issue with lead status not using name on update ([#3599](https://github.com/n8n-io/n8n/issues/3599)) ([7ccae7c](https://github.com/n8n-io/n8n/commit/7ccae7c9b22f2848a8aa357227d145241801ba82))

### Features

- **Clockify Node:** Add more resources and improvements ([#3411](https://github.com/n8n-io/n8n/issues/3411)) ([447d190](https://github.com/n8n-io/n8n/commit/447d19024c512eea8e290d8ebc6c3ce82a53f002))
- **core:** Expose item index being processed ([#3590](https://github.com/n8n-io/n8n/issues/3590)) ([1e4fd9e](https://github.com/n8n-io/n8n/commit/1e4fd9e4df524fdee8195de7be244ff03d97f917))
- **core:** Give access to getBinaryDataBuffer in preSend method ([#3588](https://github.com/n8n-io/n8n/issues/3588)) ([522b31a](https://github.com/n8n-io/n8n/commit/522b31a47b4f4e9990e07dcc504ef2821a1fd0a5))
- Migrated to npm release of riot-tmpl fork ([#3581](https://github.com/n8n-io/n8n/issues/3581)) ([891844e](https://github.com/n8n-io/n8n/commit/891844ea8b3248195355f736d7331fd967ee99e1))

# [0.183.0](https://github.com/n8n-io/n8n/compare/n8n@0.182.1...n8n@0.183.0) (2022-06-21)

### Bug Fixes

- **core:** Do allow OPTIONS requests from any source ([#3555](https://github.com/n8n-io/n8n/issues/3555)) ([74e6b06](https://github.com/n8n-io/n8n/commit/74e6b06467f8d0059c8cc45154e2d2822dc9b0c5))
- **core:** Fix issue that GET /workflows/:id does not return tags ([#3522](https://github.com/n8n-io/n8n/issues/3522)) ([f75f5d7](https://github.com/n8n-io/n8n/commit/f75f5d711f886892a1afcebff722ab476390f4f0))
- **core:** Fix issue that some predefined credentials do not show up on HTTP Request Node ([#3556](https://github.com/n8n-io/n8n/issues/3556)) ([d417ea7](https://github.com/n8n-io/n8n/commit/d417ea7ffad9e2210f3b2b5e7122ffbe70f2ba27))
- **core:** Return correct error message if Axios error ([#3478](https://github.com/n8n-io/n8n/issues/3478)) ([1bef4df](https://github.com/n8n-io/n8n/commit/1bef4df75f999ac2e413b6c179baab3321c52fa2))
- **core:** Updated expressions allowlist and denylist. ([#3424](https://github.com/n8n-io/n8n/issues/3424)) ([d18a29d](https://github.com/n8n-io/n8n/commit/d18a29d5882fb8f4475258189f6badcd0a573b34))

### Features

- **editor:** Improve trigger panel ([#3509](https://github.com/n8n-io/n8n/issues/3509)) ([a2f6289](https://github.com/n8n-io/n8n/commit/a2f628927dff7ea6741ef8e4a60bcafd95dac7bf))
- **Hubspot Node:** Allow to set Stage on Ticket Update ([#3317](https://github.com/n8n-io/n8n/issues/3317)) ([0ac9e3f](https://github.com/n8n-io/n8n/commit/0ac9e3f975b73e88acabb66de8b8565f881f64ec))
- **Todoist Node:** Make it possible to move tasks between sections ([#3074](https://github.com/n8n-io/n8n/issues/3074)) ([049e454](https://github.com/n8n-io/n8n/commit/049e4544d9ccc0acce2a596aced06ec86992e09a))
- **Twake Node:** Update icon, add cred test and custom operation support ([#3431](https://github.com/n8n-io/n8n/issues/3431)) ([6d64e84](https://github.com/n8n-io/n8n/commit/6d64e84f5e19d5f6d83ccc0a55cdcbd256e5804f))

## [0.182.1](https://github.com/n8n-io/n8n/compare/n8n@0.182.0...n8n@0.182.1) (2022-06-16)

### Bug Fixes

- **core:** Fix issue with restarting waiting executions ([#3531](https://github.com/n8n-io/n8n/issues/3531)) ([c9273bc](https://github.com/n8n-io/n8n/commit/c9273bcd3862217b4918ac8abb37fae9c2e64622))

# [0.182.0](https://github.com/n8n-io/n8n/compare/n8n@0.181.2...n8n@0.182.0) (2022-06-14)

### Bug Fixes

- **core:** Fix issue that parameters got lost in some edge cases ([04f0bf5](https://github.com/n8n-io/n8n/commit/04f0bf5b65c8224a4fdfd3c9d2c896f63dfbcc1d))
- **core:** Fix issue with combined expression not resolving if one is invalid ([#3506](https://github.com/n8n-io/n8n/issues/3506)) ([9ff5762](https://github.com/n8n-io/n8n/commit/9ff57629c5afb2f0fd4aee84cda79c9a6f7962d0))
- **core:** Fix Public API failing to build on Windows ([#3499](https://github.com/n8n-io/n8n/issues/3499)) ([c121952](https://github.com/n8n-io/n8n/commit/c121952324619434e8a7be540970c167df715b13))
- **editor:** Fix issue that some errors did not show up correctly ([#3507](https://github.com/n8n-io/n8n/issues/3507)) ([955db0a](https://github.com/n8n-io/n8n/commit/955db0ab101feb17efffe760c79ec2820e1d4c3b))
- **HTTP Request Node:** Fix issue with requests that return null ([#3498](https://github.com/n8n-io/n8n/issues/3498)) ([7346da0](https://github.com/n8n-io/n8n/commit/7346da0b34b5fdf7ab630ccc5cda102cf80c8036))
- **Pipedrive Node:** Fix limit issue with Lead -> GetAll ([#3436](https://github.com/n8n-io/n8n/issues/3436)) ([34e891c](https://github.com/n8n-io/n8n/commit/34e891c0f8c987c9be9cff463422b9972f02269f))
- **PostBin Node:** Fix issue with it throwing unnecessary error ([#3494](https://github.com/n8n-io/n8n/issues/3494)) ([9df3e30](https://github.com/n8n-io/n8n/commit/9df3e30d36104d8e31972c773cb71f4cc82f6970))

### Features

- **core:** Add "Client Credentials" grant type to OAuth2 ([#3489](https://github.com/n8n-io/n8n/issues/3489)) ([e29c597](https://github.com/n8n-io/n8n/commit/e29c5975e1f1ad089167df46021203e9f67c8ef1))
- **Twilio Node:** Add ability to make a voice call using TTS ([#3467](https://github.com/n8n-io/n8n/issues/3467)) ([eff97e8](https://github.com/n8n-io/n8n/commit/eff97e8d67cd3f0342bbb9648503b351f4691f46))
- **Wise Node:** Add Support to download statements as JSON, CSV or PDF ([#3468](https://github.com/n8n-io/n8n/issues/3468)) ([51663c1](https://github.com/n8n-io/n8n/commit/51663c1fcbe879e29790af942b73318e95065d8f))

## [0.181.2](https://github.com/n8n-io/n8n/compare/n8n@0.181.1...n8n@0.181.2) (2022-06-09)

### Bug Fixes

- **core:** Fix issue when a node does not return data ([5eea3cd](https://github.com/n8n-io/n8n/commit/5eea3cd6d0b59963dc7c7a9e1ca597137cf3ce98))

## [0.181.1](https://github.com/n8n-io/n8n/compare/n8n@0.181.0...n8n@0.181.1) (2022-06-09)

### Bug Fixes

- **core:** Fix another possible issue with multi input nodes ([e88fab5](https://github.com/n8n-io/n8n/commit/e88fab5ee2b82665c3d68c52894a5479ce6eccf6))
- **core:** Fix issue with multi input nodes ([f79675d](https://github.com/n8n-io/n8n/commit/f79675d5c7876875065fc29504eb0590678d67d3))

# [0.181.0](https://github.com/n8n-io/n8n/compare/n8n@0.180.0...n8n@0.181.0) (2022-06-08)

### Bug Fixes

- **core:** Properly resolve expressions in declarative node design ([1999f4b](https://github.com/n8n-io/n8n/commit/1999f4b066784cc1dd6a962f51d7c11641577a8b))

### Features

- Add n8n Public API ([#3064](https://github.com/n8n-io/n8n/issues/3064)) ([a18081d](https://github.com/n8n-io/n8n/commit/a18081d749c51d497645d43614fdccb220344607))
- **core:** Make it possible to block access to environment variables ([ddb3baa](https://github.com/n8n-io/n8n/commit/ddb3baa4eddeb85e2f7abe4465ac4ff4058e1ece))

# [0.180.0](https://github.com/n8n-io/n8n/compare/n8n@0.179.0...n8n@0.180.0) (2022-06-07)

### Bug Fixes

- **core:** Allow "window" again in expressions ([#3474](https://github.com/n8n-io/n8n/issues/3474)) ([ca92ff7](https://github.com/n8n-io/n8n/commit/ca92ff70d7789e7d0af812cff7c7351e499ddfa2))
- **core:** Fix `user-management:reset` command ([#3403](https://github.com/n8n-io/n8n/issues/3403)) ([58ecadf](https://github.com/n8n-io/n8n/commit/58ecadf53c35ee0dc897eb7eb29f345f8e797b2b))
- **core:** Fix crashes in queue mode ([#3397](https://github.com/n8n-io/n8n/issues/3397)) ([042b8da](https://github.com/n8n-io/n8n/commit/042b8daf1cd16822e2da03cf18a69091477d4451))
- **editor:** Fix delete button hover spacing ([#3412](https://github.com/n8n-io/n8n/issues/3412)) ([50ff75e](https://github.com/n8n-io/n8n/commit/50ff75ecb2b42dfdb00e9c086cf604f1ca699360))
- **editor:** Fix stuck loading states ([#3428](https://github.com/n8n-io/n8n/issues/3428)) ([450a9aa](https://github.com/n8n-io/n8n/commit/450a9aafea0e44c5d6e6541a9e0872a9d3ac7dee))
- **EmailReadImap Node:** Improve error handling ([#3465](https://github.com/n8n-io/n8n/issues/3465)) ([3806d63](https://github.com/n8n-io/n8n/commit/3806d6355d4af4ad1222bac20cb36f5ef586501a))
- **Hubspot Node:** Fix loading of Contacts ([#3426](https://github.com/n8n-io/n8n/issues/3426)) ([f02421b](https://github.com/n8n-io/n8n/commit/f02421b5f3c4946aac6257bbd806d72d0031313f))

### Features

- **Cal Trigger Node:** Add cal.com Trigger Node ([#3439](https://github.com/n8n-io/n8n/issues/3439)) ([1fa445e](https://github.com/n8n-io/n8n/commit/1fa445e0e74462dd28fc81329230b868137dcbd5))
- **core:** Add support for pairedItem (beta) ([#3012](https://github.com/n8n-io/n8n/issues/3012)) ([bdb8413](https://github.com/n8n-io/n8n/commit/bdb84130d687811d65337ff6b025e7cb0eae8256))
- **core:** Add support to import/export tags ([#3130](https://github.com/n8n-io/n8n/issues/3130)) ([15a20d2](https://github.com/n8n-io/n8n/commit/15a20d257d7b6b35224c0a654f0f1988081d06d2))
- **core:** Run Error Workflow also on trigger activation error ([#3470](https://github.com/n8n-io/n8n/issues/3470)) ([b5535e4](https://github.com/n8n-io/n8n/commit/b5535e4a6233d397060308ad1b8c254b28a2d57e))
- **editor:** Display Credential-Selector after Authentication Type-Selector ([#3461](https://github.com/n8n-io/n8n/issues/3461)) ([59a59e0](https://github.com/n8n-io/n8n/commit/59a59e0c5f1a5207a7124655b5768ac9fededcdc))
- **editor:** Display node specific settings above general ones ([50ca9c4](https://github.com/n8n-io/n8n/commit/50ca9c4c7e39e1ba176724c4b20dbbab12695cc4))
- **GitHub Node:**: Add Organization -> Get All operation ([#3247](https://github.com/n8n-io/n8n/pull/3247))
- **QuickBooks Node:** Add optional Tax item field ([#3404](https://github.com/n8n-io/n8n/issues/3404)) ([c341b45](https://github.com/n8n-io/n8n/commit/c341b45396c7282da087046ade16265c99c8d9dd))

# [0.179.0](https://github.com/n8n-io/n8n/compare/n8n@0.178.2...n8n@0.179.0) (2022-05-30)

### Bug Fixes

- **core:** Fix issue that "closeFunction" got called twice ([1910299](https://github.com/n8n-io/n8n/commit/1910299a884e8d4d80d4aa6656eb4892b0fcb713))
- **core:** Fix migrations on non-public Postgres schema ([#3356](https://github.com/n8n-io/n8n/issues/3356)) ([b49d493](https://github.com/n8n-io/n8n/commit/b49d49365398f06376e53d86e6c8c5dc15f67e57))
- **core:** Fix problem with uploading large files ([#3370](https://github.com/n8n-io/n8n/issues/3370)) ([d3cecfc](https://github.com/n8n-io/n8n/commit/d3cecfc55baf547b2a2bedddebf7e890510187e0))
- **core:** Prevent expressions XSS ([#3366](https://github.com/n8n-io/n8n/issues/3366)) ([993554f](https://github.com/n8n-io/n8n/commit/993554f22a575d68f7b4424fbcf7d5e0dd8a7186))
- **Discord Node:** Fix broken rate limit handling ([#3311](https://github.com/n8n-io/n8n/issues/3311)) ([b687ba1](https://github.com/n8n-io/n8n/commit/b687ba11ccac0dfb5a5c61e5db2604ffa8b5dec0))
- **editor:** Fix component in executions list failing custom validator ([#3284](https://github.com/n8n-io/n8n/issues/3284)) ([d719678](https://github.com/n8n-io/n8n/commit/d71967878f0ef43b8a464aa9e3703f80f5a08ed7))
- **editor:** Fix conflicting hover states between sticky button and node view ([#3368](https://github.com/n8n-io/n8n/issues/3368)) ([96a109a](https://github.com/n8n-io/n8n/commit/96a109a57c808943f3ab6121ff3e830b12e82d96))
- **editor:** Fix credential display bug ([#3372](https://github.com/n8n-io/n8n/issues/3372)) ([ed69c3c](https://github.com/n8n-io/n8n/commit/ed69c3cc18d47f906f8cf5c2a6784ee20ae390bd))
- **Gmail Node:** Fix sending attachments when filesystem mode is used ([#3396](https://github.com/n8n-io/n8n/issues/3396)) ([3a09da9](https://github.com/n8n-io/n8n/commit/3a09da92be556df1b840c0e16e020b0618ce7643))
- **Google Sheet Node:** Fix issue with null values and "Use Header Names as JSON Paths" option ([#3395](https://github.com/n8n-io/n8n/issues/3395)) ([fbf6019](https://github.com/n8n-io/n8n/commit/fbf60199d95d2448f9f34d0175da316fc18a80b7))
- **NextCloud Node:** Fix folder list with Nextcloud v24 ([#3386](https://github.com/n8n-io/n8n/issues/3386)) ([5f3bed3](https://github.com/n8n-io/n8n/commit/5f3bed3d4e9134b96d6964ca28b5b5dfb1adc1c3))

### Features

- **PostBin Node:** Add PostBin node ([#3236](https://github.com/n8n-io/n8n/issues/3236)) ([06c407d](https://github.com/n8n-io/n8n/commit/06c407def88e5872b2478ac240430006055a2a22))
- **RabbitMQ Trigger Node:** Make message acknowledgement and parallel processing configurable ([#3385](https://github.com/n8n-io/n8n/issues/3385)) ([b851289](https://github.com/n8n-io/n8n/commit/b85128900187b1709a7bf13eb5c5d5c4a5528fde))
- **ServiceNow Node:** Add attachment functionality ([#3137](https://github.com/n8n-io/n8n/issues/3137)) ([c38f6af](https://github.com/n8n-io/n8n/commit/c38f6af4993cd695888ff18b3f95e0d900e65711))
- **Todoist Node:** Add support for specifying the parent task when adding and listing tasks ([#3161](https://github.com/n8n-io/n8n/issues/3161)) ([dc77594](https://github.com/n8n-io/n8n/commit/dc77594a1eaec73fa34ed09c52d108482002ffff))

## [0.178.2](https://github.com/n8n-io/n8n/compare/n8n@0.178.1...n8n@0.178.2) (2022-05-25)

### Bug Fixes

- **editor:** Fix parameter loading bug ([#3374](https://github.com/n8n-io/n8n/issues/3374)) ([c7c2061](https://github.com/n8n-io/n8n/commit/c7c2061590493a1b24a8ab4e2615d6d9eb2641e1))

## [0.178.1](https://github.com/n8n-io/n8n/compare/n8n@0.178.0...n8n@0.178.1) (2022-05-24)

### Bug Fixes

- **editor:** Fix problem with HTTP Request Node 1 credentials to be set ([#3371](https://github.com/n8n-io/n8n/issues/3371)) ([c5fc3bc](https://github.com/n8n-io/n8n/commit/c5fc3bc45e80eec47f4c06b950ab8b3ddaf66f2f))

# [0.178.0](https://github.com/n8n-io/n8n/compare/n8n@0.177.0...n8n@0.178.0) (2022-05-24)

### Bug Fixes

- **editor:** Do not display diving line unless necessary ([68db12c](https://github.com/n8n-io/n8n/commit/68db12ce6d8bfc99cd0891cfa44f8b64674dada7))
- **editor:** Do not display welcome sticky in template workflows ([#3320](https://github.com/n8n-io/n8n/issues/3320)) ([29ddac3](https://github.com/n8n-io/n8n/commit/29ddac30d33caff1cf8a061d619742fdb3402d49))
- **Slack Node:** Fix Channel->Kick ([#3365](https://github.com/n8n-io/n8n/issues/3365)) ([0212d65](https://github.com/n8n-io/n8n/commit/0212d65dae885a6a153c67095f04215f5e1f8278))

### Features

- **core:** Allow credential reuse on HTTP Request node ([#3228](https://github.com/n8n-io/n8n/issues/3228)) ([336fc9e](https://github.com/n8n-io/n8n/commit/336fc9e2a820476931a9e9b482e4be284c0337d0)), closes [#3230](https://github.com/n8n-io/n8n/issues/3230) [#3231](https://github.com/n8n-io/n8n/issues/3231) [#3222](https://github.com/n8n-io/n8n/issues/3222) [#3229](https://github.com/n8n-io/n8n/issues/3229) [#3304](https://github.com/n8n-io/n8n/issues/3304) [#3282](https://github.com/n8n-io/n8n/issues/3282) [#3359](https://github.com/n8n-io/n8n/issues/3359)
- **editor:** Add input panel to NDV ([#3204](https://github.com/n8n-io/n8n/issues/3204)) ([3af0abd](https://github.com/n8n-io/n8n/commit/3af0abd9e066a721ac873f255eeb9311ebe6dd27))
- **Salesforce Node:** Add country field ([#3314](https://github.com/n8n-io/n8n/issues/3314)) ([90a1bc1](https://github.com/n8n-io/n8n/commit/90a1bc120bc2e291432c977768929da773dcb96e))

# [0.177.0](https://github.com/n8n-io/n8n/compare/n8n@0.176.0...n8n@0.177.0) (2022-05-16)

### Bug Fixes

- **core:** Fix call to `/executions-current` with unsaved workflow ([#3280](https://github.com/n8n-io/n8n/issues/3280)) ([7090a79](https://github.com/n8n-io/n8n/commit/7090a79b5da611d829da4d027a0194fcb60b4755))
- **core:** Fix issue with fixedCollection having all default values ([7ced654](https://github.com/n8n-io/n8n/commit/7ced65484fa7c91e10e96f70d6791b689a5686d3))
- **Edit Image Node:** Fix font selection ([#3287](https://github.com/n8n-io/n8n/issues/3287)) ([8a8feb1](https://github.com/n8n-io/n8n/commit/8a8feb11c8e22e6a548e077b55e40702f2fb724a))
- **Ghost Node:** Fix post tags and add credential tests ([#3278](https://github.com/n8n-io/n8n/issues/3278)) ([a14d85e](https://github.com/n8n-io/n8n/commit/a14d85ea481b8227ba306f07e13263f45eafa6ca))
- **Google Calendar Node:** Make it work with public calendars and clean up ([#3283](https://github.com/n8n-io/n8n/issues/3283)) ([a7d960c](https://github.com/n8n-io/n8n/commit/a7d960c56122bd3b602f0e9a121919916e5d6174))
- **KoBoToolbox Node:** Fix query and sort + use question name in attachments ([#3017](https://github.com/n8n-io/n8n/issues/3017)) ([c885115](https://github.com/n8n-io/n8n/commit/c8851157684fe15c77db1fe716fa4333b54450cb))
- **Mailjet Trigger Node:** Fix issue that node could not get activated ([#3281](https://github.com/n8n-io/n8n/issues/3281)) ([e09e349](https://github.com/n8n-io/n8n/commit/e09e349fedfe067929556e328a70a32d30759e4d))
- **Pipedrive Node:** Fix resolve properties when multi option field is used ([#3277](https://github.com/n8n-io/n8n/issues/3277)) ([7eb1261](https://github.com/n8n-io/n8n/commit/7eb12615cf3eebac29e3561a079451017f80de5c))

### Features

- **core:** Automatically convert Luxon Dates to string ([#3266](https://github.com/n8n-io/n8n/issues/3266)) ([3fcee14](https://github.com/n8n-io/n8n/commit/3fcee14bf5c61ec11fc1d4f30256f5ceba09e7f4))
- **editor:** Improve n8n welcome experience ([#3289](https://github.com/n8n-io/n8n/issues/3289)) ([35f2ce2](https://github.com/n8n-io/n8n/commit/35f2ce2359bb84437ad6fc68a7115081daeb46fe))
- **Google Drive Node:** Add Shared Drive support for operations upload, delete and share ([#3294](https://github.com/n8n-io/n8n/issues/3294)) ([03cdb1f](https://github.com/n8n-io/n8n/commit/03cdb1fea4fa4967eaafa861f3a9ff4ff7ca625a))
- **Microsoft OneDrive Node:** Add rename option for files and folders ([#3224](https://github.com/n8n-io/n8n/issues/3224)) ([50246d1](https://github.com/n8n-io/n8n/commit/50246d174a274fc9ba3dea44fc83c3605b4db691))

# [0.176.0](https://github.com/n8n-io/n8n/compare/n8n@0.175.1...n8n@0.176.0) (2022-05-10)

### Bug Fixes

- **core:** Fix executions list filtering by waiting status ([#3241](https://github.com/n8n-io/n8n/issues/3241)) ([71afcd6](https://github.com/n8n-io/n8n/commit/71afcd6314a73ab6cc04e22afd69e86ca764bd42))
- **core:** Improve webhook error messages ([49d0e3e](https://github.com/n8n-io/n8n/commit/49d0e3e885003b11092cf3c890847154426dee41))
- **Edit Image Node:** Make node work with binary-data-mode 'filesystem' ([#3274](https://github.com/n8n-io/n8n/issues/3274)) ([a4db0d0](https://github.com/n8n-io/n8n/commit/a4db0d051b18bc224c6cd69faeabf03cf5fba659))

### Features

- **Pipedrive Node:** Add support for filters to getAll:organization ([#3211](https://github.com/n8n-io/n8n/issues/3211)) ([1ef10dd](https://github.com/n8n-io/n8n/commit/1ef10dd23fef0b2e3e0ef76c8116d3bebc36bc4e))
- **Pushover Node:** Add 'HTML Formatting' option and credential test ([#3082](https://github.com/n8n-io/n8n/issues/3082)) ([b3dc6d9](https://github.com/n8n-io/n8n/commit/b3dc6d9d9c640f1e0f04cb56d0fabe2aafb948b6))
- **UProc Node:** Add new tools ([#3104](https://github.com/n8n-io/n8n/issues/3104)) ([ff2bf11](https://github.com/n8n-io/n8n/commit/ff2bf1112f07b7c3fd75f60e8faefdef4e2a02af))

## [0.175.1](https://github.com/n8n-io/n8n/compare/n8n@0.175.0...n8n@0.175.1) (2022-05-03)

### Bug Fixes

- **editor:** Fix bug with node version ([ed56481](https://github.com/n8n-io/n8n/commit/ed564812435a279760a32e76f3935f492f84f487))

# [0.175.0](https://github.com/n8n-io/n8n/compare/n8n@0.174.0...n8n@0.175.0) (2022-05-02)

### Bug Fixes

- **core:** Do not applying auth if UM is disabled ([#3218](https://github.com/n8n-io/n8n/issues/3218)) ([4ceac38](https://github.com/n8n-io/n8n/commit/4ceac38e0397be91bfc1b50d8a06ebf20de8c32e))
- **core:** Skip credential check of disabled nodes and improve error ([79ced8f](https://github.com/n8n-io/n8n/commit/79ced8f6774cc70d63369001d7c56d1d4a340261))
- **editor:** Fix bug with touchscreens ([#3206](https://github.com/n8n-io/n8n/issues/3206)) ([8d9e05e](https://github.com/n8n-io/n8n/commit/8d9e05e3c3ef61cd5a65ec00d3d1474f1195f653))
- **Hubspot Node:** Fix search operators ([#3208](https://github.com/n8n-io/n8n/issues/3208)) ([ea4a8b8](https://github.com/n8n-io/n8n/commit/ea4a8b88c9bbfde3304073070a430f2421477921))
- **Sendgrid Node:** Fix issue sending attachments ([#3213](https://github.com/n8n-io/n8n/issues/3213)) ([2b00881](https://github.com/n8n-io/n8n/commit/2b008815cad82619a66d4b30d1f79630c82be978))
- **Wise Node:** Respect time parameter on get: exchangeRate ([#3227](https://github.com/n8n-io/n8n/issues/3227)) ([c7d525a](https://github.com/n8n-io/n8n/commit/c7d525a60fda4aad653017cb90253426cce98b3b))

### Features

- **core:** Introduce simplified node versioning ([#3205](https://github.com/n8n-io/n8n/issues/3205)) ([d5b9b0c](https://github.com/n8n-io/n8n/commit/d5b9b0cb9596688b3bcad0010b65888428c297c6))
- **Google Sheets Node:** Allow to use header names as JSON path ([#3165](https://github.com/n8n-io/n8n/issues/3165)) ([770c4fe](https://github.com/n8n-io/n8n/commit/770c4fe6ebe70c7a507ee5e57348508b98fda11d))
- **Microsoft Dynamics CRM Node:** Add support for other regions than North America ([#3157](https://github.com/n8n-io/n8n/issues/3157)) ([4bdd607](https://github.com/n8n-io/n8n/commit/4bdd607fdf00f6c2155c9b3e3c9e74ac50e317f4))
- **Telegram Node:** Allow querying chat administrators ([#3226](https://github.com/n8n-io/n8n/issues/3226)) ([c02d259](https://github.com/n8n-io/n8n/commit/c02d259453f2f5b444569f4c1e06fbfc95cd3305)), closes [#3157](https://github.com/n8n-io/n8n/issues/3157)

# [0.174.0](https://github.com/n8n-io/n8n/compare/n8n@0.173.1...n8n@0.174.0) (2022-04-25)

### Bug Fixes

- **core:** Open oauth callback endpoints to be public ([#3168](https://github.com/n8n-io/n8n/issues/3168)) ([01807d6](https://github.com/n8n-io/n8n/commit/01807d613654eb14dad0eb82defa4fab234a1d71))
- **MicrosoftOneDrive Node:** Fix issue with filenames that contain special characters from uploading ([#3183](https://github.com/n8n-io/n8n/issues/3183)) ([ff26a98](https://github.com/n8n-io/n8n/commit/ff26a987fe244b30f67d6516d84f1f43fed3ec43))
- **Slack Node:** Fix credential test ([#3151](https://github.com/n8n-io/n8n/issues/3151)) ([15e6d92](https://github.com/n8n-io/n8n/commit/15e6d9274ad0627dd5ebc30e70757878368042bc))

### Features

- **All AWS Nodes:** Enable support for AWS temporary credentials ([#2587](https://github.com/n8n-io/n8n/issues/2587)) ([ce79e6b](https://github.com/n8n-io/n8n/commit/ce79e6b74f6d94694f16988c8601f7c0639a04b3))
- **editor:** Add Workflow Stickies (Notes) ([#3154](https://github.com/n8n-io/n8n/issues/3154)) ([31dd01f](https://github.com/n8n-io/n8n/commit/31dd01f9cb7e1b6908a89c3402c78515a6475e61))
- **Google Sheets Node:** Add upsert support ([#2733](https://github.com/n8n-io/n8n/issues/2733)) ([aeb5a12](https://github.com/n8n-io/n8n/commit/aeb5a1234aa610b333525512085fe3b3bd60abef))
- **Microsoft Teams Node:** Enhancements and cleanup ([#2940](https://github.com/n8n-io/n8n/issues/2940)) ([d446f9e](https://github.com/n8n-io/n8n/commit/d446f9e28176e6ae2875d526cf4b6ac769dc750c))
- **MongoDB Node:** Allow parsing dates using dot notation ([#2487](https://github.com/n8n-io/n8n/issues/2487)) ([83998a1](https://github.com/n8n-io/n8n/commit/83998a15b0b4bea94aa07984136bdc56523d4f89))

# [0.173.1](https://github.com/n8n-io/n8n/compare/n8n@0.173.0...n8n@0.173.1) (2022-04-19)

### Bug Fixes

- **Discord Node:** Fix icon name

# [0.173.0](https://github.com/n8n-io/n8n/compare/n8n@0.172.0...n8n@0.173.0) (2022-04-19)

### Bug Fixes

- **core:** Add "rawBody" also for xml requests ([#3143](https://github.com/n8n-io/n8n/issues/3143)) ([5719e44](https://github.com/n8n-io/n8n/commit/5719e44b5999bb84e2fd50c8a469cc8934539747))
- **core:** Make email for UM case insensitive ([#3078](https://github.com/n8n-io/n8n/issues/3078)) ([8532b00](https://github.com/n8n-io/n8n/commit/8532b0030dbdeb85b2f74ce078adb44f43a7c4d3))
- **Discourse Node:** Fix issue with not all posts getting returned and add credential test ([#3007](https://github.com/n8n-io/n8n/issues/3007)) ([d68b7a4](https://github.com/n8n-io/n8n/commit/d68b7a4cf4b1025ce19e23f6bfc9e423595b6c0b))
- **editor:** Fix breaking Drop-downs after removing expressions ([#3094](https://github.com/n8n-io/n8n/issues/3094)) ([17b0cd8](https://github.com/n8n-io/n8n/commit/17b0cd8f765ce262241c827a635e64c189acc0f8))
- **Postgres Node:** Fix issue with columns containing spaces ([#2989](https://github.com/n8n-io/n8n/issues/2989)) ([0081d02](https://github.com/n8n-io/n8n/commit/0081d02b979ff5d98c5a834c60d8d8b5e83924ef))
- **ui:** Reset text-edit input value when pressing esc key to have matching input values ([#3098](https://github.com/n8n-io/n8n/issues/3098)) ([29fdd77](https://github.com/n8n-io/n8n/commit/29fdd77d7b4ac3bbb9faae73b0932183d48ae9a6))
- **ZendeskTrigger Node:** Fix deprecated targets, replaced with webhooks ([#3025](https://github.com/n8n-io/n8n/issues/3025)) ([794ad7c](https://github.com/n8n-io/n8n/commit/794ad7c756c68e0459d8f105acc3bcc1347d1e59))
- **Zoho Node:** Fix pagination issue ([#3129](https://github.com/n8n-io/n8n/issues/3129)) ([47bbe98](https://github.com/n8n-io/n8n/commit/47bbe9857b5f3321c9402595041afcb6b96411c4))

### Features

- **Discord Node:** Add additional options ([#2918](https://github.com/n8n-io/n8n/issues/2918)) ([310bffe](https://github.com/n8n-io/n8n/commit/310bffe7137f6baf36b93719c1e5abe8596dd346))
- **editor:** Add drag and drop from nodes panel ([#3123](https://github.com/n8n-io/n8n/issues/3123)) ([f566569](https://github.com/n8n-io/n8n/commit/f56656929992b98a3473944fd2a395e05d5c42f0))
- **Google Cloud Realtime Database Node:** Make it possible to select region ([#3096](https://github.com/n8n-io/n8n/issues/3096)) ([176538e](https://github.com/n8n-io/n8n/commit/176538e5f21f14ea3e5964dbe905fe4af89faaef))
- **GoogleBigQuery Node:** Add support for service account authentication ([#3128](https://github.com/n8n-io/n8n/issues/3128)) ([ac5f357](https://github.com/n8n-io/n8n/commit/ac5f357001b6887d649f65bc32a30e30aa75584b))
- **Markdown Node:** Add new node to covert between Markdown <> HTML ([#1728](https://github.com/n8n-io/n8n/issues/1728)) ([5d1ddb0](https://github.com/n8n-io/n8n/commit/5d1ddb0e9b56d999ec4d9278b81262aafceb43a9))
- **PagerDuty Node:** Add support for additional details in incidents ([#3140](https://github.com/n8n-io/n8n/issues/3140)) ([6ca7454](https://github.com/n8n-io/n8n/commit/6ca74540782623ac2301550b62f3382e88b8ed83)), closes [#3094](https://github.com/n8n-io/n8n/issues/3094) [#3105](https://github.com/n8n-io/n8n/issues/3105) [#3112](https://github.com/n8n-io/n8n/issues/3112) [#3078](https://github.com/n8n-io/n8n/issues/3078) [#3133](https://github.com/n8n-io/n8n/issues/3133) [#2918](https://github.com/n8n-io/n8n/issues/2918)
- **Slack Node:** Add blocks to slack message update ([#2182](https://github.com/n8n-io/n8n/issues/2182)) ([b5b6000](https://github.com/n8n-io/n8n/commit/b5b60008d680cd843a418390d451743fc13cac9c)), closes [#1728](https://github.com/n8n-io/n8n/issues/1728)

# [0.172.0](https://github.com/n8n-io/n8n/compare/n8n@0.171.1...n8n@0.172.0) (2022-04-11)

### Bug Fixes

- **Action Network Node:** Fix pagination issue and add credential test ([#3011](https://github.com/n8n-io/n8n/issues/3011)) ([9ef339e](https://github.com/n8n-io/n8n/commit/9ef339e5257e4aa79600554c815cb32fd226753d))
- **core:** Set correct timezone in luxon ([#3115](https://github.com/n8n-io/n8n/issues/3115)) ([3763f81](https://github.com/n8n-io/n8n/commit/3763f815bd14dcc45786efb9b97bb85695bbf734))
- **editor:** Fix i18n issues ([#3072](https://github.com/n8n-io/n8n/issues/3072)) ([4ae0f5b](https://github.com/n8n-io/n8n/commit/4ae0f5b6fba65bfa8f236657d89358f53e465c69)), closes [#3097](https://github.com/n8n-io/n8n/issues/3097)

### Features

- **editor:** Refactor Node Output Panel [PR#3097](https://github.com/PR/issues/3097)
- **Magento 2 Node:** Add credential tests ([#3086](https://github.com/n8n-io/n8n/issues/3086)) ([a11b00a](https://github.com/n8n-io/n8n/commit/a11b00a0374359f0ba8fe91a1df402f32de61b15))
- **PayPal Node:** Add auth test, fix typo and update API URL ([#3084](https://github.com/n8n-io/n8n/issues/3084)) ([c7a037e](https://github.com/n8n-io/n8n/commit/c7a037e9feed94b641e6aab92301c8a647a2934c)), closes [PR#2568](https://github.com/PR/issues/2568)

## [0.171.1](https://github.com/n8n-io/n8n/compare/n8n@0.171.0...n8n@0.171.1) (2022-04-06)

### Bug Fixes

- **core:** Fix issue with current executions not getting displayed ([#3093](https://github.com/n8n-io/n8n/issues/3093)) ([4af5168](https://github.com/n8n-io/n8n/commit/4af5168b3bc92578dc807bab1c11e3d90e151928))
- **core:** Fix issue with falsely skip authorizing ([#3087](https://github.com/n8n-io/n8n/issues/3087)) ([358a683](https://github.com/n8n-io/n8n/commit/358a683f381aa8eb7edd4886d6bdfe7ada61ec35))
- **WooCommerce Node:** Fix pagination issue with "Get All" operation ([#2529](https://github.com/n8n-io/n8n/issues/2529)) ([c2a5e0d](https://github.com/n8n-io/n8n/commit/c2a5e0d1b6a89cb7397b93bbb0f0be9be0df9c86))

# [0.171.0](https://github.com/n8n-io/n8n/compare/n8n@0.170.0...n8n@0.171.0) (2022-04-03)

### Bug Fixes

- **core:** Fix crash on webhook when last node did not return data ([c50d04a](https://github.com/n8n-io/n8n/commit/c50d04af9eb033d82860c336fc7350b5c3f22242))
- **EmailReadImap Node:** Fix issue that crashed process if node was configured wrong ([#3079](https://github.com/n8n-io/n8n/issues/3079)) ([85f15d4](https://github.com/n8n-io/n8n/commit/85f15d49896d876fa3ab84e9fa1846f856851274))
- **Google Tasks Node:** Fix "Show Completed" option and hide title field where not needed ([#2741](https://github.com/n8n-io/n8n/issues/2741)) ([9d703e3](https://github.com/n8n-io/n8n/commit/9d703e366b8e191e0f588469892ebb7b6d03c1d3))
- **NocoDB Node:** Fix pagination ([#3081](https://github.com/n8n-io/n8n/issues/3081)) ([5f44b0d](https://github.com/n8n-io/n8n/commit/5f44b0dad5254fe9f985b314db8f7d43ab48c712))
- **Salesforce Node:** Fix issue that "status" did not get used for Case => Create & Update ([#2212](https://github.com/n8n-io/n8n/issues/2212)) ([1018146](https://github.com/n8n-io/n8n/commit/1018146f21c47eda9f888bd19e92d1106c49267a))

### Features

- **editor:** Add download button for binary data ([#2992](https://github.com/n8n-io/n8n/issues/2992)) ([13a9db7](https://github.com/n8n-io/n8n/commit/13a9db774576a00d4e3ce1988557654d00067073))
- **Emelia Node:** Add Campaign > Duplicate functionality ([#3000](https://github.com/n8n-io/n8n/issues/3000)) ([0b08be1](https://github.com/n8n-io/n8n/commit/0b08be1c0b2961f235fc2446a36afe3995b4d847)), closes [#3065](https://github.com/n8n-io/n8n/issues/3065) [#2741](https://github.com/n8n-io/n8n/issues/2741) [#3075](https://github.com/n8n-io/n8n/issues/3075)
- **FTP Node:** Add option to recursively create directories on rename ([#3001](https://github.com/n8n-io/n8n/issues/3001)) ([39a6f41](https://github.com/n8n-io/n8n/commit/39a6f417203b76cfa2c68816c49e86dc7236aba4))
- **Mautic Node:** Add credential test and allow trailing slash in host ([#3080](https://github.com/n8n-io/n8n/issues/3080)) ([0a75539](https://github.com/n8n-io/n8n/commit/0a75539cc3d696a8946d7db5ff5842ff54835134))
- **Microsoft Teams Node:** Add chat message support ([#2635](https://github.com/n8n-io/n8n/issues/2635)) ([984f62d](https://github.com/n8n-io/n8n/commit/984f62df9ed92cdf297b3b56300c9f23bf128d2d))
- **Mocean Node:** Add "Delivery Report URL" option and credential tests ([#3075](https://github.com/n8n-io/n8n/issues/3075)) ([c89d2b1](https://github.com/n8n-io/n8n/commit/c89d2b10f2461ff8e90209b8f29c222f9430dba5))
- **ServiceNow Node:** Add basicAuth support and fix getColumns loadOptions ([#2712](https://github.com/n8n-io/n8n/issues/2712)) ([2c72584](https://github.com/n8n-io/n8n/commit/2c72584b55521b437baa20ddad7c919807fd9f8f)), closes [#2741](https://github.com/n8n-io/n8n/issues/2741) [#3075](https://github.com/n8n-io/n8n/issues/3075) [#3000](https://github.com/n8n-io/n8n/issues/3000) [#3065](https://github.com/n8n-io/n8n/issues/3065) [#2741](https://github.com/n8n-io/n8n/issues/2741) [#3075](https://github.com/n8n-io/n8n/issues/3075) [#3071](https://github.com/n8n-io/n8n/issues/3071) [#3001](https://github.com/n8n-io/n8n/issues/3001) [#2635](https://github.com/n8n-io/n8n/issues/2635) [#3080](https://github.com/n8n-io/n8n/issues/3080) [#3061](https://github.com/n8n-io/n8n/issues/3061) [#3081](https://github.com/n8n-io/n8n/issues/3081) [#2582](https://github.com/n8n-io/n8n/issues/2582) [#2212](https://github.com/n8n-io/n8n/issues/2212)
- **Strava Node:** Add "Get Streams" operation ([#2582](https://github.com/n8n-io/n8n/issues/2582)) ([6bbb4df](https://github.com/n8n-io/n8n/commit/6bbb4df05925362404f844a23a695f186d27b72e))

# [0.170.0](https://github.com/n8n-io/n8n/compare/n8n@0.169.0...n8n@0.170.0) (2022-03-27)

### Bug Fixes

- **core:** Add logs and error catches for possible failures in queue mode ([#3032](https://github.com/n8n-io/n8n/issues/3032)) ([3b4a97d](https://github.com/n8n-io/n8n/commit/3b4a97dd576bd3c2f53f958266964d3e02f01c96))
- **AWS Lambda Node:** Fix "Invocation Type" > "Continue Workflow" ([#3010](https://github.com/n8n-io/n8n/issues/3010)) ([9547a08](https://github.com/n8n-io/n8n/commit/9547a08f0344825e42f5580da035bb1f21c03368))
- **Supabase Node:** Fix Row > Get operation ([#3045](https://github.com/n8n-io/n8n/issues/3045)) ([b9aa440](https://github.com/n8n-io/n8n/commit/b9aa440be3d52bf412990b93cfc3758353fb4943))
- **Supabase Node:** Send token also via Authorization Bearer ([#2814](https://github.com/n8n-io/n8n/issues/2814)) ([5774dd8](https://github.com/n8n-io/n8n/commit/5774dd8885a87a1ebe70f4ef4a06a42013112afe))
- **Xero Node:** Fix some operations and add support for setting address and phone number ([#3048](https://github.com/n8n-io/n8n/issues/3048)) ([ab08c0d](https://github.com/n8n-io/n8n/commit/ab08c0df1599d44326b45c37f80918e5c107cc6a))
- **Wise Node:** Fix issue when executing a transfer ([#3039](https://github.com/n8n-io/n8n/issues/3039)) ([b90bf45](https://github.com/n8n-io/n8n/commit/b90bf4576c6e3f86000d61606f412ea0544b59ef))

### Features

- **Crypto Node:** Add Generate operation to generate random values ([#2541](https://github.com/n8n-io/n8n/issues/2541)) ([b5ecccb](https://github.com/n8n-io/n8n/commit/b5ecccb84080362880a307e3f9d76d429bd1d537))
- **HTTP Request Node:** Add support for OPTIONS method ([#3030](https://github.com/n8n-io/n8n/issues/3030)) ([bd9064c](https://github.com/n8n-io/n8n/commit/bd9064cd0ea8833b49a7e3860f12bfa37c286947))
- **Jira Node:** Add Simplify Output option to Issue > Get ([#2408](https://github.com/n8n-io/n8n/issues/2408)) ([016aeaa](https://github.com/n8n-io/n8n/commit/016aeaaa791205c5ee3d16eef25f856603cf0085))
- **Reddit Node:** Add possibility to query saved posts ([#3034](https://github.com/n8n-io/n8n/issues/3034)) ([5ba4c27](https://github.com/n8n-io/n8n/commit/5ba4c27d8c417964187af89a15d5dd4ce9f3271a))
- **Zendesk Node:** Add ticket status "On-hold" ([2b20a46](https://github.com/n8n-io/n8n/commit/2b20a460915655791647d62b48dde97dad3b2fd3))

# [0.169.0](https://github.com/n8n-io/n8n/compare/n8n@0.168.2...n8n@0.169.0) (2022-03-20)

### License change

From [Apache 2.0 with Commons Clause](https://github.com/n8n-io/n8n/blob/181ba3c4e236279b65d102a8a33ae6896f160487/LICENSE.md) to [Sustainable Use License](https://github.com/n8n-io/n8n/blob/master/LICENSE.md)

### Bug Fixes

- **GitHub Node:** Fix credential tests and File > List operation ([#2999](https://github.com/n8n-io/n8n/issues/2999)) ([ec618e2](https://github.com/n8n-io/n8n/commit/ec618e25bba5e36592ff37e7c560d738387c9112))
- **Telegram Node:** Fix sending binary data when disable notification is set ([#2990](https://github.com/n8n-io/n8n/issues/2990)) ([26a7c61](https://github.com/n8n-io/n8n/commit/26a7c61175c1aadc101e055067224aa0797db5c5))

### Features

- Add support for reading ids from file with executeBatch command ([#3008](https://github.com/n8n-io/n8n/issues/3008)) ([5658593](https://github.com/n8n-io/n8n/commit/5658593df4cde8615f3a8383f1045d8659fffb04))
- **HTTP Request Node:** Allow Delete requests with body ([#2900](https://github.com/n8n-io/n8n/issues/2900)) ([8a88f94](https://github.com/n8n-io/n8n/commit/8a88f948f2bb6ab780a58cd284c0f6d4f499f9c6))
- **KoBoToolbox Node:** Add KoBoToolbox Regular and Trigger Node ([#2765](https://github.com/n8n-io/n8n/issues/2765)) ([1a7f0a4](https://github.com/n8n-io/n8n/commit/1a7f0a42465574f46f00e4d9d50cf71d947dc2bc)), closes [#2510](https://github.com/n8n-io/n8n/issues/2510)
- **Linear Node:** Add Linear Node ([#2971](https://github.com/n8n-io/n8n/issues/2971)) ([8d04474](https://github.com/n8n-io/n8n/commit/8d04474e30dc9109ad84fc945cc734483d0d067b))
- **Mailjet Node:** Add credential tests and support for sandbox, JSON parameters & variables ([#2987](https://github.com/n8n-io/n8n/issues/2987)) ([d2756de](https://github.com/n8n-io/n8n/commit/d2756de090f2628f9025ba2f4436870e67576367))
- **Mattermost Node:** Add support for Channel Search ([#2687](https://github.com/n8n-io/n8n/issues/2687)) ([1b993e4](https://github.com/n8n-io/n8n/commit/1b993e402297ac400c5167d1bcfa78e9a73c07df))

## [0.168.2](https://github.com/n8n-io/n8n/compare/n8n@0.168.1...n8n@0.168.2) (2022-03-16)

### Bug Fixes

- Fix issue with n8n not authenticating oauth requests ([#2998](https://github.com/n8n-io/n8n/issues/2998))

## [0.168.1](https://github.com/n8n-io/n8n/compare/n8n@0.168.0...n8n@0.168.1) (2022-03-15)

### Bug Fixes

- Add missing email templates

# [0.168.0](https://github.com/n8n-io/n8n/compare/n8n@0.167.0...n8n@0.168.0) (2022-03-14)

### Features

- Add User Management ([#2636](https://github.com/n8n-io/n8n/issues/2636)) ([7264239](https://github.com/n8n-io/n8n/commit/7264239b839b8e92b7ea667ec70e5c3edb578277))

# 0.167.0 (2022-03-13)

### Bug Fixes

- Fix issue with long credential type names ([#2961](https://github.com/n8n-io/n8n/issues/2961)) ([535dfe0](https://github.com/n8n-io/n8n/commit/535dfe08384fdd0a4ea86521e917b28f7091ff82))
- Fix workflow deactivating bug ([195f104](https://github.com/n8n-io/n8n/commit/195f104ef51b722fd5e3756ed3d0cc47ef523362))
- **GoogleCalendar Node:** Fix timezone ([3c5df3f](https://github.com/n8n-io/n8n/commit/3c5df3f892d89e1ae79dfcc0cd5b1886d1f623db))
- **SeaTableTrigger Node:** Fix timezone issues ([#2726](https://github.com/n8n-io/n8n/issues/2726)) ([2d8ac4b](https://github.com/n8n-io/n8n/commit/2d8ac4b477f8fb381a35eba34710084d5e4d3402))
- **Strapi Node:** Add support for Strapi v4 ([2a3cbf3](https://github.com/n8n-io/n8n/commit/2a3cbf3fc85f64e9b4b5814f1206249261743021))

### Features

- Add new expression variables and support for luxon ([e8500e6](https://github.com/n8n-io/n8n/commit/e8500e69371ad4b205d1586c7837120267595c70))
- **Facebook Node:** Add support for Facebook Graph API versions 13 ([53b5444](https://github.com/n8n-io/n8n/commit/53b54440d7532f439c3533676758b6c83136d48c))
- **Hubspot:** Add support for Private App Token Authentication ([f73100a](https://github.com/n8n-io/n8n/commit/f73100a0bdebd05b25517532358c71feed040eeb))
- **If Node,Switch Node:** Add negative operations ([6412546](https://github.com/n8n-io/n8n/commit/6412546c0c5465b17ab2a289f45d8c8fa325eb68))
- **MongoDb Node:** Add Aggregate Operation ([2c9a06e](https://github.com/n8n-io/n8n/commit/2c9a06e86346a9e21f877cb508d13a1401c700a9))
- **Redis Node:** Add Redis Trigger node and publish operation to regular node ([5c2deb4](https://github.com/n8n-io/n8n/commit/5c2deb468867ec77a05d09ef324d4855210e17d4))
- **Wordpress Node:** Add Status option to Get All operation of Posts resource ([4d4db7f](https://github.com/n8n-io/n8n/commit/4d4db7f805673758dfb379c9e86e98815f265db2))

> **Note:** for changelogs before 0.167.0, refer to the [Release notes](https://docs.n8n.io/reference/release-notes.html) in the documentation.
