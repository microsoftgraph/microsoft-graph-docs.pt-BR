# <a name="message-copy"></a><span data-ttu-id="d520c-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="d520c-101">message: copy</span></span>

<span data-ttu-id="d520c-102">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d520c-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d520c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d520c-103">Permissions</span></span>
<span data-ttu-id="d520c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d520c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d520c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d520c-106">Permission type</span></span>      | <span data-ttu-id="d520c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d520c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d520c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d520c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d520c-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d520c-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d520c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d520c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d520c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d520c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d520c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d520c-112">Application</span></span> | <span data-ttu-id="d520c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d520c-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d520c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d520c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="d520c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d520c-115">Request headers</span></span>
| <span data-ttu-id="d520c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="d520c-116">Name</span></span>       | <span data-ttu-id="d520c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="d520c-117">Type</span></span> | <span data-ttu-id="d520c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d520c-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d520c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d520c-119">Authorization</span></span>  | <span data-ttu-id="d520c-120">string</span><span class="sxs-lookup"><span data-stu-id="d520c-120">string</span></span>  | <span data-ttu-id="d520c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d520c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d520c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d520c-123">Content-Type</span></span> | <span data-ttu-id="d520c-124">string</span><span class="sxs-lookup"><span data-stu-id="d520c-124">string</span></span>  | <span data-ttu-id="d520c-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d520c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d520c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d520c-127">Request body</span></span>
<span data-ttu-id="d520c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d520c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d520c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d520c-129">Parameter</span></span>    | <span data-ttu-id="d520c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d520c-130">Type</span></span>   |<span data-ttu-id="d520c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d520c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d520c-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="d520c-132">destinationId</span></span>|<span data-ttu-id="d520c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d520c-133">String</span></span>|<span data-ttu-id="d520c-134">O ID da pasta de destino ou nomes de pasta bem conhecidos, como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="d520c-134">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="d520c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d520c-135">Response</span></span>

<span data-ttu-id="d520c-136">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d520c-136">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d520c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d520c-137">Example</span></span>
<span data-ttu-id="d520c-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d520c-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d520c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d520c-139">Request</span></span>
<span data-ttu-id="d520c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d520c-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d520c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d520c-141">Response</span></span>
<span data-ttu-id="d520c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d520c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
