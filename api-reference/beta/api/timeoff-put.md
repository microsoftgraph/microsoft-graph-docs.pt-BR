---
title: Substituir timeOff
description: Substitua um timeOff existente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d666f9834e5377e5145b2fe0feea801842cb8f5f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048971"
---
# <a name="replace-timeoff"></a><span data-ttu-id="926e0-103">Substituir timeOff</span><span class="sxs-lookup"><span data-stu-id="926e0-103">Replace timeOff</span></span>

<span data-ttu-id="926e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="926e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="926e0-105">Substitua um [timeOff existente.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="926e0-105">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="926e0-106">Se o [timeOff](../resources/timeoff.md) especificado não existir, este método retornará `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="926e0-106">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="926e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="926e0-107">Permissions</span></span>

<span data-ttu-id="926e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="926e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="926e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="926e0-110">Permission type</span></span>      | <span data-ttu-id="926e0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="926e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="926e0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="926e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="926e0-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="926e0-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="926e0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="926e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="926e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="926e0-115">Not supported.</span></span>    |
|<span data-ttu-id="926e0-116">Application</span><span class="sxs-lookup"><span data-stu-id="926e0-116">Application</span></span> | <span data-ttu-id="926e0-117">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="926e0-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="926e0-118">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="926e0-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="926e0-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="926e0-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="926e0-120">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="926e0-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="926e0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="926e0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="926e0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="926e0-122">Request headers</span></span>

| <span data-ttu-id="926e0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="926e0-123">Header</span></span>       | <span data-ttu-id="926e0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="926e0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="926e0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="926e0-125">Authorization</span></span>  | <span data-ttu-id="926e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="926e0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="926e0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="926e0-128">Content-Type</span></span>  | <span data-ttu-id="926e0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="926e0-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="926e0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="926e0-131">Request body</span></span>

<span data-ttu-id="926e0-132">No corpo da solicitação, fornece uma representação JSON de um [objeto timeOff.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="926e0-132">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="926e0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="926e0-133">Response</span></span>

<span data-ttu-id="926e0-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="926e0-134">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="926e0-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="926e0-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="926e0-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="926e0-136">Request</span></span>

<span data-ttu-id="926e0-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="926e0-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="926e0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="926e0-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="926e0-139">C#</span><span class="sxs-lookup"><span data-stu-id="926e0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="926e0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="926e0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="926e0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="926e0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="926e0-142">Java</span><span class="sxs-lookup"><span data-stu-id="926e0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="926e0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="926e0-143">Response</span></span>

<span data-ttu-id="926e0-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="926e0-144">The following is an example of the response.</span></span> 

><span data-ttu-id="926e0-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="926e0-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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


