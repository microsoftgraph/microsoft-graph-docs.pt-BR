---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 174e3ad1c27b3a0c2e87b5c3cf3630b00168bc3b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262320"
---
# <a name="delete-call"></a><span data-ttu-id="4972a-103">Excluir chamada</span><span class="sxs-lookup"><span data-stu-id="4972a-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4972a-104">Excluir ou desligar uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="4972a-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="4972a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4972a-105">Permissions</span></span>

<span data-ttu-id="4972a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4972a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4972a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4972a-108">Permission type</span></span> | <span data-ttu-id="4972a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4972a-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="4972a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4972a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4972a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4972a-111">Not Supported.</span></span>                         |
| <span data-ttu-id="4972a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4972a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4972a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4972a-113">Not Supported.</span></span>                         |
| <span data-ttu-id="4972a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4972a-114">Application</span></span>                            | <span data-ttu-id="4972a-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4972a-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="4972a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4972a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4972a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4972a-117">Request headers</span></span>
| <span data-ttu-id="4972a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4972a-118">Name</span></span>          | <span data-ttu-id="4972a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4972a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4972a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4972a-120">Authorization</span></span> | <span data-ttu-id="4972a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4972a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4972a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4972a-123">Request body</span></span>
<span data-ttu-id="4972a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4972a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4972a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4972a-125">Response</span></span>
<span data-ttu-id="4972a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4972a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4972a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4972a-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4972a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4972a-129">Request</span></span>
<span data-ttu-id="4972a-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4972a-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="4972a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4972a-131">Response</span></span>

> <span data-ttu-id="4972a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4972a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4972a-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4972a-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4972a-135">C#</span><span class="sxs-lookup"><span data-stu-id="4972a-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-call-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4972a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="4972a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-call-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4972a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4972a-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete-call-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---terminating"></a><span data-ttu-id="4972a-138">Notificação-encerramento</span><span class="sxs-lookup"><span data-stu-id="4972a-138">Notification - terminating</span></span>

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
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="4972a-139">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="4972a-139">Notification - terminated</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
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
    "Error: /api-reference/beta/api/call-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
