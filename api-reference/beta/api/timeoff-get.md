---
title: Obter timeOff
description: Obter um timeOff por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed27e604d15ae7df87b9f180a378bfec480d7632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787482"
---
# <a name="get-timeoff"></a><span data-ttu-id="14e90-103">Obter timeOff</span><span class="sxs-lookup"><span data-stu-id="14e90-103">Get timeOff</span></span>

<span data-ttu-id="14e90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14e90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14e90-105">Recupere as propriedades e as relações de um [objeto timeOff](../resources/timeoff.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="14e90-105">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="14e90-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="14e90-106">Permissions</span></span>

<span data-ttu-id="14e90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14e90-109">Permission type</span></span>      | <span data-ttu-id="14e90-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14e90-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14e90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14e90-111">Delegated (work or school account)</span></span> | <span data-ttu-id="14e90-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e90-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14e90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14e90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14e90-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14e90-114">Not supported.</span></span>    |
|<span data-ttu-id="14e90-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14e90-115">Application</span></span> | <span data-ttu-id="14e90-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="14e90-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="14e90-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="14e90-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="14e90-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="14e90-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="14e90-119">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="14e90-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="14e90-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14e90-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14e90-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14e90-121">Optional query parameters</span></span>

<span data-ttu-id="14e90-122">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14e90-122">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="14e90-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14e90-123">Request headers</span></span>

| <span data-ttu-id="14e90-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14e90-124">Header</span></span>       | <span data-ttu-id="14e90-125">Valor</span><span class="sxs-lookup"><span data-stu-id="14e90-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14e90-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="14e90-126">Authorization</span></span>  | <span data-ttu-id="14e90-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14e90-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14e90-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14e90-129">Request body</span></span>
<span data-ttu-id="14e90-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14e90-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14e90-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e90-131">Response</span></span>

<span data-ttu-id="14e90-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [timeOff](../resources/timeoff.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14e90-132">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14e90-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14e90-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="14e90-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14e90-134">Request</span></span>

<span data-ttu-id="14e90-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14e90-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14e90-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="14e90-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="14e90-137">C#</span><span class="sxs-lookup"><span data-stu-id="14e90-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14e90-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14e90-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14e90-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14e90-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14e90-140">Java</span><span class="sxs-lookup"><span data-stu-id="14e90-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14e90-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="14e90-141">Response</span></span>

<span data-ttu-id="14e90-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14e90-142">The following is an example of the response.</span></span> 

><span data-ttu-id="14e90-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14e90-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->


