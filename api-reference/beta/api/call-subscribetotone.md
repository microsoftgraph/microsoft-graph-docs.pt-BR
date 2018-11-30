---
title: 'chamar: subscribeToTone'
description: " telefone."
ms.openlocfilehash: c3793931c2f06e54cdac278f0f0539b42d7e622c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037685"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="8e2ac-103">chamar: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="8e2ac-103">call: subscribeToTone</span></span>

> <span data-ttu-id="8e2ac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e2ac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e2ac-106">Assine DTMF (dual-tone multi-frequency sinalização).</span><span class="sxs-lookup"><span data-stu-id="8e2ac-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="8e2ac-107">Isso permite que você seja notificado quando o usuário pressiona teclas em um telefone "discagem por tom".</span><span class="sxs-lookup"><span data-stu-id="8e2ac-107">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e2ac-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="8e2ac-108">Permissions</span></span>
<span data-ttu-id="8e2ac-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e2ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e2ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e2ac-111">Permission type</span></span> | <span data-ttu-id="8e2ac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e2ac-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8e2ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e2ac-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e2ac-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8e2ac-114">Not Supported</span></span>        |
| <span data-ttu-id="8e2ac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e2ac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e2ac-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8e2ac-116">Not Supported</span></span>        |
| <span data-ttu-id="8e2ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e2ac-117">Application</span></span>     | <span data-ttu-id="8e2ac-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="8e2ac-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="8e2ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e2ac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="8e2ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e2ac-120">Request headers</span></span>
| <span data-ttu-id="8e2ac-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8e2ac-121">Name</span></span>          | <span data-ttu-id="8e2ac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e2ac-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8e2ac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e2ac-123">Authorization</span></span> | <span data-ttu-id="8e2ac-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e2ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e2ac-126">Request body</span></span>
<span data-ttu-id="8e2ac-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e2ac-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8e2ac-128">Parameter</span></span>      | <span data-ttu-id="8e2ac-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e2ac-129">Type</span></span>    | <span data-ttu-id="8e2ac-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e2ac-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="8e2ac-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="8e2ac-131">clientContext</span></span>  | <span data-ttu-id="8e2ac-132">String</span><span class="sxs-lookup"><span data-stu-id="8e2ac-132">String</span></span>  | <span data-ttu-id="8e2ac-133">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-133">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="8e2ac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e2ac-134">Response</span></span>
<span data-ttu-id="8e2ac-135">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="8e2ac-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e2ac-136">Example</span></span>
<span data-ttu-id="8e2ac-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8e2ac-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e2ac-138">Request</span></span>
<span data-ttu-id="8e2ac-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="8e2ac-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e2ac-140">Response</span></span>

> <span data-ttu-id="8e2ac-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e2ac-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="8e2ac-143">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="8e2ac-143">Notification - operation completed</span></span>

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
