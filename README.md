# mcskindl

mcskindl is a Minecraft: Java Edition player skin downloader written in `bash`.

## Requirements

- bash (tested with 5.2.x)
- curl for fetching (if HTTPS works then it should work). Set the `MCSKINDL_USE_WGET` environment variable to `yes` if you prefer using wget
- jq for processing JSON data (core)
- base64 for decoding Base64 data (should be included with coreutils or busybox or any other implementations that supports it)
- sed (for substituting some HTTP URLs to HTTPS, remove any calls of sed if you don't want this behavior.

> [!WARNING]
> The CGI script mode is NOT intended for production use due to performance and security issues.

## TODO

- Detect if the input is a valid UUID otherwise it is a Username.

## Credits

- <https://minecraft.wiki/w/Mojang_API>: Documentation
- [shellcheck](https://github.com/koalaman/shellcheck)
- <https://github.com/matejak/argbash>

---

**NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**
