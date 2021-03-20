---
title: Atualizar shiftPreferences
description: Atualize as preferências de turno de um usuário.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 12eb1020f2daad820d9fbbf9fe20005e8ec00447
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945800"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="dbaaf-103">Atualizar shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="dbaaf-103">Update shiftPreferences</span></span>

<span data-ttu-id="dbaaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbaaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbaaf-105">Atualize as propriedades e as relações de um [objeto shiftPreferences.](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="dbaaf-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbaaf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbaaf-106">Permissions</span></span>

<span data-ttu-id="dbaaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbaaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbaaf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbaaf-109">Permission type</span></span>      | <span data-ttu-id="dbaaf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbaaf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbaaf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbaaf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbaaf-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbaaf-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbaaf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbaaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbaaf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-114">Not supported.</span></span>    |
|<span data-ttu-id="dbaaf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbaaf-115">Application</span></span> | <span data-ttu-id="dbaaf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbaaf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbaaf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="dbaaf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbaaf-118">Request headers</span></span>

| <span data-ttu-id="dbaaf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbaaf-119">Header</span></span>       | <span data-ttu-id="dbaaf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dbaaf-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dbaaf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbaaf-121">Authorization</span></span>  | <span data-ttu-id="dbaaf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dbaaf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbaaf-124">Content-Type</span></span>  | <span data-ttu-id="dbaaf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbaaf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbaaf-127">Request body</span></span>
<span data-ttu-id="dbaaf-128">No corpo da solicitação, fornece uma representação JSON de um [objeto shiftPreferences.](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="dbaaf-128">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dbaaf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbaaf-129">Response</span></span>

<span data-ttu-id="dbaaf-130">Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-130">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dbaaf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbaaf-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dbaaf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbaaf-132">Request</span></span>

<span data-ttu-id="dbaaf-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dbaaf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbaaf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-3"
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
# <a name="c"></a>[<span data-ttu-id="dbaaf-135">C#</span><span class="sxs-lookup"><span data-stu-id="dbaaf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbaaf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbaaf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbaaf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbaaf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dbaaf-138">Java</span><span class="sxs-lookup"><span data-stu-id="dbaaf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbaaf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbaaf-139">Response</span></span>

<span data-ttu-id="dbaaf-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dbaaf-140">The following is an example of the response.</span></span>

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


