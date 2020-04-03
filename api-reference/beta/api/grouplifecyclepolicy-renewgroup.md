---
title: 'groupLifecyclePolicy: renovar'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 09776750c3c3bba64b81c75ee0f32af395a3f6b1
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123948"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="bed91-104">groupLifecyclePolicy: renovar</span><span class="sxs-lookup"><span data-stu-id="bed91-104">groupLifecyclePolicy: renewGroup</span></span>

<span data-ttu-id="bed91-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bed91-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bed91-106">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="bed91-106">Renews a group's expiration.</span></span> <span data-ttu-id="bed91-107">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="bed91-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="bed91-108">**Observação:** Em V 1.0, [use o recurso de grupo para fazer solicitações de renovação](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="bed91-108">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="bed91-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="bed91-109">Permissions</span></span>

<span data-ttu-id="bed91-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed91-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="bed91-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bed91-112">Permission type</span></span>      | <span data-ttu-id="bed91-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bed91-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bed91-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bed91-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bed91-115">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed91-115">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="bed91-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bed91-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bed91-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bed91-117">Not supported</span></span> |
|<span data-ttu-id="bed91-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bed91-118">Application</span></span> | <span data-ttu-id="bed91-119">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed91-119">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bed91-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bed91-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="bed91-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bed91-121">Request headers</span></span>

| <span data-ttu-id="bed91-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bed91-122">Name</span></span> | <span data-ttu-id="bed91-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed91-123">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bed91-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bed91-124">Authorization</span></span> | <span data-ttu-id="bed91-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bed91-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bed91-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bed91-127">Content-Type</span></span>  | <span data-ttu-id="bed91-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bed91-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bed91-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bed91-129">Request body</span></span>
<span data-ttu-id="bed91-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bed91-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bed91-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bed91-131">Parameter</span></span> | <span data-ttu-id="bed91-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bed91-132">Type</span></span> | <span data-ttu-id="bed91-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed91-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bed91-134">groupId</span><span class="sxs-lookup"><span data-stu-id="bed91-134">groupId</span></span>|<span data-ttu-id="bed91-135">Guid</span><span class="sxs-lookup"><span data-stu-id="bed91-135">Guid</span></span>| <span data-ttu-id="bed91-136">A ID do grupo a ser renovado.</span><span class="sxs-lookup"><span data-stu-id="bed91-136">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="bed91-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed91-137">Response</span></span>

<span data-ttu-id="bed91-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bed91-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed91-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bed91-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bed91-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bed91-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bed91-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="bed91-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bed91-143">C#</span><span class="sxs-lookup"><span data-stu-id="bed91-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bed91-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bed91-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bed91-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bed91-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bed91-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed91-146">Response</span></span>

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
