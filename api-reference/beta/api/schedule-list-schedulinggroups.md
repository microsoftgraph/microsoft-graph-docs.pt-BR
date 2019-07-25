---
title: Lista schedulingGroups
description: Obtenha a lista de um The Scheduling neste cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0bbfe0110dccbeb5642f6d9fe94db9fe40db9ba0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870937"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="485c2-103">Listar scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="485c2-103">List scheduleGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="485c2-104">Obtenha a lista de [schedulingGroups](../resources/schedulinggroup.md) neste [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="485c2-104">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="485c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="485c2-105">Permissions</span></span>

<span data-ttu-id="485c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="485c2-108">Permission type</span></span>      | <span data-ttu-id="485c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="485c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="485c2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="485c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="485c2-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="485c2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="485c2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="485c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="485c2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="485c2-113">Not supported.</span></span>    |
|<span data-ttu-id="485c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="485c2-114">Application</span></span> | <span data-ttu-id="485c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="485c2-115">Not supported.</span></span> |

> <span data-ttu-id="485c2-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="485c2-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="485c2-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="485c2-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="485c2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="485c2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="485c2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="485c2-119">Request headers</span></span>

| <span data-ttu-id="485c2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="485c2-120">Header</span></span>       | <span data-ttu-id="485c2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="485c2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="485c2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="485c2-122">Authorization</span></span>  | <span data-ttu-id="485c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="485c2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="485c2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="485c2-125">Content-Type</span></span>  | <span data-ttu-id="485c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="485c2-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="485c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="485c2-127">Request body</span></span>
<span data-ttu-id="485c2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="485c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="485c2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="485c2-129">Response</span></span>

<span data-ttu-id="485c2-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de grupo de [agendamento](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="485c2-130">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485c2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="485c2-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="485c2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="485c2-132">Request</span></span>

<span data-ttu-id="485c2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="485c2-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="485c2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="485c2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="485c2-135">C#</span><span class="sxs-lookup"><span data-stu-id="485c2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="485c2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="485c2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="485c2-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="485c2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="485c2-138">Java</span><span class="sxs-lookup"><span data-stu-id="485c2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="485c2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="485c2-139">Response</span></span>

<span data-ttu-id="485c2-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="485c2-140">The following is an example of the response.</span></span> 

><span data-ttu-id="485c2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="485c2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
