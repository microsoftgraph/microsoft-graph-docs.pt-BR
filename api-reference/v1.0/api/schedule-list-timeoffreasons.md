---
title: Listar timeOffReasons
description: Obtenha a lista de timeOffReasons em um cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e2198026c4fa431cfd7e9395d552e64b79137e07
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155149"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="96fe9-103">Listar timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="96fe9-103">List timeOffReasons</span></span>

<span data-ttu-id="96fe9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96fe9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96fe9-105">Obtenha a lista de [timeOffReasons](../resources/timeoffreason.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="96fe9-105">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96fe9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96fe9-106">Permissions</span></span>

<span data-ttu-id="96fe9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96fe9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96fe9-109">Permission type</span></span>      | <span data-ttu-id="96fe9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96fe9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96fe9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96fe9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96fe9-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96fe9-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96fe9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96fe9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96fe9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96fe9-114">Not supported.</span></span>    |
|<span data-ttu-id="96fe9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96fe9-115">Application</span></span> | <span data-ttu-id="96fe9-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96fe9-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="96fe9-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="96fe9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="96fe9-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="96fe9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="96fe9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96fe9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="96fe9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96fe9-120">Request headers</span></span>

| <span data-ttu-id="96fe9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96fe9-121">Header</span></span>       | <span data-ttu-id="96fe9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96fe9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96fe9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96fe9-123">Authorization</span></span>  | <span data-ttu-id="96fe9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96fe9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96fe9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96fe9-126">Request body</span></span>
<span data-ttu-id="96fe9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96fe9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96fe9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="96fe9-128">Response</span></span>

<span data-ttu-id="96fe9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96fe9-129">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96fe9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96fe9-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="96fe9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96fe9-131">Request</span></span>

<span data-ttu-id="96fe9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96fe9-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
```
---


#### <a name="response"></a><span data-ttu-id="96fe9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="96fe9-133">Response</span></span>

<span data-ttu-id="96fe9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96fe9-134">The following is an example of the response.</span></span> 

><span data-ttu-id="96fe9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96fe9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
      "createdDateTime": "2019-03-12T22:10:38.242Z",
      "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
      "displayName": "Vacation",
      "iconType": "plane",
      "isActive": true,
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
