---
title: 'chamar: rejeitar'
description: Rejeite uma chamada de entrada.
author: VinodRavichandran
ms.openlocfilehash: 2516ead8d9fa158192a0d9c7c02ac8adb44f764a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343453"
---
# <a name="call-reject"></a><span data-ttu-id="175ab-103">chamar: rejeitar</span><span class="sxs-lookup"><span data-stu-id="175ab-103">call: reject</span></span>

> <span data-ttu-id="175ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="175ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="175ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="175ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="175ab-106">Rejeite uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="175ab-106">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="175ab-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="175ab-107">Permissions</span></span>
<span data-ttu-id="175ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="175ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="175ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="175ab-110">Permission type</span></span> | <span data-ttu-id="175ab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="175ab-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="175ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="175ab-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="175ab-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="175ab-113">Not Supported</span></span>                       |
| <span data-ttu-id="175ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="175ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="175ab-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="175ab-115">Not Supported</span></span>                       |
| <span data-ttu-id="175ab-116">Application</span><span class="sxs-lookup"><span data-stu-id="175ab-116">Application</span></span>     | <span data-ttu-id="175ab-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="175ab-117">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="175ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="175ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="175ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="175ab-119">Request headers</span></span>
| <span data-ttu-id="175ab-120">Nome</span><span class="sxs-lookup"><span data-stu-id="175ab-120">Name</span></span>          | <span data-ttu-id="175ab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="175ab-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="175ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="175ab-122">Authorization</span></span> | <span data-ttu-id="175ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="175ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="175ab-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="175ab-125">Request body</span></span>
<span data-ttu-id="175ab-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="175ab-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="175ab-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="175ab-127">Parameter</span></span>      | <span data-ttu-id="175ab-128">Type</span><span class="sxs-lookup"><span data-stu-id="175ab-128">Type</span></span>    |<span data-ttu-id="175ab-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="175ab-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="175ab-130">motivo</span><span class="sxs-lookup"><span data-stu-id="175ab-130">reason</span></span>|<span data-ttu-id="175ab-131">String</span><span class="sxs-lookup"><span data-stu-id="175ab-131">String</span></span>|<span data-ttu-id="175ab-132">O motivo de rejeição.</span><span class="sxs-lookup"><span data-stu-id="175ab-132">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="175ab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="175ab-133">Response</span></span>
<span data-ttu-id="175ab-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="175ab-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="175ab-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="175ab-136">Example</span></span>
<span data-ttu-id="175ab-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="175ab-137">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="175ab-138">Notificação - entrada</span><span class="sxs-lookup"><span data-stu-id="175ab-138">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="175ab-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="175ab-139">Request</span></span>
<span data-ttu-id="175ab-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="175ab-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="175ab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="175ab-141">Response</span></span>
<span data-ttu-id="175ab-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="175ab-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="175ab-143">Notificação - excluída</span><span class="sxs-lookup"><span data-stu-id="175ab-143">Notification - deleted</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
