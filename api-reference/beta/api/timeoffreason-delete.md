---
title: Excluir timeOffReason
description: Marcar um timeOffReason como inativo Configurando a propriedade IsActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 45df0c9644e9845b9d86c591fb6871af455502ee
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270529"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="a190d-103">Excluir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="a190d-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a190d-104">Marque uma [timeOffReason](../resources/timeoffreason.md) como inativa definindo a propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="a190d-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="a190d-105">Este método não remove a instância especificada do [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="a190d-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="a190d-106">as instâncias do [timeOffItem](../resources/timeoffitem.md) que foram atribuídas essa razão permanecem atribuídas a esse motivo.</span><span class="sxs-lookup"><span data-stu-id="a190d-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="a190d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a190d-107">Permissions</span></span>

<span data-ttu-id="a190d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a190d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a190d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a190d-110">Permission type</span></span>      | <span data-ttu-id="a190d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a190d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a190d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a190d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a190d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a190d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a190d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a190d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a190d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a190d-115">Not supported.</span></span>    |
|<span data-ttu-id="a190d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a190d-116">Application</span></span> | <span data-ttu-id="a190d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a190d-117">Not supported.</span></span> |

> <span data-ttu-id="a190d-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a190d-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a190d-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a190d-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a190d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a190d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="a190d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a190d-121">Request headers</span></span>

| <span data-ttu-id="a190d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a190d-122">Header</span></span>       | <span data-ttu-id="a190d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a190d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a190d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a190d-124">Authorization</span></span>  | <span data-ttu-id="a190d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a190d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a190d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a190d-127">Content-Type</span></span>  | <span data-ttu-id="a190d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a190d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a190d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a190d-129">Request body</span></span>
<span data-ttu-id="a190d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a190d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a190d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a190d-131">Response</span></span>

<span data-ttu-id="a190d-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a190d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a190d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a190d-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a190d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a190d-135">Request</span></span>

<span data-ttu-id="a190d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a190d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="a190d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a190d-137">Response</span></span>

<span data-ttu-id="a190d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a190d-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a190d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a190d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a190d-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a190d-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a190d-142">C#</span><span class="sxs-lookup"><span data-stu-id="a190d-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoffreason-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a190d-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="a190d-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoffreason-delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a190d-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a190d-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoffreason-delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoffreason-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
