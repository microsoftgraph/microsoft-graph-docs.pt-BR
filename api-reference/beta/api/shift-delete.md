---
title: Excluir Shift
description: Exclui uma alteração do cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c6c918d32cde14701688d318797546ae10a64ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991349"
---
# <a name="delete-shift"></a><span data-ttu-id="3b2ea-103">Excluir Shift</span><span class="sxs-lookup"><span data-stu-id="3b2ea-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b2ea-104">Exclui uma [alteração](../resources/shift.md) do cronograma.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b2ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b2ea-105">Permissions</span></span>

<span data-ttu-id="3b2ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b2ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b2ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b2ea-108">Permission type</span></span>      | <span data-ttu-id="3b2ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b2ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b2ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b2ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b2ea-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b2ea-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b2ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b2ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b2ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-113">Not supported.</span></span>    |
|<span data-ttu-id="3b2ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b2ea-114">Application</span></span> | <span data-ttu-id="3b2ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-115">Not supported.</span></span> |

> <span data-ttu-id="3b2ea-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3b2ea-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3b2ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b2ea-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="3b2ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b2ea-119">Request headers</span></span>

| <span data-ttu-id="3b2ea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b2ea-120">Header</span></span>       | <span data-ttu-id="3b2ea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b2ea-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b2ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b2ea-122">Authorization</span></span>  | <span data-ttu-id="3b2ea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b2ea-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b2ea-125">Content-Type</span></span>  | <span data-ttu-id="3b2ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b2ea-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b2ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b2ea-127">Request body</span></span>
<span data-ttu-id="3b2ea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b2ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b2ea-129">Response</span></span>

<span data-ttu-id="3b2ea-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b2ea-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b2ea-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3b2ea-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b2ea-133">Request</span></span>

<span data-ttu-id="3b2ea-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3b2ea-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b2ea-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b2ea-136">C#</span><span class="sxs-lookup"><span data-stu-id="3b2ea-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b2ea-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3b2ea-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b2ea-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3b2ea-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3b2ea-139">Java</span><span class="sxs-lookup"><span data-stu-id="3b2ea-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b2ea-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b2ea-140">Response</span></span>

<span data-ttu-id="3b2ea-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-141">The following is an example of the response.</span></span> 

><span data-ttu-id="3b2ea-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
