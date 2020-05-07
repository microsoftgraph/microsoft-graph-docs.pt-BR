---
title: Lista schedulingGroups
description: Obtenha a lista de um The Scheduling neste cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 254a492e7afbcdac706ad1f437e3d5e3078d33dc
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155163"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="f23cd-103">Listar scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="f23cd-103">List scheduleGroups</span></span>

<span data-ttu-id="f23cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f23cd-105">Obtenha a lista de [schedulingGroups](../resources/schedulinggroup.md) neste [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f23cd-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f23cd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f23cd-106">Permissions</span></span>

<span data-ttu-id="f23cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f23cd-109">Permission type</span></span>      | <span data-ttu-id="f23cd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f23cd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f23cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f23cd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f23cd-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f23cd-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f23cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f23cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f23cd-114">Not supported.</span></span>    |
|<span data-ttu-id="f23cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f23cd-115">Application</span></span> | <span data-ttu-id="f23cd-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f23cd-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="f23cd-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="f23cd-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f23cd-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="f23cd-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f23cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f23cd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="f23cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f23cd-120">Request headers</span></span>

| <span data-ttu-id="f23cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f23cd-121">Header</span></span>       | <span data-ttu-id="f23cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f23cd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f23cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f23cd-123">Authorization</span></span>  | <span data-ttu-id="f23cd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f23cd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f23cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f23cd-126">Request body</span></span>
<span data-ttu-id="f23cd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f23cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f23cd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23cd-128">Response</span></span>

<span data-ttu-id="f23cd-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de grupo de [agendamento](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f23cd-129">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23cd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f23cd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f23cd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f23cd-131">Request</span></span>

<span data-ttu-id="f23cd-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f23cd-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
```

---


### <a name="response"></a><span data-ttu-id="f23cd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23cd-133">Response</span></span>

<span data-ttu-id="f23cd-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f23cd-134">The following is an example of the response.</span></span> 

><span data-ttu-id="f23cd-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f23cd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
        "@odata.type":"microsoft.graph.identitySet",
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of schedulingGroup in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
