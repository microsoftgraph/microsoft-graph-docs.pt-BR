---
title: 'chamar: redirecionar'
description: Redirecione uma chamada recebida.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20470a57358caea08116bbacf6348d659d0d3636
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921721"
---
# <a name="call-redirect"></a><span data-ttu-id="4b832-103">chamar: redirecionar</span><span class="sxs-lookup"><span data-stu-id="4b832-103">call: redirect</span></span>

> <span data-ttu-id="4b832-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b832-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b832-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b832-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b832-106">Redirecione uma chamada recebida.</span><span class="sxs-lookup"><span data-stu-id="4b832-106">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b832-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4b832-107">Permissions</span></span>
<span data-ttu-id="4b832-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b832-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b832-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b832-110">Permission type</span></span> | <span data-ttu-id="4b832-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b832-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="4b832-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b832-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b832-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4b832-113">Not Supported</span></span>                |
| <span data-ttu-id="4b832-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b832-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b832-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4b832-115">Not Supported</span></span>                |
| <span data-ttu-id="4b832-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b832-116">Application</span></span>     | <span data-ttu-id="4b832-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="4b832-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="4b832-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b832-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="4b832-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b832-119">Request headers</span></span>
| <span data-ttu-id="4b832-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4b832-120">Name</span></span>          | <span data-ttu-id="4b832-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b832-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4b832-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b832-122">Authorization</span></span> | <span data-ttu-id="4b832-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b832-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b832-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b832-125">Request body</span></span>
<span data-ttu-id="4b832-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b832-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b832-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b832-127">Parameter</span></span>      | <span data-ttu-id="4b832-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b832-128">Type</span></span>    |<span data-ttu-id="4b832-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b832-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b832-130">destinos</span><span class="sxs-lookup"><span data-stu-id="4b832-130">targets</span></span>|<span data-ttu-id="4b832-131">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="4b832-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="4b832-132">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="4b832-132">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="4b832-133">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="4b832-133">targetDisposition</span></span>|<span data-ttu-id="4b832-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b832-134">String</span></span>|<span data-ttu-id="4b832-135">O valor possível é:`default`</span><span class="sxs-lookup"><span data-stu-id="4b832-135">The possible value is: `default`</span></span>|
|<span data-ttu-id="4b832-136">timeout</span><span class="sxs-lookup"><span data-stu-id="4b832-136">timeout</span></span>|<span data-ttu-id="4b832-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4b832-137">Int32</span></span>|<span data-ttu-id="4b832-138">O tempo limite em segundos para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="4b832-138">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="4b832-139">maskCallee</span><span class="sxs-lookup"><span data-stu-id="4b832-139">maskCallee</span></span>|<span data-ttu-id="4b832-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b832-140">Boolean</span></span>|<span data-ttu-id="4b832-141">Indica se o receptor de máscara.</span><span class="sxs-lookup"><span data-stu-id="4b832-141">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="4b832-142">maskCaller</span><span class="sxs-lookup"><span data-stu-id="4b832-142">maskCaller</span></span>|<span data-ttu-id="4b832-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b832-143">Boolean</span></span>|<span data-ttu-id="4b832-144">Indica se o chamador de máscara.</span><span class="sxs-lookup"><span data-stu-id="4b832-144">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="4b832-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b832-145">Response</span></span>
<span data-ttu-id="4b832-146">Retorna `202 Accepted` código de resposta</span><span class="sxs-lookup"><span data-stu-id="4b832-146">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="4b832-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b832-147">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="4b832-148">Redirecionar uma chamada</span><span class="sxs-lookup"><span data-stu-id="4b832-148">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="4b832-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b832-149">Request</span></span>
<span data-ttu-id="4b832-150">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b832-150">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/redirect
Content-Type: application/json
Content-Length: 515

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 99,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="4b832-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b832-151">Response</span></span>

> <span data-ttu-id="4b832-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b832-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="4b832-154">Encaminhar uma chamada</span><span class="sxs-lookup"><span data-stu-id="4b832-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="4b832-155">Notificação - entrada</span><span class="sxs-lookup"><span data-stu-id="4b832-155">Notification - incoming</span></span>

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
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="4b832-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b832-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/redirect
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 60,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="4b832-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b832-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="4b832-158">Notificação - redirecionando</span><span class="sxs-lookup"><span data-stu-id="4b832-158">Notification - redirecting</span></span>

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
        "state": "redirecting"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="4b832-159">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="4b832-159">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "answeredBy": {
          "identity": {
            "user": {
              "displayName": "Test User 2",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
            }
          }
        },
        "terminationReason": "AppRedirected"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
