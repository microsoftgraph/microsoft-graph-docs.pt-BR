---
title: 'groupLifecyclePolicy: renovar'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 95d43455bca46a3814ecd7bff62391857c2a73d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857748"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="e28e2-104">groupLifecyclePolicy: renovar</span><span class="sxs-lookup"><span data-stu-id="e28e2-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e28e2-105">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="e28e2-105">Renews a group's expiration.</span></span> <span data-ttu-id="e28e2-106">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="e28e2-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="e28e2-107">**Observação:** Em V 1.0, [use o recurso de grupo para fazer solicitações de renovação](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e28e2-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="e28e2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e28e2-108">Permissions</span></span>

<span data-ttu-id="e28e2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e28e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="e28e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e28e2-111">Permission type</span></span>      | <span data-ttu-id="e28e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e28e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e28e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e28e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e28e2-114">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e28e2-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e28e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e28e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e28e2-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e28e2-116">Not supported</span></span> |
|<span data-ttu-id="e28e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e28e2-117">Application</span></span> | <span data-ttu-id="e28e2-118">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e28e2-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e28e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e28e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="e28e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e28e2-120">Request headers</span></span>

| <span data-ttu-id="e28e2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e28e2-121">Name</span></span> | <span data-ttu-id="e28e2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e28e2-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e28e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e28e2-123">Authorization</span></span> | <span data-ttu-id="e28e2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e28e2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e28e2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e28e2-126">Content-Type</span></span>  | <span data-ttu-id="e28e2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e28e2-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e28e2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e28e2-128">Request body</span></span>
<span data-ttu-id="e28e2-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e28e2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e28e2-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e28e2-130">Parameter</span></span> | <span data-ttu-id="e28e2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e28e2-131">Type</span></span> | <span data-ttu-id="e28e2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e28e2-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e28e2-133">groupId</span><span class="sxs-lookup"><span data-stu-id="e28e2-133">groupId</span></span>|<span data-ttu-id="e28e2-134">Guid</span><span class="sxs-lookup"><span data-stu-id="e28e2-134">Guid</span></span>| <span data-ttu-id="e28e2-135">A ID do grupo a ser renovado.</span><span class="sxs-lookup"><span data-stu-id="e28e2-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="e28e2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e28e2-136">Response</span></span>

<span data-ttu-id="e28e2-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e28e2-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e28e2-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e28e2-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e28e2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e28e2-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e28e2-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e28e2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e28e2-142">C#</span><span class="sxs-lookup"><span data-stu-id="e28e2-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e28e2-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="e28e2-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e28e2-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e28e2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e28e2-145">Java</span><span class="sxs-lookup"><span data-stu-id="e28e2-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e28e2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e28e2-146">Response</span></span>

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
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
