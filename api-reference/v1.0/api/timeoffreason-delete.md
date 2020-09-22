---
title: Excluir timeOffReason
description: Marque uma timeOffReason como inativa definindo a propriedade IsActive.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e23f4e9255bc1ff50e901cd366e50540be0dbe57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978221"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="6f64a-103">Excluir timeOffReason</span><span class="sxs-lookup"><span data-stu-id="6f64a-103">Delete timeOffReason</span></span>

<span data-ttu-id="6f64a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f64a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f64a-105">Marque uma [timeOffReason](../resources/timeoffreason.md) como inativa definindo a propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="6f64a-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="6f64a-106">Cada equipe deve incluir pelo menos um motivo de timeoff.</span><span class="sxs-lookup"><span data-stu-id="6f64a-106">Every team must include at least one timeoff reason.</span></span>

<span data-ttu-id="6f64a-107">Este método não remove a instância especificada do [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="6f64a-107">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="6f64a-108">as instâncias do [timeOffItem](../resources/timeoffitem.md) que foram atribuídas essa razão permanecem atribuídas a esse motivo.</span><span class="sxs-lookup"><span data-stu-id="6f64a-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f64a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f64a-109">Permissions</span></span>

<span data-ttu-id="6f64a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f64a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f64a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f64a-112">Permission type</span></span>      | <span data-ttu-id="6f64a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f64a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f64a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f64a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6f64a-115">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6f64a-115">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f64a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f64a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f64a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f64a-117">Not supported.</span></span>    |
|<span data-ttu-id="6f64a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f64a-118">Application</span></span> | <span data-ttu-id="6f64a-119">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f64a-119">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="6f64a-120">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6f64a-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6f64a-121">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="6f64a-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6f64a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f64a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="6f64a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f64a-123">Request headers</span></span>

| <span data-ttu-id="6f64a-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f64a-124">Header</span></span>       | <span data-ttu-id="6f64a-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6f64a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6f64a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f64a-126">Authorization</span></span>  | <span data-ttu-id="6f64a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f64a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f64a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f64a-129">Request body</span></span>
<span data-ttu-id="6f64a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f64a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f64a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f64a-131">Response</span></span>

<span data-ttu-id="6f64a-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f64a-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f64a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f64a-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f64a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f64a-135">Request</span></span>

<span data-ttu-id="6f64a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f64a-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f64a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f64a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="6f64a-138">C#</span><span class="sxs-lookup"><span data-stu-id="6f64a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f64a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f64a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f64a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f64a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f64a-141">Java</span><span class="sxs-lookup"><span data-stu-id="6f64a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="6f64a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f64a-142">Response</span></span>

<span data-ttu-id="6f64a-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f64a-143">The following is an example of the response.</span></span> 

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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

