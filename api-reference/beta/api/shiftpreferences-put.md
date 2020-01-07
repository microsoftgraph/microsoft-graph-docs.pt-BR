---
title: Atualizar shiftPreferences
description: Atualize as preferências de turno de um usuário.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83bec268e918bc65f1ce139081ff88c0290acf4d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952080"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="84b1c-103">Atualizar shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="84b1c-103">Update shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84b1c-104">Atualizar as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="84b1c-104">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84b1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="84b1c-105">Permissions</span></span>

<span data-ttu-id="84b1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84b1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84b1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84b1c-108">Permission type</span></span>      | <span data-ttu-id="84b1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84b1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84b1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84b1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84b1c-111">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b1c-111">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="84b1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84b1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84b1c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84b1c-113">Not supported.</span></span>    |
|<span data-ttu-id="84b1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84b1c-114">Application</span></span> | <span data-ttu-id="84b1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84b1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84b1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84b1c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="84b1c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84b1c-117">Request headers</span></span>

| <span data-ttu-id="84b1c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84b1c-118">Header</span></span>       | <span data-ttu-id="84b1c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="84b1c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84b1c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="84b1c-120">Authorization</span></span>  | <span data-ttu-id="84b1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84b1c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="84b1c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84b1c-123">Content-Type</span></span>  | <span data-ttu-id="84b1c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84b1c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84b1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84b1c-126">Request body</span></span>
<span data-ttu-id="84b1c-127">Forneça o novo objeto [shiftPreferences](../resources/shiftpreferences.md) no corpo da solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="84b1c-127">Provide the new [shiftPreferences](../resources/shiftpreferences.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84b1c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="84b1c-128">Response</span></span>

<span data-ttu-id="84b1c-129">Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="84b1c-129">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84b1c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84b1c-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="84b1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84b1c-131">Request</span></span>

<span data-ttu-id="84b1c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84b1c-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84b1c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84b1c-133">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="84b1c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="84b1c-134">Response</span></span>

<span data-ttu-id="84b1c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84b1c-135">The following is an example of the response.</span></span>

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
