# <a name="get-message"></a><span data-ttu-id="1f170-101">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="1f170-101">Get message</span></span>

<span data-ttu-id="1f170-102">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="1f170-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="1f170-103">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="1f170-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="1f170-104">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="1f170-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f170-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f170-105">Prerequisites</span></span>
<span data-ttu-id="1f170-106">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="1f170-106">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>  
## <a name="http-request"></a><span data-ttu-id="1f170-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f170-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f170-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f170-108">Optional query parameters</span></span>
<span data-ttu-id="1f170-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f170-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1f170-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f170-110">Request headers</span></span>
| <span data-ttu-id="1f170-111">Nome</span><span class="sxs-lookup"><span data-stu-id="1f170-111">Name</span></span>       | <span data-ttu-id="1f170-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f170-112">Type</span></span> | <span data-ttu-id="1f170-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f170-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f170-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f170-114">Authorization</span></span>  | <span data-ttu-id="1f170-115">string</span><span class="sxs-lookup"><span data-stu-id="1f170-115">string</span></span>  | <span data-ttu-id="1f170-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f170-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f170-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f170-118">Request body</span></span>
<span data-ttu-id="1f170-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f170-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f170-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f170-120">Response</span></span>

<span data-ttu-id="1f170-121">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f170-121">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f170-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f170-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f170-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f170-123">Request</span></span>
<span data-ttu-id="1f170-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f170-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="1f170-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f170-125">Response</span></span>
<span data-ttu-id="1f170-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f170-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="1f170-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="1f170-129">See also</span></span>

- [<span data-ttu-id="1f170-130">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1f170-130">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="1f170-131">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1f170-131">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
