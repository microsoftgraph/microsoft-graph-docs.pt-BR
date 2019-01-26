---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 78f030e49f5e9caad5cf505be0118eee5b732752
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573666"
---
# <a name="update-message"></a><span data-ttu-id="036f4-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="036f4-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="036f4-104">Atualize as propriedades de um objeto de mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="036f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="036f4-105">Permissions</span></span>
<span data-ttu-id="036f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="036f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="036f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="036f4-108">Permission type</span></span>      | <span data-ttu-id="036f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="036f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="036f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="036f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="036f4-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="036f4-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="036f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="036f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="036f4-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="036f4-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="036f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="036f4-114">Application</span></span> | <span data-ttu-id="036f4-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="036f4-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="036f4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="036f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="036f4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="036f4-117">Request headers</span></span>
| <span data-ttu-id="036f4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="036f4-118">Name</span></span>       | <span data-ttu-id="036f4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="036f4-119">Type</span></span> | <span data-ttu-id="036f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="036f4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="036f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="036f4-121">Authorization</span></span>  | <span data-ttu-id="036f4-122">string</span><span class="sxs-lookup"><span data-stu-id="036f4-122">string</span></span>  | <span data-ttu-id="036f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="036f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="036f4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="036f4-125">Content-Type</span></span> | <span data-ttu-id="036f4-126">string</span><span class="sxs-lookup"><span data-stu-id="036f4-126">string</span></span>  | <span data-ttu-id="036f4-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="036f4-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="036f4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="036f4-129">Request body</span></span>
<span data-ttu-id="036f4-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="036f4-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="036f4-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="036f4-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="036f4-132">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="036f4-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="036f4-133">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="036f4-133">The following properties can be updated.</span></span>

