---
title: 'chamar: resposta'
description: Atenda uma chamada de entrada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d3927c41df6558b1c0d266afbdb25f1c12ac1e49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971610"
---
# <a name="call-answer"></a><span data-ttu-id="4cc4f-103">chamar: resposta</span><span class="sxs-lookup"><span data-stu-id="4cc4f-103">call: answer</span></span>

> <span data-ttu-id="4cc4f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cc4f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4cc4f-106">Atenda uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-106">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cc4f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4cc4f-107">Permissions</span></span>
<span data-ttu-id="4cc4f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cc4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cc4f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cc4f-110">Permission type</span></span> | <span data-ttu-id="4cc4f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cc4f-111">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="4cc4f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cc4f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cc4f-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4cc4f-113">Not Supported</span></span>                        |
| <span data-ttu-id="4cc4f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cc4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cc4f-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4cc4f-115">Not Supported</span></span>                        |
| <span data-ttu-id="4cc4f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cc4f-116">Application</span></span>     | <span data-ttu-id="4cc4f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cc4f-117">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="4cc4f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cc4f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="4cc4f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc4f-119">Request headers</span></span>
| <span data-ttu-id="4cc4f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4cc4f-120">Name</span></span>          | <span data-ttu-id="4cc4f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cc4f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4cc4f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cc4f-122">Authorization</span></span> | <span data-ttu-id="4cc4f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cc4f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc4f-125">Request body</span></span>
<span data-ttu-id="4cc4f-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4cc4f-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4cc4f-127">Parameter</span></span>        | <span data-ttu-id="4cc4f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cc4f-128">Type</span></span>                                     |<span data-ttu-id="4cc4f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cc4f-129">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4cc4f-130">callbackUri</span><span class="sxs-lookup"><span data-stu-id="4cc4f-130">callbackUri</span></span>       |<span data-ttu-id="4cc4f-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cc4f-131">String</span></span>                                    |<span data-ttu-id="4cc4f-132">A ID de inscrição ou de retorno de chamada no qual serão entregues retornos de chamada.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-132">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="4cc4f-133">(Necessário)</span><span class="sxs-lookup"><span data-stu-id="4cc4f-133">(Required)</span></span>                                                               |
|<span data-ttu-id="4cc4f-134">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="4cc4f-134">acceptedModalities</span></span>|<span data-ttu-id="4cc4f-135">String collection</span><span class="sxs-lookup"><span data-stu-id="4cc4f-135">String collection</span></span>                         |<span data-ttu-id="4cc4f-136">A lista de aceitar modalidades.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-136">The list of accept modalities.</span></span> <span data-ttu-id="4cc4f-137">Valores possíveis são: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-137">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="4cc4f-138">(Necessário)</span><span class="sxs-lookup"><span data-stu-id="4cc4f-138">(Required)</span></span> |
|<span data-ttu-id="4cc4f-139">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="4cc4f-139">mediaConfig</span></span>       |[<span data-ttu-id="4cc4f-140">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="4cc4f-140">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="4cc4f-141">A configuração de mídia.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-141">The media configuration.</span></span> <span data-ttu-id="4cc4f-142">(Necessário)</span><span class="sxs-lookup"><span data-stu-id="4cc4f-142">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="4cc4f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cc4f-143">Response</span></span>
<span data-ttu-id="4cc4f-144">Esse método retorna `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-144">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4cc4f-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4cc4f-145">Examples</span></span>
<span data-ttu-id="4cc4f-146">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-146">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4cc4f-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc4f-147">Request</span></span>
<span data-ttu-id="4cc4f-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="4cc4f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cc4f-149">Response</span></span>
<span data-ttu-id="4cc4f-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cc4f-150">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="4cc4f-151">Atender a chamada VOIP com mídia de serviço hospedado</span><span class="sxs-lookup"><span data-stu-id="4cc4f-151">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="4cc4f-152">Notificação - entrada</span><span class="sxs-lookup"><span data-stu-id="4cc4f-152">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="4cc4f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc4f-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="4cc4f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cc4f-154">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="4cc4f-155">Notificação - estabelecendo</span><span class="sxs-lookup"><span data-stu-id="4cc4f-155">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="4cc4f-156">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="4cc4f-156">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="4cc4f-157">Atender a chamada VOIP com mídia de aplicativo hospedado</span><span class="sxs-lookup"><span data-stu-id="4cc4f-157">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="4cc4f-158">Notificação - entrada</span><span class="sxs-lookup"><span data-stu-id="4cc4f-158">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="4cc4f-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc4f-159">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="4cc4f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cc4f-160">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="4cc4f-161">Notificação - estabelecendo</span><span class="sxs-lookup"><span data-stu-id="4cc4f-161">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="4cc4f-162">Notificação - estabelecida</span><span class="sxs-lookup"><span data-stu-id="4cc4f-162">Notification - established</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
