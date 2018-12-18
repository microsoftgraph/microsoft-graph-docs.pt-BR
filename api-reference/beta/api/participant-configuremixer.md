---
title: 'participante: configureMixer'
description: Configure como áudio misto para diferentes participantes em uma conversa com vários participantes.
author: VinodRavichandran
ms.openlocfilehash: e300d842ce0bad870160d2f3788b059de6d41784
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351986"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="fa8df-103">participante: configureMixer</span><span class="sxs-lookup"><span data-stu-id="fa8df-103">participant: configureMixer</span></span>

> <span data-ttu-id="fa8df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fa8df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa8df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fa8df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa8df-106">Configure como áudio misto para diferentes participantes em uma conversa com vários participantes.</span><span class="sxs-lookup"><span data-stu-id="fa8df-106">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa8df-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa8df-107">Permissions</span></span>
<span data-ttu-id="fa8df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa8df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa8df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa8df-110">Permission type</span></span> | <span data-ttu-id="fa8df-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa8df-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="fa8df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa8df-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa8df-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="fa8df-113">Not Supported</span></span>        |
| <span data-ttu-id="fa8df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa8df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa8df-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="fa8df-115">Not Supported</span></span>        |
| <span data-ttu-id="fa8df-116">Application</span><span class="sxs-lookup"><span data-stu-id="fa8df-116">Application</span></span>     | <span data-ttu-id="fa8df-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="fa8df-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa8df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa8df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="fa8df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa8df-119">Request headers</span></span>
| <span data-ttu-id="fa8df-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fa8df-120">Name</span></span>          | <span data-ttu-id="fa8df-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa8df-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fa8df-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa8df-122">Authorization</span></span> | <span data-ttu-id="fa8df-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa8df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa8df-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa8df-125">Request body</span></span>
<span data-ttu-id="fa8df-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa8df-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa8df-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa8df-127">Parameter</span></span>      | <span data-ttu-id="fa8df-128">Type</span><span class="sxs-lookup"><span data-stu-id="fa8df-128">Type</span></span>    |<span data-ttu-id="fa8df-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa8df-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa8df-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="fa8df-130">participantMixerLevels</span></span>|<span data-ttu-id="fa8df-131">coleção [participantMixerLevel](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="fa8df-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="fa8df-132">Configuração do mixer redistribui para determinados participante de áudio.</span><span class="sxs-lookup"><span data-stu-id="fa8df-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="fa8df-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="fa8df-133">clientContext</span></span>|<span data-ttu-id="fa8df-134">String</span><span class="sxs-lookup"><span data-stu-id="fa8df-134">String</span></span>|<span data-ttu-id="fa8df-135">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="fa8df-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="fa8df-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa8df-136">Response</span></span>
<span data-ttu-id="fa8df-137">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa8df-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="fa8df-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa8df-138">Example</span></span>
<span data-ttu-id="fa8df-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fa8df-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fa8df-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa8df-140">Request</span></span>
<span data-ttu-id="fa8df-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa8df-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant_configureMixer"
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

##### <a name="response"></a><span data-ttu-id="fa8df-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa8df-142">Response</span></span>

> <span data-ttu-id="fa8df-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa8df-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="fa8df-145">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="fa8df-145">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
