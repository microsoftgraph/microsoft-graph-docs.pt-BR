---
title: Obter schedulingGroup
description: Recupere as propriedades e os relacionamentos de um The [Scheduling](../resources/schedulinggroup.md) por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f58d41c588c9937645480d3d0f5075c9753fda17
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154189"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="629ed-103">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="629ed-103">Get schedulingGroup</span></span>

<span data-ttu-id="629ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="629ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="629ed-105">Recupere as propriedades e os relacionamentos de um The [Scheduling](../resources/schedulinggroup.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="629ed-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="629ed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="629ed-106">Permissions</span></span>

<span data-ttu-id="629ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="629ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="629ed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="629ed-109">Permission type</span></span>      | <span data-ttu-id="629ed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="629ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="629ed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629ed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="629ed-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="629ed-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="629ed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629ed-114">Not supported.</span></span>    |
|<span data-ttu-id="629ed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629ed-115">Application</span></span> | <span data-ttu-id="629ed-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="629ed-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |


> <span data-ttu-id="629ed-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="629ed-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="629ed-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="629ed-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="629ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="629ed-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="629ed-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="629ed-120">Optional query parameters</span></span>

<span data-ttu-id="629ed-121">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="629ed-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="629ed-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="629ed-122">Request headers</span></span>

| <span data-ttu-id="629ed-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="629ed-123">Header</span></span>       | <span data-ttu-id="629ed-124">Valor</span><span class="sxs-lookup"><span data-stu-id="629ed-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="629ed-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="629ed-125">Authorization</span></span>  | <span data-ttu-id="629ed-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="629ed-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="629ed-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="629ed-128">Request body</span></span>
<span data-ttu-id="629ed-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="629ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="629ed-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="629ed-130">Response</span></span>

<span data-ttu-id="629ed-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de forma de [plano](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="629ed-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="629ed-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="629ed-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="629ed-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="629ed-133">Request</span></span>

<span data-ttu-id="629ed-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="629ed-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
---


### <a name="response"></a><span data-ttu-id="629ed-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="629ed-135">Response</span></span>

<span data-ttu-id="629ed-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="629ed-136">The following is an example of the response.</span></span> 

><span data-ttu-id="629ed-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="629ed-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
