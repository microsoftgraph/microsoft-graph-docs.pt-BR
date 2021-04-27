---
title: Lista schedulingGroups
description: Obter a lista de scheduleingGroup nesta agenda.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e4d45bb7b3948a6e8626299fd35adc1308a33a6c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053507"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="37185-103">Listar scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="37185-103">List scheduleGroups</span></span>

<span data-ttu-id="37185-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37185-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37185-105">Obter a lista de [scheduleingGroups](../resources/schedulinggroup.md) nesta [agenda](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="37185-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37185-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37185-106">Permissions</span></span>

<span data-ttu-id="37185-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37185-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37185-109">Permission type</span></span>      | <span data-ttu-id="37185-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37185-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37185-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37185-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37185-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37185-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="37185-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37185-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37185-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37185-114">Not supported.</span></span>    |
|<span data-ttu-id="37185-115">Application</span><span class="sxs-lookup"><span data-stu-id="37185-115">Application</span></span> | <span data-ttu-id="37185-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37185-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37185-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37185-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="37185-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37185-118">Request headers</span></span>

| <span data-ttu-id="37185-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37185-119">Header</span></span>       | <span data-ttu-id="37185-120">Valor</span><span class="sxs-lookup"><span data-stu-id="37185-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37185-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37185-121">Authorization</span></span>  | <span data-ttu-id="37185-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37185-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37185-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37185-124">Request body</span></span>
<span data-ttu-id="37185-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37185-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37185-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="37185-126">Response</span></span>

<span data-ttu-id="37185-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos schedulingGroup](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37185-127">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37185-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37185-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="37185-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37185-129">Request</span></span>

<span data-ttu-id="37185-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37185-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37185-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="37185-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="37185-132">C#</span><span class="sxs-lookup"><span data-stu-id="37185-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37185-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37185-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37185-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37185-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37185-135">Java</span><span class="sxs-lookup"><span data-stu-id="37185-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37185-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="37185-136">Response</span></span>

<span data-ttu-id="37185-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37185-137">The following is an example of the response.</span></span> 

><span data-ttu-id="37185-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37185-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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


