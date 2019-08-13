---
title: Substituir timeOff
description: Substitua um timeOff existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79dd3e8d631a51338ff3f8db09d1ed915a6fdcbe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362616"
---
# <a name="replace-timeoff"></a><span data-ttu-id="a1871-103">Substituir timeOff</span><span class="sxs-lookup"><span data-stu-id="a1871-103">Replace timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1871-104">Substitua um [timeOff](../resources/timeoff.md)existente.</span><span class="sxs-lookup"><span data-stu-id="a1871-104">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="a1871-105">Se o [timeOff](../resources/timeoff.md) especificado não existir, este método retornará `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="a1871-105">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1871-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1871-106">Permissions</span></span>

<span data-ttu-id="a1871-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1871-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1871-109">Permission type</span></span>      | <span data-ttu-id="a1871-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1871-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1871-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1871-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a1871-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1871-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1871-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1871-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1871-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1871-114">Not supported.</span></span>    |
|<span data-ttu-id="a1871-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1871-115">Application</span></span> | <span data-ttu-id="a1871-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1871-116">Not supported.</span></span> |

> <span data-ttu-id="a1871-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a1871-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a1871-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a1871-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a1871-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1871-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="a1871-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1871-120">Request headers</span></span>

| <span data-ttu-id="a1871-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1871-121">Header</span></span>       | <span data-ttu-id="a1871-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1871-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a1871-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1871-123">Authorization</span></span>  | <span data-ttu-id="a1871-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1871-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a1871-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1871-126">Content-Type</span></span>  | <span data-ttu-id="a1871-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1871-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1871-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1871-128">Request body</span></span>

<span data-ttu-id="a1871-129">No corpo da solicitação, forneça uma representação JSON de um objeto [timeOff](../resources/timeoff.md) .</span><span class="sxs-lookup"><span data-stu-id="a1871-129">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a1871-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1871-130">Response</span></span>

<span data-ttu-id="a1871-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1871-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1871-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1871-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a1871-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1871-133">Request</span></span>

<span data-ttu-id="a1871-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1871-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1871-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1871-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1871-136">C#</span><span class="sxs-lookup"><span data-stu-id="a1871-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1871-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1871-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1871-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a1871-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a1871-139">Java</span><span class="sxs-lookup"><span data-stu-id="a1871-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a1871-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1871-140">Response</span></span>

<span data-ttu-id="a1871-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1871-141">The following is an example of the response.</span></span> 

><span data-ttu-id="a1871-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1871-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "@odata.type":"microsoft.graph.identitySet",
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
