---
title: Obter timeOff
description: Obtenha um timeOff por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f1fdd14a155c7113425916081ed38f5745267e2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637529"
---
# <a name="get-timeoff"></a><span data-ttu-id="91649-103">Obter timeOff</span><span class="sxs-lookup"><span data-stu-id="91649-103">Get timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91649-104">Recupere as propriedades e os relacionamentos de um objeto [timeOff](../resources/timeoff.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="91649-104">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="91649-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="91649-105">Permissions</span></span>

<span data-ttu-id="91649-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91649-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91649-108">Permission type</span></span>      | <span data-ttu-id="91649-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91649-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91649-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91649-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91649-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91649-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91649-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91649-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91649-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91649-113">Not supported.</span></span>    |
|<span data-ttu-id="91649-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91649-114">Application</span></span> | <span data-ttu-id="91649-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91649-115">Not supported.</span></span> |

> <span data-ttu-id="91649-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="91649-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="91649-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="91649-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="91649-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91649-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="91649-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91649-119">Request headers</span></span>

| <span data-ttu-id="91649-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91649-120">Header</span></span>       | <span data-ttu-id="91649-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91649-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91649-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91649-122">Authorization</span></span>  | <span data-ttu-id="91649-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91649-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91649-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91649-125">Content-Type</span></span>  | <span data-ttu-id="91649-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91649-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91649-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91649-127">Request body</span></span>
<span data-ttu-id="91649-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91649-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91649-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="91649-129">Response</span></span>

<span data-ttu-id="91649-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91649-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91649-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91649-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="91649-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91649-132">Request</span></span>

<span data-ttu-id="91649-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91649-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="91649-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="91649-134">Response</span></span>

<span data-ttu-id="91649-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91649-135">The following is an example of the response.</span></span> 

><span data-ttu-id="91649-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91649-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="91649-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="91649-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="91649-139">Basic</span><span class="sxs-lookup"><span data-stu-id="91649-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91649-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91649-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-get-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
