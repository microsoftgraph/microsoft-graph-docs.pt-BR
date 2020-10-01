---
title: Lista schedulingGroups
description: Obtenha a lista de um The Scheduling neste cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7628c20df5e72e5c780361e3c858648b586d7c8d
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315088"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="8acd0-103">Listar scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="8acd0-103">List scheduleGroups</span></span>

<span data-ttu-id="8acd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8acd0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8acd0-105">Obtenha a lista de [schedulingGroups](../resources/schedulinggroup.md) neste [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8acd0-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8acd0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8acd0-106">Permissions</span></span>

<span data-ttu-id="8acd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8acd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8acd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8acd0-109">Permission type</span></span>      | <span data-ttu-id="8acd0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8acd0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8acd0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8acd0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8acd0-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8acd0-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8acd0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8acd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8acd0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8acd0-114">Not supported.</span></span>    |
|<span data-ttu-id="8acd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8acd0-115">Application</span></span> | <span data-ttu-id="8acd0-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8acd0-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8acd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8acd0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="8acd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8acd0-118">Request headers</span></span>

| <span data-ttu-id="8acd0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8acd0-119">Header</span></span>       | <span data-ttu-id="8acd0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8acd0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8acd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8acd0-121">Authorization</span></span>  | <span data-ttu-id="8acd0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8acd0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8acd0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8acd0-124">Request body</span></span>
<span data-ttu-id="8acd0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8acd0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8acd0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8acd0-126">Response</span></span>

<span data-ttu-id="8acd0-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de grupo de [agendamento](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8acd0-127">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8acd0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8acd0-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="8acd0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8acd0-129">Request</span></span>

<span data-ttu-id="8acd0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8acd0-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8acd0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8acd0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="8acd0-132">C#</span><span class="sxs-lookup"><span data-stu-id="8acd0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8acd0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8acd0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8acd0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8acd0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8acd0-135">Java</span><span class="sxs-lookup"><span data-stu-id="8acd0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="8acd0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8acd0-136">Response</span></span>

<span data-ttu-id="8acd0-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8acd0-137">The following is an example of the response.</span></span> 

><span data-ttu-id="8acd0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8acd0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

