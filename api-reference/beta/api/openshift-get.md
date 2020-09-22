---
title: Obter openShift
description: Recupere as propriedades e os relacionamentos do objeto openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5d8e17d81281adb77c510f3cc80427ebcfb4bcff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010721"
---
# <a name="get-openshift"></a><span data-ttu-id="bb968-103">Obter openShift</span><span class="sxs-lookup"><span data-stu-id="bb968-103">Get openShift</span></span>

<span data-ttu-id="bb968-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb968-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb968-105">Recupere as propriedades e os relacionamentos de um objeto [openshift](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="bb968-105">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb968-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb968-106">Permissions</span></span>

<span data-ttu-id="bb968-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb968-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb968-109">Permission type</span></span>                        | <span data-ttu-id="bb968-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb968-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb968-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb968-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb968-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb968-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bb968-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb968-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb968-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb968-114">Not supported.</span></span> |
| <span data-ttu-id="bb968-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb968-115">Application</span></span>                            | <span data-ttu-id="bb968-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb968-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb968-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb968-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb968-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb968-118">Optional query parameters</span></span>

<span data-ttu-id="bb968-119">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb968-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb968-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb968-120">Request headers</span></span>

| <span data-ttu-id="bb968-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bb968-121">Name</span></span>      |<span data-ttu-id="bb968-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb968-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb968-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb968-123">Authorization</span></span> | <span data-ttu-id="bb968-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb968-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb968-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb968-126">Request body</span></span>

<span data-ttu-id="bb968-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb968-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb968-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb968-128">Response</span></span>

<span data-ttu-id="bb968-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [openShift](../resources/openshift.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb968-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb968-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb968-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb968-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb968-131">Request</span></span>

<span data-ttu-id="bb968-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb968-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb968-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb968-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="bb968-134">C#</span><span class="sxs-lookup"><span data-stu-id="bb968-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb968-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb968-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb968-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb968-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb968-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb968-137">Response</span></span>

<span data-ttu-id="bb968-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb968-138">The following is an example of the response.</span></span>

> <span data-ttu-id="bb968-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb968-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


