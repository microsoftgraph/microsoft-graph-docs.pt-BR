# <a name="message-copy"></a><span data-ttu-id="53127-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="53127-101">message: copy</span></span>

<span data-ttu-id="53127-102">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="53127-102">Copy a message to a folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53127-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53127-103">Prerequisites</span></span>
<span data-ttu-id="53127-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="53127-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="53127-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53127-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="53127-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53127-106">Request headers</span></span>
| <span data-ttu-id="53127-107">Nome</span><span class="sxs-lookup"><span data-stu-id="53127-107">Name</span></span>       | <span data-ttu-id="53127-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="53127-108">Type</span></span> | <span data-ttu-id="53127-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="53127-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53127-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="53127-110">Authorization</span></span>  | <span data-ttu-id="53127-111">string</span><span class="sxs-lookup"><span data-stu-id="53127-111">string</span></span>  | <span data-ttu-id="53127-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53127-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53127-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53127-114">Content-Type</span></span> | <span data-ttu-id="53127-115">string</span><span class="sxs-lookup"><span data-stu-id="53127-115">string</span></span>  | <span data-ttu-id="53127-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53127-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53127-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53127-118">Request body</span></span>
<span data-ttu-id="53127-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53127-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53127-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="53127-120">Parameter</span></span>    | <span data-ttu-id="53127-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="53127-121">Type</span></span>   |<span data-ttu-id="53127-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="53127-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53127-123">destinationId</span><span class="sxs-lookup"><span data-stu-id="53127-123">destinationId</span></span>|<span data-ttu-id="53127-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53127-124">String</span></span>|<span data-ttu-id="53127-125">O ID da pasta de destino ou nomes de pasta bem conhecidos, como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="53127-125">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="53127-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="53127-126">Response</span></span>

<span data-ttu-id="53127-127">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53127-127">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53127-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53127-128">Example</span></span>
<span data-ttu-id="53127-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="53127-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53127-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53127-130">Request</span></span>
<span data-ttu-id="53127-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53127-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="53127-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="53127-132">Response</span></span>
<span data-ttu-id="53127-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53127-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
