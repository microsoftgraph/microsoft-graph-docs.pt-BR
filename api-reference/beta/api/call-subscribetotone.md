---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um telefone de ' toque '.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2c7960d7e42f9845551cf3396bff9b00d43cc409
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317575"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="d098c-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="d098c-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d098c-105">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="d098c-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="d098c-106">Isso permite que você seja notificado quando o usuário pressionar teclas em um telefone de "toque".</span><span class="sxs-lookup"><span data-stu-id="d098c-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="d098c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d098c-107">Permissions</span></span>
<span data-ttu-id="d098c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d098c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d098c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d098c-110">Permission type</span></span> | <span data-ttu-id="d098c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d098c-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="d098c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d098c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d098c-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d098c-113">Not Supported</span></span>        |
| <span data-ttu-id="d098c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d098c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d098c-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d098c-115">Not Supported</span></span>        |
| <span data-ttu-id="d098c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d098c-116">Application</span></span>     | <span data-ttu-id="d098c-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="d098c-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="d098c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d098c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="d098c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d098c-119">Request headers</span></span>
| <span data-ttu-id="d098c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d098c-120">Name</span></span>          | <span data-ttu-id="d098c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d098c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d098c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d098c-122">Authorization</span></span> | <span data-ttu-id="d098c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d098c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d098c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d098c-125">Request body</span></span>
<span data-ttu-id="d098c-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d098c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d098c-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d098c-127">Parameter</span></span>      | <span data-ttu-id="d098c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d098c-128">Type</span></span>    | <span data-ttu-id="d098c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d098c-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="d098c-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="d098c-130">clientContext</span></span>  | <span data-ttu-id="d098c-131">String</span><span class="sxs-lookup"><span data-stu-id="d098c-131">String</span></span>  | <span data-ttu-id="d098c-132">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="d098c-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="d098c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d098c-133">Response</span></span>
<span data-ttu-id="d098c-134">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="d098c-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="d098c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d098c-135">Example</span></span>
<span data-ttu-id="d098c-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d098c-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d098c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d098c-137">Request</span></span>
<span data-ttu-id="d098c-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d098c-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d098c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d098c-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d098c-140">C#</span><span class="sxs-lookup"><span data-stu-id="d098c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d098c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d098c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d098c-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d098c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d098c-143">Java</span><span class="sxs-lookup"><span data-stu-id="d098c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d098c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d098c-144">Response</span></span>

> <span data-ttu-id="d098c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d098c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="d098c-147">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="d098c-147">Notification - operation completed</span></span>

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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
