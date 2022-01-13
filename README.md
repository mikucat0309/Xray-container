# Xray-core Container Image

## Supported architectures

- `386`
- `amd64`
- `arm/v5`
- `arm/v6`
- `arm/v7`
- `arm64/v8`
- `ppc64`
- `ppc64le`
- `mips`
- `mipsle`
- `mips64`
- `mips64le`
- `riscv64`
- `s390x`

## Usage

Expose port 443 by default.

### Mount

- `/config.json` : Xray config  
    [example](https://github.com/XTLS/Xray-examples)  
    [reference](https://xtls.github.io/config/) (Chinese)  
    [v2ray reference](https://www.v2fly.org/en_US/config/overview.html) (Chinese & English)  

### Environment variables

None  

## Build

### Requirements

- buildah
- qemu-user-static

### Default

```bash
make
```

### Specific architecture

```bash
make arm/v7
```

### Specific version

```bash
make version=1.5.2
```

