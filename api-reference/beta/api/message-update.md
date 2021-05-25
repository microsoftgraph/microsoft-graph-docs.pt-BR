---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto mensagem.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c9c3e9f13a592738ebd4245015a9458a0856dda8
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645336"
---
# <a name="update-message"></a><span data-ttu-id="d92c8-103">Atualizar mensagem</span><span class="sxs-lookup"><span data-stu-id="d92c8-103">Update message</span></span>

<span data-ttu-id="d92c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d92c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d92c8-105">Atualizar as propriedades de um objeto mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-105">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d92c8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d92c8-106">Permissions</span></span>
<span data-ttu-id="d92c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d92c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d92c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d92c8-109">Permission type</span></span>      | <span data-ttu-id="d92c8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d92c8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d92c8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d92c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d92c8-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d92c8-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d92c8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d92c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d92c8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d92c8-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d92c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d92c8-115">Application</span></span> | <span data-ttu-id="d92c8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d92c8-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d92c8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d92c8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d92c8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d92c8-118">Request headers</span></span>
| <span data-ttu-id="d92c8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d92c8-119">Name</span></span>       | <span data-ttu-id="d92c8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d92c8-120">Type</span></span> | <span data-ttu-id="d92c8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d92c8-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d92c8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d92c8-122">Authorization</span></span>  | <span data-ttu-id="d92c8-123">string</span><span class="sxs-lookup"><span data-stu-id="d92c8-123">string</span></span>  | <span data-ttu-id="d92c8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d92c8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d92c8-126">Content-Type</span></span> | <span data-ttu-id="d92c8-127">string</span><span class="sxs-lookup"><span data-stu-id="d92c8-127">string</span></span>  | <span data-ttu-id="d92c8-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d92c8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d92c8-130">Request body</span></span>
<span data-ttu-id="d92c8-p104">No corpo de solicitação, forneça os valores para os campos relevantes que devem ser atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas mudanças de outros valores de propriedade. Para obter o melhor desempenho, você não deve incluir valores existentes que não tenham sido alterados. As seguintes propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following properties can be updated.</span></span>

