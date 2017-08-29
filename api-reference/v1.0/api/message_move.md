# <a name="message-move"></a><span data-ttu-id="81104-101">message: move</span><span class="sxs-lookup"><span data-stu-id="81104-101">message: move</span></span>

<span data-ttu-id="81104-p101">Mova uma mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="81104-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="81104-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="81104-104">Permissions</span></span>
<span data-ttu-id="81104-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81104-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="81104-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81104-107">Permission type</span></span>      | <span data-ttu-id="81104-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81104-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81104-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81104-109">Delegated (work or school account)</span></span> | <span data-ttu-id="81104-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81104-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81104-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81104-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81104-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81104-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="81104-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81104-113">Application</span></span> | <span data-ttu-id="81104-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81104-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81104-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81104-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="81104-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81104-116">Request headers</span></span>
| <span data-ttu-id="81104-117">Nome</span><span class="sxs-lookup"><span data-stu-id="81104-117">Name</span></span>       | <span data-ttu-id="81104-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="81104-118">Type</span></span> | <span data-ttu-id="81104-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="81104-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81104-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="81104-120">Authorization</span></span>  | <span data-ttu-id="81104-121">string</span><span class="sxs-lookup"><span data-stu-id="81104-121">string</span></span>  | <span data-ttu-id="81104-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81104-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81104-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81104-124">Content-Type</span></span> | <span data-ttu-id="81104-125">string</span><span class="sxs-lookup"><span data-stu-id="81104-125">string</span></span>  | <span data-ttu-id="81104-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81104-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81104-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81104-128">Request body</span></span>
<span data-ttu-id="81104-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81104-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81104-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="81104-130">Parameter</span></span>    | <span data-ttu-id="81104-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="81104-131">Type</span></span>   |<span data-ttu-id="81104-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81104-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81104-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="81104-133">DestinationId</span></span>|<span data-ttu-id="81104-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81104-134">String</span></span>|<span data-ttu-id="81104-135">O ID da pasta de destino ou nomes de pasta bem conhecidos, como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="81104-135">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="81104-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="81104-136">Response</span></span>

<span data-ttu-id="81104-137">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81104-137">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81104-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81104-138">Example</span></span>
<span data-ttu-id="81104-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="81104-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81104-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81104-140">Request</span></span>
<span data-ttu-id="81104-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81104-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="81104-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="81104-142">Response</span></span>
<span data-ttu-id="81104-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81104-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
