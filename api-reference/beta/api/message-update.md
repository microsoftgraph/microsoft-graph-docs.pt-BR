---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto message.
author: angelgolfer-ms
ms.openlocfilehash: 9c717e913c641b6dffd582252538965961369a7f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321473"
---
# <a name="update-message"></a><span data-ttu-id="9cf90-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="9cf90-103">Update message</span></span>

> <span data-ttu-id="9cf90-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9cf90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cf90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9cf90-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9cf90-106">Atualizar as propriedades do objeto message.</span><span class="sxs-lookup"><span data-stu-id="9cf90-106">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cf90-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cf90-107">Permissions</span></span>
<span data-ttu-id="9cf90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf90-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cf90-110">Permission type</span></span>      | <span data-ttu-id="9cf90-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cf90-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cf90-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cf90-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9cf90-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cf90-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9cf90-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cf90-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cf90-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cf90-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9cf90-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cf90-116">Application</span></span> | <span data-ttu-id="9cf90-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cf90-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cf90-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf90-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9cf90-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf90-119">Request headers</span></span>
| <span data-ttu-id="9cf90-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9cf90-120">Name</span></span>       | <span data-ttu-id="9cf90-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf90-121">Type</span></span> | <span data-ttu-id="9cf90-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf90-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9cf90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cf90-123">Authorization</span></span>  | <span data-ttu-id="9cf90-124">string</span><span class="sxs-lookup"><span data-stu-id="9cf90-124">string</span></span>  | <span data-ttu-id="9cf90-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cf90-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cf90-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cf90-127">Content-Type</span></span> | <span data-ttu-id="9cf90-128">string</span><span class="sxs-lookup"><span data-stu-id="9cf90-128">string</span></span>  | <span data-ttu-id="9cf90-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cf90-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="9cf90-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf90-131">Request body</span></span>
<span data-ttu-id="9cf90-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="9cf90-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="9cf90-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cf90-136">Property</span></span>     | <span data-ttu-id="9cf90-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf90-137">Type</span></span>   |<span data-ttu-id="9cf90-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf90-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cf90-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="9cf90-139">bccRecipients</span></span>|<span data-ttu-id="9cf90-140">Destinatário</span><span class="sxs-lookup"><span data-stu-id="9cf90-140">Recipient</span></span>|<span data-ttu-id="9cf90-141">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-141">The Bcc recipients for the message.</span></span> <span data-ttu-id="9cf90-142">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-142">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9cf90-143">categories</span><span class="sxs-lookup"><span data-stu-id="9cf90-143">categories</span></span>|<span data-ttu-id="9cf90-144">String collection</span><span class="sxs-lookup"><span data-stu-id="9cf90-144">String collection</span></span>|<span data-ttu-id="9cf90-145">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-145">The categories associated with the message.</span></span>|
|<span data-ttu-id="9cf90-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="9cf90-146">ccRecipients</span></span>|<span data-ttu-id="9cf90-147">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="9cf90-147">Recipient collection</span></span>|<span data-ttu-id="9cf90-148">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-148">The Cc recipients for the message.</span></span> <span data-ttu-id="9cf90-149">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-149">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9cf90-150">from</span><span class="sxs-lookup"><span data-stu-id="9cf90-150">from</span></span>|<span data-ttu-id="9cf90-151">Destinatário</span><span class="sxs-lookup"><span data-stu-id="9cf90-151">Recipient</span></span>|<span data-ttu-id="9cf90-152">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="9cf90-153">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-153">Updatable only if isDraft = true.</span></span> <span data-ttu-id="9cf90-154">Deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="9cf90-154">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="9cf90-155">importance</span><span class="sxs-lookup"><span data-stu-id="9cf90-155">importance</span></span>|<span data-ttu-id="9cf90-156">String</span><span class="sxs-lookup"><span data-stu-id="9cf90-156">String</span></span>|<span data-ttu-id="9cf90-p109">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="9cf90-p109">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="9cf90-159">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="9cf90-159">inferenceClassification</span></span> | <span data-ttu-id="9cf90-160">String</span><span class="sxs-lookup"><span data-stu-id="9cf90-160">String</span></span> | <span data-ttu-id="9cf90-p110">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="9cf90-p110">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="9cf90-163">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="9cf90-163">internetMessageId</span></span> |<span data-ttu-id="9cf90-164">String</span><span class="sxs-lookup"><span data-stu-id="9cf90-164">String</span></span> |<span data-ttu-id="9cf90-165">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="9cf90-165">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="9cf90-166">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-166">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9cf90-167">isRead</span><span class="sxs-lookup"><span data-stu-id="9cf90-167">isRead</span></span>|<span data-ttu-id="9cf90-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf90-168">Boolean</span></span>|<span data-ttu-id="9cf90-169">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="9cf90-169">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="9cf90-170">replyTo</span><span class="sxs-lookup"><span data-stu-id="9cf90-170">replyTo</span></span>|<span data-ttu-id="9cf90-171">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="9cf90-171">Recipient collection</span></span>|<span data-ttu-id="9cf90-172">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="9cf90-172">The email addresses to use when replying.</span></span> <span data-ttu-id="9cf90-173">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-173">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9cf90-174">sender</span><span class="sxs-lookup"><span data-stu-id="9cf90-174">sender</span></span>|<span data-ttu-id="9cf90-175">Destinatário</span><span class="sxs-lookup"><span data-stu-id="9cf90-175">Recipient</span></span>|<span data-ttu-id="9cf90-176">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-176">The account that is actually used to generate the message.</span></span> <span data-ttu-id="9cf90-177">Somente se atualizável isDraft = verdadeiro e quando enviando uma mensagem a partir de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviando uma mensagem como um [representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="9cf90-177">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="9cf90-178">Em qualquer caso, o valor deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="9cf90-178">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="9cf90-179">toRecipients</span><span class="sxs-lookup"><span data-stu-id="9cf90-179">toRecipients</span></span>|<span data-ttu-id="9cf90-180">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="9cf90-180">Recipient collection</span></span>|<span data-ttu-id="9cf90-181">Dos destinatários da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-181">The To recipients for the message.</span></span> <span data-ttu-id="9cf90-182">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9cf90-183">corpo</span><span class="sxs-lookup"><span data-stu-id="9cf90-183">body</span></span>|<span data-ttu-id="9cf90-184">ItemBody</span><span class="sxs-lookup"><span data-stu-id="9cf90-184">ItemBody</span></span>|<span data-ttu-id="9cf90-185">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-185">The body of the message.</span></span> <span data-ttu-id="9cf90-186">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="9cf90-187">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="9cf90-187">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="9cf90-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf90-188">Boolean</span></span>|<span data-ttu-id="9cf90-189">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-189">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="9cf90-190">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="9cf90-190">isReadReceiptRequested</span></span>|<span data-ttu-id="9cf90-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf90-191">Boolean</span></span>|<span data-ttu-id="9cf90-192">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-192">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="9cf90-193">subject</span><span class="sxs-lookup"><span data-stu-id="9cf90-193">subject</span></span>|<span data-ttu-id="9cf90-194">String</span><span class="sxs-lookup"><span data-stu-id="9cf90-194">String</span></span>|<span data-ttu-id="9cf90-195">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="9cf90-195">The subject of the message.</span></span> <span data-ttu-id="9cf90-196">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="9cf90-196">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="9cf90-197">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="9cf90-197">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="9cf90-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf90-198">Response</span></span>

<span data-ttu-id="9cf90-199">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf90-199">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cf90-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cf90-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cf90-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf90-201">Request</span></span>
<span data-ttu-id="9cf90-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cf90-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
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
##### <a name="response"></a><span data-ttu-id="9cf90-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf90-203">Response</span></span>
<span data-ttu-id="9cf90-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cf90-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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

## <a name="see-also"></a><span data-ttu-id="9cf90-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="9cf90-207">See also</span></span>

- [<span data-ttu-id="9cf90-208">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="9cf90-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9cf90-209">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="9cf90-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9cf90-210">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="9cf90-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