| <span data-ttu-id="d92c8-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d92c8-135">Property</span></span>     | <span data-ttu-id="d92c8-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d92c8-136">Type</span></span>   |<span data-ttu-id="d92c8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d92c8-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d92c8-138">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="d92c8-138">bccRecipients</span></span>|<span data-ttu-id="d92c8-139">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d92c8-139">Recipient</span></span>|<span data-ttu-id="d92c8-140">Os destinatários Cco da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-140">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="d92c8-141">corpo</span><span class="sxs-lookup"><span data-stu-id="d92c8-141">body</span></span>|<span data-ttu-id="d92c8-142">ItemBody</span><span class="sxs-lookup"><span data-stu-id="d92c8-142">ItemBody</span></span>|<span data-ttu-id="d92c8-p105">O corpo da mensagem. Atualizável somente se isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p105">The body of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d92c8-145">Categorias</span><span class="sxs-lookup"><span data-stu-id="d92c8-145">categories</span></span>|<span data-ttu-id="d92c8-146">String collection</span><span class="sxs-lookup"><span data-stu-id="d92c8-146">String collection</span></span>|<span data-ttu-id="d92c8-147">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-147">The categories associated with the message.</span></span>|
|<span data-ttu-id="d92c8-148">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="d92c8-148">ccRecipients</span></span>|<span data-ttu-id="d92c8-149">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d92c8-149">Recipient collection</span></span>|<span data-ttu-id="d92c8-150">Os destinatários Cc da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-150">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="d92c8-151">sinalizador</span><span class="sxs-lookup"><span data-stu-id="d92c8-151">flag</span></span>|[<span data-ttu-id="d92c8-152">followupFlag</span><span class="sxs-lookup"><span data-stu-id="d92c8-152">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="d92c8-153">O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-153">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="d92c8-154">from</span><span class="sxs-lookup"><span data-stu-id="d92c8-154">from</span></span>|<span data-ttu-id="d92c8-155">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d92c8-155">Recipient</span></span>|<span data-ttu-id="d92c8-156">O proprietário da caixa de correio e o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-156">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="d92c8-157">Devem corresponder à caixa de correio real que foi usada.</span><span class="sxs-lookup"><span data-stu-id="d92c8-157">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="d92c8-158">importância</span><span class="sxs-lookup"><span data-stu-id="d92c8-158">importance</span></span>|<span data-ttu-id="d92c8-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d92c8-159">String</span></span>|<span data-ttu-id="d92c8-p107">A importância da mensagem. Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="d92c8-162">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="d92c8-162">inferenceClassification</span></span> | <span data-ttu-id="d92c8-163">String</span><span class="sxs-lookup"><span data-stu-id="d92c8-163">String</span></span> | <span data-ttu-id="d92c8-p108">A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="d92c8-166">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="d92c8-166">internetMessageId</span></span> |<span data-ttu-id="d92c8-167">String</span><span class="sxs-lookup"><span data-stu-id="d92c8-167">String</span></span> |<span data-ttu-id="d92c8-p109">O ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Atualizável apenas se isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p109">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d92c8-170">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d92c8-170">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="d92c8-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="d92c8-171">Boolean</span></span>|<span data-ttu-id="d92c8-172">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-172">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d92c8-173">isRead</span><span class="sxs-lookup"><span data-stu-id="d92c8-173">isRead</span></span>|<span data-ttu-id="d92c8-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="d92c8-174">Boolean</span></span>|<span data-ttu-id="d92c8-175">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="d92c8-175">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="d92c8-176">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d92c8-176">isReadReceiptRequested</span></span>|<span data-ttu-id="d92c8-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="d92c8-177">Boolean</span></span>|<span data-ttu-id="d92c8-178">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-178">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d92c8-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d92c8-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="d92c8-180">Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d92c8-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d92c8-p110">A coleção de propriedades estendidas de vários valores definidas para a mensagem. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p110">The collection of multi-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="d92c8-183">replyTo</span><span class="sxs-lookup"><span data-stu-id="d92c8-183">replyTo</span></span>|<span data-ttu-id="d92c8-184">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d92c8-184">Recipient collection</span></span>|<span data-ttu-id="d92c8-p111">Os endereços de email para usar ao responder. Atualizável somente se isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p111">The email addresses to use when replying. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d92c8-187">remetente</span><span class="sxs-lookup"><span data-stu-id="d92c8-187">sender</span></span>|<span data-ttu-id="d92c8-188">Destinatário</span><span class="sxs-lookup"><span data-stu-id="d92c8-188">Recipient</span></span>|<span data-ttu-id="d92c8-189">A conta que é realmente usada para gerar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-189">The account that is actually used to generate the message.</span></span> <span data-ttu-id="d92c8-190">Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), ou enviar uma mensagem como um [delegado](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="d92c8-190">Updatable when sending a message from a [shared mailbox](/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="d92c8-191">De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada.</span><span class="sxs-lookup"><span data-stu-id="d92c8-191">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="d92c8-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d92c8-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="d92c8-193">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d92c8-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d92c8-p113">A coleção de propriedades estendidas de valor único definidas para a mensagem. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p113">The collection of single-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="d92c8-196">Assunto</span><span class="sxs-lookup"><span data-stu-id="d92c8-196">subject</span></span>|<span data-ttu-id="d92c8-197">String</span><span class="sxs-lookup"><span data-stu-id="d92c8-197">String</span></span>|<span data-ttu-id="d92c8-p114">O assunto da mensagem. Atualizável somente se isDraft = true.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p114">The subject of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="d92c8-200">toRecipients</span><span class="sxs-lookup"><span data-stu-id="d92c8-200">toRecipients</span></span>|<span data-ttu-id="d92c8-201">Coleção Recipient</span><span class="sxs-lookup"><span data-stu-id="d92c8-201">Recipient collection</span></span>|<span data-ttu-id="d92c8-202">Os destinatários Para da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d92c8-202">The To recipients for the message.</span></span> |

<span data-ttu-id="d92c8-203">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.</span><span class="sxs-lookup"><span data-stu-id="d92c8-203">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="d92c8-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="d92c8-204">Response</span></span>

<span data-ttu-id="d92c8-205">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d92c8-205">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d92c8-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d92c8-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d92c8-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d92c8-207">Request</span></span>
<span data-ttu-id="d92c8-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d92c8-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d92c8-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="d92c8-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d92c8-210">C#</span><span class="sxs-lookup"><span data-stu-id="d92c8-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d92c8-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d92c8-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d92c8-212">Java</span><span class="sxs-lookup"><span data-stu-id="d92c8-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d92c8-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="d92c8-213">Response</span></span>
<span data-ttu-id="d92c8-p115">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="d92c8-p115">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d92c8-216">Confira também</span><span class="sxs-lookup"><span data-stu-id="d92c8-216">See also</span></span>

- [<span data-ttu-id="d92c8-217">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d92c8-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d92c8-218">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="d92c8-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d92c8-219">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="d92c8-219">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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


