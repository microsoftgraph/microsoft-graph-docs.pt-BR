---
title: Criar timeOff
description: Crie um novo timeOff.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 14cda6031e07ecf694ce771ad3a08a014057c25e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039045"
---
# <a name="create-timeoff"></a><span data-ttu-id="6ad99-103">Criar timeOff</span><span class="sxs-lookup"><span data-stu-id="6ad99-103">Create timeOff</span></span>

<span data-ttu-id="6ad99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ad99-105">Crie uma nova [instância timeOff](../resources/timeoff.md) em um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="6ad99-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ad99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ad99-106">Permissions</span></span>

<span data-ttu-id="6ad99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ad99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ad99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ad99-109">Permission type</span></span>      | <span data-ttu-id="6ad99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ad99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ad99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ad99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ad99-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad99-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ad99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ad99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ad99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ad99-114">Not supported.</span></span>    |
|<span data-ttu-id="6ad99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ad99-115">Application</span></span> | <span data-ttu-id="6ad99-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad99-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="6ad99-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6ad99-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6ad99-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="6ad99-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6ad99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ad99-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="6ad99-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad99-120">Request headers</span></span>

| <span data-ttu-id="6ad99-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ad99-121">Header</span></span>       | <span data-ttu-id="6ad99-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ad99-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ad99-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ad99-123">Authorization</span></span>  | <span data-ttu-id="6ad99-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ad99-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6ad99-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ad99-126">Content-Type</span></span>  | <span data-ttu-id="6ad99-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ad99-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="6ad99-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ad99-129">Response</span></span>

<span data-ttu-id="6ad99-130">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ad99-130">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ad99-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ad99-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ad99-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ad99-132">Request</span></span>

<span data-ttu-id="6ad99-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ad99-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ad99-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ad99-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff
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
# <a name="c"></a>[<span data-ttu-id="6ad99-135">C#</span><span class="sxs-lookup"><span data-stu-id="6ad99-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ad99-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ad99-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ad99-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ad99-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ad99-138">Java</span><span class="sxs-lookup"><span data-stu-id="6ad99-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="6ad99-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ad99-139">Response</span></span>

<span data-ttu-id="6ad99-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ad99-140">The following is an example of the response.</span></span> 

><span data-ttu-id="6ad99-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ad99-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

