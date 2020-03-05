---
title: 'Call: cancelMediaProcessing'
description: Cancela o processamento de mídia para qualquer operação PlayPrompt ou RecordResponse em andamento.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0f9ec0eaede3383d6e99a05e4aa4023dd914d9b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440882"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="4deef-103">Call: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="4deef-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="4deef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4deef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4deef-105">Cancela o processamento de todas as operações de [resposta de gravação](./call-record.md) ou [aviso de execução](./call-playprompt.md) em andamento.</span><span class="sxs-lookup"><span data-stu-id="4deef-105">Cancels processing for any in-progress [play prompt](./call-playprompt.md) or [record response](./call-record.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="4deef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4deef-106">Permissions</span></span>
<span data-ttu-id="4deef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4deef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4deef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4deef-109">Permission type</span></span>                        | <span data-ttu-id="4deef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4deef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4deef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4deef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4deef-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4deef-112">Not Supported.</span></span>                              |
| <span data-ttu-id="4deef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4deef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4deef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4deef-114">Not Supported.</span></span>                              |
| <span data-ttu-id="4deef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4deef-115">Application</span></span>                            | <span data-ttu-id="4deef-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4deef-116">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="4deef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4deef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="4deef-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="4deef-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="4deef-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="4deef-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4deef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4deef-120">Request headers</span></span>
| <span data-ttu-id="4deef-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4deef-121">Name</span></span>          | <span data-ttu-id="4deef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4deef-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4deef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4deef-123">Authorization</span></span> | <span data-ttu-id="4deef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4deef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4deef-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4deef-126">Content-type</span></span> | <span data-ttu-id="4deef-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4deef-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4deef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4deef-129">Request body</span></span>
<span data-ttu-id="4deef-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4deef-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4deef-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4deef-131">Parameter</span></span>      | <span data-ttu-id="4deef-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4deef-132">Type</span></span>    | <span data-ttu-id="4deef-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4deef-133">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="4deef-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="4deef-134">clientContext</span></span>  | <span data-ttu-id="4deef-135">String</span><span class="sxs-lookup"><span data-stu-id="4deef-135">String</span></span>  | <span data-ttu-id="4deef-136">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="4deef-136">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="4deef-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4deef-137">Response</span></span>
<span data-ttu-id="4deef-138">Se tiver êxito, este método retornará `200 OK` um código de resposta http e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="4deef-138">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="4deef-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4deef-139">Example</span></span>
<span data-ttu-id="4deef-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4deef-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4deef-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4deef-141">Request</span></span>
<span data-ttu-id="4deef-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4deef-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4deef-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4deef-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4deef-144">C#</span><span class="sxs-lookup"><span data-stu-id="4deef-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4deef-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4deef-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4deef-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4deef-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4deef-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4deef-147">Response</span></span>

> <span data-ttu-id="4deef-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4deef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5"
}
```

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="4deef-150">Notificação-operação cancelada para recordResponse</span><span class="sxs-lookup"><span data-stu-id="4deef-150">Notification - Operation canceled for recordResponse</span></span>

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
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "failed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 400,
          "subcode": 8508,
          "message": "Action falied, the operation was cancelled."
        },
        "recordingLocation": "",
        "recordingAccessToken": "",
        "completionReason": "operationCanceled"
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
