---
title: 'chamar: redirecionar'
description: Redirecione uma chamada recebida.
author: VinodRavichandran
ms.openlocfilehash: 9fff752f07f66cf3c236982495897234c9a1c38d
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380216"
---
# <a name="call-redirect"></a><span data-ttu-id="887cd-103">chamar: redirecionar</span><span class="sxs-lookup"><span data-stu-id="887cd-103">call: redirect</span></span>

> <span data-ttu-id="887cd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="887cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="887cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="887cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="887cd-106">Redirecione uma chamada recebida.</span><span class="sxs-lookup"><span data-stu-id="887cd-106">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="887cd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="887cd-107">Permissions</span></span>
<span data-ttu-id="887cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="887cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="887cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="887cd-110">Permission type</span></span> | <span data-ttu-id="887cd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="887cd-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="887cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="887cd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="887cd-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="887cd-113">Not Supported</span></span>                |
| <span data-ttu-id="887cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="887cd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="887cd-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="887cd-115">Not Supported</span></span>                |
| <span data-ttu-id="887cd-116">Application</span><span class="sxs-lookup"><span data-stu-id="887cd-116">Application</span></span>     | <span data-ttu-id="887cd-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="887cd-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="887cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="887cd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="887cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="887cd-119">Request headers</span></span>
| <span data-ttu-id="887cd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="887cd-120">Name</span></span>          | <span data-ttu-id="887cd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="887cd-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="887cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="887cd-122">Authorization</span></span> | <span data-ttu-id="887cd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="887cd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="887cd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="887cd-125">Request body</span></span>
<span data-ttu-id="887cd-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="887cd-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="887cd-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="887cd-127">Parameter</span></span>      | <span data-ttu-id="887cd-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="887cd-128">Type</span></span>    |<span data-ttu-id="887cd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="887cd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="887cd-130">destinos</span><span class="sxs-lookup"><span data-stu-id="887cd-130">targets</span></span>|<span data-ttu-id="887cd-131">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="887cd-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="887cd-132">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="887cd-132">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="887cd-133">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="887cd-133">targetDisposition</span></span>|<span data-ttu-id="887cd-134">String</span><span class="sxs-lookup"><span data-stu-id="887cd-134">String</span></span>|<span data-ttu-id="887cd-135">O valor possível é:`default`</span><span class="sxs-lookup"><span data-stu-id="887cd-135">The possible value is: `default`</span></span>|
|<span data-ttu-id="887cd-136">timeout</span><span class="sxs-lookup"><span data-stu-id="887cd-136">timeout</span></span>|<span data-ttu-id="887cd-137">Int32</span><span class="sxs-lookup"><span data-stu-id="887cd-137">Int32</span></span>|<span data-ttu-id="887cd-138">O tempo limite em segundos para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="887cd-138">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="887cd-139">maskCallee</span><span class="sxs-lookup"><span data-stu-id="887cd-139">maskCallee</span></span>|<span data-ttu-id="887cd-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="887cd-140">Boolean</span></span>|<span data-ttu-id="887cd-141">Indica se o receptor de máscara.</span><span class="sxs-lookup"><span data-stu-id="887cd-141">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="887cd-142">maskCaller</span><span class="sxs-lookup"><span data-stu-id="887cd-142">maskCaller</span></span>|<span data-ttu-id="887cd-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="887cd-143">Boolean</span></span>|<span data-ttu-id="887cd-144">Indica se o chamador de máscara.</span><span class="sxs-lookup"><span data-stu-id="887cd-144">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="887cd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="887cd-145">Response</span></span>
<span data-ttu-id="887cd-146">Retorna `202 Accepted` código de resposta</span><span class="sxs-lookup"><span data-stu-id="887cd-146">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="887cd-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="887cd-147">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="887cd-148">Redirecionar uma chamada</span><span class="sxs-lookup"><span data-stu-id="887cd-148">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="887cd-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="887cd-149">Request</span></span>
<span data-ttu-id="887cd-150">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="887cd-150">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="887cd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="887cd-151">Response</span></span>

> <span data-ttu-id="887cd-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="887cd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="887cd-154">Encaminhar uma chamada</span><span class="sxs-lookup"><span data-stu-id="887cd-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="887cd-155">Notificação - entrada</span><span class="sxs-lookup"><span data-stu-id="887cd-155">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="887cd-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="887cd-156">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="887cd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="887cd-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="887cd-158">Notificação - redirecionando</span><span class="sxs-lookup"><span data-stu-id="887cd-158">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="887cd-159">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="887cd-159">Notification - terminated</span></span>

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