| <span data-ttu-id="036f4-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="036f4-134">Property</span></span>     | <span data-ttu-id="036f4-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="036f4-135">Type</span></span>   |<span data-ttu-id="036f4-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="036f4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="036f4-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="036f4-137">bccRecipients</span></span>|<span data-ttu-id="036f4-138">Destinatário</span><span class="sxs-lookup"><span data-stu-id="036f4-138">Recipient</span></span>|<span data-ttu-id="036f4-139">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="036f4-140">corpo</span><span class="sxs-lookup"><span data-stu-id="036f4-140">body</span></span>|<span data-ttu-id="036f4-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="036f4-141">ItemBody</span></span>|<span data-ttu-id="036f4-142">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-142">The body of the message.</span></span> <span data-ttu-id="036f4-143">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="036f4-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="036f4-144">categories</span><span class="sxs-lookup"><span data-stu-id="036f4-144">categories</span></span>|<span data-ttu-id="036f4-145">String collection</span><span class="sxs-lookup"><span data-stu-id="036f4-145">String collection</span></span>|<span data-ttu-id="036f4-146">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="036f4-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="036f4-147">ccRecipients</span></span>|<span data-ttu-id="036f4-148">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="036f4-148">Recipient collection</span></span>|<span data-ttu-id="036f4-149">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="036f4-150">from</span><span class="sxs-lookup"><span data-stu-id="036f4-150">from</span></span>|<span data-ttu-id="036f4-151">Destinatário</span><span class="sxs-lookup"><span data-stu-id="036f4-151">Recipient</span></span>|<span data-ttu-id="036f4-152">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="036f4-153">Deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="036f4-153">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="036f4-154">importance</span><span class="sxs-lookup"><span data-stu-id="036f4-154">importance</span></span>|<span data-ttu-id="036f4-155">String</span><span class="sxs-lookup"><span data-stu-id="036f4-155">String</span></span>|<span data-ttu-id="036f4-p107">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="036f4-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="036f4-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="036f4-158">inferenceClassification</span></span> | <span data-ttu-id="036f4-159">String</span><span class="sxs-lookup"><span data-stu-id="036f4-159">String</span></span> | <span data-ttu-id="036f4-p108">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="036f4-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="036f4-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="036f4-162">internetMessageId</span></span> |<span data-ttu-id="036f4-163">String</span><span class="sxs-lookup"><span data-stu-id="036f4-163">String</span></span> |<span data-ttu-id="036f4-164">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="036f4-164">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="036f4-165">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="036f4-165">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="036f4-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="036f4-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="036f4-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="036f4-167">Boolean</span></span>|<span data-ttu-id="036f4-168">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="036f4-169">isRead</span><span class="sxs-lookup"><span data-stu-id="036f4-169">isRead</span></span>|<span data-ttu-id="036f4-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="036f4-170">Boolean</span></span>|<span data-ttu-id="036f4-171">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="036f4-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="036f4-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="036f4-172">isReadReceiptRequested</span></span>|<span data-ttu-id="036f4-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="036f4-173">Boolean</span></span>|<span data-ttu-id="036f4-174">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="036f4-175">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="036f4-175">multiValueLegacyExtendedProperty</span></span>| <span data-ttu-id="036f4-176">Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="036f4-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="036f4-177">A coleção de propriedades estendidas de múltiplos valores definidos para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="036f4-178">Anulável.</span><span class="sxs-lookup"><span data-stu-id="036f4-178">Nullable.</span></span>|
|<span data-ttu-id="036f4-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="036f4-179">replyTo</span></span>|<span data-ttu-id="036f4-180">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="036f4-180">Recipient collection</span></span>|<span data-ttu-id="036f4-181">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="036f4-181">The email addresses to use when replying.</span></span> <span data-ttu-id="036f4-182">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="036f4-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="036f4-183">sender</span><span class="sxs-lookup"><span data-stu-id="036f4-183">sender</span></span>|<span data-ttu-id="036f4-184">Destinatário</span><span class="sxs-lookup"><span data-stu-id="036f4-184">Recipient</span></span>|<span data-ttu-id="036f4-185">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="036f4-186">Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviando uma mensagem como um [representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="036f4-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="036f4-187">Em qualquer caso, o valor deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="036f4-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="036f4-188">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="036f4-188">singleValueLegacyExtendedProperty</span></span>| <span data-ttu-id="036f4-189">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="036f4-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="036f4-190">A coleção de propriedades estendidas de valor único definidas para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="036f4-191">Anulável.</span><span class="sxs-lookup"><span data-stu-id="036f4-191">Nullable.</span></span>|
|<span data-ttu-id="036f4-192">subject</span><span class="sxs-lookup"><span data-stu-id="036f4-192">subject</span></span>|<span data-ttu-id="036f4-193">String</span><span class="sxs-lookup"><span data-stu-id="036f4-193">String</span></span>|<span data-ttu-id="036f4-194">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-194">The subject of the message.</span></span> <span data-ttu-id="036f4-195">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="036f4-195">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="036f4-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="036f4-196">toRecipients</span></span>|<span data-ttu-id="036f4-197">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="036f4-197">Recipient collection</span></span>|<span data-ttu-id="036f4-198">Dos destinatários da mensagem.</span><span class="sxs-lookup"><span data-stu-id="036f4-198">The To recipients for the message.</span></span> |

<span data-ttu-id="036f4-199">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="036f4-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="036f4-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="036f4-200">Response</span></span>

<span data-ttu-id="036f4-201">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="036f4-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="036f4-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="036f4-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="036f4-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="036f4-203">Request</span></span>
<span data-ttu-id="036f4-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="036f4-204">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="036f4-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="036f4-205">Response</span></span>
<span data-ttu-id="036f4-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="036f4-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="036f4-209">Confira também</span><span class="sxs-lookup"><span data-stu-id="036f4-209">See also</span></span>

- [<span data-ttu-id="036f4-210">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="036f4-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="036f4-211">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="036f4-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="036f4-212">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="036f4-212">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/message-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
