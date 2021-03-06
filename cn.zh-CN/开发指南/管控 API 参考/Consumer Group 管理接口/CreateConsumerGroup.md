# CreateConsumerGroup {#doc_api_alikafka_CreateConsumerGroup .reference}

调用 CreateConsumerGroup 创建 Consumer Group。

您在调用 CreateConsumerGroup 创建 Consumer Group 时，请注意：单用户请求频率限制为 1 QPS。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=alikafka&api=CreateConsumerGroup&type=RPC&version=2018-10-15)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateConsumerGroup|要执行的动作。取值：**CreateConsumerGroup**

 |
|ConsumerId|String|是|consumer\_group\_test|Consumer Group 名称。

 -   只能包含字母、数字、短横线（-）、下划线（\_）。
-   长度限制在 **3-64** 个字符，多于 **64** 个字符将被自动截取。
-   一旦创建后不能再修改。

 |
|InstanceId|String|是|alikafka\_pre-cn-0pp1954n\*\*\*\*|实例 ID。可调用 [GetInstanceList](https://help.aliyun.com/document_detail/94533.html?spm=a2c4g.11186623.2.11.6efb754byCLl4z#concept-94533-zh) 获取。

 |
|RegionId|String|是|cn-hangzhou|地域 ID。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|Code|Integer|200|返回码。返回 **200** 为成功。

 |
|Message|String|operation success|返回信息。

 |
|RequestId|String|B191CC4D-B067-4508-987A-ACDA8D89\*\*\*\*|请求 ID。

 |
|Success|Boolean|true|调用是否成功。

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateConsumerGroup
&ConsumerId=consumer_group_test
&InstanceId=alikafka_pre-cn-0pp1954n****
&RegionId=cn-hangzhou
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateConsumerGroupResponse>
      <Message>operation success</Message>
      <RequestId>B191CC4D-B067-4508-987A-ACDA8D89****</RequestId>
      <Success>true</Success>
      <Code>200</Code>
</CreateConsumerGroupResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Message":"operation success",
	"RequestId":"B191CC4D-B067-4508-987A-ACDA8D89****",
	"Success":true,
	"Code":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/alikafka)查看更多错误码。

