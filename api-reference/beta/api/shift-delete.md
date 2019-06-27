---
title: Excluir Shift
description: Exclui uma alteração do cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c8d700543da53bb44e2dc3d4edb1b66116f14e19
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269556"
---
# <a name="delete-shift"></a><span data-ttu-id="e1521-103">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="e1521-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1521-104">Exclui uma [alteração](../resources/shift.md) do cronograma.</span><span class="sxs-lookup"><span data-stu-id="e1521-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1521-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1521-105">Permissions</span></span>

<span data-ttu-id="e1521-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1521-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1521-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1521-108">Permission type</span></span>      | <span data-ttu-id="e1521-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1521-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1521-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1521-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1521-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1521-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1521-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1521-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1521-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1521-113">Not supported.</span></span>    |
|<span data-ttu-id="e1521-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1521-114">Application</span></span> | <span data-ttu-id="e1521-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1521-115">Not supported.</span></span> |

> <span data-ttu-id="e1521-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e1521-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e1521-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e1521-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1521-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1521-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="e1521-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1521-119">Request headers</span></span>

| <span data-ttu-id="e1521-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1521-120">Header</span></span>       | <span data-ttu-id="e1521-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1521-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1521-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1521-122">Authorization</span></span>  | <span data-ttu-id="e1521-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1521-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1521-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1521-125">Content-Type</span></span>  | <span data-ttu-id="e1521-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1521-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1521-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1521-127">Request body</span></span>
<span data-ttu-id="e1521-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1521-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1521-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1521-129">Response</span></span>

<span data-ttu-id="e1521-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1521-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1521-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1521-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e1521-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1521-133">Request</span></span>

<span data-ttu-id="e1521-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1521-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="e1521-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1521-135">Response</span></span>

<span data-ttu-id="e1521-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1521-136">The following is an example of the response.</span></span> 

><span data-ttu-id="e1521-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1521-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1521-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e1521-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1521-140">C#</span><span class="sxs-lookup"><span data-stu-id="e1521-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shift-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1521-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1521-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shift-delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1521-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e1521-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/shift-delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
