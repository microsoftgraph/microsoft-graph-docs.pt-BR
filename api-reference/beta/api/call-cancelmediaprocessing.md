---
title: 'Call: cancelMediaProcessing'
description: Cancela o processamento de mídia para todas as operações de PlayPrompt ou registro em andamento.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1463489c82d1595e1bdcaa9629e5f306b95aa19f
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006358"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="b584b-103">Call: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="b584b-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b584b-104">Cancela o processamento de mídia para todas as operações de PlayPrompt ou registro em andamento.</span><span class="sxs-lookup"><span data-stu-id="b584b-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="b584b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b584b-105">Permissions</span></span>
<span data-ttu-id="b584b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b584b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b584b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b584b-108">Permission type</span></span>                        | <span data-ttu-id="b584b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b584b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b584b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b584b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b584b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b584b-111">Not Supported.</span></span>                              |
| <span data-ttu-id="b584b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b584b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b584b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b584b-113">Not Supported.</span></span>                              |
| <span data-ttu-id="b584b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b584b-114">Application</span></span>                            | <span data-ttu-id="b584b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b584b-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="b584b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b584b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="b584b-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="b584b-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b584b-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="b584b-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b584b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b584b-119">Request headers</span></span>
| <span data-ttu-id="b584b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b584b-120">Name</span></span>          | <span data-ttu-id="b584b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b584b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b584b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b584b-122">Authorization</span></span> | <span data-ttu-id="b584b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b584b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b584b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b584b-125">Request body</span></span>
<span data-ttu-id="b584b-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b584b-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b584b-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b584b-127">Parameter</span></span>      | <span data-ttu-id="b584b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b584b-128">Type</span></span>    | <span data-ttu-id="b584b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b584b-129">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="b584b-130">todos os</span><span class="sxs-lookup"><span data-stu-id="b584b-130">all</span></span>            | <span data-ttu-id="b584b-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="b584b-131">Boolean</span></span> | <span data-ttu-id="b584b-132">O sinalizador que indica se todas as operações ou o atual devem ser interrompidos.</span><span class="sxs-lookup"><span data-stu-id="b584b-132">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="b584b-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="b584b-133">clientContext</span></span>  | <span data-ttu-id="b584b-134">String</span><span class="sxs-lookup"><span data-stu-id="b584b-134">String</span></span>  | <span data-ttu-id="b584b-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="b584b-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="b584b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b584b-136">Response</span></span>
<span data-ttu-id="b584b-137">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="b584b-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b584b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b584b-138">Example</span></span>
<span data-ttu-id="b584b-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b584b-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b584b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b584b-140">Request</span></span>
<span data-ttu-id="b584b-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b584b-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b584b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b584b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b584b-143">C#</span><span class="sxs-lookup"><span data-stu-id="b584b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b584b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b584b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b584b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b584b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b584b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b584b-146">Response</span></span>

> <span data-ttu-id="b584b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b584b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
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

##### <a name="notification---operation-completed"></a><span data-ttu-id="b584b-149">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="b584b-149">Notification - operation completed</span></span>

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
  ]
}
-->
