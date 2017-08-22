# <a name="create-message"></a><span data-ttu-id="400c0-101">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="400c0-101">Create Message</span></span>

<span data-ttu-id="400c0-102">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="400c0-102">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="400c0-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="400c0-103">Prerequisites</span></span>
<span data-ttu-id="400c0-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="400c0-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="400c0-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="400c0-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="400c0-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="400c0-106">Request headers</span></span>
| <span data-ttu-id="400c0-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="400c0-107">Header</span></span>       | <span data-ttu-id="400c0-108">Valor</span><span class="sxs-lookup"><span data-stu-id="400c0-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="400c0-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="400c0-109">Authorization</span></span>  | <span data-ttu-id="400c0-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="400c0-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="400c0-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="400c0-112">Content-Type</span></span>  | <span data-ttu-id="400c0-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="400c0-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="400c0-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="400c0-115">Request body</span></span>
<span data-ttu-id="400c0-116">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="400c0-116">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="400c0-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="400c0-117">Response</span></span>

<span data-ttu-id="400c0-118">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="400c0-118">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="400c0-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="400c0-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="400c0-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="400c0-120">Request</span></span>
<span data-ttu-id="400c0-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="400c0-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
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
<span data-ttu-id="400c0-122">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="400c0-122">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="400c0-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="400c0-123">Response</span></span>
<span data-ttu-id="400c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="400c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
