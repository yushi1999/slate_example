--- 

title: Qwi API 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

This is a sample server server server. 

**Version:** 1.0 

# /REGISTERVERIFICATIONID
## ***POST*** 

**Summary:** VerificationIDを生成する

### HTTP Request 
`***POST*** /registerVerificationID` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| organizationID | formData | organizationID | Yes | string |
| email | formData | verificationID生成対象アカウントのemailアドレス | Yes | string |
| otp | formData | アプリに表示されたワンタイムパスワード | Yes | integer |
| apiKey | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | 処理が正常終了 |
| 400 | 失敗 |

# /GETVERIFICATIONSTATUS
## ***GET*** 

### HTTP Request 
`***GET*** /getVerificationStatus` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| organizationID | formData | organizationID | Yes | string |
| apiKey | header |  | Yes | string |
| verificationID | formData |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
