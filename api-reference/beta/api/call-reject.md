---
title: 'Call: rejeitar'
description: Rejeite as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3a9d3f8a7c25b2617e3fa97c9e872eaba92d17e4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635726"
---
# <a name="call-reject"></a><span data-ttu-id="ed548-103">Call: rejeitar</span><span class="sxs-lookup"><span data-stu-id="ed548-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed548-104">Rejeite as chamadas recebidas.</span><span class="sxs-lookup"><span data-stu-id="ed548-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed548-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed548-105">Permissions</span></span>
<span data-ttu-id="ed548-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed548-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed548-108">Permission type</span></span> | <span data-ttu-id="ed548-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed548-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="ed548-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed548-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed548-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="ed548-111">Not Supported</span></span>                       |
| <span data-ttu-id="ed548-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed548-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed548-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="ed548-113">Not Supported</span></span>                       |
| <span data-ttu-id="ed548-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed548-114">Application</span></span>     | <span data-ttu-id="ed548-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed548-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="ed548-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed548-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="ed548-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed548-117">Request headers</span></span>
| <span data-ttu-id="ed548-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ed548-118">Name</span></span>          | <span data-ttu-id="ed548-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed548-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ed548-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed548-120">Authorization</span></span> | <span data-ttu-id="ed548-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed548-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed548-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed548-123">Request body</span></span>
<span data-ttu-id="ed548-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed548-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ed548-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ed548-125">Parameter</span></span>      | <span data-ttu-id="ed548-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed548-126">Type</span></span>    |<span data-ttu-id="ed548-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed548-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed548-128">motivos</span><span class="sxs-lookup"><span data-stu-id="ed548-128">reason</span></span>|<span data-ttu-id="ed548-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed548-129">String</span></span>|<span data-ttu-id="ed548-130">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="ed548-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="ed548-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed548-131">Response</span></span>
<span data-ttu-id="ed548-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed548-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="ed548-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed548-134">Example</span></span>
<span data-ttu-id="ed548-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ed548-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="ed548-136">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="ed548-136">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="ed548-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed548-137">Request</span></span>
<span data-ttu-id="ed548-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed548-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="ed548-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed548-139">Response</span></span>
<span data-ttu-id="ed548-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed548-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed548-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ed548-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ed548-142">Basic</span><span class="sxs-lookup"><span data-stu-id="ed548-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-reject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed548-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed548-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-reject-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---deleted"></a><span data-ttu-id="ed548-144">Notificação-excluído</span><span class="sxs-lookup"><span data-stu-id="ed548-144">Notification - deleted</span></span>

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
        "@odata.etag": "W/\"5445\""
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
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-reject.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-reject.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
