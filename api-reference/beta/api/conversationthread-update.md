---
title: Atualizar conversationthread
description: Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e7948c9f988e7d829f6a49292b0b09ba1f7eda52
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047004"
---
# <a name="update-conversationthread"></a><span data-ttu-id="9a492-103">Atualizar conversationthread</span><span class="sxs-lookup"><span data-stu-id="9a492-103">Update conversationthread</span></span>

<span data-ttu-id="9a492-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a492-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a492-105">Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.</span><span class="sxs-lookup"><span data-stu-id="9a492-105">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a492-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a492-106">Permissions</span></span>
<span data-ttu-id="9a492-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a492-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a492-109">Permission type</span></span>      | <span data-ttu-id="9a492-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a492-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a492-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a492-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a492-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a492-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a492-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a492-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a492-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a492-114">Not supported.</span></span>    |
|<span data-ttu-id="9a492-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a492-115">Application</span></span> | <span data-ttu-id="9a492-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a492-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a492-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a492-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9a492-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a492-118">Request headers</span></span>
| <span data-ttu-id="9a492-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a492-119">Header</span></span>       | <span data-ttu-id="9a492-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9a492-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a492-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a492-121">Authorization</span></span>  | <span data-ttu-id="9a492-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a492-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9a492-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a492-124">Content-Type</span></span>  | <span data-ttu-id="9a492-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a492-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a492-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a492-127">Request body</span></span>
<span data-ttu-id="9a492-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9a492-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a492-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a492-131">Property</span></span>     | <span data-ttu-id="9a492-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a492-132">Type</span></span>   |<span data-ttu-id="9a492-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a492-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a492-134">isLocked</span><span class="sxs-lookup"><span data-stu-id="9a492-134">isLocked</span></span>|<span data-ttu-id="9a492-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a492-135">Boolean</span></span>|<span data-ttu-id="9a492-p105">Indica se o thread está bloqueado. Defina como `true` para proibir a postagem.</span><span class="sxs-lookup"><span data-stu-id="9a492-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="9a492-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a492-138">Response</span></span>

<span data-ttu-id="9a492-139">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a492-139">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a492-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a492-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a492-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a492-141">Request</span></span>
<span data-ttu-id="9a492-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a492-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a492-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a492-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
# <a name="c"></a>[<span data-ttu-id="9a492-144">C#</span><span class="sxs-lookup"><span data-stu-id="9a492-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a492-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a492-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a492-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a492-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a492-147">Java</span><span class="sxs-lookup"><span data-stu-id="9a492-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a492-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a492-148">Response</span></span>
<span data-ttu-id="9a492-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a492-149">Here is an example of the response.</span></span> <span data-ttu-id="9a492-150">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a492-150">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


