---
title: 'participante: configureMixer'
description: Configure o modo como o áudio é misturado para diferentes participantes em uma conversa de várias partes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f1a7650ea3195cdb28af6d49a71983129e0e322a
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636831"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="cb585-103">participante: configureMixer</span><span class="sxs-lookup"><span data-stu-id="cb585-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb585-104">Configure o modo como o áudio é misturado para diferentes participantes em uma conversa de várias partes.</span><span class="sxs-lookup"><span data-stu-id="cb585-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb585-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb585-105">Permissions</span></span>
<span data-ttu-id="cb585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb585-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb585-108">Permission type</span></span> | <span data-ttu-id="cb585-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb585-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="cb585-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb585-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb585-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cb585-111">Not Supported</span></span>        |
| <span data-ttu-id="cb585-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb585-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb585-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cb585-113">Not Supported</span></span>        |
| <span data-ttu-id="cb585-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb585-114">Application</span></span>     | <span data-ttu-id="cb585-115">Calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="cb585-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb585-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb585-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="cb585-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="cb585-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="cb585-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="cb585-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb585-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb585-119">Request headers</span></span>
| <span data-ttu-id="cb585-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cb585-120">Name</span></span>          | <span data-ttu-id="cb585-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb585-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cb585-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb585-122">Authorization</span></span> | <span data-ttu-id="cb585-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb585-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb585-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb585-125">Request body</span></span>
<span data-ttu-id="cb585-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb585-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb585-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cb585-127">Parameter</span></span>      | <span data-ttu-id="cb585-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb585-128">Type</span></span>    |<span data-ttu-id="cb585-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb585-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb585-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="cb585-130">participantMixerLevels</span></span>|<span data-ttu-id="cb585-131">coleção [participantMixerLevel](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="cb585-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="cb585-132">Configuração dos níveis de mixer para determinado participante de áudio.</span><span class="sxs-lookup"><span data-stu-id="cb585-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="cb585-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="cb585-133">clientContext</span></span>|<span data-ttu-id="cb585-134">String</span><span class="sxs-lookup"><span data-stu-id="cb585-134">String</span></span>|<span data-ttu-id="cb585-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="cb585-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="cb585-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb585-136">Response</span></span>
<span data-ttu-id="cb585-137">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb585-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="cb585-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb585-138">Example</span></span>
<span data-ttu-id="cb585-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cb585-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cb585-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb585-140">Request</span></span>
<span data-ttu-id="cb585-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb585-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb585-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb585-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb585-143">C#</span><span class="sxs-lookup"><span data-stu-id="cb585-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb585-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb585-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb585-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb585-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cb585-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb585-146">Response</span></span>

> <span data-ttu-id="cb585-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb585-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-configureMixer",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "running"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="cb585-149">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="cb585-149">Notification - operation completed</span></span>

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
      "@odata.type": "#microsoft.graph.commsOperation",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
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
