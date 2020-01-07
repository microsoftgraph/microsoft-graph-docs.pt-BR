---
title: Obter turno
description: Obter um turno por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9602457402e833674e24f5ee40ec72691975f5e3
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951693"
---
# <a name="get-shift"></a><span data-ttu-id="8bec8-103">Obter turno</span><span class="sxs-lookup"><span data-stu-id="8bec8-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bec8-104">Recupere as propriedades e os relacionamentos de um objeto [Shift](../resources/shift.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="8bec8-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bec8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bec8-105">Permissions</span></span>

<span data-ttu-id="8bec8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bec8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bec8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bec8-108">Permission type</span></span>      | <span data-ttu-id="8bec8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bec8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bec8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bec8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bec8-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bec8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bec8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bec8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bec8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bec8-113">Not supported.</span></span>    |<span data-ttu-id="8bec8-114">s</span><span class="sxs-lookup"><span data-stu-id="8bec8-114">s</span></span>
|<span data-ttu-id="8bec8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bec8-115">Application</span></span> | <span data-ttu-id="8bec8-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="8bec8-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="8bec8-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="8bec8-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="8bec8-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8bec8-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8bec8-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8bec8-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8bec8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bec8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="8bec8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bec8-121">Request headers</span></span>

| <span data-ttu-id="8bec8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bec8-122">Header</span></span>       | <span data-ttu-id="8bec8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8bec8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8bec8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bec8-124">Authorization</span></span>  | <span data-ttu-id="8bec8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bec8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8bec8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bec8-127">Request body</span></span>
<span data-ttu-id="8bec8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bec8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bec8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bec8-129">Response</span></span>

<span data-ttu-id="8bec8-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Shift](../resources/shift.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bec8-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bec8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bec8-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8bec8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bec8-132">Request</span></span>

<span data-ttu-id="8bec8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bec8-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bec8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bec8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bec8-135">C#</span><span class="sxs-lookup"><span data-stu-id="8bec8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bec8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bec8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bec8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bec8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8bec8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bec8-138">Response</span></span>

<span data-ttu-id="8bec8-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bec8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="8bec8-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bec8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
