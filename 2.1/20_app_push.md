#融资申请推送
## 描述

## API代码
loan\_app:app:push


## 请求参数
| 名称 | 类型 | 是否必须 | 描述 | 示例值 |
| --- | --- | --- | --- | --- |
| app_id | String | 是 | 申请ID（[融资申请创建API](20_app_push.md)返回的结果） | 0092728480d24f5d87bf63639b5cfe1c |
| mt_app_type_cd | String | 是 | 申请类型: CP_PUSH_APP-企业融资申请；CS_PUSH_APP-个人融资申请 | CP_PUSH_APP |

## 响应参数
| 名称 | 类型 | 描述 |示例值 |
| --- | --- | --- | --- |
| app_id | String | 申请ID | 0092728480d24f5d87bf63639b5cfe1c |
| mt_app_sts_cd | String | 申请状态代码，详细规则见[附件](2.1.2_申请状态查询.html) | APPROVED |

## 错误码
| 描述 | HTTP状态码 | 语义 |
| --- | --- | --- | 
| app_id未找到 | 400 | 请输入正确的app_id,或检查申请类型与申请ID是否匹配 |

## 示例
### 请求示例
```javascript
{
    "app_id":"0092728480d24f5d87bf63639b5cfe1c",
    "mt_app_type_cd":"CP_PUSH_APP"
}
```
### 返回示例
```javascript
{
    "app_id":"0092728480d24f5d87bf63639b5cfe1c",
    "mt_app_sts_cd":"APPROVED"
}
```
## FAQ
关于此文档暂时还没有FAQ