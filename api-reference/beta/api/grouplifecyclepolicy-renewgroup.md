---
title: 'groupLifecyclePolicy: renovar'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5815d7d12677419fc04cbfd383c8456c0b26e180
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592312"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="a4376-104">groupLifecyclePolicy: renovar</span><span class="sxs-lookup"><span data-stu-id="a4376-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4376-105">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="a4376-105">Renews a group's expiration.</span></span> <span data-ttu-id="a4376-106">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="a4376-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="a4376-107">**Observação:** Em V 1.0, [use o recurso de grupo para fazer solicitações de renovação](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="a4376-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4376-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4376-108">Permissions</span></span>

<span data-ttu-id="a4376-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4376-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="a4376-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4376-111">Permission type</span></span>      | <span data-ttu-id="a4376-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4376-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4376-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4376-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a4376-114">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4376-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4376-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4376-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4376-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a4376-116">Not supported</span></span> |
|<span data-ttu-id="a4376-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4376-117">Application</span></span> | <span data-ttu-id="a4376-118">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4376-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4376-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4376-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="a4376-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4376-120">Request headers</span></span>

| <span data-ttu-id="a4376-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a4376-121">Name</span></span> | <span data-ttu-id="a4376-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4376-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a4376-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4376-123">Authorization</span></span> | <span data-ttu-id="a4376-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4376-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4376-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4376-126">Content-Type</span></span>  | <span data-ttu-id="a4376-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a4376-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4376-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4376-128">Request body</span></span>
<span data-ttu-id="a4376-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4376-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4376-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4376-130">Parameter</span></span> | <span data-ttu-id="a4376-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4376-131">Type</span></span> | <span data-ttu-id="a4376-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4376-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a4376-133">groupId</span><span class="sxs-lookup"><span data-stu-id="a4376-133">groupId</span></span>|<span data-ttu-id="a4376-134">Guid</span><span class="sxs-lookup"><span data-stu-id="a4376-134">Guid</span></span>| <span data-ttu-id="a4376-135">A ID do grupo a ser renovado.</span><span class="sxs-lookup"><span data-stu-id="a4376-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="a4376-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4376-136">Response</span></span>

<span data-ttu-id="a4376-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4376-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4376-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4376-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a4376-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4376-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="a4376-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4376-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a4376-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a4376-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a4376-143">Basic</span><span class="sxs-lookup"><span data-stu-id="a4376-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4376-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4376-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
