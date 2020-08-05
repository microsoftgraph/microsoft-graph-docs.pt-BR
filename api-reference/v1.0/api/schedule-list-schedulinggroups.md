---
title: Lista schedulingGroups
description: Obtenha a lista de um The Scheduling neste cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4778696b4a10bbf4f826e9c414904275d62c60f4
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/04/2020
ms.locfileid: "44218115"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="80038-103">Listar scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="80038-103">List scheduleGroups</span></span>

<span data-ttu-id="80038-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80038-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80038-105">Obtenha a lista de [schedulingGroups](../resources/schedulinggroup.md) neste [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="80038-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80038-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="80038-106">Permissions</span></span>

<span data-ttu-id="80038-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80038-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80038-109">Permission type</span></span>      | <span data-ttu-id="80038-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80038-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80038-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80038-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80038-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80038-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="80038-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80038-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80038-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80038-114">Not supported.</span></span>    |
|<span data-ttu-id="80038-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80038-115">Application</span></span> | <span data-ttu-id="80038-116">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80038-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="80038-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="80038-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="80038-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="80038-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="80038-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80038-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="80038-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80038-120">Request headers</span></span>

| <span data-ttu-id="80038-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80038-121">Header</span></span>       | <span data-ttu-id="80038-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80038-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80038-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80038-123">Authorization</span></span>  | <span data-ttu-id="80038-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80038-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80038-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80038-126">Request body</span></span>
<span data-ttu-id="80038-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80038-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80038-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="80038-128">Response</span></span>

<span data-ttu-id="80038-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de grupo de [agendamento](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80038-129">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80038-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80038-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="80038-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80038-131">Request</span></span>

<span data-ttu-id="80038-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="80038-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="80038-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80038-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="80038-134">C#</span><span class="sxs-lookup"><span data-stu-id="80038-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80038-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80038-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80038-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80038-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80038-137">Java</span><span class="sxs-lookup"><span data-stu-id="80038-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="80038-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="80038-138">Response</span></span>

<span data-ttu-id="80038-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="80038-139">The following is an example of the response.</span></span> 

><span data-ttu-id="80038-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80038-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
