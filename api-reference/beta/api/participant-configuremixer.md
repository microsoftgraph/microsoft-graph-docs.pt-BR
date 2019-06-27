---
title: 'participante: configureMixer'
description: Configure o modo como o áudio é misturado para diferentes participantes em uma conversa de várias partes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cf45c37ba01f32f1d8c494fef76521c20167e8a6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268506"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="6c8d4-103">participante: configureMixer</span><span class="sxs-lookup"><span data-stu-id="6c8d4-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c8d4-104">Configure o modo como o áudio é misturado para diferentes participantes em uma conversa de várias partes.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c8d4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c8d4-105">Permissions</span></span>
<span data-ttu-id="6c8d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c8d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c8d4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c8d4-108">Permission type</span></span> | <span data-ttu-id="6c8d4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c8d4-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="6c8d4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c8d4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c8d4-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6c8d4-111">Not Supported</span></span>        |
| <span data-ttu-id="6c8d4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c8d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c8d4-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6c8d4-113">Not Supported</span></span>        |
| <span data-ttu-id="6c8d4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c8d4-114">Application</span></span>     | <span data-ttu-id="6c8d4-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="6c8d4-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c8d4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c8d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="6c8d4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8d4-117">Request headers</span></span>
| <span data-ttu-id="6c8d4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6c8d4-118">Name</span></span>          | <span data-ttu-id="6c8d4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8d4-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6c8d4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c8d4-120">Authorization</span></span> | <span data-ttu-id="6c8d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c8d4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8d4-123">Request body</span></span>
<span data-ttu-id="6c8d4-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c8d4-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6c8d4-125">Parameter</span></span>      | <span data-ttu-id="6c8d4-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c8d4-126">Type</span></span>    |<span data-ttu-id="6c8d4-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c8d4-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c8d4-128">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="6c8d4-128">participantMixerLevels</span></span>|<span data-ttu-id="6c8d4-129">coleção [participantMixerLevel](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="6c8d4-129">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="6c8d4-130">Configuração dos níveis de mixer para determinado participante de áudio.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-130">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="6c8d4-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="6c8d4-131">clientContext</span></span>|<span data-ttu-id="6c8d4-132">String</span><span class="sxs-lookup"><span data-stu-id="6c8d4-132">String</span></span>|<span data-ttu-id="6c8d4-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="6c8d4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c8d4-134">Response</span></span>
<span data-ttu-id="6c8d4-135">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="6c8d4-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c8d4-136">Example</span></span>
<span data-ttu-id="6c8d4-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6c8d4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c8d4-138">Request</span></span>
<span data-ttu-id="6c8d4-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6c8d4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c8d4-140">Response</span></span>

> <span data-ttu-id="6c8d4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c8d4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c8d4-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6c8d4-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c8d4-144">C#</span><span class="sxs-lookup"><span data-stu-id="6c8d4-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/participant-configureMixer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c8d4-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c8d4-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/participant-configureMixer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6c8d4-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6c8d4-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/participant-configureMixer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="6c8d4-147">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="6c8d4-147">Notification - operation completed</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"1\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
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
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
