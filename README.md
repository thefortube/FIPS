# FIPs

ForTube Improvement Proposals (FIPs) describe standards for the ForTube platform, including core protocol specifications, client APIs, and contract standards.

## Contributing

 1. Review [FIP-0](FIPS/fip-0.md).
 2. Fork the repository by clicking "Fork" button. Here is [a description](template/git-cmd.md).
 3. Add your FIP to your fork of the repository. There is a [template FIP here](template/fip-X.md).
 4. Submit a Pull Request to ForTube's [FIPs repository](https://github.com/thefortube/FIPS/).

Your first PR should be a first draft of the final FIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new FIP and assign it a number before merging it. Make sure you include a `discussions-to` header with the URL to a new thread on [forum.for.tube](https://forum.for.tube/) where people can discuss the FIP as a whole.

If your FIP requires images, the image files should be included in a subdirectory of the `assets` folder for that FIP as follow: `assets/fip-X` (for fip **X**). When linking to an image in the FIP, use relative links such as `../assets/fip-X/image.png`.

When you believe your FIP is mature and ready to progress past the WIP phase, you should ask to have your issue added to the next governance call where it can be discussed for inclusion in a future platform upgrade. If the community agrees to include it, the FIP editors will update the state of your FIP to 'Approved'.

## FIP Statuses

* **Work in progress (WIP)** - a FIP that is still being developed.
* **Proposed** - a FIP that is ready to be reviewed in a governance call.
* **Approved** - a FIP that has been accepted for implementation by the ForTube community.
* **Implemented** - a FIP that has been released to mainnet.
* **Rejected** - a FIP that has been rejected.

## Validation

FIPs must pass some validation tests.  The FIP repository ensures this by running tests using [html-proofer](https://rubygems.org/gems/html-proofer) and [ips_validator](https://rubygems.org/gems/ips_validator).

It is possible to run the FIP validator locally:
```
gem install ips_validator
ips_validator fip <INPUT_FILES>
```

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).


# FIPs

ForTube改进提案（FIP）描述了ForTube平台的标准，包括核心协议规范，客户端API和合约标准。

## 步骤

 1. 查看[FIP-0](https://github.com/ForTube-Protocol/FIPs/blob/master/FIPS/fip-0.md)。
 2. 单击“Fork”按钮Fork存储库。查看[说明](https://github.com/ForTube-Protocol/FIPs/blob/master/template/git-cmd.md)。
 3. 将你的FIP添加到Fork的存储库中。查看此处[FIP模板](https://github.com/ForTube-Protocol/FIPs/blob/master/template/fip-X.md)。
 4. 提交一个Pull Request到ForTube的FIPs[存储库](https://github.com/ForTube-Protocol/FIPs/)。


你的第一个提案，应该是最终FIP的草案。 它必须满足所需的格式设置标准（主要是报头中的正确元数据） 。编辑者将手动查看新FIP的第一个提案，并在合并前为其分配一个编号。 确保你在[forum.for.tube](https://forum.for.tube/)上新帖子的URL中包含一个`discussions-to` 的报头，以便社区用户讨论FIP。

如果你的FIP包含图片，则图片文件应包含在该FIP的`assets` 文件夹的子目录中，如下所示： `assets/fip-X` (for fip **X**)。 链接到FIP中的图像时，请使用相对链接，例如 `../assets/fip-X/image.png`。

当你认为自己的FIP已经成熟, 并且准备好通过WIP阶段时，您需要发起请求,将您的问题添加到下一个治理会议中，以便在讨论将来的平台升级时，将此问题纳入讨论。 如果社区同意，则FIP编辑会将你的FIP状态更新为“已批准”。


## FIP 状态

* **进行中 (WIP)** -仍然处于推进过程中的FIPs。
* **已提交** - 已准备好在治理会议中进行审核的FIPs。
* **已批准** - 已被ForTube社区接受用于实施的FIPs。
* **已实施** - 已发布到主网的FIPs。
* **已驳回** - 已被拒绝的FIPs。


## 验证

FIP必须通过一些验证测试。 FIP 存储库确保通过使用 [html-proofer](https://rubygems.org/gems/html-proofer) 和[ips_validator](https://rubygems.org/gems/ips_validator) 来运行测试。

也可以在本地环境运行FIP验证器：
```
gem install ips_validator
ips_validator fip <INPUT_FILES>
```

## 版权

通过[CC0](https://creativecommons.org/publicdomain/zero/1.0/)放弃版权和相关权利。



