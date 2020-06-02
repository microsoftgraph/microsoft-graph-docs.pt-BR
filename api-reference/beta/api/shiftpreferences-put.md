---
title: Atualizar shiftPreferences
description: Atualize as preferências de turno de um usuário.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b3f87e6981abf18a4f082839c3e3e47455d36961
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154322"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="f097d-103">Atualizar shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="f097d-103">Update shiftPreferences</span></span>

<span data-ttu-id="f097d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f097d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f097d-105">Atualizar as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="f097d-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f097d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f097d-106">Permissions</span></span>

<span data-ttu-id="f097d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f097d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f097d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f097d-109">Permission type</span></span>      | <span data-ttu-id="f097d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f097d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f097d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f097d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f097d-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f097d-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="f097d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f097d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f097d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f097d-114">Not supported.</span></span>    |
|<span data-ttu-id="f097d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f097d-115">Application</span></span> | <span data-ttu-id="f097d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f097d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f097d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f097d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="f097d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f097d-118">Request headers</span></span>

| <span data-ttu-id="f097d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f097d-119">Header</span></span>       | <span data-ttu-id="f097d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f097d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f097d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f097d-121">Authorization</span></span>  | <span data-ttu-id="f097d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f097d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f097d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f097d-124">Content-Type</span></span>  | <span data-ttu-id="f097d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f097d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f097d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f097d-127">Request body</span></span>
<span data-ttu-id="f097d-128">No corpo da solicitação, forneça uma representação JSON de um objeto [shiftPreferences](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="f097d-128">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f097d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f097d-129">Response</span></span>

<span data-ttu-id="f097d-130">Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="f097d-130">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f097d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f097d-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f097d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f097d-132">Request</span></span>

<span data-ttu-id="f097d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f097d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f097d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f097d-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f097d-135">C#</span><span class="sxs-lookup"><span data-stu-id="f097d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f097d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f097d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f097d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f097d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f097d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f097d-138">Response</span></span>

<span data-ttu-id="f097d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f097d-139">The following is an example of the response.</span></span>

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
