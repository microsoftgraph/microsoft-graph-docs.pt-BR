---
title: 'groupLifecyclePolicy: renewGroup'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
ms.openlocfilehash: 5472927769175912736f66a2d848f103cfb5b8c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833317"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="5dbff-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="5dbff-104">groupLifecyclePolicy: renewGroup</span></span>

> <span data-ttu-id="5dbff-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5dbff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dbff-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5dbff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5dbff-107">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="5dbff-107">Renews a group's expiration.</span></span> <span data-ttu-id="5dbff-108">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="5dbff-108">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="5dbff-109">**Observação:** Na versão 1.0, [use o recurso de grupo para tornar renovar solicitações](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="5dbff-109">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="5dbff-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="5dbff-110">Permissions</span></span>

<span data-ttu-id="5dbff-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dbff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="5dbff-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dbff-113">Permission type</span></span>      | <span data-ttu-id="5dbff-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dbff-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dbff-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dbff-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5dbff-116">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dbff-116">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="5dbff-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dbff-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dbff-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5dbff-118">Not supported</span></span> |
|<span data-ttu-id="5dbff-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dbff-119">Application</span></span> | <span data-ttu-id="5dbff-120">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dbff-120">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dbff-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dbff-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="5dbff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dbff-122">Request headers</span></span>

| <span data-ttu-id="5dbff-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5dbff-123">Name</span></span> | <span data-ttu-id="5dbff-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dbff-124">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5dbff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dbff-125">Authorization</span></span> | <span data-ttu-id="5dbff-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dbff-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5dbff-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5dbff-128">Content-Type</span></span>  | <span data-ttu-id="5dbff-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5dbff-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dbff-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dbff-130">Request body</span></span>
<span data-ttu-id="5dbff-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dbff-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5dbff-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5dbff-132">Parameter</span></span> | <span data-ttu-id="5dbff-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dbff-133">Type</span></span> | <span data-ttu-id="5dbff-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dbff-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5dbff-135">groupId</span><span class="sxs-lookup"><span data-stu-id="5dbff-135">groupId</span></span>|<span data-ttu-id="5dbff-136">Guid</span><span class="sxs-lookup"><span data-stu-id="5dbff-136">Guid</span></span>| <span data-ttu-id="5dbff-137">A identificação do grupo renovar.</span><span class="sxs-lookup"><span data-stu-id="5dbff-137">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="5dbff-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dbff-138">Response</span></span>

<span data-ttu-id="5dbff-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dbff-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dbff-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dbff-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5dbff-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dbff-142">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="5dbff-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dbff-143">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
