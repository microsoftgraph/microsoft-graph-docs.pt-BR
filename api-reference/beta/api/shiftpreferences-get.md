---
title: Obter shiftPreferences
description: Obtenha uma preferência de mudança por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 30837607b484d98856f5296e1fd0a1a30ca3a619
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453293"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="7f1d6-103">Obter shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="7f1d6-103">Get shiftPreferences</span></span>

<span data-ttu-id="7f1d6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f1d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f1d6-105">Recupere as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f1d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f1d6-106">Permissions</span></span>

<span data-ttu-id="7f1d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f1d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f1d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f1d6-109">Permission type</span></span>      | <span data-ttu-id="7f1d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f1d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f1d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f1d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f1d6-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f1d6-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f1d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f1d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f1d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-114">Not supported.</span></span>    |
|<span data-ttu-id="7f1d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f1d6-115">Application</span></span> | <span data-ttu-id="7f1d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f1d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f1d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="7f1d6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f1d6-118">Request headers</span></span>

| <span data-ttu-id="7f1d6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f1d6-119">Header</span></span>       | <span data-ttu-id="7f1d6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7f1d6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f1d6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f1d6-121">Authorization</span></span>  | <span data-ttu-id="7f1d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f1d6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f1d6-124">Request body</span></span>
<span data-ttu-id="7f1d6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f1d6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f1d6-126">Response</span></span>

<span data-ttu-id="7f1d6-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [shiftPreferences](../resources/shiftpreferences.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-127">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f1d6-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f1d6-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f1d6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f1d6-129">Request</span></span>

<span data-ttu-id="7f1d6-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f1d6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f1d6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="7f1d6-132">C#</span><span class="sxs-lookup"><span data-stu-id="7f1d6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f1d6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f1d6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f1d6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f1d6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f1d6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f1d6-135">Response</span></span>

<span data-ttu-id="7f1d6-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-136">The following is an example of the response.</span></span>

><span data-ttu-id="7f1d6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f1d6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
