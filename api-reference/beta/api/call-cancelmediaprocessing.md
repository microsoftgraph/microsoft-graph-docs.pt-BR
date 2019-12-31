---
title: 'Call: cancelMediaProcessing'
description: Cancela o processamento de mídia para qualquer operação PlayPrompt ou RecordResponse em andamento.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a11b42affaa2cc4c21dd50e2d2474f3e2ffa77d1
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912914"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="e9a1f-103">Call: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="e9a1f-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a1f-104">Cancela o processamento de todas as operações de [resposta de gravação](./call-record.md) ou [aviso de execução](./call-playprompt.md) em andamento.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-104">Cancels processing for any in-progress [play prompt](./call-playprompt.md) or [record response](./call-record.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9a1f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9a1f-105">Permissions</span></span>
<span data-ttu-id="e9a1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9a1f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9a1f-108">Permission type</span></span>                        | <span data-ttu-id="e9a1f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9a1f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9a1f-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9a1f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9a1f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-111">Not Supported.</span></span>                              |
| <span data-ttu-id="e9a1f-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9a1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9a1f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-113">Not Supported.</span></span>                              |
| <span data-ttu-id="e9a1f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9a1f-114">Application</span></span>                            | <span data-ttu-id="e9a1f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="e9a1f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="e9a1f-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e9a1f-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9a1f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a1f-119">Request headers</span></span>
| <span data-ttu-id="e9a1f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e9a1f-120">Name</span></span>          | <span data-ttu-id="e9a1f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9a1f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e9a1f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9a1f-122">Authorization</span></span> | <span data-ttu-id="e9a1f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9a1f-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e9a1f-125">Content-type</span></span> | <span data-ttu-id="e9a1f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9a1f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a1f-128">Request body</span></span>
<span data-ttu-id="e9a1f-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9a1f-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e9a1f-130">Parameter</span></span>      | <span data-ttu-id="e9a1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9a1f-131">Type</span></span>    | <span data-ttu-id="e9a1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9a1f-132">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="e9a1f-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="e9a1f-133">clientContext</span></span>  | <span data-ttu-id="e9a1f-134">String</span><span class="sxs-lookup"><span data-stu-id="e9a1f-134">String</span></span>  | <span data-ttu-id="e9a1f-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="e9a1f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a1f-136">Response</span></span>
<span data-ttu-id="e9a1f-137">Se tiver êxito, este método retornará `200 OK` um código de resposta http e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-137">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="e9a1f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9a1f-138">Example</span></span>
<span data-ttu-id="e9a1f-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e9a1f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a1f-140">Request</span></span>
<span data-ttu-id="e9a1f-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e9a1f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a1f-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9a1f-143">C#</span><span class="sxs-lookup"><span data-stu-id="e9a1f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9a1f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9a1f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9a1f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9a1f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e9a1f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a1f-146">Response</span></span>

> <span data-ttu-id="e9a1f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9a1f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="e9a1f-149">Notificação-operação cancelada para recordResponse</span><span class="sxs-lookup"><span data-stu-id="e9a1f-149">Notification - Operation canceled for recordResponse</span></span>

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
