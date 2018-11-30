---
title: 'chamar: playPrompt'
description: Reproduza um prompt na chamada.
ms.openlocfilehash: a5fb5d34264298726add6cf2742d1319bfcb6c95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037768"
---
# <a name="call-playprompt"></a><span data-ttu-id="6c782-103">chamar: playPrompt</span><span class="sxs-lookup"><span data-stu-id="6c782-103">call: playPrompt</span></span>

> <span data-ttu-id="6c782-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c782-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c782-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c782-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c782-106">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="6c782-106">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c782-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6c782-107">Permissions</span></span>
<span data-ttu-id="6c782-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c782-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c782-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c782-110">Permission type</span></span>                        | <span data-ttu-id="6c782-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c782-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c782-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c782-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c782-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="6c782-113">Not Supported.</span></span>                               |
| <span data-ttu-id="6c782-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c782-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c782-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="6c782-115">Not Supported.</span></span>                               |
| <span data-ttu-id="6c782-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c782-116">Application</span></span>                            | <span data-ttu-id="6c782-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6c782-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="6c782-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c782-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="6c782-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c782-119">Request headers</span></span>
| <span data-ttu-id="6c782-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6c782-120">Name</span></span>          | <span data-ttu-id="6c782-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c782-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6c782-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c782-122">Authorization</span></span> | <span data-ttu-id="6c782-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c782-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c782-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c782-125">Request body</span></span>
<span data-ttu-id="6c782-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c782-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c782-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6c782-127">Parameter</span></span>      | <span data-ttu-id="6c782-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c782-128">Type</span></span>    |<span data-ttu-id="6c782-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c782-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c782-130">solicita</span><span class="sxs-lookup"><span data-stu-id="6c782-130">prompts</span></span>|<span data-ttu-id="6c782-131">coleção de [prompt](../resources/prompt.md)</span><span class="sxs-lookup"><span data-stu-id="6c782-131">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="6c782-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="6c782-132">clientContext</span></span>|<span data-ttu-id="6c782-133">String</span><span class="sxs-lookup"><span data-stu-id="6c782-133">String</span></span>|<span data-ttu-id="6c782-134">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="6c782-134">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="6c782-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c782-135">Response</span></span>
<span data-ttu-id="6c782-136">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c782-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="6c782-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c782-137">Example</span></span>
<span data-ttu-id="6c782-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6c782-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6c782-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c782-139">Request</span></span>
<span data-ttu-id="6c782-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c782-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6c782-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c782-141">Response</span></span>

> <span data-ttu-id="6c782-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c782-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="6c782-144">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="6c782-144">Notification - operation completed</span></span>

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
        "@odata.etag": "W/\"54451\"",
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
