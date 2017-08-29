# <a name="get-message"></a><span data-ttu-id="31d2c-101">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="31d2c-101">Get message</span></span>

<span data-ttu-id="31d2c-102">Recupere as propriedades e os relacionamentos de um objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="31d2c-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="31d2c-103">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="31d2c-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="31d2c-104">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="31d2c-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="31d2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="31d2c-105">Permissions</span></span>
<span data-ttu-id="31d2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31d2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31d2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31d2c-108">Permission type</span></span>      | <span data-ttu-id="31d2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31d2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31d2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31d2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31d2c-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31d2c-111">Mail.Read</span></span>    |
|<span data-ttu-id="31d2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31d2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31d2c-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31d2c-113">Mail.Read</span></span>    |
|<span data-ttu-id="31d2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31d2c-114">Application</span></span> | <span data-ttu-id="31d2c-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31d2c-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="31d2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31d2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31d2c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="31d2c-117">Optional query parameters</span></span>
<span data-ttu-id="31d2c-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="31d2c-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="31d2c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31d2c-119">Request headers</span></span>
| <span data-ttu-id="31d2c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="31d2c-120">Name</span></span>       | <span data-ttu-id="31d2c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="31d2c-121">Type</span></span> | <span data-ttu-id="31d2c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="31d2c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="31d2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31d2c-123">Authorization</span></span>  | <span data-ttu-id="31d2c-124">string</span><span class="sxs-lookup"><span data-stu-id="31d2c-124">string</span></span>  | <span data-ttu-id="31d2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31d2c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31d2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31d2c-127">Request body</span></span>
<span data-ttu-id="31d2c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31d2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31d2c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d2c-129">Response</span></span>

<span data-ttu-id="31d2c-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31d2c-130">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31d2c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31d2c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31d2c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31d2c-132">Request</span></span>
<span data-ttu-id="31d2c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31d2c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="31d2c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d2c-134">Response</span></span>
<span data-ttu-id="31d2c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31d2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="31d2c-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="31d2c-138">See also</span></span>

- [<span data-ttu-id="31d2c-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="31d2c-139">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="31d2c-140">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="31d2c-140">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
