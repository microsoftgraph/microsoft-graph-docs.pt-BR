---
title: Subtituir schedulingGroup
description: Substitua um existente.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c56fc696469cce89a82d4dd9a46ef6d61e07e495
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154182"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="e9560-103">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="e9560-103">Replace schedulingGroup</span></span>

<span data-ttu-id="e9560-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9560-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9560-105">Substitua [um existente.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="e9560-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="e9560-106">Se o The [Scheduling](../resources/schedulinggroup.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="e9560-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9560-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9560-107">Permissions</span></span>

<span data-ttu-id="e9560-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9560-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9560-110">Permission type</span></span>      | <span data-ttu-id="e9560-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9560-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9560-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9560-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9560-113">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e9560-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9560-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9560-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9560-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9560-115">Not supported.</span></span>    |
|<span data-ttu-id="e9560-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9560-116">Application</span></span> | <span data-ttu-id="e9560-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9560-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e9560-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e9560-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e9560-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e9560-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9560-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9560-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="e9560-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9560-121">Request headers</span></span>

| <span data-ttu-id="e9560-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9560-122">Header</span></span>       | <span data-ttu-id="e9560-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e9560-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9560-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9560-124">Authorization</span></span>  | <span data-ttu-id="e9560-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9560-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e9560-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9560-127">Content-Type</span></span>  | <span data-ttu-id="e9560-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9560-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9560-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9560-130">Request body</span></span>

<span data-ttu-id="e9560-131">No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [plano](../resources/schedulinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="e9560-131">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e9560-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9560-132">Response</span></span>

<span data-ttu-id="e9560-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9560-133">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9560-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9560-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9560-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9560-135">Request</span></span>

<span data-ttu-id="e9560-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9560-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
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
---


### <a name="response"></a><span data-ttu-id="e9560-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9560-137">Response</span></span>

<span data-ttu-id="e9560-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9560-138">The following is an example of the response.</span></span> 

><span data-ttu-id="e9560-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9560-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
