---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto message.
author: angelgolfer-ms
ms.openlocfilehash: b8f39dc9648203f86749ba06b88bf2f74b79d88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337538"
---
# <a name="update-message"></a><span data-ttu-id="eaf56-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="eaf56-103">Update message</span></span>

<span data-ttu-id="eaf56-104">Atualizar as propriedades do objeto message.</span><span class="sxs-lookup"><span data-stu-id="eaf56-104">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eaf56-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaf56-105">Permissions</span></span>
<span data-ttu-id="eaf56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf56-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaf56-108">Permission type</span></span>      | <span data-ttu-id="eaf56-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaf56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaf56-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaf56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eaf56-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaf56-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eaf56-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaf56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaf56-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaf56-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eaf56-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaf56-114">Application</span></span> | <span data-ttu-id="eaf56-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaf56-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaf56-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaf56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eaf56-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf56-117">Request headers</span></span>
| <span data-ttu-id="eaf56-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eaf56-118">Name</span></span>       | <span data-ttu-id="eaf56-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf56-119">Type</span></span> | <span data-ttu-id="eaf56-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf56-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eaf56-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaf56-121">Authorization</span></span>  | <span data-ttu-id="eaf56-122">string</span><span class="sxs-lookup"><span data-stu-id="eaf56-122">string</span></span>  | <span data-ttu-id="eaf56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaf56-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eaf56-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eaf56-125">Content-Type</span></span> | <span data-ttu-id="eaf56-126">string</span><span class="sxs-lookup"><span data-stu-id="eaf56-126">string</span></span>  | <span data-ttu-id="eaf56-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaf56-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="eaf56-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf56-129">Request body</span></span>
<span data-ttu-id="eaf56-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="eaf56-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="eaf56-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaf56-134">Property</span></span>     | <span data-ttu-id="eaf56-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf56-135">Type</span></span>   |<span data-ttu-id="eaf56-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf56-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaf56-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="eaf56-137">bccRecipients</span></span>|<span data-ttu-id="eaf56-138">Destinatário</span><span class="sxs-lookup"><span data-stu-id="eaf56-138">Recipient</span></span>|<span data-ttu-id="eaf56-139">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-139">The Bcc recipients for the message.</span></span> <span data-ttu-id="eaf56-140">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-140">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="eaf56-141">categories</span><span class="sxs-lookup"><span data-stu-id="eaf56-141">categories</span></span>|<span data-ttu-id="eaf56-142">String collection</span><span class="sxs-lookup"><span data-stu-id="eaf56-142">String collection</span></span>|<span data-ttu-id="eaf56-143">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-143">The categories associated with the message.</span></span>|
|<span data-ttu-id="eaf56-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="eaf56-144">ccRecipients</span></span>|<span data-ttu-id="eaf56-145">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="eaf56-145">Recipient collection</span></span>|<span data-ttu-id="eaf56-146">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-146">The Cc recipients for the message.</span></span> <span data-ttu-id="eaf56-147">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-147">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="eaf56-148">from</span><span class="sxs-lookup"><span data-stu-id="eaf56-148">from</span></span>|<span data-ttu-id="eaf56-149">Destinatário</span><span class="sxs-lookup"><span data-stu-id="eaf56-149">Recipient</span></span>|<span data-ttu-id="eaf56-150">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-150">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="eaf56-151">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-151">Updatable only if isDraft = true.</span></span> <span data-ttu-id="eaf56-152">Deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="eaf56-152">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="eaf56-153">importance</span><span class="sxs-lookup"><span data-stu-id="eaf56-153">importance</span></span>|<span data-ttu-id="eaf56-154">String</span><span class="sxs-lookup"><span data-stu-id="eaf56-154">String</span></span>|<span data-ttu-id="eaf56-155">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-155">The importance of the message.</span></span> <span data-ttu-id="eaf56-156">Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="eaf56-156">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="eaf56-157">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="eaf56-157">inferenceClassification</span></span> | <span data-ttu-id="eaf56-158">String</span><span class="sxs-lookup"><span data-stu-id="eaf56-158">String</span></span> | <span data-ttu-id="eaf56-159">A classificação da mensagem para o usuário, com base na relevância deduzida ou importância, ou em um caso de sobreposição explícito.</span><span class="sxs-lookup"><span data-stu-id="eaf56-159">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="eaf56-160">Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="eaf56-160">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="eaf56-161">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="eaf56-161">internetMessageId</span></span> |<span data-ttu-id="eaf56-162">String</span><span class="sxs-lookup"><span data-stu-id="eaf56-162">String</span></span> |<span data-ttu-id="eaf56-163">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="eaf56-163">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="eaf56-164">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-164">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="eaf56-165">isRead</span><span class="sxs-lookup"><span data-stu-id="eaf56-165">isRead</span></span>|<span data-ttu-id="eaf56-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf56-166">Boolean</span></span>|<span data-ttu-id="eaf56-167">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="eaf56-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="eaf56-168">replyTo</span><span class="sxs-lookup"><span data-stu-id="eaf56-168">replyTo</span></span>|<span data-ttu-id="eaf56-169">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="eaf56-169">Recipient collection</span></span>|<span data-ttu-id="eaf56-170">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="eaf56-170">The email addresses to use when replying.</span></span> <span data-ttu-id="eaf56-171">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-171">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="eaf56-172">sender</span><span class="sxs-lookup"><span data-stu-id="eaf56-172">sender</span></span>|<span data-ttu-id="eaf56-173">Destinatário</span><span class="sxs-lookup"><span data-stu-id="eaf56-173">Recipient</span></span>|<span data-ttu-id="eaf56-174">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-174">The account that is actually used to generate the message.</span></span> <span data-ttu-id="eaf56-175">Somente se atualizável isDraft = verdadeiro e quando enviando uma mensagem a partir de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviando uma mensagem como um [representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="eaf56-175">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="eaf56-176">Em qualquer caso, o valor deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="eaf56-176">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="eaf56-177">toRecipients</span><span class="sxs-lookup"><span data-stu-id="eaf56-177">toRecipients</span></span>|<span data-ttu-id="eaf56-178">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="eaf56-178">Recipient collection</span></span>|<span data-ttu-id="eaf56-179">Dos destinatários da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-179">The To recipients for the message.</span></span> <span data-ttu-id="eaf56-180">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-180">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="eaf56-181">corpo</span><span class="sxs-lookup"><span data-stu-id="eaf56-181">body</span></span>|<span data-ttu-id="eaf56-182">ItemBody</span><span class="sxs-lookup"><span data-stu-id="eaf56-182">ItemBody</span></span>|<span data-ttu-id="eaf56-183">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-183">The body of the message.</span></span> <span data-ttu-id="eaf56-184">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="eaf56-185">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="eaf56-185">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="eaf56-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf56-186">Boolean</span></span>|<span data-ttu-id="eaf56-187">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-187">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="eaf56-188">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="eaf56-188">isReadReceiptRequested</span></span>|<span data-ttu-id="eaf56-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf56-189">Boolean</span></span>|<span data-ttu-id="eaf56-190">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-190">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="eaf56-191">subject</span><span class="sxs-lookup"><span data-stu-id="eaf56-191">subject</span></span>|<span data-ttu-id="eaf56-192">String</span><span class="sxs-lookup"><span data-stu-id="eaf56-192">String</span></span>|<span data-ttu-id="eaf56-193">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="eaf56-193">The subject of the message.</span></span> <span data-ttu-id="eaf56-194">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="eaf56-194">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="eaf56-195">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="eaf56-195">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="eaf56-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf56-196">Response</span></span>

<span data-ttu-id="eaf56-197">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaf56-197">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eaf56-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaf56-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaf56-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf56-199">Request</span></span>
<span data-ttu-id="eaf56-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaf56-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="eaf56-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf56-201">Response</span></span>
<span data-ttu-id="eaf56-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaf56-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="eaf56-205">Confira também</span><span class="sxs-lookup"><span data-stu-id="eaf56-205">See also</span></span>

- [<span data-ttu-id="eaf56-206">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="eaf56-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eaf56-207">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="eaf56-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
