---
title: 'groupLifecyclePolicy: renewGroup'
description: Renovar a expiração de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: be7f1222933b5923b475d55c0b7c6b8a4bcf24aa
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681110"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="ccf33-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="ccf33-104">groupLifecyclePolicy: renewGroup</span></span>

<span data-ttu-id="ccf33-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccf33-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccf33-106">Renovar a expiração de um grupo.</span><span class="sxs-lookup"><span data-stu-id="ccf33-106">Renew a group's expiration.</span></span> <span data-ttu-id="ccf33-107">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="ccf33-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="ccf33-108">**Observação:** Ao chamar o ponto de extremidade v1.0, use o [método Renovar grupo.](/graph/api/group-renew?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ccf33-108">**Note:** When calling the v1.0 endpoint, use the [Renew group](/graph/api/group-renew?view=graph-rest-1.0&preserve-view=true) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccf33-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccf33-109">Permissions</span></span>

<span data-ttu-id="ccf33-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccf33-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="ccf33-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccf33-112">Permission type</span></span>      | <span data-ttu-id="ccf33-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccf33-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccf33-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccf33-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ccf33-115">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccf33-115">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ccf33-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccf33-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccf33-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ccf33-117">Not supported</span></span> |
|<span data-ttu-id="ccf33-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccf33-118">Application</span></span> | <span data-ttu-id="ccf33-119">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccf33-119">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccf33-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccf33-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="ccf33-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccf33-121">Request headers</span></span>

| <span data-ttu-id="ccf33-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ccf33-122">Name</span></span> | <span data-ttu-id="ccf33-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccf33-123">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ccf33-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccf33-124">Authorization</span></span> | <span data-ttu-id="ccf33-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccf33-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccf33-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccf33-127">Content-Type</span></span>  | <span data-ttu-id="ccf33-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ccf33-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccf33-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccf33-129">Request body</span></span>
<span data-ttu-id="ccf33-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccf33-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ccf33-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ccf33-131">Parameter</span></span> | <span data-ttu-id="ccf33-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccf33-132">Type</span></span> | <span data-ttu-id="ccf33-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccf33-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ccf33-134">groupId</span><span class="sxs-lookup"><span data-stu-id="ccf33-134">groupId</span></span>|<span data-ttu-id="ccf33-135">Guid</span><span class="sxs-lookup"><span data-stu-id="ccf33-135">Guid</span></span>| <span data-ttu-id="ccf33-136">A id do grupo a ser renovado.</span><span class="sxs-lookup"><span data-stu-id="ccf33-136">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="ccf33-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccf33-137">Response</span></span>

<span data-ttu-id="ccf33-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccf33-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccf33-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccf33-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ccf33-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccf33-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ccf33-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccf33-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ccf33-143">C#</span><span class="sxs-lookup"><span data-stu-id="ccf33-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccf33-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccf33-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccf33-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccf33-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccf33-146">Java</span><span class="sxs-lookup"><span data-stu-id="ccf33-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ccf33-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccf33-147">Response</span></span>

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
