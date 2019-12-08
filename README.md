# React Code Generator

<div align="center">
<a href="https://www.npmjs.com/package/@samnoh/react-gen"><img src="https://img.shields.io/npm/v/%40samnoh%2Freact-gen"></a> <a href="https://github.com/samnoh/react-code-generator/blob/master/LICENSE"><img src="https://img.shields.io/npm/l/%40samnoh%2Freact-gen"></a>
</div>

## Install

```bash
npm install -g @samnoh/react-gen
```

## Usage

-   Create a class-based 'Button' component in the '/src' directory

```bash
reactgen -o /src -n Button -c
```

-   Create a functional 'AuthTemplate' typescript component in the default directory

```bash
reactgen -n AuthTemplate -t
```

## Config

-   You can set default values in `package.json`

```json
"config": {
    "reactgen": {
        "defaultName": "Component",
        "baseDir": "/src/components",
        "modules": {
            "styled": "styled-components",
            "{ Link }": "react-router-dom"
        },
        "typescript": false,
        "classBased": false
    }
}
```
