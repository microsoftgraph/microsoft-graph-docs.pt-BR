---
title: Lista schedulingGroups
description: Obtenha a lista de um The Scheduling neste cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 587faefe773a1ce8e5dc9e5977b819c00815c0ed
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866980"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="625c9-103">Listar scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="625c9-103">List scheduleGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="625c9-104">Obtenha a lista de [schedulingGroups](../resources/schedulinggroup.md) neste [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="625c9-104">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="625c9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="625c9-105">Permissions</span></span>

<span data-ttu-id="625c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="625c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="625c9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="625c9-108">Permission type</span></span>      | <span data-ttu-id="625c9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="625c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="625c9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="625c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="625c9-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625c9-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="625c9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="625c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="625c9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="625c9-113">Not supported.</span></span>    |
|<span data-ttu-id="625c9-114">Application</span><span class="sxs-lookup"><span data-stu-id="625c9-114">Application</span></span> | <span data-ttu-id="625c9-115">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="625c9-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="625c9-116">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="625c9-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="625c9-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="625c9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="625c9-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="625c9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="625c9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="625c9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="625c9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="625c9-120">Request headers</span></span>

| <span data-ttu-id="625c9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="625c9-121">Header</span></span>       | <span data-ttu-id="625c9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="625c9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="625c9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="625c9-123">Authorization</span></span>  | <span data-ttu-id="625c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="625c9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="625c9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="625c9-126">Request body</span></span>
<span data-ttu-id="625c9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="625c9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="625c9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="625c9-128">Response</span></span>

<span data-ttu-id="625c9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de grupo de [agendamento](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="625c9-129">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="625c9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="625c9-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="625c9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="625c9-131">Request</span></span>

<span data-ttu-id="625c9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="625c9-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="625c9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="625c9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="625c9-134">C#</span><span class="sxs-lookup"><span data-stu-id="625c9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="625c9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="625c9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="625c9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="625c9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="625c9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="625c9-137">Response</span></span>

<span data-ttu-id="625c9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="625c9-138">The following is an example of the response.</span></span> 

><span data-ttu-id="625c9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="625c9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
