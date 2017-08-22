# <a name="message-createreplyall"></a><span data-ttu-id="5f443-101">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="5f443-101">message: createReplyAll</span></span>

<span data-ttu-id="5f443-p101">Crie um rascunho da mensagem de resposta a todos. Você poderá, então, [update](../api/message_update.md) ou [send](../api/message_send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="5f443-p101">Create a draft of the Reply All message. You can then [update](../api/message_update.md) or [send](../api/message_send.md) the draft.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f443-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5f443-104">Prerequisites</span></span>
<span data-ttu-id="5f443-105">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="5f443-105">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="5f443-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f443-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="5f443-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f443-107">Request headers</span></span>
| <span data-ttu-id="5f443-108">Nome</span><span class="sxs-lookup"><span data-stu-id="5f443-108">Name</span></span>       | <span data-ttu-id="5f443-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f443-109">Type</span></span> | <span data-ttu-id="5f443-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f443-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f443-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f443-111">Authorization</span></span>  | <span data-ttu-id="5f443-112">string</span><span class="sxs-lookup"><span data-stu-id="5f443-112">string</span></span>  | <span data-ttu-id="5f443-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f443-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f443-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f443-115">Content-Type</span></span> | <span data-ttu-id="5f443-116">string</span><span class="sxs-lookup"><span data-stu-id="5f443-116">string</span></span>  | <span data-ttu-id="5f443-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f443-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f443-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f443-119">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5f443-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f443-120">Response</span></span>

<span data-ttu-id="5f443-121">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f443-121">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f443-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f443-122">Example</span></span>
<span data-ttu-id="5f443-123">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5f443-123">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f443-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f443-124">Request</span></span>
<span data-ttu-id="5f443-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f443-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
Content-type: application/json
Content-length: 248

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="5f443-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f443-126">Response</span></span>
<span data-ttu-id="5f443-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f443-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
