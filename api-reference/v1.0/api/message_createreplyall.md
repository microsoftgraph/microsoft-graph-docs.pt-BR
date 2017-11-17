# <a name="message-createreplyall"></a><span data-ttu-id="1f037-101">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="1f037-101">message: createReplyAll</span></span>

<span data-ttu-id="1f037-102">Crie um rascunho para responder ao remetente e a todos os destinatários da [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="1f037-102">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="1f037-103">Você pode [atualizar](../api/message_update.md) o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente [enviar](../api/message_send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="1f037-103">You can then [update](../api/message_update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f037-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f037-104">Permissions</span></span>
<span data-ttu-id="1f037-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f037-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f037-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f037-107">Permission type</span></span>      | <span data-ttu-id="1f037-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f037-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f037-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f037-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1f037-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f037-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1f037-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f037-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f037-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f037-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1f037-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f037-113">Application</span></span> | <span data-ttu-id="1f037-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f037-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f037-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f037-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="1f037-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f037-116">Request headers</span></span>
| <span data-ttu-id="1f037-117">Nome</span><span class="sxs-lookup"><span data-stu-id="1f037-117">Name</span></span>       | <span data-ttu-id="1f037-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f037-118">Type</span></span> | <span data-ttu-id="1f037-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f037-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f037-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f037-120">Authorization</span></span>  | <span data-ttu-id="1f037-121">string</span><span class="sxs-lookup"><span data-stu-id="1f037-121">string</span></span>  | <span data-ttu-id="1f037-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f037-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f037-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f037-124">Request body</span></span>
<span data-ttu-id="1f037-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f037-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f037-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f037-126">Response</span></span>

<span data-ttu-id="1f037-127">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f037-127">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f037-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f037-128">Example</span></span>
<span data-ttu-id="1f037-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1f037-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1f037-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f037-130">Request</span></span>
<span data-ttu-id="1f037-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f037-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="1f037-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f037-132">Response</span></span>
<span data-ttu-id="1f037-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f037-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
