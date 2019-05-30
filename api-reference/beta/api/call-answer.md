---
title: 'Call: resposta'
description: Atenda às chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ce79ff0e471882576ed885e4ab85d686a6cdb0de
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536054"
---
# <a name="call-answer"></a><span data-ttu-id="f38bf-103">Call: resposta</span><span class="sxs-lookup"><span data-stu-id="f38bf-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f38bf-104">Atenda às chamadas recebidas.</span><span class="sxs-lookup"><span data-stu-id="f38bf-104">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f38bf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f38bf-105">Permissions</span></span>
<span data-ttu-id="f38bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f38bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f38bf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f38bf-108">Permission type</span></span> | <span data-ttu-id="f38bf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f38bf-109">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="f38bf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f38bf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f38bf-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f38bf-111">Not Supported</span></span>                        |
| <span data-ttu-id="f38bf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f38bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f38bf-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f38bf-113">Not Supported</span></span>                        |
| <span data-ttu-id="f38bf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f38bf-114">Application</span></span>     | <span data-ttu-id="f38bf-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f38bf-115">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="f38bf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f38bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="f38bf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f38bf-117">Request headers</span></span>
| <span data-ttu-id="f38bf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f38bf-118">Name</span></span>          | <span data-ttu-id="f38bf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38bf-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f38bf-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f38bf-120">Authorization</span></span> | <span data-ttu-id="f38bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f38bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f38bf-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f38bf-123">Request body</span></span>
<span data-ttu-id="f38bf-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f38bf-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f38bf-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f38bf-125">Parameter</span></span>        | <span data-ttu-id="f38bf-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38bf-126">Type</span></span>                                     |<span data-ttu-id="f38bf-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38bf-127">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f38bf-128">callbackUri</span><span class="sxs-lookup"><span data-stu-id="f38bf-128">callbackUri</span></span>       |<span data-ttu-id="f38bf-129">String</span><span class="sxs-lookup"><span data-stu-id="f38bf-129">String</span></span>                                    |<span data-ttu-id="f38bf-130">A ID de retorno de chamada ou de assinatura à qual os retornos serão entregues.</span><span class="sxs-lookup"><span data-stu-id="f38bf-130">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="f38bf-131">Precisam</span><span class="sxs-lookup"><span data-stu-id="f38bf-131">(Required)</span></span>                                                               |
|<span data-ttu-id="f38bf-132">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="f38bf-132">acceptedModalities</span></span>|<span data-ttu-id="f38bf-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f38bf-133">String collection</span></span>                         |<span data-ttu-id="f38bf-134">A lista de aceitar modalidades.</span><span class="sxs-lookup"><span data-stu-id="f38bf-134">The list of accept modalities.</span></span> <span data-ttu-id="f38bf-135">O valor possível são `unknown`: `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`,.</span><span class="sxs-lookup"><span data-stu-id="f38bf-135">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="f38bf-136">Precisam</span><span class="sxs-lookup"><span data-stu-id="f38bf-136">(Required)</span></span> |
|<span data-ttu-id="f38bf-137">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="f38bf-137">mediaConfig</span></span>       |[<span data-ttu-id="f38bf-138">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="f38bf-138">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="f38bf-139">A configuração de mídia.</span><span class="sxs-lookup"><span data-stu-id="f38bf-139">The media configuration.</span></span> <span data-ttu-id="f38bf-140">Precisam</span><span class="sxs-lookup"><span data-stu-id="f38bf-140">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="f38bf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38bf-141">Response</span></span>
<span data-ttu-id="f38bf-142">Este método retorna `202 Accepted` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="f38bf-142">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f38bf-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f38bf-143">Examples</span></span>
<span data-ttu-id="f38bf-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f38bf-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f38bf-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f38bf-145">Request</span></span>
<span data-ttu-id="f38bf-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f38bf-146">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f38bf-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38bf-147">Response</span></span>
<span data-ttu-id="f38bf-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f38bf-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f38bf-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f38bf-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f38bf-150">C#</span><span class="sxs-lookup"><span data-stu-id="f38bf-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-answer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f38bf-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="f38bf-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-answer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="f38bf-152">Responder chamada VOIP com mídia hospedada pelo serviço</span><span class="sxs-lookup"><span data-stu-id="f38bf-152">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="f38bf-153">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="f38bf-153">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "callRoutes": [
          {
            "routingType": "lookup",
            "original": {
              "phone": {
                "id": "+14258828080"
              }
            },
            "final": {
              "user": {
                "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
                "displayName": "Heidi Steen"
              }
            }
          }
        ],
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="f38bf-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f38bf-154">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="f38bf-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38bf-155">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="f38bf-156">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="f38bf-156">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="f38bf-157">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="f38bf-157">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="f38bf-158">Responder chamada VOIP com mídia hospedada por aplicativo</span><span class="sxs-lookup"><span data-stu-id="f38bf-158">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="f38bf-159">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="f38bf-159">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="f38bf-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f38bf-160">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  }
}
```

##### <a name="response"></a><span data-ttu-id="f38bf-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38bf-161">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="f38bf-162">Notificação-estabelecimento</span><span class="sxs-lookup"><span data-stu-id="f38bf-162">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="f38bf-163">Estabelecido em notificação</span><span class="sxs-lookup"><span data-stu-id="f38bf-163">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
