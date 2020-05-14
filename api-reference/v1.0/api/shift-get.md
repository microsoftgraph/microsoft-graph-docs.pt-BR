---
title: Obter turno
description: Obter um turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dbeedc59e39e6efe06a2989199ef53d7ced20b1e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216683"
---
# <a name="get-shift"></a><span data-ttu-id="685c4-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="685c4-103">Get shift</span></span>

<span data-ttu-id="685c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="685c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="685c4-105">Recupere as propriedades e os relacionamentos de um objeto [Shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="685c4-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="685c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="685c4-106">Permissions</span></span>

<span data-ttu-id="685c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="685c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="685c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="685c4-109">Permission type</span></span>      | <span data-ttu-id="685c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="685c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="685c4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="685c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="685c4-112">Schedule. Read. All, Group. Read. All, Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="685c4-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="685c4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="685c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="685c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="685c4-114">Not supported.</span></span>    |<span data-ttu-id="685c4-115">s</span><span class="sxs-lookup"><span data-stu-id="685c4-115">s</span></span>
|<span data-ttu-id="685c4-116">Application</span><span class="sxs-lookup"><span data-stu-id="685c4-116">Application</span></span> | <span data-ttu-id="685c4-117">Schedule. Read. All, Schedule. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="685c4-117">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="685c4-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="685c4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="685c4-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="685c4-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="685c4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="685c4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="685c4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="685c4-121">Optional query parameters</span></span>

<span data-ttu-id="685c4-122">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="685c4-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="685c4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="685c4-123">Request headers</span></span>

| <span data-ttu-id="685c4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="685c4-124">Header</span></span>       | <span data-ttu-id="685c4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="685c4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="685c4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="685c4-126">Authorization</span></span>  | <span data-ttu-id="685c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="685c4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="685c4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="685c4-129">Request body</span></span>
<span data-ttu-id="685c4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="685c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="685c4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="685c4-131">Response</span></span>

<span data-ttu-id="685c4-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="685c4-132">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="685c4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="685c4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="685c4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="685c4-134">Request</span></span>

<span data-ttu-id="685c4-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="685c4-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="685c4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="685c4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="685c4-137">C#</span><span class="sxs-lookup"><span data-stu-id="685c4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="685c4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="685c4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="685c4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="685c4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="685c4-140">Java</span><span class="sxs-lookup"><span data-stu-id="685c4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="685c4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="685c4-141">Response</span></span>

<span data-ttu-id="685c4-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="685c4-142">The following is an example of the response.</span></span>

><span data-ttu-id="685c4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="685c4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
