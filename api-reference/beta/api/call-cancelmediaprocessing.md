---
title: 'chamar: cancelMediaProcessing'
description: Mídia cancela o processamento para todos quaisquer operações PlayPrompt ou o registro em andamento.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: db5a918f630fc54cc6eb574896e9e42af179c05a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921994"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="b4155-103">chamar: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="b4155-103">call: cancelMediaProcessing</span></span>

> <span data-ttu-id="b4155-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4155-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4155-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4155-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4155-106">Mídia cancela o processamento para todos quaisquer operações PlayPrompt ou o registro em andamento.</span><span class="sxs-lookup"><span data-stu-id="b4155-106">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4155-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4155-107">Permissions</span></span>
<span data-ttu-id="b4155-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4155-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4155-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4155-110">Permission type</span></span>                        | <span data-ttu-id="b4155-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4155-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4155-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4155-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4155-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="b4155-113">Not Supported.</span></span>                              |
| <span data-ttu-id="b4155-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4155-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4155-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="b4155-115">Not Supported.</span></span>                              |
| <span data-ttu-id="b4155-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4155-116">Application</span></span>                            | <span data-ttu-id="b4155-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b4155-117">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="b4155-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4155-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="b4155-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4155-119">Request headers</span></span>
| <span data-ttu-id="b4155-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b4155-120">Name</span></span>          | <span data-ttu-id="b4155-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4155-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b4155-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4155-122">Authorization</span></span> | <span data-ttu-id="b4155-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4155-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4155-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4155-125">Request body</span></span>
<span data-ttu-id="b4155-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4155-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4155-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b4155-127">Parameter</span></span>      | <span data-ttu-id="b4155-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4155-128">Type</span></span>    | <span data-ttu-id="b4155-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4155-129">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="b4155-130">todos os</span><span class="sxs-lookup"><span data-stu-id="b4155-130">all</span></span>            | <span data-ttu-id="b4155-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4155-131">Boolean</span></span> | <span data-ttu-id="b4155-132">O sinalizador indicando se pare todas as operações ou atual.</span><span class="sxs-lookup"><span data-stu-id="b4155-132">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="b4155-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="b4155-133">clientContext</span></span>  | <span data-ttu-id="b4155-134">String</span><span class="sxs-lookup"><span data-stu-id="b4155-134">String</span></span>  | <span data-ttu-id="b4155-135">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="b4155-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="b4155-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4155-136">Response</span></span>
<span data-ttu-id="b4155-137">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4155-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b4155-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4155-138">Example</span></span>
<span data-ttu-id="b4155-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b4155-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b4155-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4155-140">Request</span></span>
<span data-ttu-id="b4155-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4155-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="b4155-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4155-142">Response</span></span>

> <span data-ttu-id="b4155-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4155-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="b4155-145">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="b4155-145">Notification - operation completed</span></span>

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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
