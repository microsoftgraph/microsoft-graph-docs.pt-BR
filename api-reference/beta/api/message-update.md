---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6553365ffd31c56348c930be5562ebd65abc734d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977763"
---
# <a name="update-message"></a><span data-ttu-id="d9226-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="d9226-103">Update message</span></span>

> <span data-ttu-id="d9226-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9226-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9226-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9226-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9226-106">Atualize as propriedades de um objeto de mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-106">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9226-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9226-107">Permissions</span></span>
<span data-ttu-id="d9226-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9226-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9226-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9226-110">Permission type</span></span>      | <span data-ttu-id="d9226-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9226-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9226-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9226-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9226-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9226-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d9226-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9226-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9226-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9226-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d9226-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9226-116">Application</span></span> | <span data-ttu-id="d9226-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9226-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9226-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9226-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d9226-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9226-119">Request headers</span></span>
| <span data-ttu-id="d9226-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d9226-120">Name</span></span>       | <span data-ttu-id="d9226-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9226-121">Type</span></span> | <span data-ttu-id="d9226-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9226-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d9226-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9226-123">Authorization</span></span>  | <span data-ttu-id="d9226-124">string</span><span class="sxs-lookup"><span data-stu-id="d9226-124">string</span></span>  | <span data-ttu-id="d9226-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9226-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9226-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9226-127">Content-Type</span></span> | <span data-ttu-id="d9226-128">string</span><span class="sxs-lookup"><span data-stu-id="d9226-128">string</span></span>  | <span data-ttu-id="d9226-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9226-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d9226-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9226-131">Request body</span></span>
<span data-ttu-id="d9226-132">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d9226-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d9226-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d9226-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d9226-134">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d9226-134">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="d9226-135">As propriedades a seguir podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d9226-135">The following properties can be updated.</span></span>

