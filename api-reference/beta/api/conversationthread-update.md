---
title: Atualizar conversationthread
description: Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 39e837656289f14978e15f723ddbc39fd4f80d8e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261051"
---
# <a name="update-conversationthread"></a><span data-ttu-id="8ff39-103">Atualizar conversationthread</span><span class="sxs-lookup"><span data-stu-id="8ff39-103">Update conversationthread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff39-104">Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.</span><span class="sxs-lookup"><span data-stu-id="8ff39-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ff39-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ff39-105">Permissions</span></span>
<span data-ttu-id="8ff39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff39-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff39-108">Permission type</span></span>      | <span data-ttu-id="8ff39-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ff39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff39-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff39-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff39-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ff39-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff39-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ff39-113">Not supported.</span></span>    |
|<span data-ttu-id="8ff39-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff39-114">Application</span></span> | <span data-ttu-id="8ff39-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff39-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff39-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff39-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8ff39-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff39-117">Request headers</span></span>
| <span data-ttu-id="8ff39-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ff39-118">Header</span></span>       | <span data-ttu-id="8ff39-119">Valor</span><span class="sxs-lookup"><span data-stu-id="8ff39-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ff39-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff39-120">Authorization</span></span>  | <span data-ttu-id="8ff39-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff39-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ff39-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ff39-123">Content-Type</span></span>  | <span data-ttu-id="8ff39-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff39-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ff39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff39-126">Request body</span></span>
<span data-ttu-id="8ff39-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8ff39-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8ff39-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ff39-130">Property</span></span>     | <span data-ttu-id="8ff39-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff39-131">Type</span></span>   |<span data-ttu-id="8ff39-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff39-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ff39-133">isLocked</span><span class="sxs-lookup"><span data-stu-id="8ff39-133">isLocked</span></span>|<span data-ttu-id="8ff39-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="8ff39-134">Boolean</span></span>|<span data-ttu-id="8ff39-p105">Indica se o thread está bloqueado. Defina como `true` para proibir a postagem.</span><span class="sxs-lookup"><span data-stu-id="8ff39-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="8ff39-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff39-137">Response</span></span>

<span data-ttu-id="8ff39-138">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff39-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ff39-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff39-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff39-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff39-140">Request</span></span>
<span data-ttu-id="8ff39-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff39-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="8ff39-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff39-142">Response</span></span>
<span data-ttu-id="8ff39-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff39-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8ff39-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8ff39-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8ff39-147">C#</span><span class="sxs-lookup"><span data-stu-id="8ff39-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_conversationthread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ff39-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ff39-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_conversationthread-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8ff39-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8ff39-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_conversationthread-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/conversationthread-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversationthread-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationthread-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
