---
title: Obter turno
description: Obter um turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7059b58689173e5e47fc96ad32babbb85dc0b046
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154210"
---
# <a name="get-shift"></a><span data-ttu-id="f79e9-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="f79e9-103">Get shift</span></span>

<span data-ttu-id="f79e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f79e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f79e9-105">Recupere as propriedades e os relacionamentos de um objeto [Shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="f79e9-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f79e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f79e9-106">Permissions</span></span>

<span data-ttu-id="f79e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f79e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f79e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f79e9-109">Permission type</span></span>      | <span data-ttu-id="f79e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f79e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f79e9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f79e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f79e9-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f79e9-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f79e9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f79e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f79e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f79e9-114">Not supported.</span></span>    |<span data-ttu-id="f79e9-115">s</span><span class="sxs-lookup"><span data-stu-id="f79e9-115">s</span></span>
|<span data-ttu-id="f79e9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f79e9-116">Application</span></span> | <span data-ttu-id="f79e9-117">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="f79e9-117">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="f79e9-118">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="f79e9-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="f79e9-119">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="f79e9-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f79e9-120">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="f79e9-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f79e9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f79e9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f79e9-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f79e9-122">Optional query parameters</span></span>

<span data-ttu-id="f79e9-123">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f79e9-123">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f79e9-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f79e9-124">Request headers</span></span>

| <span data-ttu-id="f79e9-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f79e9-125">Header</span></span>       | <span data-ttu-id="f79e9-126">Valor</span><span class="sxs-lookup"><span data-stu-id="f79e9-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f79e9-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f79e9-127">Authorization</span></span>  | <span data-ttu-id="f79e9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f79e9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f79e9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f79e9-130">Request body</span></span>
<span data-ttu-id="f79e9-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f79e9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f79e9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f79e9-132">Response</span></span>

<span data-ttu-id="f79e9-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f79e9-133">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f79e9-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f79e9-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f79e9-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f79e9-135">Request</span></span>

<span data-ttu-id="f79e9-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f79e9-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f79e9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f79e9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="f79e9-138">C#</span><span class="sxs-lookup"><span data-stu-id="f79e9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f79e9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f79e9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f79e9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f79e9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f79e9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f79e9-141">Response</span></span>

<span data-ttu-id="f79e9-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f79e9-142">The following is an example of the response.</span></span> 

><span data-ttu-id="f79e9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f79e9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
