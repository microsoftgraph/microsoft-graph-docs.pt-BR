---
title: 'chamar: cancelMediaProcessing'
description: Mídia cancela o processamento para todos quaisquer operações PlayPrompt ou o registro em andamento.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 77c35cb0cfeaea6ebb2e623b32b1fa3c70f65777
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527847"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="154f4-103">chamar: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="154f4-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="154f4-104">Mídia cancela o processamento para todos quaisquer operações PlayPrompt ou o registro em andamento.</span><span class="sxs-lookup"><span data-stu-id="154f4-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="154f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="154f4-105">Permissions</span></span>
<span data-ttu-id="154f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="154f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="154f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="154f4-108">Permission type</span></span>                        | <span data-ttu-id="154f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="154f4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="154f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="154f4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="154f4-111">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="154f4-111">Not Supported.</span></span>                              |
| <span data-ttu-id="154f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="154f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="154f4-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="154f4-113">Not Supported.</span></span>                              |
| <span data-ttu-id="154f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="154f4-114">Application</span></span>                            | <span data-ttu-id="154f4-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="154f4-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="154f4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="154f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="154f4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="154f4-117">Request headers</span></span>
| <span data-ttu-id="154f4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="154f4-118">Name</span></span>          | <span data-ttu-id="154f4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="154f4-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="154f4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="154f4-120">Authorization</span></span> | <span data-ttu-id="154f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="154f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="154f4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="154f4-123">Request body</span></span>
<span data-ttu-id="154f4-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="154f4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="154f4-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="154f4-125">Parameter</span></span>      | <span data-ttu-id="154f4-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="154f4-126">Type</span></span>    | <span data-ttu-id="154f4-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="154f4-127">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="154f4-128">ALL</span><span class="sxs-lookup"><span data-stu-id="154f4-128">all</span></span>            | <span data-ttu-id="154f4-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="154f4-129">Boolean</span></span> | <span data-ttu-id="154f4-130">O sinalizador indicando se pare todas as operações ou atual.</span><span class="sxs-lookup"><span data-stu-id="154f4-130">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="154f4-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="154f4-131">clientContext</span></span>  | <span data-ttu-id="154f4-132">String</span><span class="sxs-lookup"><span data-stu-id="154f4-132">String</span></span>  | <span data-ttu-id="154f4-133">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="154f4-133">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="154f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="154f4-134">Response</span></span>
<span data-ttu-id="154f4-135">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="154f4-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="154f4-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="154f4-136">Example</span></span>
<span data-ttu-id="154f4-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="154f4-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="154f4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="154f4-138">Request</span></span>
<span data-ttu-id="154f4-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="154f4-139">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="154f4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="154f4-140">Response</span></span>

> <span data-ttu-id="154f4-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="154f4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="154f4-143">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="154f4-143">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-cancelmediaprocessing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
