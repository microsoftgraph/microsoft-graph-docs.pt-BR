---
title: 'participante: configureMixer'
description: Configure como o áudio é misto para diferentes participantes em uma conversa de várias partes.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9b8efa45be5163e088bef06e2d71959e80cae58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037911"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="65191-103">participante: configureMixer</span><span class="sxs-lookup"><span data-stu-id="65191-103">participant: configureMixer</span></span>

<span data-ttu-id="65191-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65191-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65191-105">Configure como o áudio é misto para diferentes participantes em uma conversa de várias partes.</span><span class="sxs-lookup"><span data-stu-id="65191-105">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="65191-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65191-106">Permissions</span></span>
<span data-ttu-id="65191-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65191-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65191-109">Permission type</span></span> | <span data-ttu-id="65191-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65191-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="65191-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65191-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65191-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="65191-112">Not Supported</span></span>        |
| <span data-ttu-id="65191-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65191-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65191-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="65191-114">Not Supported</span></span>        |
| <span data-ttu-id="65191-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65191-115">Application</span></span>     | <span data-ttu-id="65191-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="65191-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65191-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65191-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="65191-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="65191-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="65191-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="65191-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65191-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65191-120">Request headers</span></span>
| <span data-ttu-id="65191-121">Nome</span><span class="sxs-lookup"><span data-stu-id="65191-121">Name</span></span>          | <span data-ttu-id="65191-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="65191-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="65191-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="65191-123">Authorization</span></span> | <span data-ttu-id="65191-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65191-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65191-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65191-126">Request body</span></span>
<span data-ttu-id="65191-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65191-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65191-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="65191-128">Parameter</span></span>      | <span data-ttu-id="65191-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="65191-129">Type</span></span>    |<span data-ttu-id="65191-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="65191-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65191-131">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="65191-131">participantMixerLevels</span></span>|<span data-ttu-id="65191-132">[Coleção participantMixerLevel](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="65191-132">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="65191-133">Configuração de níveis de mistura para determinado participante de áudio.</span><span class="sxs-lookup"><span data-stu-id="65191-133">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="65191-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="65191-134">clientContext</span></span>|<span data-ttu-id="65191-135">String</span><span class="sxs-lookup"><span data-stu-id="65191-135">String</span></span>|<span data-ttu-id="65191-136">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="65191-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="65191-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="65191-137">Response</span></span>
<span data-ttu-id="65191-138">Retorna `202 Accepted` o código de resposta e um header location com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="65191-138">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="65191-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65191-139">Example</span></span>
<span data-ttu-id="65191-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="65191-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="65191-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65191-141">Request</span></span>
<span data-ttu-id="65191-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="65191-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="65191-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="65191-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="65191-144">C#</span><span class="sxs-lookup"><span data-stu-id="65191-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65191-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65191-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65191-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65191-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65191-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="65191-147">Response</span></span>

> <span data-ttu-id="65191-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65191-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="65191-149">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="65191-149">Notification - operation completed</span></span>

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


