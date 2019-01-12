---
title: 'chamar: subscribeToTone'
description: Assine DTMF (dual-tone multi-frequency sinalização). Isso permite que você seja notificado quando o usuário pressiona teclas em um telefone 'discagem por tom'.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 929fac43017df2bdee106dd9687c221c65a20fbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916877"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="97045-104">chamar: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="97045-104">call: subscribeToTone</span></span>

> <span data-ttu-id="97045-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97045-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97045-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97045-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97045-107">Assine DTMF (dual-tone multi-frequency sinalização).</span><span class="sxs-lookup"><span data-stu-id="97045-107">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="97045-108">Isso permite que você seja notificado quando o usuário pressiona teclas em um telefone "discagem por tom".</span><span class="sxs-lookup"><span data-stu-id="97045-108">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="97045-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="97045-109">Permissions</span></span>
<span data-ttu-id="97045-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97045-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97045-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97045-112">Permission type</span></span> | <span data-ttu-id="97045-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97045-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="97045-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97045-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="97045-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="97045-115">Not Supported</span></span>        |
| <span data-ttu-id="97045-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97045-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97045-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="97045-117">Not Supported</span></span>        |
| <span data-ttu-id="97045-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97045-118">Application</span></span>     | <span data-ttu-id="97045-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="97045-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="97045-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97045-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="97045-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97045-121">Request headers</span></span>
| <span data-ttu-id="97045-122">Nome</span><span class="sxs-lookup"><span data-stu-id="97045-122">Name</span></span>          | <span data-ttu-id="97045-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="97045-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="97045-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="97045-124">Authorization</span></span> | <span data-ttu-id="97045-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97045-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97045-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97045-127">Request body</span></span>
<span data-ttu-id="97045-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97045-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="97045-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="97045-129">Parameter</span></span>      | <span data-ttu-id="97045-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="97045-130">Type</span></span>    | <span data-ttu-id="97045-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="97045-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="97045-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="97045-132">clientContext</span></span>  | <span data-ttu-id="97045-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97045-133">String</span></span>  | <span data-ttu-id="97045-134">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="97045-134">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="97045-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="97045-135">Response</span></span>
<span data-ttu-id="97045-136">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="97045-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="97045-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97045-137">Example</span></span>
<span data-ttu-id="97045-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="97045-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="97045-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97045-139">Request</span></span>
<span data-ttu-id="97045-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="97045-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="97045-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="97045-141">Response</span></span>

> <span data-ttu-id="97045-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97045-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="97045-144">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="97045-144">Notification - operation completed</span></span>

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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
