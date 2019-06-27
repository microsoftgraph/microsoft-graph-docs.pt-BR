---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 12140967ef2d0825ffc210a4da17e525a1bff33c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262248"
---
# <a name="call-redirect"></a><span data-ttu-id="cb809-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="cb809-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb809-104">Redirecione as chamadas recebidas.</span><span class="sxs-lookup"><span data-stu-id="cb809-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb809-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb809-105">Permissions</span></span>
<span data-ttu-id="cb809-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb809-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb809-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb809-108">Permission type</span></span> | <span data-ttu-id="cb809-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb809-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="cb809-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb809-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb809-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cb809-111">Not Supported</span></span>                |
| <span data-ttu-id="cb809-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb809-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb809-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cb809-113">Not Supported</span></span>                |
| <span data-ttu-id="cb809-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb809-114">Application</span></span>     | <span data-ttu-id="cb809-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="cb809-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="cb809-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb809-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="cb809-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb809-117">Request headers</span></span>
| <span data-ttu-id="cb809-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cb809-118">Name</span></span>          | <span data-ttu-id="cb809-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb809-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cb809-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb809-120">Authorization</span></span> | <span data-ttu-id="cb809-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb809-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb809-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb809-123">Request body</span></span>
<span data-ttu-id="cb809-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb809-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb809-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cb809-125">Parameter</span></span>      | <span data-ttu-id="cb809-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb809-126">Type</span></span>    |<span data-ttu-id="cb809-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb809-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb809-128">targets</span><span class="sxs-lookup"><span data-stu-id="cb809-128">targets</span></span>|<span data-ttu-id="cb809-129">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="cb809-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="cb809-130">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="cb809-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="cb809-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="cb809-131">targetDisposition</span></span>|<span data-ttu-id="cb809-132">String</span><span class="sxs-lookup"><span data-stu-id="cb809-132">String</span></span>|<span data-ttu-id="cb809-133">O valor possível é:`default`</span><span class="sxs-lookup"><span data-stu-id="cb809-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="cb809-134">timeout</span><span class="sxs-lookup"><span data-stu-id="cb809-134">timeout</span></span>|<span data-ttu-id="cb809-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cb809-135">Int32</span></span>|<span data-ttu-id="cb809-136">O tempo limite em segundos para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="cb809-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="cb809-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="cb809-137">maskCallee</span></span>|<span data-ttu-id="cb809-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="cb809-138">Boolean</span></span>|<span data-ttu-id="cb809-139">Indica se o receptor deve ser mascarado.</span><span class="sxs-lookup"><span data-stu-id="cb809-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="cb809-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="cb809-140">maskCaller</span></span>|<span data-ttu-id="cb809-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="cb809-141">Boolean</span></span>|<span data-ttu-id="cb809-142">Indica se o chamador deve ser mascarado.</span><span class="sxs-lookup"><span data-stu-id="cb809-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="cb809-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb809-143">Response</span></span>
<span data-ttu-id="cb809-144">Retorna `202 Accepted` o código de resposta</span><span class="sxs-lookup"><span data-stu-id="cb809-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="cb809-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb809-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="cb809-146">Redirecionar uma chamada</span><span class="sxs-lookup"><span data-stu-id="cb809-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="cb809-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb809-147">Request</span></span>
<span data-ttu-id="cb809-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb809-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="cb809-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb809-149">Response</span></span>

> <span data-ttu-id="cb809-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb809-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cb809-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cb809-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cb809-153">C#</span><span class="sxs-lookup"><span data-stu-id="cb809-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-redirect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb809-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb809-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-redirect-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cb809-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cb809-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-redirect-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="forward-a-call"></a><span data-ttu-id="cb809-156">Encaminhar uma chamada</span><span class="sxs-lookup"><span data-stu-id="cb809-156">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="cb809-157">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="cb809-157">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="cb809-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb809-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="cb809-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb809-159">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="cb809-160">Notificação-redirecionamento</span><span class="sxs-lookup"><span data-stu-id="cb809-160">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="cb809-161">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="cb809-161">Notification - terminated</span></span>

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
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
