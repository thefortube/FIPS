

# FIPs 

ForTube Improvement Proposals (FIPs) describe standards for the ForTube platform, including core protocol specifications, client APIs, and contract standards.

## Contributing

 1. Review [YIP-0](YIPS/yip-0.md).
 2. Fork the repository by clicking "Fork" in the top right.
  4. Add your YIP to your fork of the repository. There is a [template YIP here](yip-X.md).
  5. Submit a Pull Request to yEarn's [YIPs repository](https://github.com/iearn-finance/YIPS/).

```bash
git clone https://github.com/yourname/FIPS.git
```

```bash
cd FIPS
git checkout -b xxx-fip (your branch name)

cd FIPS
add your fip-xxx.md here

git add .
git commit -m "(your commit message)"

git push origin xxx-fip
```

Then go to your "FIPS" repository, click the "Pull request" button below the "Code" button.The link should be "https://github.com/xxx/FIPS/pull/new/master".And choose correct repository and branch name on right.

Your first PR should be a first draft of the final YIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new YIP and assign it a number before merging it. Make sure you include a `discussions-to` header with the URL to a new thread on [gov.yearn.finance](https://gov.yearn.finance/) where people can discuss the YIP as a whole.

If your YIP requires images, the image files should be included in a subdirectory of the `assets` folder for that YIP as follow: `assets/yip-X` (for yip **X**). When linking to an image in the YIP, use relative links such as `../assets/yip-X/image.png`.

When you believe your YIP is mature and ready to progress past the WIP phase, you should ask to have your issue added to the next governance call where it can be discussed for inclusion in a future platform upgrade. If the community agrees to include it, the YIP editors will update the state of your YIP to 'Approved'.

## YIP Statuses

* **WIP** - a YIP that is still being developed.
* **Proposed** - a YIP that is ready to be reviewed in a governance call.
* **Approved** - a YIP that has been accepted for implementation by the yEarn community.
* **Implemented** - a YIP that has been released to mainnet.
* **Rejected** - a YIP that has been rejected.
* **Withdrawn** - a YIP that has been withdrawn by the author(s).
* **Deferred** - a YIP that is pending another YIP/some other change that should be bundled with it together.
* **Moribund** - a YIP that was implemented but is now obsolete and requires no explicit replacement.

## Validation

YIPs must pass some validation tests.  The YIP repository ensures this by running tests using [html-proofer](https://rubygems.org/gems/html-proofer) and [yip_validator](https://rubygems.org/gems/yip_validator).

It is possible to run the YIP validator locally:
```
gem install yip_validator
yip_validator <INPUT_FILES>
```

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
