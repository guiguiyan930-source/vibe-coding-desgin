# RESTful API 设计规范

## 响应格式

```json
{
  "success": true,
  "data": {},
  "message": "操作成功"
}
```

## 错误响应

```json
{
  "success": false,
  "message": "错误描述",
  "error": "详细错误信息（开发环境）"
}
```

## HTTP 状态码

| 状态码 | 含义 |
|--------|------|
| 200 | 请求成功 |
| 201 | 创建成功 |
| 400 | 请求参数错误 |
| 404 | 资源不存在 |
| 500 | 服务器内部错误 |

## 路由命名规范

```
GET    /api/resources       # 获取列表
GET    /api/resources/:id   # 获取详情
POST   /api/resources       # 创建资源
PUT    /api/resources/:id   # 更新资源
DELETE /api/resources/:id   # 删除资源
```
