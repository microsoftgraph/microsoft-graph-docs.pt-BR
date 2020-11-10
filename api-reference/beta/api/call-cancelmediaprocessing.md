---
title: 'Call: cancelMediaProcessing'
description: Cancela o processamento de mídia para qualquer operação playPrompt ou recordResponse em andamento.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 695b7e235e4337c2d7550668bd6be4996efe335f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959820"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="d81d0-103">Call: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="d81d0-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="d81d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d81d0-105">Cancela o processamento de todas as operações de mídia em andamento.</span><span class="sxs-lookup"><span data-stu-id="d81d0-105">Cancels processing for any in-progress media operations.</span></span>

<span data-ttu-id="d81d0-106">Operações de mídia consulte as operações IVR [playPrompt](./call-playprompt.md) e [recordResponse](./call-record.md), que são, por padrão, enfileiradas para processar na ordem.</span><span class="sxs-lookup"><span data-stu-id="d81d0-106">Media operations refer to the IVR operations [playPrompt](./call-playprompt.md) and [recordResponse](./call-record.md), which are by default queued to process in order.</span></span> <span data-ttu-id="d81d0-107">O método **cancelMediaProcessing** cancela qualquer operação em processo, bem como operações que são enfileiradas.</span><span class="sxs-lookup"><span data-stu-id="d81d0-107">The **cancelMediaProcessing** method cancels any operation that is in-process as well as operations that are queued.</span></span> <span data-ttu-id="d81d0-108">Por exemplo, essa API pode ser usada para limpar a fila de operação IVR para uma nova operação de mídia.</span><span class="sxs-lookup"><span data-stu-id="d81d0-108">For example, this API can be used to clean up the IVR operation queue for a new media operation.</span></span> <span data-ttu-id="d81d0-109">No entanto, ele não cancelará uma operação do **ubscribeToTone** , pois ele funciona independentemente de qualquer fila de operação.</span><span class="sxs-lookup"><span data-stu-id="d81d0-109">However, it will not cancel a **ubscribeToTone** operation because it operates independent of any operation queue.</span></span>

## <a name="permissions"></a><span data-ttu-id="d81d0-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d81d0-110">Permissions</span></span>
<span data-ttu-id="d81d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d81d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d81d0-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d81d0-113">Permission type</span></span>                        | <span data-ttu-id="d81d0-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d81d0-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d81d0-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d81d0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d81d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81d0-116">Not Supported.</span></span>                              |
| <span data-ttu-id="d81d0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d81d0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81d0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81d0-118">Not Supported.</span></span>                              |
| <span data-ttu-id="d81d0-119">Application</span><span class="sxs-lookup"><span data-stu-id="d81d0-119">Application</span></span>                            | <span data-ttu-id="d81d0-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d81d0-120">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="d81d0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d81d0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="d81d0-122">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="d81d0-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d81d0-123">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d81d0-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d81d0-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d81d0-124">Request headers</span></span>
| <span data-ttu-id="d81d0-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d81d0-125">Name</span></span>          | <span data-ttu-id="d81d0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81d0-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d81d0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d81d0-127">Authorization</span></span> | <span data-ttu-id="d81d0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81d0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d81d0-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="d81d0-130">Content-type</span></span> | <span data-ttu-id="d81d0-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81d0-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d81d0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d81d0-133">Request body</span></span>
<span data-ttu-id="d81d0-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81d0-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d81d0-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d81d0-135">Parameter</span></span>      | <span data-ttu-id="d81d0-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d81d0-136">Type</span></span>    | <span data-ttu-id="d81d0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81d0-137">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="d81d0-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="d81d0-138">clientContext</span></span>  | <span data-ttu-id="d81d0-139">String</span><span class="sxs-lookup"><span data-stu-id="d81d0-139">String</span></span>  | <span data-ttu-id="d81d0-140">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="d81d0-140">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="d81d0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81d0-141">Response</span></span>
<span data-ttu-id="d81d0-142">Se tiver êxito, este método retornará um `200 OK` código de resposta http e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81d0-142">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="d81d0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d81d0-143">Example</span></span>
<span data-ttu-id="d81d0-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d81d0-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d81d0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81d0-145">Request</span></span>
<span data-ttu-id="d81d0-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81d0-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d81d0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81d0-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d81d0-148">C#</span><span class="sxs-lookup"><span data-stu-id="d81d0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81d0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81d0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81d0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81d0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81d0-151">Java</span><span class="sxs-lookup"><span data-stu-id="d81d0-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-cancelmediaprocessing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d81d0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81d0-152">Response</span></span>

> <span data-ttu-id="d81d0-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d81d0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="d81d0-155">Notificação-operação cancelada para recordResponse</span><span class="sxs-lookup"><span data-stu-id="d81d0-155">Notification - Operation canceled for recordResponse</span></span>

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
          "message": "Action failed, the operation was cancelled."
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


