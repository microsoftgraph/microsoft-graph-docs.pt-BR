---
title: Obter turno
description: Obter um turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 729fd92406ff1d6e301e4520737a954a1b300d6f
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845425"
---
# <a name="get-shift"></a><span data-ttu-id="447d8-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="447d8-103">Get shift</span></span>

<span data-ttu-id="447d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="447d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="447d8-105">Recupere as propriedades e os relacionamentos de um objeto [Shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="447d8-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="447d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="447d8-106">Permissions</span></span>

<span data-ttu-id="447d8-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="447d8-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="447d8-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="447d8-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="447d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="447d8-109">Permission type</span></span>                        | <span data-ttu-id="447d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="447d8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="447d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="447d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="447d8-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="447d8-112">Group.Read.All, Group.ReadWrite.All</span></span>         |
| <span data-ttu-id="447d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="447d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="447d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="447d8-114">Not supported.</span></span>                              |
| <span data-ttu-id="447d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="447d8-115">Application</span></span>                            | <span data-ttu-id="447d8-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="447d8-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="447d8-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="447d8-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="447d8-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="447d8-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="447d8-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="447d8-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="447d8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="447d8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="447d8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="447d8-121">Optional query parameters</span></span>

<span data-ttu-id="447d8-122">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="447d8-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="447d8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="447d8-123">Request headers</span></span>

| <span data-ttu-id="447d8-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="447d8-124">Header</span></span>       | <span data-ttu-id="447d8-125">Valor</span><span class="sxs-lookup"><span data-stu-id="447d8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="447d8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="447d8-126">Authorization</span></span>  | <span data-ttu-id="447d8-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="447d8-127">Bearer {token}.</span></span> <span data-ttu-id="447d8-128">Required.</span><span class="sxs-lookup"><span data-stu-id="447d8-128">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="447d8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="447d8-129">Request body</span></span>
<span data-ttu-id="447d8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="447d8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="447d8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="447d8-131">Response</span></span>

<span data-ttu-id="447d8-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="447d8-132">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="447d8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="447d8-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="447d8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="447d8-134">Request</span></span>

<span data-ttu-id="447d8-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="447d8-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="447d8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="447d8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="447d8-137">C#</span><span class="sxs-lookup"><span data-stu-id="447d8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="447d8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="447d8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="447d8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="447d8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="447d8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="447d8-140">Response</span></span>

<span data-ttu-id="447d8-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="447d8-141">The following is an example of the response.</span></span>

><span data-ttu-id="447d8-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="447d8-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="447d8-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="447d8-143">All the properties will be returned from an actual call.</span></span>
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
