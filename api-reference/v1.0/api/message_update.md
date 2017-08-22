# <a name="update-message"></a><span data-ttu-id="d5139-101">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="d5139-101">Update message</span></span>

<span data-ttu-id="d5139-102">Atualize as propriedades do objeto message.</span><span class="sxs-lookup"><span data-stu-id="d5139-102">Update the properties of message object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5139-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5139-103">Prerequisites</span></span>
<span data-ttu-id="d5139-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="d5139-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="d5139-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5139-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d5139-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5139-106">Request headers</span></span>
| <span data-ttu-id="d5139-107">Nome</span><span class="sxs-lookup"><span data-stu-id="d5139-107">Name</span></span>       | <span data-ttu-id="d5139-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5139-108">Type</span></span> | <span data-ttu-id="d5139-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5139-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d5139-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5139-110">Authorization</span></span>  | <span data-ttu-id="d5139-111">string</span><span class="sxs-lookup"><span data-stu-id="d5139-111">string</span></span>  | <span data-ttu-id="d5139-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5139-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5139-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5139-114">Content-Type</span></span> | <span data-ttu-id="d5139-115">string</span><span class="sxs-lookup"><span data-stu-id="d5139-115">string</span></span>  | <span data-ttu-id="d5139-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5139-p102">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d5139-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5139-118">Request body</span></span>
<span data-ttu-id="d5139-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="d5139-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="d5139-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5139-123">Property</span></span>     | <span data-ttu-id="d5139-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5139-124">Type</span></span>   |<span data-ttu-id="d5139-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5139-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5139-126">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="d5139-126">bccRecipients</span></span>|<span data-ttu-id="d5139-127">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d5139-127">Recipient</span></span>|<span data-ttu-id="d5139-p104">Os destinatários Cco da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p104">The Bcc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-130">categories</span><span class="sxs-lookup"><span data-stu-id="d5139-130">categories</span></span>|<span data-ttu-id="d5139-131">String collection</span><span class="sxs-lookup"><span data-stu-id="d5139-131">String collection</span></span>|<span data-ttu-id="d5139-132">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="d5139-132">The categories associated with the message.</span></span>|
|<span data-ttu-id="d5139-133">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="d5139-133">ccRecipients</span></span>|<span data-ttu-id="d5139-134">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d5139-134">Recipient collection</span></span>|<span data-ttu-id="d5139-p105">Os destinatários Cc da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p105">The Cc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-137">from</span><span class="sxs-lookup"><span data-stu-id="d5139-137">from</span></span>|<span data-ttu-id="d5139-138">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d5139-138">Recipient</span></span>|<span data-ttu-id="d5139-p106">O proprietário da caixa de correio e o remetente da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p106">The mailbox owner and sender of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-141">importance</span><span class="sxs-lookup"><span data-stu-id="d5139-141">importance</span></span>|<span data-ttu-id="d5139-142">String</span><span class="sxs-lookup"><span data-stu-id="d5139-142">String</span></span>|<span data-ttu-id="d5139-p107">A importância da mensagem. Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="d5139-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="d5139-145">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="d5139-145">inferenceClassification</span></span> | <span data-ttu-id="d5139-146">String</span><span class="sxs-lookup"><span data-stu-id="d5139-146">String</span></span> | <span data-ttu-id="d5139-p108">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="d5139-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="d5139-149">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="d5139-149">internetMessageId</span></span> |<span data-ttu-id="d5139-150">String</span><span class="sxs-lookup"><span data-stu-id="d5139-150">String</span></span> |<span data-ttu-id="d5139-p109">A ID da mensagem no formato especificado por [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p109">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-153">isRead</span><span class="sxs-lookup"><span data-stu-id="d5139-153">isRead</span></span>|<span data-ttu-id="d5139-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5139-154">Boolean</span></span>|<span data-ttu-id="d5139-155">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="d5139-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="d5139-156">replyTo</span><span class="sxs-lookup"><span data-stu-id="d5139-156">replyTo</span></span>|<span data-ttu-id="d5139-157">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d5139-157">Recipient collection</span></span>|<span data-ttu-id="d5139-p110">Os endereços de email a serem usados ao responder. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p110">The email addresses to use when replying. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-160">sender</span><span class="sxs-lookup"><span data-stu-id="d5139-160">sender</span></span>|<span data-ttu-id="d5139-161">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d5139-161">Recipient</span></span>|<span data-ttu-id="d5139-p111">A conta que é realmente usada para gerar a mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p111">The account that is actually used to generate the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-164">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d5139-164">toRecipients</span></span>|<span data-ttu-id="d5139-165">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d5139-165">Recipient collection</span></span>|<span data-ttu-id="d5139-p112">Os destinatários Para da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p112">The To recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-168">corpo</span><span class="sxs-lookup"><span data-stu-id="d5139-168">body</span></span>|<span data-ttu-id="d5139-169">ItemBody</span><span class="sxs-lookup"><span data-stu-id="d5139-169">ItemBody</span></span>|<span data-ttu-id="d5139-p113">O corpo da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p113">The body of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="d5139-172">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d5139-172">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="d5139-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5139-173">Boolean</span></span>|<span data-ttu-id="d5139-174">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d5139-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d5139-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d5139-175">isReadReceiptRequested</span></span>|<span data-ttu-id="d5139-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5139-176">Boolean</span></span>|<span data-ttu-id="d5139-177">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d5139-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d5139-178">subject</span><span class="sxs-lookup"><span data-stu-id="d5139-178">subject</span></span>|<span data-ttu-id="d5139-179">String</span><span class="sxs-lookup"><span data-stu-id="d5139-179">String</span></span>|<span data-ttu-id="d5139-p114">O assunto da mensagem. Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d5139-p114">The subject of the message. Updatable only if IsDraft = true.</span></span>|

<span data-ttu-id="d5139-182">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="d5139-182">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="d5139-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5139-183">Response</span></span>

<span data-ttu-id="d5139-184">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5139-184">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5139-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5139-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5139-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5139-186">Request</span></span>
<span data-ttu-id="d5139-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5139-187">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d5139-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5139-188">Response</span></span>
<span data-ttu-id="d5139-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5139-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d5139-192">Ver também</span><span class="sxs-lookup"><span data-stu-id="d5139-192">See also</span></span>

- [<span data-ttu-id="d5139-193">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d5139-193">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d5139-194">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="d5139-194">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
