---
title: Excluir timeOff
description: Excluir uma instância do timeOff de um agendamento.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ee20d51fe5cf2c3cc01db23e65398deba2263e68
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270585"
---
# <a name="delete-timeoff"></a><span data-ttu-id="dfc5b-103">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="dfc5b-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfc5b-104">Excluir uma instância do [timeOff](../resources/timeoff.md) de um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="dfc5b-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfc5b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfc5b-105">Permissions</span></span>

<span data-ttu-id="dfc5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfc5b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfc5b-108">Permission type</span></span>      | <span data-ttu-id="dfc5b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfc5b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfc5b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfc5b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc5b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc5b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfc5b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfc5b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc5b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-113">Not supported.</span></span>    |
|<span data-ttu-id="dfc5b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfc5b-114">Application</span></span> | <span data-ttu-id="dfc5b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-115">Not supported.</span></span> |

> <span data-ttu-id="dfc5b-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dfc5b-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dfc5b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc5b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="dfc5b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc5b-119">Request headers</span></span>

| <span data-ttu-id="dfc5b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfc5b-120">Header</span></span>       | <span data-ttu-id="dfc5b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dfc5b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfc5b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfc5b-122">Authorization</span></span>  | <span data-ttu-id="dfc5b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dfc5b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfc5b-125">Content-Type</span></span>  | <span data-ttu-id="dfc5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfc5b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfc5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc5b-127">Request body</span></span>
<span data-ttu-id="dfc5b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc5b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc5b-129">Response</span></span>

<span data-ttu-id="dfc5b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfc5b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfc5b-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dfc5b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc5b-133">Request</span></span>

<span data-ttu-id="dfc5b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="dfc5b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc5b-135">Response</span></span>

<span data-ttu-id="dfc5b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-136">The following is an example of the response.</span></span> 

><span data-ttu-id="dfc5b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfc5b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfc5b-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dfc5b-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfc5b-140">C#</span><span class="sxs-lookup"><span data-stu-id="dfc5b-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfc5b-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfc5b-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfc5b-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dfc5b-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoff-delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
