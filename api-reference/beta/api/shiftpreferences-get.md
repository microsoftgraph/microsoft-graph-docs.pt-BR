---
title: Obter shiftPreferences
description: Obtenha uma preferência de mudança por ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0ef9a067cfb106c6cee5fadb113da5aabfa7f3a
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952115"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="562a3-103">Obter shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="562a3-103">Get shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="562a3-104">Recupere as propriedades e os relacionamentos de um objeto [shiftPreferences](../resources/shiftpreferences.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="562a3-104">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="562a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="562a3-105">Permissions</span></span>

<span data-ttu-id="562a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="562a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="562a3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="562a3-108">Permission type</span></span>      | <span data-ttu-id="562a3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="562a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="562a3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="562a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="562a3-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="562a3-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="562a3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="562a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="562a3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="562a3-113">Not supported.</span></span>    |
|<span data-ttu-id="562a3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="562a3-114">Application</span></span> | <span data-ttu-id="562a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="562a3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="562a3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="562a3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="562a3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="562a3-117">Request headers</span></span>

| <span data-ttu-id="562a3-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="562a3-118">Header</span></span>       | <span data-ttu-id="562a3-119">Valor</span><span class="sxs-lookup"><span data-stu-id="562a3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="562a3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="562a3-120">Authorization</span></span>  | <span data-ttu-id="562a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="562a3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="562a3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="562a3-123">Request body</span></span>
<span data-ttu-id="562a3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="562a3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="562a3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="562a3-125">Response</span></span>

<span data-ttu-id="562a3-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [shiftPreferences](../resources/shiftpreferences.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="562a3-126">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="562a3-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="562a3-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="562a3-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="562a3-128">Request</span></span>

<span data-ttu-id="562a3-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="562a3-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="562a3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="562a3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```

#### <a name="response"></a><span data-ttu-id="562a3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="562a3-131">Response</span></span>

<span data-ttu-id="562a3-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="562a3-132">The following is an example of the response.</span></span>

><span data-ttu-id="562a3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="562a3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
