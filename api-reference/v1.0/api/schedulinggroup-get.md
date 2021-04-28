---
title: Obter schedulingGroup
description: Recupere as propriedades e as relações de um [schedulingGroup](../resources/schedulinggroup.md) por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d9b483dd038c7b36688332628fbe7fb94e3a2df2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039031"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="5d6aa-103">Obter schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="5d6aa-103">Get schedulingGroup</span></span>

<span data-ttu-id="5d6aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d6aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d6aa-105">Recupere as propriedades e as relações de um [schedulingGroup](../resources/schedulinggroup.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d6aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d6aa-106">Permissions</span></span>

<span data-ttu-id="5d6aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d6aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d6aa-109">Permission type</span></span>      | <span data-ttu-id="5d6aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d6aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d6aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d6aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d6aa-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d6aa-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d6aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d6aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d6aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-114">Not supported.</span></span>    |
|<span data-ttu-id="5d6aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d6aa-115">Application</span></span> | <span data-ttu-id="5d6aa-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d6aa-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d6aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d6aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d6aa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d6aa-118">Optional query parameters</span></span>

<span data-ttu-id="5d6aa-119">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d6aa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d6aa-120">Request headers</span></span>

| <span data-ttu-id="5d6aa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d6aa-121">Header</span></span>       | <span data-ttu-id="5d6aa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5d6aa-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d6aa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d6aa-123">Authorization</span></span>  | <span data-ttu-id="5d6aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d6aa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d6aa-126">Request body</span></span>
<span data-ttu-id="5d6aa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d6aa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d6aa-128">Response</span></span>

<span data-ttu-id="5d6aa-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto schedulingGroup](../resources/schedulinggroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-129">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d6aa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d6aa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d6aa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d6aa-131">Request</span></span>

<span data-ttu-id="5d6aa-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d6aa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d6aa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="5d6aa-134">C#</span><span class="sxs-lookup"><span data-stu-id="5d6aa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d6aa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d6aa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d6aa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d6aa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d6aa-137">Java</span><span class="sxs-lookup"><span data-stu-id="5d6aa-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="5d6aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d6aa-138">Response</span></span>

<span data-ttu-id="5d6aa-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-139">The following is an example of the response.</span></span> 

><span data-ttu-id="5d6aa-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d6aa-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

