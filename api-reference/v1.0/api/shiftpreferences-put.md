---
title: Atualizar shiftPreferences
description: Atualize as preferências de turno de um usuário.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 44d2b1261ed2984963c4b9ff6e15abb91f7a2ee1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954741"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="5663f-103">Atualizar shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="5663f-103">Update shiftPreferences</span></span>

<span data-ttu-id="5663f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5663f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5663f-105">Atualize as propriedades e as relações de um [objeto shiftPreferences.](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="5663f-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5663f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5663f-106">Permissions</span></span>

<span data-ttu-id="5663f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5663f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5663f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5663f-109">Permission type</span></span>      | <span data-ttu-id="5663f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5663f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5663f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5663f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5663f-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5663f-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="5663f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5663f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5663f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5663f-114">Not supported.</span></span>    |
|<span data-ttu-id="5663f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5663f-115">Application</span></span> | <span data-ttu-id="5663f-116">UserShiftPreferences.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5663f-116">UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="5663f-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5663f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5663f-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="5663f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5663f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5663f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="5663f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5663f-120">Request headers</span></span>

| <span data-ttu-id="5663f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5663f-121">Header</span></span>       | <span data-ttu-id="5663f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5663f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5663f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5663f-123">Authorization</span></span>  | <span data-ttu-id="5663f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5663f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5663f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5663f-126">Content-Type</span></span>  | <span data-ttu-id="5663f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5663f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5663f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5663f-129">Request body</span></span>
<span data-ttu-id="5663f-130">No corpo da solicitação, fornece uma representação JSON de um [objeto shiftPreferences.](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="5663f-130">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5663f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5663f-131">Response</span></span>

<span data-ttu-id="5663f-132">Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="5663f-132">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5663f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5663f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5663f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5663f-134">Request</span></span>

<span data-ttu-id="5663f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5663f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5663f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5663f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-2"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
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
# <a name="c"></a>[<span data-ttu-id="5663f-137">C#</span><span class="sxs-lookup"><span data-stu-id="5663f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5663f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5663f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5663f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5663f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5663f-140">Java</span><span class="sxs-lookup"><span data-stu-id="5663f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="5663f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5663f-141">Response</span></span>

<span data-ttu-id="5663f-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5663f-142">The following is an example of the response.</span></span>

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

