---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a43f9c6164e69315d60f39c2ae0b9c1ba3df2c9f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418891"
---
# <a name="call-redirect"></a><span data-ttu-id="6fdd8-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="6fdd8-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fdd8-104">Redirecione as chamadas recebidas.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fdd8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fdd8-105">Permissions</span></span>
<span data-ttu-id="6fdd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fdd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fdd8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fdd8-108">Permission type</span></span> | <span data-ttu-id="6fdd8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fdd8-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="6fdd8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fdd8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fdd8-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6fdd8-111">Not Supported</span></span>                |
| <span data-ttu-id="6fdd8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fdd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fdd8-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6fdd8-113">Not Supported</span></span>                |
| <span data-ttu-id="6fdd8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fdd8-114">Application</span></span>     | <span data-ttu-id="6fdd8-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="6fdd8-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6fdd8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fdd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="6fdd8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fdd8-117">Request headers</span></span>
| <span data-ttu-id="6fdd8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6fdd8-118">Name</span></span>          | <span data-ttu-id="6fdd8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdd8-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6fdd8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fdd8-120">Authorization</span></span> | <span data-ttu-id="6fdd8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fdd8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fdd8-123">Request body</span></span>
<span data-ttu-id="6fdd8-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6fdd8-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6fdd8-125">Parameter</span></span>      | <span data-ttu-id="6fdd8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fdd8-126">Type</span></span>    |<span data-ttu-id="6fdd8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdd8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fdd8-128">targets</span><span class="sxs-lookup"><span data-stu-id="6fdd8-128">targets</span></span>|<span data-ttu-id="6fdd8-129">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6fdd8-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="6fdd8-130">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="6fdd8-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="6fdd8-131">targetDisposition</span></span>|<span data-ttu-id="6fdd8-132">String</span><span class="sxs-lookup"><span data-stu-id="6fdd8-132">String</span></span>|<span data-ttu-id="6fdd8-133">O valor possível é:`default`</span><span class="sxs-lookup"><span data-stu-id="6fdd8-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="6fdd8-134">timeout</span><span class="sxs-lookup"><span data-stu-id="6fdd8-134">timeout</span></span>|<span data-ttu-id="6fdd8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6fdd8-135">Int32</span></span>|<span data-ttu-id="6fdd8-136">O tempo limite em segundos para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="6fdd8-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="6fdd8-137">maskCallee</span></span>|<span data-ttu-id="6fdd8-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="6fdd8-138">Boolean</span></span>|<span data-ttu-id="6fdd8-139">Indica se o receptor deve ser mascarado.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="6fdd8-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="6fdd8-140">maskCaller</span></span>|<span data-ttu-id="6fdd8-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="6fdd8-141">Boolean</span></span>|<span data-ttu-id="6fdd8-142">Indica se o chamador deve ser mascarado.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="6fdd8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fdd8-143">Response</span></span>
<span data-ttu-id="6fdd8-144">Retorna `202 Accepted` o código de resposta</span><span class="sxs-lookup"><span data-stu-id="6fdd8-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="6fdd8-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6fdd8-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="6fdd8-146">Redirecionar uma chamada</span><span class="sxs-lookup"><span data-stu-id="6fdd8-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="6fdd8-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fdd8-147">Request</span></span>
<span data-ttu-id="6fdd8-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-148">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6fdd8-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fdd8-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fdd8-150">C#</span><span class="sxs-lookup"><span data-stu-id="6fdd8-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fdd8-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fdd8-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fdd8-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6fdd8-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6fdd8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fdd8-153">Response</span></span>

> <span data-ttu-id="6fdd8-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fdd8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="6fdd8-156">Encaminhar uma chamada</span><span class="sxs-lookup"><span data-stu-id="6fdd8-156">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6fdd8-157">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="6fdd8-157">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6fdd8-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fdd8-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="6fdd8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fdd8-159">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="6fdd8-160">Notificação-redirecionamento</span><span class="sxs-lookup"><span data-stu-id="6fdd8-160">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="6fdd8-161">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="6fdd8-161">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
