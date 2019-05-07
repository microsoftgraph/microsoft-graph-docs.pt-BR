---
title: Subtituir schedulingGroup
description: Substitua um existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bf4fad282db9ec014ebbdfeb729da933d7346970
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638925"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="68b45-103">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="68b45-103">Replace schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68b45-104">Substitua um existente [](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="68b45-104">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="68b45-105">Se o The [Scheduling](../resources/schedulinggroup.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="68b45-105">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="68b45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68b45-106">Permissions</span></span>

<span data-ttu-id="68b45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68b45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68b45-109">Permission type</span></span>      | <span data-ttu-id="68b45-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68b45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68b45-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68b45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="68b45-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68b45-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="68b45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68b45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68b45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68b45-114">Not supported.</span></span>    |
|<span data-ttu-id="68b45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68b45-115">Application</span></span> | <span data-ttu-id="68b45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68b45-116">Not supported.</span></span> |

> <span data-ttu-id="68b45-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="68b45-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="68b45-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="68b45-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="68b45-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68b45-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="68b45-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68b45-120">Request headers</span></span>

| <span data-ttu-id="68b45-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68b45-121">Header</span></span>       | <span data-ttu-id="68b45-122">Valor</span><span class="sxs-lookup"><span data-stu-id="68b45-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68b45-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="68b45-123">Authorization</span></span>  | <span data-ttu-id="68b45-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68b45-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68b45-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68b45-126">Content-Type</span></span>  | <span data-ttu-id="68b45-127">application/json</span><span class="sxs-lookup"><span data-stu-id="68b45-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68b45-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68b45-128">Request body</span></span>

<span data-ttu-id="68b45-129">No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [plano](../resources/schedulinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="68b45-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68b45-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="68b45-130">Response</span></span>

<span data-ttu-id="68b45-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68b45-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68b45-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68b45-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="68b45-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68b45-133">Request</span></span>

<span data-ttu-id="68b45-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68b45-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="68b45-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="68b45-135">Response</span></span>

<span data-ttu-id="68b45-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68b45-136">The following is an example of the response.</span></span> 

><span data-ttu-id="68b45-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68b45-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="68b45-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="68b45-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="68b45-140">Basic</span><span class="sxs-lookup"><span data-stu-id="68b45-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-put-schedulinggroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68b45-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68b45-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-put-schedulinggroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/schedulinggroup-put.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedulinggroup-put.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
