---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto mensagem.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5c087c9ecb423d305681567b68bfb8726dbe3e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456877"
---
# <a name="update-message"></a><span data-ttu-id="54fa5-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="54fa5-103">Update message</span></span>

<span data-ttu-id="54fa5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="54fa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54fa5-105">Atualizar as propriedades de um objeto mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-105">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54fa5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54fa5-106">Permissions</span></span>
<span data-ttu-id="54fa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54fa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54fa5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54fa5-109">Permission type</span></span>      | <span data-ttu-id="54fa5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54fa5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54fa5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54fa5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54fa5-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54fa5-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="54fa5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54fa5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54fa5-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54fa5-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="54fa5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54fa5-115">Application</span></span> | <span data-ttu-id="54fa5-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54fa5-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="54fa5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54fa5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="54fa5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54fa5-118">Request headers</span></span>
| <span data-ttu-id="54fa5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54fa5-119">Name</span></span>       | <span data-ttu-id="54fa5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="54fa5-120">Type</span></span> | <span data-ttu-id="54fa5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="54fa5-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54fa5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="54fa5-122">Authorization</span></span>  | <span data-ttu-id="54fa5-123">string</span><span class="sxs-lookup"><span data-stu-id="54fa5-123">string</span></span>  | <span data-ttu-id="54fa5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54fa5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54fa5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54fa5-126">Content-Type</span></span> | <span data-ttu-id="54fa5-127">string</span><span class="sxs-lookup"><span data-stu-id="54fa5-127">string</span></span>  | <span data-ttu-id="54fa5-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54fa5-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="54fa5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54fa5-130">Request body</span></span>
<span data-ttu-id="54fa5-131">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="54fa5-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="54fa5-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="54fa5-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="54fa5-133">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="54fa5-133">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="54fa5-134">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="54fa5-134">The following properties can be updated.</span></span>

