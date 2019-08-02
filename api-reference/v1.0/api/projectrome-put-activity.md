---
title: Criar ou substituir uma atividade
description: Criar um novo ou substituir uma atividade de usuário existente para seu aplicativo. Se quiser criar uma atividade de usuário e seus **historyItems** relacionados em uma solicitação, você poderá usar a inserção profunda.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 8f80d17f64b4f04816670d8e007ca7db82755c0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025369"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="8b734-104">Criar ou substituir uma atividade</span><span class="sxs-lookup"><span data-stu-id="8b734-104">Create or replace an activity</span></span>

<span data-ttu-id="8b734-105">Criar um novo ou substituir uma atividade de usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b734-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="8b734-106">Se quiser criar uma atividade de usuário e seus **historyItems** relacionados em uma solicitação, você poderá usar a [inserção profunda](#example-2-deep-insert).</span><span class="sxs-lookup"><span data-stu-id="8b734-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b734-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b734-107">Permissions</span></span>

<span data-ttu-id="8b734-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b734-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b734-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b734-110">Permission type</span></span>                        | <span data-ttu-id="8b734-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b734-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="8b734-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b734-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b734-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="8b734-113">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="8b734-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b734-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b734-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="8b734-115">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="8b734-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b734-116">Application</span></span>                            | <span data-ttu-id="8b734-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b734-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="8b734-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b734-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="8b734-119">**Observação:** O appActivityId na URL precisa ser de URL segura (todos os caracteres, exceto os caracteres não reservados RFC 2396, devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser URL-seguro.</span><span class="sxs-lookup"><span data-stu-id="8b734-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b734-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b734-120">Request headers</span></span>

| <span data-ttu-id="8b734-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8b734-121">Name</span></span>          | <span data-ttu-id="8b734-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b734-122">Type</span></span>   | <span data-ttu-id="8b734-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b734-123">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="8b734-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b734-124">Authorization</span></span> | <span data-ttu-id="8b734-125">string</span><span class="sxs-lookup"><span data-stu-id="8b734-125">string</span></span> | <span data-ttu-id="8b734-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b734-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b734-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b734-128">Request body</span></span>

<span data-ttu-id="8b734-129">No corpo da solicitação, forneça uma representação JSON de um objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="8b734-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8b734-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b734-130">Response</span></span>

<span data-ttu-id="8b734-131">Se tiver êxito, este método retornará `201 Created` o código de resposta se a atividade foi `200 OK` criada ou se a atividade foi substituída.</span><span class="sxs-lookup"><span data-stu-id="8b734-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="8b734-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b734-132">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="8b734-133">Exemplo 1: criar uma atividade</span><span class="sxs-lookup"><span data-stu-id="8b734-133">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="8b734-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b734-134">Request</span></span>

<span data-ttu-id="8b734-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b734-135">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "addImageQuery": false
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8b734-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b734-136">Response</span></span>

<span data-ttu-id="8b734-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b734-137">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  }
}
```

### <a name="example-2-deep-insert"></a><span data-ttu-id="8b734-138">Exemplo 2: inserção profunda</span><span class="sxs-lookup"><span data-stu-id="8b734-138">Example 2: Deep insert</span></span>

<span data-ttu-id="8b734-139">Este exemplo cria uma nova atividade e um item de histórico para essa atividade em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b734-139">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="8b734-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b734-140">Request</span></span>

<span data-ttu-id="8b734-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b734-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "historyItems": [
    {
      "userTimezone": "Africa/Casablanca",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="8b734-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b734-142">Response</span></span>

<span data-ttu-id="8b734-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b734-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  "historyItems": [
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
