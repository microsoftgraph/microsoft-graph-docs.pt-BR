# <a name="update-message"></a><span data-ttu-id="da17b-101">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="da17b-101">Update message</span></span>

<span data-ttu-id="da17b-102">Atualizar as propriedades do objeto message.</span><span class="sxs-lookup"><span data-stu-id="da17b-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da17b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="da17b-103">Permissions</span></span>
<span data-ttu-id="da17b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da17b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da17b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da17b-106">Permission type</span></span>      | <span data-ttu-id="da17b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da17b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da17b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da17b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="da17b-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da17b-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da17b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da17b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da17b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da17b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da17b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da17b-112">Application</span></span> | <span data-ttu-id="da17b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da17b-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da17b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da17b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da17b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da17b-115">Request headers</span></span>
| <span data-ttu-id="da17b-116">Nome</span><span class="sxs-lookup"><span data-stu-id="da17b-116">Name</span></span>       | <span data-ttu-id="da17b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="da17b-117">Type</span></span> | <span data-ttu-id="da17b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="da17b-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da17b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="da17b-119">Authorization</span></span>  | <span data-ttu-id="da17b-120">string</span><span class="sxs-lookup"><span data-stu-id="da17b-120">string</span></span>  | <span data-ttu-id="da17b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da17b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da17b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da17b-123">Content-Type</span></span> | <span data-ttu-id="da17b-124">string</span><span class="sxs-lookup"><span data-stu-id="da17b-124">string</span></span>  | <span data-ttu-id="da17b-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da17b-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="da17b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da17b-127">Request body</span></span>
<span data-ttu-id="da17b-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="da17b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="da17b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da17b-132">Property</span></span>     | <span data-ttu-id="da17b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="da17b-133">Type</span></span>   |<span data-ttu-id="da17b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="da17b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da17b-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="da17b-135">bccRecipients</span></span>|<span data-ttu-id="da17b-136">Destinatário</span><span class="sxs-lookup"><span data-stu-id="da17b-136">Recipient</span></span>|<span data-ttu-id="da17b-137">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-137">The Bcc recipients for the message.</span></span> <span data-ttu-id="da17b-138">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-138">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="da17b-139">categories</span><span class="sxs-lookup"><span data-stu-id="da17b-139">categories</span></span>|<span data-ttu-id="da17b-140">String collection</span><span class="sxs-lookup"><span data-stu-id="da17b-140">String collection</span></span>|<span data-ttu-id="da17b-141">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="da17b-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="da17b-142">ccRecipients</span></span>|<span data-ttu-id="da17b-143">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="da17b-143">Recipient collection</span></span>|<span data-ttu-id="da17b-144">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-144">The Cc recipients for the message.</span></span> <span data-ttu-id="da17b-145">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="da17b-146">from</span><span class="sxs-lookup"><span data-stu-id="da17b-146">from</span></span>|<span data-ttu-id="da17b-147">Destinatário</span><span class="sxs-lookup"><span data-stu-id="da17b-147">Recipient</span></span>|<span data-ttu-id="da17b-148">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-148">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="da17b-149">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-149">Updatable only if isDraft = true.</span></span> <span data-ttu-id="da17b-150">Deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="da17b-150">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="da17b-151">importance</span><span class="sxs-lookup"><span data-stu-id="da17b-151">importance</span></span>|<span data-ttu-id="da17b-152">String</span><span class="sxs-lookup"><span data-stu-id="da17b-152">String</span></span>|<span data-ttu-id="da17b-153">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-153">The importance of the message.</span></span> <span data-ttu-id="da17b-154">Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="da17b-154">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="da17b-155">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="da17b-155">inferenceClassification</span></span> | <span data-ttu-id="da17b-156">String</span><span class="sxs-lookup"><span data-stu-id="da17b-156">String</span></span> | <span data-ttu-id="da17b-157">A classificação da mensagem para o usuário, com base na relevância deduzida ou importância, ou em um caso de sobreposição explícito.</span><span class="sxs-lookup"><span data-stu-id="da17b-157">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="da17b-158">Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="da17b-158">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="da17b-159">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="da17b-159">internetMessageId</span></span> |<span data-ttu-id="da17b-160">String</span><span class="sxs-lookup"><span data-stu-id="da17b-160">String</span></span> |<span data-ttu-id="da17b-161">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="da17b-161">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="da17b-162">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-162">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="da17b-163">isRead</span><span class="sxs-lookup"><span data-stu-id="da17b-163">isRead</span></span>|<span data-ttu-id="da17b-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="da17b-164">Boolean</span></span>|<span data-ttu-id="da17b-165">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="da17b-165">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="da17b-166">replyTo</span><span class="sxs-lookup"><span data-stu-id="da17b-166">replyTo</span></span>|<span data-ttu-id="da17b-167">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="da17b-167">Recipient collection</span></span>|<span data-ttu-id="da17b-168">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="da17b-168">The email addresses to use when replying.</span></span> <span data-ttu-id="da17b-169">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="da17b-170">sender</span><span class="sxs-lookup"><span data-stu-id="da17b-170">sender</span></span>|<span data-ttu-id="da17b-171">Destinatário</span><span class="sxs-lookup"><span data-stu-id="da17b-171">Recipient</span></span>|<span data-ttu-id="da17b-172">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-172">The account that is actually used to generate the message.</span></span> <span data-ttu-id="da17b-173">Somente se atualizável isDraft = verdadeiro e quando enviando uma mensagem a partir de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviando uma mensagem como um [representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="da17b-173">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="da17b-174">Em qualquer caso, o valor deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="da17b-174">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="da17b-175">toRecipients</span><span class="sxs-lookup"><span data-stu-id="da17b-175">toRecipients</span></span>|<span data-ttu-id="da17b-176">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="da17b-176">Recipient collection</span></span>|<span data-ttu-id="da17b-177">Dos destinatários da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-177">The To recipients for the message.</span></span> <span data-ttu-id="da17b-178">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-178">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="da17b-179">corpo</span><span class="sxs-lookup"><span data-stu-id="da17b-179">body</span></span>|<span data-ttu-id="da17b-180">ItemBody</span><span class="sxs-lookup"><span data-stu-id="da17b-180">ItemBody</span></span>|<span data-ttu-id="da17b-181">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-181">The body of the message.</span></span> <span data-ttu-id="da17b-182">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="da17b-183">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="da17b-183">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="da17b-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="da17b-184">Boolean</span></span>|<span data-ttu-id="da17b-185">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-185">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="da17b-186">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="da17b-186">isReadReceiptRequested</span></span>|<span data-ttu-id="da17b-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="da17b-187">Boolean</span></span>|<span data-ttu-id="da17b-188">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-188">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="da17b-189">subject</span><span class="sxs-lookup"><span data-stu-id="da17b-189">subject</span></span>|<span data-ttu-id="da17b-190">String</span><span class="sxs-lookup"><span data-stu-id="da17b-190">String</span></span>|<span data-ttu-id="da17b-191">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="da17b-191">The subject of the message.</span></span> <span data-ttu-id="da17b-192">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="da17b-192">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="da17b-193">Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="da17b-193">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="da17b-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="da17b-194">Response</span></span>

<span data-ttu-id="da17b-195">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da17b-195">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da17b-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da17b-196">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da17b-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da17b-197">Request</span></span>
<span data-ttu-id="da17b-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da17b-198">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="da17b-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="da17b-199">Response</span></span>
<span data-ttu-id="da17b-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da17b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="da17b-203">Confira também</span><span class="sxs-lookup"><span data-stu-id="da17b-203">See also</span></span>

- [<span data-ttu-id="da17b-204">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="da17b-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="da17b-205">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="da17b-205">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