| <span data-ttu-id="d9226-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9226-136">Property</span></span>     | <span data-ttu-id="d9226-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9226-137">Type</span></span>   |<span data-ttu-id="d9226-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9226-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9226-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="d9226-139">bccRecipients</span></span>|<span data-ttu-id="d9226-140">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d9226-140">Recipient</span></span>|<span data-ttu-id="d9226-141">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-141">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="d9226-142">corpo</span><span class="sxs-lookup"><span data-stu-id="d9226-142">body</span></span>|<span data-ttu-id="d9226-143">ItemBody</span><span class="sxs-lookup"><span data-stu-id="d9226-143">ItemBody</span></span>|<span data-ttu-id="d9226-144">O corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-144">The body of the message.</span></span> <span data-ttu-id="d9226-145">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d9226-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d9226-146">categories</span><span class="sxs-lookup"><span data-stu-id="d9226-146">categories</span></span>|<span data-ttu-id="d9226-147">String collection</span><span class="sxs-lookup"><span data-stu-id="d9226-147">String collection</span></span>|<span data-ttu-id="d9226-148">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-148">The categories associated with the message.</span></span>|
|<span data-ttu-id="d9226-149">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="d9226-149">ccRecipients</span></span>|<span data-ttu-id="d9226-150">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d9226-150">Recipient collection</span></span>|<span data-ttu-id="d9226-151">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-151">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="d9226-152">from</span><span class="sxs-lookup"><span data-stu-id="d9226-152">from</span></span>|<span data-ttu-id="d9226-153">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d9226-153">Recipient</span></span>|<span data-ttu-id="d9226-154">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-154">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="d9226-155">Deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="d9226-155">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="d9226-156">importance</span><span class="sxs-lookup"><span data-stu-id="d9226-156">importance</span></span>|<span data-ttu-id="d9226-157">String</span><span class="sxs-lookup"><span data-stu-id="d9226-157">String</span></span>|<span data-ttu-id="d9226-p108">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="d9226-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="d9226-160">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="d9226-160">inferenceClassification</span></span> | <span data-ttu-id="d9226-161">String</span><span class="sxs-lookup"><span data-stu-id="d9226-161">String</span></span> | <span data-ttu-id="d9226-p109">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="d9226-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="d9226-164">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="d9226-164">internetMessageId</span></span> |<span data-ttu-id="d9226-165">String</span><span class="sxs-lookup"><span data-stu-id="d9226-165">String</span></span> |<span data-ttu-id="d9226-166">A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span><span class="sxs-lookup"><span data-stu-id="d9226-166">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="d9226-167">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d9226-167">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d9226-168">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d9226-168">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="d9226-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9226-169">Boolean</span></span>|<span data-ttu-id="d9226-170">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-170">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d9226-171">isRead</span><span class="sxs-lookup"><span data-stu-id="d9226-171">isRead</span></span>|<span data-ttu-id="d9226-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9226-172">Boolean</span></span>|<span data-ttu-id="d9226-173">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="d9226-173">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="d9226-174">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d9226-174">isReadReceiptRequested</span></span>|<span data-ttu-id="d9226-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9226-175">Boolean</span></span>|<span data-ttu-id="d9226-176">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-176">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d9226-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d9226-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="d9226-178">Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d9226-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d9226-179">A coleção de propriedades estendidas de múltiplos valores definidos para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-179">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="d9226-180">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d9226-180">Nullable.</span></span>|
|<span data-ttu-id="d9226-181">replyTo</span><span class="sxs-lookup"><span data-stu-id="d9226-181">replyTo</span></span>|<span data-ttu-id="d9226-182">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d9226-182">Recipient collection</span></span>|<span data-ttu-id="d9226-183">Os endereços de email a serem usados ao responder.</span><span class="sxs-lookup"><span data-stu-id="d9226-183">The email addresses to use when replying.</span></span> <span data-ttu-id="d9226-184">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d9226-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d9226-185">sender</span><span class="sxs-lookup"><span data-stu-id="d9226-185">sender</span></span>|<span data-ttu-id="d9226-186">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d9226-186">Recipient</span></span>|<span data-ttu-id="d9226-187">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-187">The account that is actually used to generate the message.</span></span> <span data-ttu-id="d9226-188">Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviando uma mensagem como um [representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="d9226-188">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="d9226-189">Em qualquer caso, o valor deve corresponder à caixa de correio real usada.</span><span class="sxs-lookup"><span data-stu-id="d9226-189">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="d9226-190">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d9226-190">singleValueExtendedProperties</span></span>|<span data-ttu-id="d9226-191">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d9226-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d9226-192">A coleção de propriedades estendidas de valor único definidas para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-192">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="d9226-193">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d9226-193">Nullable.</span></span>|
|<span data-ttu-id="d9226-194">subject</span><span class="sxs-lookup"><span data-stu-id="d9226-194">subject</span></span>|<span data-ttu-id="d9226-195">String</span><span class="sxs-lookup"><span data-stu-id="d9226-195">String</span></span>|<span data-ttu-id="d9226-196">O assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-196">The subject of the message.</span></span> <span data-ttu-id="d9226-197">Somente se atualizável isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d9226-197">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d9226-198">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d9226-198">toRecipients</span></span>|<span data-ttu-id="d9226-199">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d9226-199">Recipient collection</span></span>|<span data-ttu-id="d9226-200">Dos destinatários da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d9226-200">The To recipients for the message.</span></span> |

<span data-ttu-id="d9226-201">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="d9226-201">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="d9226-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9226-202">Response</span></span>

<span data-ttu-id="d9226-203">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9226-203">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9226-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9226-204">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9226-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9226-205">Request</span></span>
<span data-ttu-id="d9226-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9226-206">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d9226-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9226-207">Response</span></span>
<span data-ttu-id="d9226-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9226-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d9226-211">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9226-211">See also</span></span>

- [<span data-ttu-id="d9226-212">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d9226-212">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d9226-213">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="d9226-213">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d9226-214">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="d9226-214">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
