## 介绍

**对 [chenshuai2144 / openapi2typescript]([asd](https://github.com/chenshuai2144/openapi2typescript)) 的修改**  
  
原库在生成接口方法时会根据 `operationId` 生成 Params 接口名，在 Swagger 文档内没有填写 `operationId` 时，会导致所有方法的 `operationId` 被错误地生成为 `undefinedParams`。  
本库由于项目需求，在原库的基础上修正了这个错误，在没有填写 `operationId` 时，会根据请求路径和HTTP方法生成 Params 接口名。  
  
随项目进展可能会有后续修改。  

## 使用

```
npm i --save-dev wnikoopenapi2typescript
```

使用方法同 [chenshuai2144 / openapi2typescript]([asd](https://github.com/chenshuai2144/openapi2typescript))  