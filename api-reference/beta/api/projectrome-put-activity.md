---
title: Criar ou substituir uma atividade
description: Criar uma nova ou substituir uma atividade do usuário existente para seu aplicativo. Se você gostaria de criar uma atividade do usuário e seu relacionados **historyItems** em uma solicitação, você pode usar Inserir aprofundada.
localization_priority: Normal
ms.openlocfilehash: 01fa9fff306dbd07af0964f27dd97b288b6bab67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871789"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="45da5-104">Criar ou substituir uma atividade</span><span class="sxs-lookup"><span data-stu-id="45da5-104">Create or replace an activity</span></span>

> <span data-ttu-id="45da5-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45da5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45da5-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45da5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45da5-107">Criar uma nova ou substituir uma atividade do usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45da5-107">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="45da5-108">Se você gostaria de criar uma atividade do usuário e seu relacionados **historyItems** em uma solicitação, você pode usar a [profundidade inserir](projectrome-put-activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="45da5-108">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="45da5-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="45da5-109">Permissions</span></span>

<span data-ttu-id="45da5-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45da5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="45da5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45da5-112">Permission type</span></span>      | <span data-ttu-id="45da5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45da5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45da5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45da5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="45da5-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="45da5-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="45da5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45da5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45da5-117">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="45da5-117">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="45da5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45da5-118">Application</span></span> | <span data-ttu-id="45da5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45da5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45da5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45da5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="45da5-121">**Observação:** O appActivityId na URL precisa ser URL-safe (todos os caracteres, com exceção do RFC 2396 caracteres não reservadas devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser URL-safe.</span><span class="sxs-lookup"><span data-stu-id="45da5-121">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45da5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45da5-122">Request headers</span></span>

|<span data-ttu-id="45da5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="45da5-123">Name</span></span> | <span data-ttu-id="45da5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="45da5-124">Type</span></span> | <span data-ttu-id="45da5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="45da5-125">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="45da5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="45da5-126">Authorization</span></span> | <span data-ttu-id="45da5-127">string</span><span class="sxs-lookup"><span data-stu-id="45da5-127">string</span></span> | <span data-ttu-id="45da5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45da5-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45da5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45da5-130">Request body</span></span>

<span data-ttu-id="45da5-131">No corpo da solicitação, fornece uma representação JSON de um objeto de [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="45da5-131">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="45da5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="45da5-132">Response</span></span>

<span data-ttu-id="45da5-133">Se tiver êxito, este método retornará o `201 Created` código de resposta se a atividade foi criada ou `200 OK` se a atividade foi substituída.</span><span class="sxs-lookup"><span data-stu-id="45da5-133">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="45da5-134">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="45da5-134">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="45da5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45da5-135">Request</span></span>

<span data-ttu-id="45da5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45da5-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
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
            "addImageQuery": "false"
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

#### <a name="response"></a><span data-ttu-id="45da5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="45da5-137">Response</span></span>

<span data-ttu-id="45da5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45da5-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

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

## <a name="example-2---deep-insert"></a><span data-ttu-id="45da5-139">Exemplo 2 - inserir profundo</span><span class="sxs-lookup"><span data-stu-id="45da5-139">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="45da5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45da5-140">Request</span></span>

<span data-ttu-id="45da5-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45da5-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
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
            "addImageQuery": "false",
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

#### <a name="response"></a><span data-ttu-id="45da5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="45da5-142">Response</span></span>

<span data-ttu-id="45da5-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45da5-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

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
