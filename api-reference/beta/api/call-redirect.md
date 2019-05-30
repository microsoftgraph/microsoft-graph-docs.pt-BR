---
title: 'Call: Redirect'
description: Redirecione as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8c0bea95767881adc10c7e209825803461df20c6
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536082"
---
# <a name="call-redirect"></a><span data-ttu-id="30a72-103">Call: Redirect</span><span class="sxs-lookup"><span data-stu-id="30a72-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a72-104">Redirecione as chamadas recebidas.</span><span class="sxs-lookup"><span data-stu-id="30a72-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="30a72-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30a72-105">Permissions</span></span>
<span data-ttu-id="30a72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30a72-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30a72-108">Permission type</span></span> | <span data-ttu-id="30a72-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30a72-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="30a72-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30a72-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="30a72-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="30a72-111">Not Supported</span></span>                |
| <span data-ttu-id="30a72-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30a72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30a72-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="30a72-113">Not Supported</span></span>                |
| <span data-ttu-id="30a72-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30a72-114">Application</span></span>     | <span data-ttu-id="30a72-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="30a72-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="30a72-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30a72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="30a72-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30a72-117">Request headers</span></span>
| <span data-ttu-id="30a72-118">Nome</span><span class="sxs-lookup"><span data-stu-id="30a72-118">Name</span></span>          | <span data-ttu-id="30a72-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="30a72-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="30a72-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="30a72-120">Authorization</span></span> | <span data-ttu-id="30a72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30a72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30a72-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30a72-123">Request body</span></span>
<span data-ttu-id="30a72-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30a72-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="30a72-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="30a72-125">Parameter</span></span>      | <span data-ttu-id="30a72-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="30a72-126">Type</span></span>    |<span data-ttu-id="30a72-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="30a72-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30a72-128">targets</span><span class="sxs-lookup"><span data-stu-id="30a72-128">targets</span></span>|<span data-ttu-id="30a72-129">coleção [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="30a72-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="30a72-130">Os participantes de destino da operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="30a72-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="30a72-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="30a72-131">targetDisposition</span></span>|<span data-ttu-id="30a72-132">String</span><span class="sxs-lookup"><span data-stu-id="30a72-132">String</span></span>|<span data-ttu-id="30a72-133">O valor possível é:`default`</span><span class="sxs-lookup"><span data-stu-id="30a72-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="30a72-134">timeout</span><span class="sxs-lookup"><span data-stu-id="30a72-134">timeout</span></span>|<span data-ttu-id="30a72-135">Int32</span><span class="sxs-lookup"><span data-stu-id="30a72-135">Int32</span></span>|<span data-ttu-id="30a72-136">O tempo limite em segundos para a operação de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="30a72-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="30a72-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="30a72-137">maskCallee</span></span>|<span data-ttu-id="30a72-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="30a72-138">Boolean</span></span>|<span data-ttu-id="30a72-139">Indica se o receptor deve ser mascarado.</span><span class="sxs-lookup"><span data-stu-id="30a72-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="30a72-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="30a72-140">maskCaller</span></span>|<span data-ttu-id="30a72-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="30a72-141">Boolean</span></span>|<span data-ttu-id="30a72-142">Indica se o chamador deve ser mascarado.</span><span class="sxs-lookup"><span data-stu-id="30a72-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="30a72-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a72-143">Response</span></span>
<span data-ttu-id="30a72-144">Retorna `202 Accepted` o código de resposta</span><span class="sxs-lookup"><span data-stu-id="30a72-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="30a72-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30a72-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="30a72-146">Redirecionar uma chamada</span><span class="sxs-lookup"><span data-stu-id="30a72-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="30a72-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30a72-147">Request</span></span>
<span data-ttu-id="30a72-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="30a72-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="30a72-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a72-149">Response</span></span>

> <span data-ttu-id="30a72-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30a72-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="30a72-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="30a72-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="30a72-153">C#</span><span class="sxs-lookup"><span data-stu-id="30a72-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-redirect-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30a72-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="30a72-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-redirect-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="forward-a-call"></a><span data-ttu-id="30a72-155">Encaminhar uma chamada</span><span class="sxs-lookup"><span data-stu-id="30a72-155">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="30a72-156">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="30a72-156">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="30a72-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30a72-157">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="30a72-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="30a72-158">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="30a72-159">Notificação-redirecionamento</span><span class="sxs-lookup"><span data-stu-id="30a72-159">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="30a72-160">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="30a72-160">Notification - terminated</span></span>

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
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
