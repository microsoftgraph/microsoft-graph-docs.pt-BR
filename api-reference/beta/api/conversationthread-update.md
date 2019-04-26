---
title: Atualizar conversationthread
description: Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e4a2fbeb8e92271294ffa9e3fb065a9d9ae64649
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326113"
---
# <a name="update-conversationthread"></a><span data-ttu-id="9e9c8-103">Atualizar conversationthread</span><span class="sxs-lookup"><span data-stu-id="9e9c8-103">Update conversationthread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e9c8-104">Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e9c8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e9c8-105">Permissions</span></span>
<span data-ttu-id="9e9c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e9c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e9c8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e9c8-108">Permission type</span></span>      | <span data-ttu-id="9e9c8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e9c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e9c8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e9c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e9c8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e9c8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e9c8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e9c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e9c8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-113">Not supported.</span></span>    |
|<span data-ttu-id="9e9c8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e9c8-114">Application</span></span> | <span data-ttu-id="9e9c8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e9c8-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e9c8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e9c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9e9c8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e9c8-117">Request headers</span></span>
| <span data-ttu-id="9e9c8-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e9c8-118">Header</span></span>       | <span data-ttu-id="9e9c8-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9e9c8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e9c8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e9c8-120">Authorization</span></span>  | <span data-ttu-id="9e9c8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9e9c8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e9c8-123">Content-Type</span></span>  | <span data-ttu-id="9e9c8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e9c8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e9c8-126">Request body</span></span>
<span data-ttu-id="9e9c8-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9e9c8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e9c8-130">Property</span></span>     | <span data-ttu-id="9e9c8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e9c8-131">Type</span></span>   |<span data-ttu-id="9e9c8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e9c8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e9c8-133">isLocked</span><span class="sxs-lookup"><span data-stu-id="9e9c8-133">isLocked</span></span>|<span data-ttu-id="9e9c8-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e9c8-134">Boolean</span></span>|<span data-ttu-id="9e9c8-p105">Indica se o thread está bloqueado. Defina como `true` para proibir a postagem.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="9e9c8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e9c8-137">Response</span></span>

<span data-ttu-id="9e9c8-138">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e9c8-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e9c8-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e9c8-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e9c8-140">Request</span></span>
<span data-ttu-id="9e9c8-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9e9c8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e9c8-142">Response</span></span>
<span data-ttu-id="9e9c8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e9c8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
