---
title: Obter timeOffReason
description: Obter um timeOffReason por ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bead10296f64422dc013dd4d9b7a01408ba19974
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048950"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="9c9b4-103">Obter timeOffReason</span><span class="sxs-lookup"><span data-stu-id="9c9b4-103">Get timeOffReason</span></span>

<span data-ttu-id="9c9b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c9b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c9b4-105">Recupere as propriedades e as relações de um [objeto timeOffReason](../resources/timeoffreason.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-105">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c9b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c9b4-106">Permissions</span></span>

<span data-ttu-id="9c9b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c9b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c9b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c9b4-109">Permission type</span></span>      | <span data-ttu-id="9c9b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c9b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c9b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c9b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c9b4-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c9b4-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c9b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c9b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c9b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-114">Not supported.</span></span>    |
|<span data-ttu-id="9c9b4-115">Application</span><span class="sxs-lookup"><span data-stu-id="9c9b4-115">Application</span></span> | <span data-ttu-id="9c9b4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="9c9b4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="9c9b4-117">\***Importante:** As permissões de aplicativo estão atualmente apenas em visualização privada e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="9c9b4-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9c9b4-119">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9c9b4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c9b4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c9b4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c9b4-121">Optional query parameters</span></span>

<span data-ttu-id="9c9b4-122">Este método não dá suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c9b4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c9b4-123">Request headers</span></span>

| <span data-ttu-id="9c9b4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c9b4-124">Header</span></span>       | <span data-ttu-id="9c9b4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="9c9b4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c9b4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c9b4-126">Authorization</span></span>  | <span data-ttu-id="9c9b4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c9b4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c9b4-129">Request body</span></span>
<span data-ttu-id="9c9b4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c9b4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c9b4-131">Response</span></span>

<span data-ttu-id="9c9b4-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-132">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c9b4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c9b4-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9c9b4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c9b4-134">Request</span></span>

<span data-ttu-id="9c9b4-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c9b4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c9b4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="9c9b4-137">C#</span><span class="sxs-lookup"><span data-stu-id="9c9b4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c9b4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c9b4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c9b4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c9b4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c9b4-140">Java</span><span class="sxs-lookup"><span data-stu-id="9c9b4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c9b4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c9b4-141">Response</span></span>

<span data-ttu-id="9c9b4-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-142">The following is an example of the response.</span></span> 

><span data-ttu-id="9c9b4-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c9b4-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


