---
title: Obter shiftPreferences
description: Obtenha uma preferência de mudança por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7dde453f22ec6a37107f14a276e3f716a095e1f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019695"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="72def-103">Obter shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="72def-103">Get shiftPreferences</span></span>

<span data-ttu-id="72def-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72def-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72def-105">Recupere as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="72def-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="72def-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72def-106">Permissions</span></span>

<span data-ttu-id="72def-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72def-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72def-109">Permission type</span></span>      | <span data-ttu-id="72def-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72def-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72def-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72def-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72def-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72def-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="72def-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72def-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72def-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72def-114">Not supported.</span></span>    |
|<span data-ttu-id="72def-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72def-115">Application</span></span> | <span data-ttu-id="72def-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72def-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72def-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72def-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72def-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72def-118">Optional query parameters</span></span>

<span data-ttu-id="72def-119">Este método não oferece suporte a parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72def-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72def-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72def-120">Request headers</span></span>

| <span data-ttu-id="72def-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72def-121">Header</span></span>       | <span data-ttu-id="72def-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72def-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72def-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72def-123">Authorization</span></span>  | <span data-ttu-id="72def-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72def-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72def-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72def-126">Request body</span></span>
<span data-ttu-id="72def-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72def-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72def-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="72def-128">Response</span></span>

<span data-ttu-id="72def-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [shiftPreferences](../resources/shiftpreferences.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72def-129">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72def-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72def-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="72def-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72def-131">Request</span></span>

<span data-ttu-id="72def-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72def-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72def-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="72def-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="72def-134">C#</span><span class="sxs-lookup"><span data-stu-id="72def-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72def-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72def-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72def-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72def-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72def-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="72def-137">Response</span></span>

<span data-ttu-id="72def-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72def-138">The following is an example of the response.</span></span>

><span data-ttu-id="72def-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72def-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shiftPreferences"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Tuesday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": [
                {
                    "startTime": "09:15:00.000000",
                    "endTime": "12:30:00.000000"
                },
                {
                    "startTime": "16:00:00.000000",
                    "endTime": "20:00:00.000000"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


