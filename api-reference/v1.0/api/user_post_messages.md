# <a name="create-message"></a><span data-ttu-id="c935d-101">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="c935d-101">Create Message</span></span>

<span data-ttu-id="c935d-p101">Use essa API para criar uma nova mensagem. Rascunhos podem ser criados em qualquer pasta e, opcionalmente, atualizados antes do envio. Para salvar na pasta Rascunhos, use o atalho /messages.</span><span class="sxs-lookup"><span data-stu-id="c935d-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="c935d-105">Ao criar o rascunho na mesma chamada de **POST**, você pode incluir um [anexo](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c935d-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c935d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c935d-106">Permissions</span></span>
<span data-ttu-id="c935d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c935d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c935d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c935d-109">Permission type</span></span>      | <span data-ttu-id="c935d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c935d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c935d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c935d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c935d-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c935d-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c935d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c935d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c935d-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c935d-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c935d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c935d-115">Application</span></span> | <span data-ttu-id="c935d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c935d-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c935d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c935d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="c935d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c935d-118">Request headers</span></span>
| <span data-ttu-id="c935d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c935d-119">Header</span></span>       | <span data-ttu-id="c935d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c935d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c935d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c935d-121">Authorization</span></span>  | <span data-ttu-id="c935d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c935d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c935d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c935d-124">Content-Type</span></span>  | <span data-ttu-id="c935d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c935d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c935d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c935d-126">Request body</span></span>
<span data-ttu-id="c935d-127">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="c935d-127">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c935d-128">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados à mensagem ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="c935d-128">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c935d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c935d-129">Response</span></span>

<span data-ttu-id="c935d-130">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c935d-130">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c935d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c935d-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c935d-132">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="c935d-132">Request 1</span></span>
<span data-ttu-id="c935d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c935d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
<span data-ttu-id="c935d-134">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="c935d-134">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="c935d-135">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="c935d-135">Response 1</span></span>
<span data-ttu-id="c935d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c935d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
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

## <a name="see-also"></a><span data-ttu-id="c935d-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="c935d-139">See also</span></span>

- [<span data-ttu-id="c935d-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c935d-140">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c935d-141">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c935d-141">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
