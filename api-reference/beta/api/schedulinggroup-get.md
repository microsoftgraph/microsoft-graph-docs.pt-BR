---
title: Obter schedulingGroup
description: Recupere as propriedades e os relacionamentos de um The [Scheduling](../resources/schedulinggroup.md) por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0ae53f154189bf1c7ab0afe2acaa7568805b3c3f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722555"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="6ac66-103">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="6ac66-103">Get schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ac66-104">Recupere as propriedades e os relacionamentos de um The [Scheduling](../resources/schedulinggroup.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="6ac66-104">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ac66-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ac66-105">Permissions</span></span>

<span data-ttu-id="6ac66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ac66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ac66-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ac66-108">Permission type</span></span>      | <span data-ttu-id="6ac66-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ac66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ac66-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ac66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ac66-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac66-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ac66-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ac66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ac66-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ac66-113">Not supported.</span></span>    |
|<span data-ttu-id="6ac66-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ac66-114">Application</span></span> | <span data-ttu-id="6ac66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ac66-115">Not supported.</span></span> |

> <span data-ttu-id="6ac66-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6ac66-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6ac66-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="6ac66-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6ac66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ac66-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="6ac66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ac66-119">Request headers</span></span>

| <span data-ttu-id="6ac66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ac66-120">Header</span></span>       | <span data-ttu-id="6ac66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6ac66-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ac66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ac66-122">Authorization</span></span>  | <span data-ttu-id="6ac66-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ac66-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6ac66-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ac66-125">Content-Type</span></span>  | <span data-ttu-id="6ac66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ac66-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ac66-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ac66-127">Request body</span></span>
<span data-ttu-id="6ac66-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ac66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ac66-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ac66-129">Response</span></span>

<span data-ttu-id="6ac66-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ac66-130">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ac66-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ac66-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6ac66-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ac66-132">Request</span></span>

<span data-ttu-id="6ac66-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ac66-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ac66-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ac66-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ac66-135">C#</span><span class="sxs-lookup"><span data-stu-id="6ac66-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ac66-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ac66-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ac66-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6ac66-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ac66-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ac66-138">Response</span></span>

<span data-ttu-id="6ac66-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ac66-139">The following is an example of the response.</span></span> 

><span data-ttu-id="6ac66-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ac66-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
