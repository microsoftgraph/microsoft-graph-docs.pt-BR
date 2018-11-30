---
title: Criar ou substituir uma atividade
description: Criar uma nova ou substituir uma atividade do usuário existente para seu aplicativo. Se você gostaria de criar uma atividade do usuário e seu relacionados **historyItems** em uma solicitação, você pode usar Inserir aprofundada.
ms.openlocfilehash: fb1efa1cb9484b5f4229883ebe2daf271598b8a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006056"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="11149-104">Criar ou substituir uma atividade</span><span class="sxs-lookup"><span data-stu-id="11149-104">Create or replace an activity</span></span>

<span data-ttu-id="11149-105">Criar uma nova ou substituir uma atividade do usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11149-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="11149-106">Se você gostaria de criar uma atividade do usuário e seu relacionados **historyItems** em uma solicitação, você pode usar a [profundidade inserir](projectrome-put-activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="11149-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="11149-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="11149-107">Permissions</span></span>

<span data-ttu-id="11149-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11149-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="11149-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11149-110">Permission type</span></span>      | <span data-ttu-id="11149-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11149-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11149-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11149-112">Delegated (work or school account)</span></span> | <span data-ttu-id="11149-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="11149-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="11149-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11149-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11149-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="11149-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="11149-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11149-116">Application</span></span> | <span data-ttu-id="11149-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11149-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11149-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11149-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="11149-119">**Observação:** O appActivityId na URL precisa ser URL-safe (todos os caracteres, com exceção do RFC 2396 caracteres não reservadas devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser URL-safe.</span><span class="sxs-lookup"><span data-stu-id="11149-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11149-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11149-120">Request headers</span></span>

|<span data-ttu-id="11149-121">Nome</span><span class="sxs-lookup"><span data-stu-id="11149-121">Name</span></span> | <span data-ttu-id="11149-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="11149-122">Type</span></span> | <span data-ttu-id="11149-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="11149-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="11149-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="11149-124">Authorization</span></span> | <span data-ttu-id="11149-125">string</span><span class="sxs-lookup"><span data-stu-id="11149-125">string</span></span> | <span data-ttu-id="11149-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11149-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11149-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11149-128">Request body</span></span>

<span data-ttu-id="11149-129">No corpo da solicitação, fornece uma representação JSON de um objeto de [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="11149-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11149-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="11149-130">Response</span></span>

<span data-ttu-id="11149-131">Se tiver êxito, este método retornará o `201 Created` código de resposta se a atividade foi criada ou `200 OK` se a atividade foi substituída.</span><span class="sxs-lookup"><span data-stu-id="11149-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="11149-132">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="11149-132">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="11149-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11149-133">Request</span></span>

<span data-ttu-id="11149-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11149-134">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="11149-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="11149-135">Response</span></span>

<span data-ttu-id="11149-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11149-136">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
        "backgroundColor": "#ff0000",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "appDisplayName": "Contoso, Ltd.",
    "userTimezone": "Africa/Casablanca",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="11149-137">Exemplo 2 - inserir profundo</span><span class="sxs-lookup"><span data-stu-id="11149-137">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="11149-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11149-138">Request</span></span>

<span data-ttu-id="11149-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11149-139">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="11149-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="11149-140">Response</span></span>

<span data-ttu-id="11149-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11149-141">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
        "backgroundColor": "#ff0000",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    },
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "appDisplayName": "Contoso, Ltd.",
    "userTimezone": "Africa/Casablanca",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "historyItems":[
        {
            "status": "updated",
            "userTimezone": "Africa/Casablanca",
            "createdDateTime": "2018-04-12T21:42:42.495Z",
            "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
            "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
            "expirationDateTime": "2018-05-12T21:42:42.495Z",
            "activeDurationSeconds": 20
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
