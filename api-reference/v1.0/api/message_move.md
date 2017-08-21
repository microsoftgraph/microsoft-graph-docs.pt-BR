# <a name="message-move"></a><span data-ttu-id="b8e83-101">message: move</span><span class="sxs-lookup"><span data-stu-id="b8e83-101">message: move</span></span>

<span data-ttu-id="b8e83-p101">Mova uma mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="b8e83-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8e83-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8e83-104">Prerequisites</span></span>
<span data-ttu-id="b8e83-105">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="b8e83-105">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="b8e83-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8e83-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="b8e83-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e83-107">Request headers</span></span>
| <span data-ttu-id="b8e83-108">Nome</span><span class="sxs-lookup"><span data-stu-id="b8e83-108">Name</span></span>       | <span data-ttu-id="b8e83-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8e83-109">Type</span></span> | <span data-ttu-id="b8e83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e83-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8e83-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8e83-111">Authorization</span></span>  | <span data-ttu-id="b8e83-112">string</span><span class="sxs-lookup"><span data-stu-id="b8e83-112">string</span></span>  | <span data-ttu-id="b8e83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8e83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8e83-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8e83-115">Content-Type</span></span> | <span data-ttu-id="b8e83-116">string</span><span class="sxs-lookup"><span data-stu-id="b8e83-116">string</span></span>  | <span data-ttu-id="b8e83-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8e83-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8e83-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e83-119">Request body</span></span>
<span data-ttu-id="b8e83-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8e83-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8e83-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8e83-121">Parameter</span></span>    | <span data-ttu-id="b8e83-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8e83-122">Type</span></span>   |<span data-ttu-id="b8e83-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e83-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8e83-124">DestinationId</span><span class="sxs-lookup"><span data-stu-id="b8e83-124">DestinationId</span></span>|<span data-ttu-id="b8e83-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e83-125">String</span></span>|<span data-ttu-id="b8e83-126">O ID da pasta de destino ou nomes de pasta bem conhecidos, como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="b8e83-126">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="b8e83-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e83-127">Response</span></span>

<span data-ttu-id="b8e83-128">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e83-128">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8e83-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8e83-129">Example</span></span>
<span data-ttu-id="b8e83-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b8e83-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b8e83-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e83-131">Request</span></span>
<span data-ttu-id="b8e83-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8e83-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/move
Content-type: application/json
Content-length: 44

{
  "DestinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="b8e83-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e83-133">Response</span></span>
<span data-ttu-id="b8e83-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8e83-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
