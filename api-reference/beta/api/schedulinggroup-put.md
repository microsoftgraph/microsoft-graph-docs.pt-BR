---
title: Subtituir schedulingGroup
description: Substitua um schedulingGroup existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 776dd553c6573455e5577156a52e9b5d69a7add8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051995"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="9c2b6-103">Subtituir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="9c2b6-103">Replace schedulingGroup</span></span>

<span data-ttu-id="9c2b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c2b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c2b6-105">Substitua um [schedulingGroup existente.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="9c2b6-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="9c2b6-106">Se o [schedulingGroup especificado](../resources/schedulinggroup.md) não existir, este método retornará `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="9c2b6-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c2b6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c2b6-107">Permissions</span></span>

<span data-ttu-id="9c2b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c2b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c2b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c2b6-110">Permission type</span></span>      | <span data-ttu-id="9c2b6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c2b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c2b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c2b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c2b6-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c2b6-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c2b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c2b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c2b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-115">Not supported.</span></span>    |
|<span data-ttu-id="9c2b6-116">Application</span><span class="sxs-lookup"><span data-stu-id="9c2b6-116">Application</span></span> | <span data-ttu-id="9c2b6-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c2b6-117">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c2b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c2b6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="9c2b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c2b6-119">Request headers</span></span>

| <span data-ttu-id="9c2b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c2b6-120">Header</span></span>       | <span data-ttu-id="9c2b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9c2b6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c2b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c2b6-122">Authorization</span></span>  | <span data-ttu-id="9c2b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9c2b6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c2b6-125">Content-Type</span></span>  | <span data-ttu-id="9c2b6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c2b6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c2b6-128">Request body</span></span>

<span data-ttu-id="9c2b6-129">No corpo da solicitação, fornece uma representação JSON de [um objeto schedulingGroup.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="9c2b6-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9c2b6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c2b6-130">Response</span></span>

<span data-ttu-id="9c2b6-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto schedulingGroup](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c2b6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c2b6-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9c2b6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c2b6-133">Request</span></span>

<span data-ttu-id="9c2b6-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c2b6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c2b6-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9c2b6-136">C#</span><span class="sxs-lookup"><span data-stu-id="9c2b6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c2b6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c2b6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c2b6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c2b6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c2b6-139">Java</span><span class="sxs-lookup"><span data-stu-id="9c2b6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-put-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c2b6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c2b6-140">Response</span></span>

<span data-ttu-id="9c2b6-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-141">The following is an example of the response.</span></span> 

><span data-ttu-id="9c2b6-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c2b6-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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


