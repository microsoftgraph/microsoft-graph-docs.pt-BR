---
title: Atualizar shiftPreferences
description: Atualize as preferências de turno de um usuário.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1df99a56ed27724d9ff670f4b100d0b7ba93e71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453279"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="6e787-103">Atualizar shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="6e787-103">Update shiftPreferences</span></span>

<span data-ttu-id="6e787-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6e787-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e787-105">Atualizar as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="6e787-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e787-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e787-106">Permissions</span></span>

<span data-ttu-id="6e787-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e787-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e787-109">Permission type</span></span>      | <span data-ttu-id="6e787-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e787-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e787-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e787-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6e787-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e787-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e787-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e787-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e787-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e787-114">Not supported.</span></span>    |
|<span data-ttu-id="6e787-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e787-115">Application</span></span> | <span data-ttu-id="6e787-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e787-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e787-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e787-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="6e787-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e787-118">Request headers</span></span>

| <span data-ttu-id="6e787-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e787-119">Header</span></span>       | <span data-ttu-id="6e787-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6e787-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e787-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e787-121">Authorization</span></span>  | <span data-ttu-id="6e787-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e787-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e787-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e787-124">Content-Type</span></span>  | <span data-ttu-id="6e787-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e787-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e787-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e787-127">Request body</span></span>
<span data-ttu-id="6e787-128">Forneça o novo objeto [shiftPreferences](../resources/shiftpreferences.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="6e787-128">Provide the new [shiftPreferences](../resources/shiftpreferences.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e787-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e787-129">Response</span></span>

<span data-ttu-id="6e787-130">Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="6e787-130">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e787-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e787-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6e787-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e787-132">Request</span></span>

<span data-ttu-id="6e787-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e787-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e787-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e787-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PUT https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
Content-type: application/json

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Monday", "Wednesday", "Friday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": null
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="6e787-135">C#</span><span class="sxs-lookup"><span data-stu-id="6e787-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e787-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e787-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e787-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e787-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6e787-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e787-138">Response</span></span>

<span data-ttu-id="6e787-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6e787-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
