---
title: Obter turno
description: Obter um turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b0a105d8002a3b257322a7841bae8927bcaee0f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960695"
---
# <a name="get-shift"></a><span data-ttu-id="b1018-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="b1018-103">Get shift</span></span>

<span data-ttu-id="b1018-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1018-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1018-105">Recupere as propriedades e as relações de um [objeto shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="b1018-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1018-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1018-106">Permissions</span></span>

<span data-ttu-id="b1018-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1018-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1018-109">Permission type</span></span>      | <span data-ttu-id="b1018-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1018-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1018-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1018-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1018-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1018-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1018-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1018-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1018-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1018-114">Not supported.</span></span>    |
|<span data-ttu-id="b1018-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1018-115">Application</span></span> | <span data-ttu-id="b1018-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1018-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1018-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1018-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1018-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1018-118">Optional query parameters</span></span>

<span data-ttu-id="b1018-119">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1018-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1018-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1018-120">Request headers</span></span>

| <span data-ttu-id="b1018-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1018-121">Header</span></span>       | <span data-ttu-id="b1018-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1018-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1018-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1018-123">Authorization</span></span>  | <span data-ttu-id="b1018-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1018-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1018-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1018-126">Request body</span></span>
<span data-ttu-id="b1018-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1018-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1018-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1018-128">Response</span></span>

<span data-ttu-id="b1018-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1018-129">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1018-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1018-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b1018-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1018-131">Request</span></span>

<span data-ttu-id="b1018-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1018-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1018-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1018-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="b1018-134">C#</span><span class="sxs-lookup"><span data-stu-id="b1018-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1018-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1018-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1018-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1018-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1018-137">Java</span><span class="sxs-lookup"><span data-stu-id="b1018-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b1018-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1018-138">Response</span></span>

<span data-ttu-id="b1018-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1018-139">The following is an example of the response.</span></span>

><span data-ttu-id="b1018-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1018-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


