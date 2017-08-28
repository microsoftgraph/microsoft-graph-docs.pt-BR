# <a name="get-eventmessage"></a><span data-ttu-id="0a776-101">Obter eventMessage</span><span class="sxs-lookup"><span data-stu-id="0a776-101">Get eventMessage</span></span>

<span data-ttu-id="0a776-102">Recupera as propriedades e relações do objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="0a776-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="0a776-103">No momento, esta operação retorna corpos de mensagens de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="0a776-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a776-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a776-104">Permissions</span></span>
<span data-ttu-id="0a776-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a776-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a776-107">Permission type</span></span>      | <span data-ttu-id="0a776-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a776-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="0a776-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a776-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0a776-110">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0a776-110">Mail.Read</span></span>    | 
|<span data-ttu-id="0a776-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a776-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a776-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0a776-112">Mail.Read</span></span>    | 
|<span data-ttu-id="0a776-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a776-113">Application</span></span> | <span data-ttu-id="0a776-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0a776-114">Mail.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0a776-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a776-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a776-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a776-116">Optional query parameters</span></span>
<span data-ttu-id="0a776-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a776-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0a776-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a776-118">Request headers</span></span>
| <span data-ttu-id="0a776-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0a776-119">Name</span></span>       | <span data-ttu-id="0a776-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a776-120">Type</span></span> | <span data-ttu-id="0a776-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a776-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0a776-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a776-122">Authorization</span></span>  | <span data-ttu-id="0a776-123">string</span><span class="sxs-lookup"><span data-stu-id="0a776-123">string</span></span>  | <span data-ttu-id="0a776-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a776-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a776-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a776-126">Request body</span></span>
<span data-ttu-id="0a776-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a776-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a776-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a776-128">Response</span></span>

<span data-ttu-id="0a776-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a776-129">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a776-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a776-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a776-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a776-131">Request</span></span>
<span data-ttu-id="0a776-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a776-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="0a776-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a776-133">Response</span></span>
<span data-ttu-id="0a776-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a776-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
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
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
