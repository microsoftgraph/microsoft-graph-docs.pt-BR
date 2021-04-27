---
title: Criar schedulingGroup
description: Criar um nov schedulingGroup.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ef8ae3c8f878d6414929997e75e5ece29434a09d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052723"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="519e5-103">Criar schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="519e5-103">Create schedulingGroup</span></span>

<span data-ttu-id="519e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="519e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="519e5-105">Criar um nov [schedulingGroup](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="519e5-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="519e5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="519e5-106">Permissions</span></span>

<span data-ttu-id="519e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="519e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="519e5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="519e5-109">Permission type</span></span>      | <span data-ttu-id="519e5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="519e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="519e5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="519e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="519e5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="519e5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="519e5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="519e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="519e5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="519e5-114">Not supported.</span></span>    |
|<span data-ttu-id="519e5-115">Application</span><span class="sxs-lookup"><span data-stu-id="519e5-115">Application</span></span> |<span data-ttu-id="519e5-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="519e5-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="519e5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="519e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="519e5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="519e5-118">Request headers</span></span>

| <span data-ttu-id="519e5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="519e5-119">Header</span></span>       | <span data-ttu-id="519e5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="519e5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="519e5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="519e5-121">Authorization</span></span>  | <span data-ttu-id="519e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="519e5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="519e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="519e5-124">Content-Type</span></span>  | <span data-ttu-id="519e5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="519e5-p103">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="519e5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="519e5-127">Response</span></span>

<span data-ttu-id="519e5-128">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto schedulingGroup](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="519e5-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="519e5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="519e5-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="519e5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="519e5-130">Request</span></span>

<span data-ttu-id="519e5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="519e5-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="519e5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="519e5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="519e5-133">C#</span><span class="sxs-lookup"><span data-stu-id="519e5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="519e5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519e5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="519e5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="519e5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="519e5-136">Java</span><span class="sxs-lookup"><span data-stu-id="519e5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519e5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="519e5-137">Response</span></span>

<span data-ttu-id="519e5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="519e5-138">The following is an example of the response.</span></span> 

><span data-ttu-id="519e5-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="519e5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


