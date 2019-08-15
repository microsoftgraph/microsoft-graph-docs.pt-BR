---
title: Subtituir schedulingGroup
description: Substitua um existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2cc22b11fdba3f4b0dfdf7d3e0289e1a9fbcc161
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410644"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="76c5b-103">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="76c5b-103">Replace schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c5b-104">Substitua um existente [](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="76c5b-104">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="76c5b-105">Se o The [Scheduling](../resources/schedulinggroup.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="76c5b-105">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="76c5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="76c5b-106">Permissions</span></span>

<span data-ttu-id="76c5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76c5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76c5b-109">Permission type</span></span>      | <span data-ttu-id="76c5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76c5b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76c5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76c5b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="76c5b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76c5b-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="76c5b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76c5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76c5b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76c5b-114">Not supported.</span></span>    |
|<span data-ttu-id="76c5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76c5b-115">Application</span></span> | <span data-ttu-id="76c5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76c5b-116">Not supported.</span></span> |

> <span data-ttu-id="76c5b-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="76c5b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="76c5b-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="76c5b-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="76c5b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76c5b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="76c5b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76c5b-120">Request headers</span></span>

| <span data-ttu-id="76c5b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76c5b-121">Header</span></span>       | <span data-ttu-id="76c5b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76c5b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76c5b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76c5b-123">Authorization</span></span>  | <span data-ttu-id="76c5b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76c5b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="76c5b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76c5b-126">Content-Type</span></span>  | <span data-ttu-id="76c5b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="76c5b-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76c5b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76c5b-128">Request body</span></span>

<span data-ttu-id="76c5b-129">No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [plano](../resources/schedulinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="76c5b-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="76c5b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="76c5b-130">Response</span></span>

<span data-ttu-id="76c5b-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76c5b-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76c5b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76c5b-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="76c5b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76c5b-133">Request</span></span>

<span data-ttu-id="76c5b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76c5b-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76c5b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="76c5b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76c5b-136">C#</span><span class="sxs-lookup"><span data-stu-id="76c5b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76c5b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76c5b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76c5b-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="76c5b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="76c5b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="76c5b-139">Response</span></span>

<span data-ttu-id="76c5b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76c5b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="76c5b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76c5b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
