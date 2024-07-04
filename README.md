# mcskindl

mcskindl is a Minecraft: Java Edition player skin downloader in bash(1)

**NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**

## Requirements

- bash (tested with 5.2.x, POSIX shell version might be available later)
- curl for fetching (if HTTPS works then it should work). Set environment variable `MCSKINDL_USE_WGET` to `yes` if you prefer using wget
- jq for processing JSON data (important)
- base64 for decoding Base64 data (should be included with coreutils or busybox any other implementations that supports decoding)
- sed (for substituting some HTTP URLs to HTTPS, remove any calls of sed if you don't want this behavior.

> [!WARNING]
> THE CGI Script mode is NOT intended for production use due to performance and security issues.

## TODO

- Detect if the input is a valid UUID otherwise it is a Username.

## Credits

Thanks to [this wiki.vg page](https://wiki.vg/Mojang_API) for providing documentations, https://github.com/koalaman/shellcheck for helping me to catch potential bugs, and also https://github.com/matejak/argbash/ for generating the code to handle command line arguments!
