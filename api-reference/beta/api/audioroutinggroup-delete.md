---
title: Excluir grupo de roteamento de áudio
description: Exclua o grupo de roteamento de áudio especificado.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2a3af19dfebe7db63e720a22efe69a68a9c819b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258314"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="83ea0-103">Excluir grupo de roteamento de áudio</span><span class="sxs-lookup"><span data-stu-id="83ea0-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83ea0-104">Exclua o [audioRoutingGroup](../resources/audioroutinggroup.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="83ea0-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83ea0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="83ea0-105">Permissions</span></span>
<span data-ttu-id="83ea0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83ea0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83ea0-108">Permission type</span></span> | <span data-ttu-id="83ea0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83ea0-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="83ea0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83ea0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="83ea0-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="83ea0-111">Not Supported</span></span>        |
| <span data-ttu-id="83ea0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83ea0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83ea0-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="83ea0-113">Not Supported</span></span>        |
| <span data-ttu-id="83ea0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83ea0-114">Application</span></span>     | <span data-ttu-id="83ea0-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="83ea0-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83ea0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83ea0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83ea0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83ea0-117">Request headers</span></span>
| <span data-ttu-id="83ea0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="83ea0-118">Name</span></span>          | <span data-ttu-id="83ea0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="83ea0-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="83ea0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="83ea0-120">Authorization</span></span> | <span data-ttu-id="83ea0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83ea0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83ea0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83ea0-123">Request body</span></span>
<span data-ttu-id="83ea0-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83ea0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83ea0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="83ea0-125">Response</span></span>
<span data-ttu-id="83ea0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83ea0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83ea0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83ea0-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83ea0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83ea0-129">Request</span></span>
<span data-ttu-id="83ea0-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="83ea0-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="83ea0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="83ea0-131">Response</span></span>

> <span data-ttu-id="83ea0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83ea0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="83ea0-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="83ea0-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="83ea0-135">C#</span><span class="sxs-lookup"><span data-stu-id="83ea0-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83ea0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="83ea0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="83ea0-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="83ea0-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
