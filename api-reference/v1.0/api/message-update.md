---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto mensagem.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 40cbde5b0f5c8f7c6047336ddfd569d72388ef59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444544"
---
# <a name="update-message"></a><span data-ttu-id="c763c-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="c763c-103">Update message</span></span>

<span data-ttu-id="c763c-104">Atualizar as propriedades de um objeto mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c763c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c763c-105">Permissions</span></span>
<span data-ttu-id="c763c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c763c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c763c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c763c-108">Permission type</span></span>      | <span data-ttu-id="c763c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c763c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c763c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c763c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c763c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c763c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c763c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c763c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c763c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c763c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c763c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c763c-114">Application</span></span> | <span data-ttu-id="c763c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c763c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c763c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c763c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c763c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c763c-117">Request headers</span></span>
| <span data-ttu-id="c763c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c763c-118">Name</span></span>       | <span data-ttu-id="c763c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c763c-119">Type</span></span> | <span data-ttu-id="c763c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c763c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c763c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c763c-121">Authorization</span></span>  | <span data-ttu-id="c763c-122">string</span><span class="sxs-lookup"><span data-stu-id="c763c-122">string</span></span>  | <span data-ttu-id="c763c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c763c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c763c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c763c-125">Content-Type</span></span> | <span data-ttu-id="c763c-126">string</span><span class="sxs-lookup"><span data-stu-id="c763c-126">string</span></span>  | <span data-ttu-id="c763c-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c763c-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="c763c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c763c-129">Request body</span></span>
<span data-ttu-id="c763c-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c763c-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c763c-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c763c-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c763c-132">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c763c-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="c763c-133">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="c763c-133">The following properties can be updated.</span></span>

