---
title: Criar ou substituir uma atividade
description: Criar um novo ou substituir uma atividade de usuário existente para seu aplicativo. Se quiser criar uma atividade de usuário e seus **historyItems** relacionados em uma solicitação, você poderá usar a inserção profunda.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: fd407967b11d7a28f0d6275bb0d6cfa045b417a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051688"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="c04f5-104">Criar ou substituir uma atividade</span><span class="sxs-lookup"><span data-stu-id="c04f5-104">Create or replace an activity</span></span>

<span data-ttu-id="c04f5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c04f5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c04f5-106">Criar um novo ou substituir uma atividade de usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c04f5-106">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="c04f5-107">Se quiser criar uma atividade de usuário e seus **historyItems** relacionados em uma solicitação, você poderá usar a [inserção profunda](#example-2-deep-insert).</span><span class="sxs-lookup"><span data-stu-id="c04f5-107">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="c04f5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c04f5-108">Permissions</span></span>

<span data-ttu-id="c04f5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c04f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c04f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c04f5-111">Permission type</span></span>                        | <span data-ttu-id="c04f5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c04f5-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="c04f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c04f5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c04f5-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c04f5-114">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="c04f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c04f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c04f5-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c04f5-116">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="c04f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c04f5-117">Application</span></span>                            | <span data-ttu-id="c04f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c04f5-118">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="c04f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c04f5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="c04f5-120">**Observação:** O appActivityId na URL precisa ser de URL segura (todos os caracteres, exceto os caracteres não reservados RFC 2396, devem ser convertidos em sua representação hexadecimal), mas o appActivityId original não precisa ser URL-seguro.</span><span class="sxs-lookup"><span data-stu-id="c04f5-120">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c04f5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c04f5-121">Request headers</span></span>

| <span data-ttu-id="c04f5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c04f5-122">Name</span></span>          | <span data-ttu-id="c04f5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c04f5-123">Type</span></span>   | <span data-ttu-id="c04f5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c04f5-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="c04f5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c04f5-125">Authorization</span></span> | <span data-ttu-id="c04f5-126">string</span><span class="sxs-lookup"><span data-stu-id="c04f5-126">string</span></span> | <span data-ttu-id="c04f5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c04f5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c04f5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c04f5-129">Request body</span></span>

<span data-ttu-id="c04f5-130">No corpo da solicitação, forneça uma representação JSON de um objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="c04f5-130">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c04f5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c04f5-131">Response</span></span>

<span data-ttu-id="c04f5-132">Se tiver êxito, este método retornará o `201 Created` código de resposta se a atividade foi criada ou `200 OK` se a atividade foi substituída.</span><span class="sxs-lookup"><span data-stu-id="c04f5-132">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="c04f5-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c04f5-133">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="c04f5-134">Exemplo 1: criar uma atividade</span><span class="sxs-lookup"><span data-stu-id="c04f5-134">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="c04f5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c04f5-135">Request</span></span>

<span data-ttu-id="c04f5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c04f5-136">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c04f5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c04f5-137">Response</span></span>

<span data-ttu-id="c04f5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c04f5-138">The following is an example of the response.</span></span>

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

### <a name="example-2-deep-insert"></a><span data-ttu-id="c04f5-139">Exemplo 2: inserção profunda</span><span class="sxs-lookup"><span data-stu-id="c04f5-139">Example 2: Deep insert</span></span>

<span data-ttu-id="c04f5-140">Este exemplo cria uma nova atividade e um item de histórico para essa atividade em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c04f5-140">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="c04f5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c04f5-141">Request</span></span>

<span data-ttu-id="c04f5-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c04f5-142">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c04f5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c04f5-143">Response</span></span>

<span data-ttu-id="c04f5-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c04f5-144">The following is an example of the response.</span></span>

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

