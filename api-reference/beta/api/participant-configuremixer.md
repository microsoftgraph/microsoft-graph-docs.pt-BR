---
title: 'participante: configureMixer'
description: Configure o modo como o áudio é misturado para diferentes participantes em uma conversa de várias partes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c59c56c7c862a62247cadf8472a042e3ea8d9af2
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006477"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="3cf8f-103">participante: configureMixer</span><span class="sxs-lookup"><span data-stu-id="3cf8f-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cf8f-104">Configure o modo como o áudio é misturado para diferentes participantes em uma conversa de várias partes.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf8f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cf8f-105">Permissions</span></span>
<span data-ttu-id="3cf8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cf8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cf8f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cf8f-108">Permission type</span></span> | <span data-ttu-id="3cf8f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cf8f-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="3cf8f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cf8f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cf8f-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3cf8f-111">Not Supported</span></span>        |
| <span data-ttu-id="3cf8f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cf8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf8f-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3cf8f-113">Not Supported</span></span>        |
| <span data-ttu-id="3cf8f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cf8f-114">Application</span></span>     | <span data-ttu-id="3cf8f-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="3cf8f-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cf8f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="3cf8f-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3cf8f-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cf8f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cf8f-119">Request headers</span></span>
| <span data-ttu-id="3cf8f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3cf8f-120">Name</span></span>          | <span data-ttu-id="3cf8f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf8f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3cf8f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cf8f-122">Authorization</span></span> | <span data-ttu-id="3cf8f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cf8f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cf8f-125">Request body</span></span>
<span data-ttu-id="3cf8f-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3cf8f-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3cf8f-127">Parameter</span></span>      | <span data-ttu-id="3cf8f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cf8f-128">Type</span></span>    |<span data-ttu-id="3cf8f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf8f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cf8f-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="3cf8f-130">participantMixerLevels</span></span>|<span data-ttu-id="3cf8f-131">coleção [participantMixerLevel](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="3cf8f-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="3cf8f-132">Configuração dos níveis de mixer para determinado participante de áudio.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="3cf8f-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="3cf8f-133">clientContext</span></span>|<span data-ttu-id="3cf8f-134">String</span><span class="sxs-lookup"><span data-stu-id="3cf8f-134">String</span></span>|<span data-ttu-id="3cf8f-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="3cf8f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cf8f-136">Response</span></span>
<span data-ttu-id="3cf8f-137">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="3cf8f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cf8f-138">Example</span></span>
<span data-ttu-id="3cf8f-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3cf8f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cf8f-140">Request</span></span>
<span data-ttu-id="3cf8f-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3cf8f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf8f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/configureMixer
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cf8f-143">C#</span><span class="sxs-lookup"><span data-stu-id="3cf8f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cf8f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cf8f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cf8f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cf8f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cf8f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cf8f-146">Response</span></span>

> <span data-ttu-id="3cf8f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cf8f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="3cf8f-149">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="3cf8f-149">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
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
  ]
}
-->
