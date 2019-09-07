---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa1d0111085fa48f6c6186e764d19210a9f10ae2
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792412"
---
# <a name="delete-call"></a><span data-ttu-id="d8d7c-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="d8d7c-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d7c-104">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-104">Delete or hang up an active call.</span></span> <span data-ttu-id="d8d7c-105">Para chamadas com vários participantes, isso só excluirá o trecho de chamada; a chamada de multipartes subjacente ainda continuará.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-105">For multiparty calls, this will only delete your call leg; the underlying multiparty call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8d7c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8d7c-106">Permissions</span></span>

<span data-ttu-id="d8d7c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8d7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8d7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8d7c-109">Permission type</span></span> | <span data-ttu-id="d8d7c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8d7c-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d8d7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8d7c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8d7c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-112">Not Supported.</span></span>                         |
| <span data-ttu-id="d8d7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8d7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8d7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-114">Not Supported.</span></span>                         |
| <span data-ttu-id="d8d7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8d7c-115">Application</span></span>                            | <span data-ttu-id="d8d7c-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d8d7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d7c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8d7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d7c-118">Request headers</span></span>
| <span data-ttu-id="d8d7c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d8d7c-119">Name</span></span>          | <span data-ttu-id="d8d7c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d7c-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d8d7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8d7c-121">Authorization</span></span> | <span data-ttu-id="d8d7c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8d7c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d7c-124">Request body</span></span>
<span data-ttu-id="d8d7c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8d7c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d7c-126">Response</span></span>
<span data-ttu-id="d8d7c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8d7c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8d7c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8d7c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d7c-130">Request</span></span>
<span data-ttu-id="d8d7c-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d8d7c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d7c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8d7c-133">C#</span><span class="sxs-lookup"><span data-stu-id="d8d7c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8d7c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8d7c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8d7c-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d8d7c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8d7c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d7c-136">Response</span></span>

> <span data-ttu-id="d8d7c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8d7c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="d8d7c-139">Notificação-encerramento</span><span class="sxs-lookup"><span data-stu-id="d8d7c-139">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

##### <a name="notification---terminated"></a><span data-ttu-id="d8d7c-140">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="d8d7c-140">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "0"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
