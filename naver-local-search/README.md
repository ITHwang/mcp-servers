# Naver Local Search

## Overview

- You can call the [Naver Local Search API](https://developers.naver.com/docs/serviceapi/search/local/local.md) with MCP.
- [네이버 지역 검색 API](https://developers.naver.com/docs/serviceapi/search/local/local.md)를 MCP로 호출할 수 있습니다.

## Usage

### 1. Build the package and run the MCP server

```bash
cd naver-local-search
uv build
uv tool install ./dist/naver_local_search-0.1.0-py3-none-any.whl
uvx naver-local-search
```

### 2. Run the package

```json
{
  "mcpServers": {
    "naver-local-search": {
      "command": "uvx",
      "args": ["naver-local-search"],
      "env": {
        "X-NAVER-CLIENT-ID": "...",
        "X-NAVER-CLIENT-SECRET": "..."
      }
    }
  }
}
```
