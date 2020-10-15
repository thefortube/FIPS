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
