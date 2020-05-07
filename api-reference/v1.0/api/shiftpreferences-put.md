---
title: Atualizar shiftPreferences
description: Atualize as preferências de turno de um usuário.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51ebeecb555c426c124975682fb85f77988d6e99
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154455"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="2ffef-103">Atualizar shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="2ffef-103">Update shiftPreferences</span></span>

<span data-ttu-id="2ffef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ffef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ffef-105">Atualizar as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="2ffef-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ffef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ffef-106">Permissions</span></span>

<span data-ttu-id="2ffef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ffef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ffef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ffef-109">Permission type</span></span>      | <span data-ttu-id="2ffef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ffef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ffef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ffef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ffef-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ffef-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ffef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ffef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ffef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ffef-114">Not supported.</span></span>    |
|<span data-ttu-id="2ffef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ffef-115">Application</span></span> | <span data-ttu-id="2ffef-116">UserShiftPreferences. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2ffef-116">UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="2ffef-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2ffef-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2ffef-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="2ffef-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2ffef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ffef-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="2ffef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffef-120">Request headers</span></span>

| <span data-ttu-id="2ffef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ffef-121">Header</span></span>       | <span data-ttu-id="2ffef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ffef-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ffef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ffef-123">Authorization</span></span>  | <span data-ttu-id="2ffef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ffef-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2ffef-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ffef-126">Content-Type</span></span>  | <span data-ttu-id="2ffef-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ffef-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ffef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffef-129">Request body</span></span>
<span data-ttu-id="2ffef-130">No corpo da solicitação, forneça uma representação JSON de um objeto [shiftPreferences](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="2ffef-130">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ffef-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ffef-131">Response</span></span>

<span data-ttu-id="2ffef-132">Se tiver êxito, este método retornará um código de resposta `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="2ffef-132">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ffef-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ffef-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ffef-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffef-134">Request</span></span>

<span data-ttu-id="2ffef-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ffef-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PUT https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
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
---


### <a name="response"></a><span data-ttu-id="2ffef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ffef-136">Response</span></span>

<span data-ttu-id="2ffef-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ffef-137">The following is an example of the response.</span></span>

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