| <span data-ttu-id="54fa5-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54fa5-135">Property</span></span>     | <span data-ttu-id="54fa5-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="54fa5-136">Type</span></span>   |<span data-ttu-id="54fa5-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="54fa5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54fa5-138">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="54fa5-138">bccRecipients</span></span>|<span data-ttu-id="54fa5-139">Destinatário</span><span class="sxs-lookup"><span data-stu-id="54fa5-139">Recipient</span></span>|<span data-ttu-id="54fa5-140">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-140">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="54fa5-141">corpo</span><span class="sxs-lookup"><span data-stu-id="54fa5-141">body</span></span>|<span data-ttu-id="54fa5-142">ItemBody</span><span class="sxs-lookup"><span data-stu-id="54fa5-142">ItemBody</span></span>|<span data-ttu-id="54fa5-143">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-143">The body of the message.</span></span> <span data-ttu-id="54fa5-144">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="54fa5-144">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="54fa5-145">Categorias</span><span class="sxs-lookup"><span data-stu-id="54fa5-145">categories</span></span>|<span data-ttu-id="54fa5-146">String collection</span><span class="sxs-lookup"><span data-stu-id="54fa5-146">String collection</span></span>|<span data-ttu-id="54fa5-147">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-147">The categories associated with the message.</span></span>|
|<span data-ttu-id="54fa5-148">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="54fa5-148">ccRecipients</span></span>|<span data-ttu-id="54fa5-149">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="54fa5-149">Recipient collection</span></span>|<span data-ttu-id="54fa5-150">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-150">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="54fa5-151">sinalizador</span><span class="sxs-lookup"><span data-stu-id="54fa5-151">flag</span></span>|[<span data-ttu-id="54fa5-152">followupFlag</span><span class="sxs-lookup"><span data-stu-id="54fa5-152">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="54fa5-153">O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-153">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="54fa5-154">from</span><span class="sxs-lookup"><span data-stu-id="54fa5-154">from</span></span>|<span data-ttu-id="54fa5-155">Destinatário</span><span class="sxs-lookup"><span data-stu-id="54fa5-155">Recipient</span></span>|<span data-ttu-id="54fa5-156">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-156">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="54fa5-157">Devem corresponder à caixa de correio real que foi usada.</span><span class="sxs-lookup"><span data-stu-id="54fa5-157">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="54fa5-158">importância</span><span class="sxs-lookup"><span data-stu-id="54fa5-158">importance</span></span>|<span data-ttu-id="54fa5-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54fa5-159">String</span></span>|<span data-ttu-id="54fa5-p107">A importância da mensagem. Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="54fa5-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="54fa5-162">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="54fa5-162">inferenceClassification</span></span> | <span data-ttu-id="54fa5-163">String</span><span class="sxs-lookup"><span data-stu-id="54fa5-163">String</span></span> | <span data-ttu-id="54fa5-p108">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="54fa5-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="54fa5-166">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="54fa5-166">internetMessageId</span></span> |<span data-ttu-id="54fa5-167">String</span><span class="sxs-lookup"><span data-stu-id="54fa5-167">String</span></span> |<span data-ttu-id="54fa5-168">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="54fa5-168">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="54fa5-169">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="54fa5-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="54fa5-170">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="54fa5-170">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="54fa5-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fa5-171">Boolean</span></span>|<span data-ttu-id="54fa5-172">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-172">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="54fa5-173">isRead</span><span class="sxs-lookup"><span data-stu-id="54fa5-173">isRead</span></span>|<span data-ttu-id="54fa5-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fa5-174">Boolean</span></span>|<span data-ttu-id="54fa5-175">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="54fa5-175">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="54fa5-176">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="54fa5-176">isReadReceiptRequested</span></span>|<span data-ttu-id="54fa5-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fa5-177">Boolean</span></span>|<span data-ttu-id="54fa5-178">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-178">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="54fa5-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="54fa5-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="54fa5-180">Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="54fa5-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="54fa5-181">A coleção de propriedades estendidas de vários valores definidas para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-181">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="54fa5-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="54fa5-182">Nullable.</span></span>|
|<span data-ttu-id="54fa5-183">replyTo</span><span class="sxs-lookup"><span data-stu-id="54fa5-183">replyTo</span></span>|<span data-ttu-id="54fa5-184">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="54fa5-184">Recipient collection</span></span>|<span data-ttu-id="54fa5-185">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="54fa5-185">The email addresses to use when replying.</span></span> <span data-ttu-id="54fa5-186">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="54fa5-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="54fa5-187">remetente</span><span class="sxs-lookup"><span data-stu-id="54fa5-187">sender</span></span>|<span data-ttu-id="54fa5-188">Destinatário</span><span class="sxs-lookup"><span data-stu-id="54fa5-188">Recipient</span></span>|<span data-ttu-id="54fa5-189">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-189">The account that is actually used to generate the message.</span></span> <span data-ttu-id="54fa5-190">Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), ou enviar uma mensagem como um [delegado](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="54fa5-190">Updatable when sending a message from a [shared mailbox](/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="54fa5-191">De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada.</span><span class="sxs-lookup"><span data-stu-id="54fa5-191">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="54fa5-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="54fa5-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="54fa5-193">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="54fa5-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="54fa5-194">A coleção de propriedades estendidas de valor único definidas para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-194">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="54fa5-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="54fa5-195">Nullable.</span></span>|
|<span data-ttu-id="54fa5-196">Assunto</span><span class="sxs-lookup"><span data-stu-id="54fa5-196">subject</span></span>|<span data-ttu-id="54fa5-197">String</span><span class="sxs-lookup"><span data-stu-id="54fa5-197">String</span></span>|<span data-ttu-id="54fa5-198">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-198">The subject of the message.</span></span> <span data-ttu-id="54fa5-199">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="54fa5-199">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="54fa5-200">toRecipients</span><span class="sxs-lookup"><span data-stu-id="54fa5-200">toRecipients</span></span>|<span data-ttu-id="54fa5-201">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="54fa5-201">Recipient collection</span></span>|<span data-ttu-id="54fa5-202">Os destinatários Para da mensagem.</span><span class="sxs-lookup"><span data-stu-id="54fa5-202">The To recipients for the message.</span></span> |

<span data-ttu-id="54fa5-203">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="54fa5-203">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="54fa5-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="54fa5-204">Response</span></span>

<span data-ttu-id="54fa5-205">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54fa5-205">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54fa5-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54fa5-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54fa5-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54fa5-207">Request</span></span>
<span data-ttu-id="54fa5-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54fa5-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54fa5-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="54fa5-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="54fa5-210">C#</span><span class="sxs-lookup"><span data-stu-id="54fa5-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54fa5-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54fa5-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54fa5-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="54fa5-212">Response</span></span>
<span data-ttu-id="54fa5-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54fa5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="54fa5-216">Confira também</span><span class="sxs-lookup"><span data-stu-id="54fa5-216">See also</span></span>

- [<span data-ttu-id="54fa5-217">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="54fa5-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="54fa5-218">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="54fa5-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="54fa5-219">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="54fa5-219">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
