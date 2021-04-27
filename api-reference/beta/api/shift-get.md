---
title: Obter turno
description: Obter um turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09e2f1542d18210b733ecd89b08972ed29d3b9e3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051862"
---
# <a name="get-shift"></a><span data-ttu-id="50f0e-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="50f0e-103">Get shift</span></span>

<span data-ttu-id="50f0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50f0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50f0e-105">Recupere as propriedades e as relações de um [objeto shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="50f0e-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="50f0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50f0e-106">Permissions</span></span>

<span data-ttu-id="50f0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50f0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50f0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50f0e-109">Permission type</span></span>      | <span data-ttu-id="50f0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50f0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50f0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50f0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50f0e-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f0e-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="50f0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50f0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50f0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50f0e-114">Not supported.</span></span>    |
|<span data-ttu-id="50f0e-115">Application</span><span class="sxs-lookup"><span data-stu-id="50f0e-115">Application</span></span> | <span data-ttu-id="50f0e-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f0e-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50f0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50f0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50f0e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50f0e-118">Optional query parameters</span></span>

<span data-ttu-id="50f0e-119">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50f0e-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50f0e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50f0e-120">Request headers</span></span>

| <span data-ttu-id="50f0e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50f0e-121">Header</span></span>       | <span data-ttu-id="50f0e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="50f0e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50f0e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="50f0e-123">Authorization</span></span>  | <span data-ttu-id="50f0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50f0e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50f0e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50f0e-126">Request body</span></span>
<span data-ttu-id="50f0e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50f0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50f0e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f0e-128">Response</span></span>

<span data-ttu-id="50f0e-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50f0e-129">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50f0e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50f0e-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="50f0e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50f0e-131">Request</span></span>

<span data-ttu-id="50f0e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50f0e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50f0e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="50f0e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="50f0e-134">C#</span><span class="sxs-lookup"><span data-stu-id="50f0e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50f0e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50f0e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50f0e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50f0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50f0e-137">Java</span><span class="sxs-lookup"><span data-stu-id="50f0e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="50f0e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="50f0e-138">Response</span></span>

<span data-ttu-id="50f0e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50f0e-139">The following is an example of the response.</span></span>

><span data-ttu-id="50f0e-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="50f0e-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHFT_ca485cdd-a42c-4b93-9e6a-6fa54fd45fe1",
    "createdDateTime": "2019-06-06T20:15:38.9Z",
    "lastModifiedDateTime": "2019-11-18T01:12:08.318Z",
    "schedulingGroupId": "TAG_d18fd675-3ac8-41b2-8038-d17fdac8b0d3",
    "userId": "a7b0c8c4-3f5c-492f-ab13-40f0e0f0ffa8",
    "draftShift": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "1c717a55-febd-4850-b5f6-101f3a29972c",
            "displayName": "Sumanth Lingom"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