| <span data-ttu-id="c763c-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c763c-134">Property</span></span>     | <span data-ttu-id="c763c-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="c763c-135">Type</span></span>   |<span data-ttu-id="c763c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c763c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c763c-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="c763c-137">bccRecipients</span></span>|<span data-ttu-id="c763c-138">Destinatário</span><span class="sxs-lookup"><span data-stu-id="c763c-138">Recipient</span></span>|<span data-ttu-id="c763c-139">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="c763c-140">corpo</span><span class="sxs-lookup"><span data-stu-id="c763c-140">body</span></span>|<span data-ttu-id="c763c-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="c763c-141">ItemBody</span></span>|<span data-ttu-id="c763c-142">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-142">The body of the message.</span></span> <span data-ttu-id="c763c-143">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="c763c-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="c763c-144">Categorias</span><span class="sxs-lookup"><span data-stu-id="c763c-144">categories</span></span>|<span data-ttu-id="c763c-145">String collection</span><span class="sxs-lookup"><span data-stu-id="c763c-145">String collection</span></span>|<span data-ttu-id="c763c-146">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="c763c-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="c763c-147">ccRecipients</span></span>|<span data-ttu-id="c763c-148">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="c763c-148">Recipient collection</span></span>|<span data-ttu-id="c763c-149">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="c763c-150">sinalizador</span><span class="sxs-lookup"><span data-stu-id="c763c-150">flag</span></span>|[<span data-ttu-id="c763c-151">followupFlag</span><span class="sxs-lookup"><span data-stu-id="c763c-151">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="c763c-152">O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-152">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="c763c-153">from</span><span class="sxs-lookup"><span data-stu-id="c763c-153">from</span></span>|<span data-ttu-id="c763c-154">Destinatário</span><span class="sxs-lookup"><span data-stu-id="c763c-154">Recipient</span></span>|<span data-ttu-id="c763c-155">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-155">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="c763c-156">Devem corresponder à caixa de correio real que foi usada.</span><span class="sxs-lookup"><span data-stu-id="c763c-156">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="c763c-157">importância</span><span class="sxs-lookup"><span data-stu-id="c763c-157">importance</span></span>|<span data-ttu-id="c763c-158">String</span><span class="sxs-lookup"><span data-stu-id="c763c-158">String</span></span>|<span data-ttu-id="c763c-159">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-159">The importance of the message.</span></span> <span data-ttu-id="c763c-160">Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="c763c-160">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="c763c-161">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="c763c-161">inferenceClassification</span></span> | <span data-ttu-id="c763c-162">String</span><span class="sxs-lookup"><span data-stu-id="c763c-162">String</span></span> | <span data-ttu-id="c763c-163">A classificação da mensagem para o usuário, com base na relevância ou importância deduzida ou em uma substituição explícita.</span><span class="sxs-lookup"><span data-stu-id="c763c-163">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="c763c-164">Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="c763c-164">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="c763c-165">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="c763c-165">internetMessageId</span></span> |<span data-ttu-id="c763c-166">String</span><span class="sxs-lookup"><span data-stu-id="c763c-166">String</span></span> |<span data-ttu-id="c763c-167">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="c763c-167">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="c763c-168">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="c763c-168">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="c763c-169">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c763c-169">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="c763c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="c763c-170">Boolean</span></span>|<span data-ttu-id="c763c-171">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-171">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="c763c-172">isRead</span><span class="sxs-lookup"><span data-stu-id="c763c-172">isRead</span></span>|<span data-ttu-id="c763c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c763c-173">Boolean</span></span>|<span data-ttu-id="c763c-174">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="c763c-174">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="c763c-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c763c-175">isReadReceiptRequested</span></span>|<span data-ttu-id="c763c-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c763c-176">Boolean</span></span>|<span data-ttu-id="c763c-177">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="c763c-178">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c763c-178">multiValueExtendedProperties</span></span>|<span data-ttu-id="c763c-179">Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c763c-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c763c-180">A coleção de propriedades estendidas de vários valores definidas para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-180">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="c763c-181">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c763c-181">Nullable.</span></span>|
|<span data-ttu-id="c763c-182">replyTo</span><span class="sxs-lookup"><span data-stu-id="c763c-182">replyTo</span></span>|<span data-ttu-id="c763c-183">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="c763c-183">Recipient collection</span></span>|<span data-ttu-id="c763c-184">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="c763c-184">The email addresses to use when replying.</span></span> <span data-ttu-id="c763c-185">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="c763c-185">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="c763c-186">remetente</span><span class="sxs-lookup"><span data-stu-id="c763c-186">sender</span></span>|<span data-ttu-id="c763c-187">Destinatário</span><span class="sxs-lookup"><span data-stu-id="c763c-187">Recipient</span></span>|<span data-ttu-id="c763c-188">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-188">The account that is actually used to generate the message.</span></span> <span data-ttu-id="c763c-189">Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](https://docs.microsoft.com/pt-BR/exchange/collaboration/shared-mailboxes/shared-mailboxes), ou enviar uma mensagem como um [delegado](https://support.office.com/pt-BR/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="c763c-189">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="c763c-190">De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada.</span><span class="sxs-lookup"><span data-stu-id="c763c-190">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="c763c-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c763c-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="c763c-192">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c763c-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c763c-193">A coleção de propriedades estendidas de valor único definidas para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-193">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="c763c-194">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c763c-194">Nullable.</span></span>|
|<span data-ttu-id="c763c-195">Assunto</span><span class="sxs-lookup"><span data-stu-id="c763c-195">subject</span></span>|<span data-ttu-id="c763c-196">String</span><span class="sxs-lookup"><span data-stu-id="c763c-196">String</span></span>|<span data-ttu-id="c763c-197">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-197">The subject of the message.</span></span> <span data-ttu-id="c763c-198">Atualizável apenas se IsDraft = true.</span><span class="sxs-lookup"><span data-stu-id="c763c-198">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="c763c-199">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c763c-199">toRecipients</span></span>|<span data-ttu-id="c763c-200">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="c763c-200">Recipient collection</span></span>|<span data-ttu-id="c763c-201">Os destinatários Para da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c763c-201">The To recipients for the message.</span></span>|

<span data-ttu-id="c763c-202">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="c763c-202">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="c763c-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="c763c-203">Response</span></span>

<span data-ttu-id="c763c-204">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c763c-204">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c763c-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c763c-205">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c763c-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c763c-206">Request</span></span>
<span data-ttu-id="c763c-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c763c-207">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c763c-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="c763c-208">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c763c-209">C#</span><span class="sxs-lookup"><span data-stu-id="c763c-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c763c-210">Javascript</span><span class="sxs-lookup"><span data-stu-id="c763c-210">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c763c-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="c763c-211">Response</span></span>
<span data-ttu-id="c763c-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c763c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c763c-215">Confira também</span><span class="sxs-lookup"><span data-stu-id="c763c-215">See also</span></span>

- [<span data-ttu-id="c763c-216">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c763c-216">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c763c-217">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c763c-217">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
