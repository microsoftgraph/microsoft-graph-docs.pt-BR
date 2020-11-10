---
title: Criar timeOff
description: Criar um novo timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34e64c600b8e25c15784ce0d5ecbf636f8b59755
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972079"
---
# <a name="create-timeoff"></a><span data-ttu-id="5e636-103">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="5e636-103">Create timeOff</span></span>

<span data-ttu-id="5e636-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e636-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e636-105">Crie uma nova instância do [timeOff](../resources/timeoff.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="5e636-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e636-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e636-106">Permissions</span></span>

<span data-ttu-id="5e636-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e636-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e636-109">Permission type</span></span>      | <span data-ttu-id="5e636-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e636-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e636-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e636-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e636-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e636-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e636-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e636-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e636-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e636-114">Not supported.</span></span>    |
|<span data-ttu-id="5e636-115">Application</span><span class="sxs-lookup"><span data-stu-id="5e636-115">Application</span></span> | <span data-ttu-id="5e636-116">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="5e636-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="5e636-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="5e636-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="5e636-118">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5e636-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="5e636-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="5e636-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5e636-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e636-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="5e636-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e636-121">Request headers</span></span>

| <span data-ttu-id="5e636-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e636-122">Header</span></span>       | <span data-ttu-id="5e636-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5e636-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e636-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e636-124">Authorization</span></span>  | <span data-ttu-id="5e636-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e636-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e636-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e636-127">Content-Type</span></span>  | <span data-ttu-id="5e636-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e636-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="5e636-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e636-130">Response</span></span>

<span data-ttu-id="5e636-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e636-131">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e636-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e636-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5e636-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e636-133">Request</span></span>

<span data-ttu-id="5e636-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e636-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e636-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e636-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5e636-136">C#</span><span class="sxs-lookup"><span data-stu-id="5e636-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e636-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e636-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e636-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e636-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e636-139">Java</span><span class="sxs-lookup"><span data-stu-id="5e636-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5e636-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e636-140">Response</span></span>

<span data-ttu-id="5e636-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e636-141">The following is an example of the response.</span></span> 

><span data-ttu-id="5e636-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e636-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


