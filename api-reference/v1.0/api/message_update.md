# <a name="update-message"></a><span data-ttu-id="193ba-101">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="193ba-101">Update message</span></span>

<span data-ttu-id="193ba-102">Atualizar as propriedades do objeto message.</span><span class="sxs-lookup"><span data-stu-id="193ba-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="193ba-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="193ba-103">Permissions</span></span>
<span data-ttu-id="193ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="193ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="193ba-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="193ba-106">Permission type</span></span>      | <span data-ttu-id="193ba-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="193ba-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="193ba-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="193ba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="193ba-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="193ba-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="193ba-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="193ba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="193ba-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="193ba-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="193ba-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="193ba-112">Application</span></span> | <span data-ttu-id="193ba-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="193ba-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="193ba-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="193ba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="193ba-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="193ba-115">Request headers</span></span>
| <span data-ttu-id="193ba-116">Nome</span><span class="sxs-lookup"><span data-stu-id="193ba-116">Name</span></span>       | <span data-ttu-id="193ba-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="193ba-117">Type</span></span> | <span data-ttu-id="193ba-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="193ba-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="193ba-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="193ba-119">Authorization</span></span>  | <span data-ttu-id="193ba-120">string</span><span class="sxs-lookup"><span data-stu-id="193ba-120">string</span></span>  | <span data-ttu-id="193ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="193ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="193ba-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="193ba-123">Content-Type</span></span> | <span data-ttu-id="193ba-124">string</span><span class="sxs-lookup"><span data-stu-id="193ba-124">string</span></span>  | <span data-ttu-id="193ba-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="193ba-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="193ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="193ba-127">Request body</span></span>
<span data-ttu-id="193ba-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="193ba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="193ba-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="193ba-132">Property</span></span>     | <span data-ttu-id="193ba-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="193ba-133">Type</span></span>   |<span data-ttu-id="193ba-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="193ba-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="193ba-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="193ba-135">bccRecipients</span></span>|<span data-ttu-id="193ba-136">Destinatário</span><span class="sxs-lookup"><span data-stu-id="193ba-136">Recipient</span></span>|<span data-ttu-id="193ba-p105">Os destinatários Cco da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p105">The Bcc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-139">categories</span><span class="sxs-lookup"><span data-stu-id="193ba-139">categories</span></span>|<span data-ttu-id="193ba-140">String collection</span><span class="sxs-lookup"><span data-stu-id="193ba-140">String collection</span></span>|<span data-ttu-id="193ba-141">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="193ba-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="193ba-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="193ba-142">ccRecipients</span></span>|<span data-ttu-id="193ba-143">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="193ba-143">Recipient collection</span></span>|<span data-ttu-id="193ba-p106">Os destinatários Cc da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p106">The Cc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-146">from</span><span class="sxs-lookup"><span data-stu-id="193ba-146">from</span></span>|<span data-ttu-id="193ba-147">Destinatário</span><span class="sxs-lookup"><span data-stu-id="193ba-147">Recipient</span></span>|<span data-ttu-id="193ba-p107">O proprietário da caixa de correio e o remetente da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p107">The mailbox owner and sender of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-150">importance</span><span class="sxs-lookup"><span data-stu-id="193ba-150">importance</span></span>|<span data-ttu-id="193ba-151">String</span><span class="sxs-lookup"><span data-stu-id="193ba-151">String</span></span>|<span data-ttu-id="193ba-p108">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="193ba-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="193ba-154">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="193ba-154">inferenceClassification</span></span> | <span data-ttu-id="193ba-155">String</span><span class="sxs-lookup"><span data-stu-id="193ba-155">String</span></span> | <span data-ttu-id="193ba-p109">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="193ba-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="193ba-158">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="193ba-158">internetMessageId</span></span> |<span data-ttu-id="193ba-159">String</span><span class="sxs-lookup"><span data-stu-id="193ba-159">String</span></span> |<span data-ttu-id="193ba-p110">A ID da mensagem no formato especificado por [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p110">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-162">isRead</span><span class="sxs-lookup"><span data-stu-id="193ba-162">isRead</span></span>|<span data-ttu-id="193ba-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="193ba-163">Boolean</span></span>|<span data-ttu-id="193ba-164">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="193ba-164">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="193ba-165">replyTo</span><span class="sxs-lookup"><span data-stu-id="193ba-165">replyTo</span></span>|<span data-ttu-id="193ba-166">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="193ba-166">Recipient collection</span></span>|<span data-ttu-id="193ba-p111">Os endereços de email a serem usados ao responder. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p111">The email addresses to use when replying. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-169">sender</span><span class="sxs-lookup"><span data-stu-id="193ba-169">sender</span></span>|<span data-ttu-id="193ba-170">Destinatário</span><span class="sxs-lookup"><span data-stu-id="193ba-170">Recipient</span></span>|<span data-ttu-id="193ba-p112">A conta que é realmente usada para gerar a mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p112">The account that is actually used to generate the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-173">toRecipients</span><span class="sxs-lookup"><span data-stu-id="193ba-173">toRecipients</span></span>|<span data-ttu-id="193ba-174">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="193ba-174">Recipient collection</span></span>|<span data-ttu-id="193ba-p113">Os destinatários Para da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p113">The To recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-177">corpo</span><span class="sxs-lookup"><span data-stu-id="193ba-177">body</span></span>|<span data-ttu-id="193ba-178">ItemBody</span><span class="sxs-lookup"><span data-stu-id="193ba-178">ItemBody</span></span>|<span data-ttu-id="193ba-p114">O corpo da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p114">The body of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="193ba-181">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="193ba-181">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="193ba-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="193ba-182">Boolean</span></span>|<span data-ttu-id="193ba-183">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="193ba-183">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="193ba-184">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="193ba-184">isReadReceiptRequested</span></span>|<span data-ttu-id="193ba-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="193ba-185">Boolean</span></span>|<span data-ttu-id="193ba-186">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="193ba-186">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="193ba-187">subject</span><span class="sxs-lookup"><span data-stu-id="193ba-187">subject</span></span>|<span data-ttu-id="193ba-188">String</span><span class="sxs-lookup"><span data-stu-id="193ba-188">String</span></span>|<span data-ttu-id="193ba-p115">O assunto da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="193ba-p115">The subject of the message. Updatable only if IsDraft = true.</span></span>|

<span data-ttu-id="193ba-191">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="193ba-191">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="193ba-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="193ba-192">Response</span></span>

<span data-ttu-id="193ba-193">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="193ba-193">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="193ba-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="193ba-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="193ba-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="193ba-195">Request</span></span>
<span data-ttu-id="193ba-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="193ba-196">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a><span data-ttu-id="193ba-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="193ba-197">Response</span></span>
<span data-ttu-id="193ba-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="193ba-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a><span data-ttu-id="193ba-201">Confira também</span><span class="sxs-lookup"><span data-stu-id="193ba-201">See also</span></span>

- [<span data-ttu-id="193ba-202">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="193ba-202">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="193ba-203">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="193ba-203">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
