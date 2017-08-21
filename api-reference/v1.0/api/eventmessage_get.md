# <a name="get-eventmessage"></a><span data-ttu-id="59738-101">Obter eventMessage</span><span class="sxs-lookup"><span data-stu-id="59738-101">Get eventMessage</span></span>

<span data-ttu-id="59738-102">Recupera as propriedades e relações do objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="59738-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="59738-103">No momento, esta operação retorna corpos de mensagens de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="59738-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59738-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59738-104">Prerequisites</span></span>
<span data-ttu-id="59738-105">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="59738-105">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="59738-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59738-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59738-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59738-107">Optional query parameters</span></span>
<span data-ttu-id="59738-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59738-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59738-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59738-109">Request headers</span></span>
| <span data-ttu-id="59738-110">Nome</span><span class="sxs-lookup"><span data-stu-id="59738-110">Name</span></span>       | <span data-ttu-id="59738-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="59738-111">Type</span></span> | <span data-ttu-id="59738-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="59738-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59738-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="59738-113">Authorization</span></span>  | <span data-ttu-id="59738-114">string</span><span class="sxs-lookup"><span data-stu-id="59738-114">string</span></span>  | <span data-ttu-id="59738-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59738-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59738-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59738-117">Request body</span></span>
<span data-ttu-id="59738-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59738-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59738-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="59738-119">Response</span></span>

<span data-ttu-id="59738-120">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59738-120">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59738-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59738-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59738-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59738-122">Request</span></span>
<span data-ttu-id="59738-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59738-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="59738-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="59738-124">Response</span></span>
<span data-ttu-id="59738-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59738-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
