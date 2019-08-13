---
title: Criar timeOff
description: Criar um novo timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b8d0199f79c31255a8430ddb8d5c3c7d082ccf9c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364483"
---
# <a name="create-timeoff"></a><span data-ttu-id="f296b-103">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="f296b-103">Create timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f296b-104">Crie uma nova instância do [timeOff](../resources/timeoff.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f296b-104">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f296b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f296b-105">Permissions</span></span>

<span data-ttu-id="f296b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f296b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f296b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f296b-108">Permission type</span></span>      | <span data-ttu-id="f296b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f296b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f296b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f296b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f296b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f296b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f296b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f296b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f296b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f296b-113">Not supported.</span></span>    |
|<span data-ttu-id="f296b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f296b-114">Application</span></span> | <span data-ttu-id="f296b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f296b-115">Not supported.</span></span> |

> <span data-ttu-id="f296b-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="f296b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f296b-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="f296b-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f296b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f296b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="f296b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f296b-119">Request headers</span></span>

| <span data-ttu-id="f296b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f296b-120">Header</span></span>       | <span data-ttu-id="f296b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f296b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f296b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f296b-122">Authorization</span></span>  | <span data-ttu-id="f296b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f296b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f296b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f296b-125">Content-Type</span></span>  | <span data-ttu-id="f296b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f296b-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="f296b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f296b-127">Response</span></span>

<span data-ttu-id="f296b-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f296b-128">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f296b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f296b-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f296b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f296b-130">Request</span></span>

<span data-ttu-id="f296b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f296b-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f296b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f296b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff
Content-type: application/json

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f296b-133">C#</span><span class="sxs-lookup"><span data-stu-id="f296b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f296b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f296b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f296b-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f296b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f296b-136">Java</span><span class="sxs-lookup"><span data-stu-id="f296b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f296b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f296b-137">Response</span></span>

<span data-ttu-id="f296b-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f296b-138">The following is an example of the response.</span></span> 

><span data-ttu-id="f296b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f296b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type":"microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 201 Created
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
