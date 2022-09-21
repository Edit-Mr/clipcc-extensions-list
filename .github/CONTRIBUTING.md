# 如何贡献您的扩展

很高兴您能为 ClipCC 扩展做出贡献。在您开始之前，请确保您已经阅读了 [ClipCC 扩展开发文档](https://doc.codingclip.com/category/for-developers)。这将指导您如何创建一个扩展。

## 扩展要求

如您所见，ClipCC 扩展 API 具有极高的自由度，但是上架到扩展商店的扩展需要对这些功能进行限制来保证用户设备的安全性。

- 扩展必须是开源的，这便于我们和用户进行源代码审查。
- 扩展不得在未明示的情况下访问用户数据。
- 扩展不得包含其他恶意代码。

您也可以向 ClipCC 的社区版编辑器提交扩展，这些扩展需要遵守以下的额外要求：

- 扩展不得请求未经 ClipCC 和第三方许可的 API。
- 扩展不得包含任何影响用户体验的功能（如破坏 DOM 等）。

## 提交扩展

您可以通过在本仓库开启 Pull Request 来提交您的扩展。

1. 您需要在 `README.md`文件中添加一行，包括您的扩展的 ID、扩展名称、作者名称、仓库链接。其中，扩展 ID 必须与您的扩展的 `info.json` 文件中的 `id` 字段相同。作者名称和扩展名称可以不同，您设置的作者和扩展名称会在扩展商店展示。

2. 您需要使用 submodules 将您的仓库链接引入到本仓库。您可以使用 `git submodule add <your-repo-url>` 来添加子模块。

3. 开启一个 Pull Request，填写相关信息，等待我们的审核。

## 扩展审核

我们会在收到您的 Pull Request 后进行审核。我们会检查您的扩展是否符合要求，如果符合要求，我们会将您的扩展合并到本仓库中。

对于所有合并进本仓库的扩展，艺术团队**可能**会为您的扩展提供美观的图标，请注意查收您仓库的 PR。这也许会在您的扩展被合并后的一段时间内进行。

## 扩展更新

如果您的扩展有更新，您可以通过开启一个 Issue 来告诉我们更新您的扩展。

## 建议

我们建议您的扩展：

- 仓库名称格式为 `clipcc-extension-*`
- 仓库中包含一个 `README.md` 文件，其中包含扩展的介绍、使用方法、截图等信息。
- 仓库中包含一个 `LICENSE` 文件，其中包含扩展的开源协议。
- 提供简洁恰当的扩展名称和扩展介绍。

感谢您为 ClipCC 做出的贡献！