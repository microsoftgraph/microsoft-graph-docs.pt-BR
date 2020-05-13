---
title: Listar openShifts
description: Listar objetos openshift em uma equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bc65d419addf58bbf7b0a715c61538491777a5ec
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "42456415"
---
# <a name="list-openshift"></a><span data-ttu-id="d29a8-103">Listar openShift</span><span class="sxs-lookup"><span data-stu-id="d29a8-103">List openShift</span></span>

<span data-ttu-id="d29a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d29a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d29a8-105">Listar objetos [openshift](../resources/openshift.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d29a8-105">List [openshift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="d29a8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d29a8-106">Permissions</span></span>

<span data-ttu-id="d29a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d29a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d29a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d29a8-109">Permission type</span></span>                        | <span data-ttu-id="d29a8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d29a8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d29a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d29a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d29a8-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d29a8-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d29a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d29a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d29a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d29a8-114">Not supported.</span></span> |
| <span data-ttu-id="d29a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d29a8-115">Application</span></span>                            | <span data-ttu-id="d29a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d29a8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d29a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d29a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d29a8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d29a8-118">Optional query parameters</span></span>

<span data-ttu-id="d29a8-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d29a8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d29a8-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d29a8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="d29a8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d29a8-121">Request headers</span></span>

| <span data-ttu-id="d29a8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d29a8-122">Name</span></span>      |<span data-ttu-id="d29a8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d29a8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d29a8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d29a8-124">Authorization</span></span> | <span data-ttu-id="d29a8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d29a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d29a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d29a8-127">Request body</span></span>

<span data-ttu-id="d29a8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d29a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d29a8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d29a8-129">Response</span></span>

<span data-ttu-id="d29a8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e todos os objetos [openShift](../resources/openshift.md) na equipe no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d29a8-130">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d29a8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d29a8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d29a8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d29a8-132">Request</span></span>

<span data-ttu-id="d29a8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d29a8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d29a8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d29a8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
```
# <a name="c"></a>[<span data-ttu-id="d29a8-135">C#</span><span class="sxs-lookup"><span data-stu-id="d29a8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d29a8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d29a8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d29a8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d29a8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d29a8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d29a8-138">Response</span></span>

<span data-ttu-id="d29a8-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d29a8-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d29a8-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d29a8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":2,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":3,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.332Z",
  "endDateTime": "2018-10-04T08:58:45.340Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T07:58:45.332Z",
  "code": "Break",
  "displayName": "Lunch"
  }
  ]
  },
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
