# zed-sql

☢️ **Doesn't work yet!** At least not for me locally.

**Dev**

Trying it out locally in Zed:
```bash
ln -s path/to/zed-sql ~/Library/Application\ Support/Zed/extensions/installed/zed-sql
```
Then run `zed: reload extensions`.

## Generating WASM for local testing

```bash
git clone git@github.com:DerekStride/tree-sitter-sql.git ../tree-sitter-sql
cd ../tree-sitter-sql
git checkout --track origin/gh-pages
tree-sitter-cli build-wasm .
mv tree-sitter-sql.wasm ../zed-sql/grammars/sql.wasm
```
