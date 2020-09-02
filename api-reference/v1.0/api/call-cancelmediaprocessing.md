---
title: 'Call: cancelMediaProcessing'
description: Cancela o processamento de mídia para qualquer operação playPrompt ou recordResponse em andamento.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ec3b50b78bb659b354ffd545ec0397909cb4511e
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319600"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="994eb-103">Call: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="994eb-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="994eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="994eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="994eb-105">Cancela o processamento de todas as operações de mídia em andamento.</span><span class="sxs-lookup"><span data-stu-id="994eb-105">Cancels processing for any in-progress media operations.</span></span>

<span data-ttu-id="994eb-106">Operações de mídia consulte as operações IVR [playPrompt](./call-playprompt.md) e [recordResponse](./call-record.md), que são, por padrão, enfileiradas para processar na ordem.</span><span class="sxs-lookup"><span data-stu-id="994eb-106">Media operations refer to the IVR operations [playPrompt](./call-playprompt.md) and [recordResponse](./call-record.md), which are by default queued to process in order.</span></span> <span data-ttu-id="994eb-107">O método **cancelMediaProcessing** cancela qualquer operação em processo, bem como operações que são enfileiradas.</span><span class="sxs-lookup"><span data-stu-id="994eb-107">The **cancelMediaProcessing** method cancels any operation that is in-process as well as operations that are queued.</span></span> <span data-ttu-id="994eb-108">Por exemplo, este método pode ser usado para limpar a fila de operação IVR para uma nova operação de mídia.</span><span class="sxs-lookup"><span data-stu-id="994eb-108">For example, this method can be used to clean up the IVR operation queue for a new media operation.</span></span> <span data-ttu-id="994eb-109">No entanto, ele não cancelará uma operação do **subscribeToTone** , pois ele funciona independentemente de qualquer fila de operação.</span><span class="sxs-lookup"><span data-stu-id="994eb-109">However, it will not cancel a **subscribeToTone** operation because it operates independent of any operation queue.</span></span>

## <a name="permissions"></a><span data-ttu-id="994eb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="994eb-110">Permissions</span></span>

<span data-ttu-id="994eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="994eb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="994eb-113">Permission type</span></span>                        | <span data-ttu-id="994eb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="994eb-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="994eb-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="994eb-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="994eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="994eb-116">Not Supported.</span></span>                              |
| <span data-ttu-id="994eb-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="994eb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994eb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="994eb-118">Not Supported.</span></span>                              |
| <span data-ttu-id="994eb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="994eb-119">Application</span></span>                            | <span data-ttu-id="994eb-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="994eb-120">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="994eb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="994eb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="994eb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="994eb-122">Request headers</span></span>

| <span data-ttu-id="994eb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="994eb-123">Name</span></span>          | <span data-ttu-id="994eb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="994eb-124">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="994eb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="994eb-125">Authorization</span></span> | <span data-ttu-id="994eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="994eb-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="994eb-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="994eb-128">Content-type</span></span>  | <span data-ttu-id="994eb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="994eb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="994eb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="994eb-131">Request body</span></span>

<span data-ttu-id="994eb-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="994eb-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="994eb-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="994eb-133">Parameter</span></span>     | <span data-ttu-id="994eb-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="994eb-134">Type</span></span>   | <span data-ttu-id="994eb-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="994eb-135">Description</span></span>         |
| :------------ | :----- | :------------------ |
| <span data-ttu-id="994eb-136">clientContext</span><span class="sxs-lookup"><span data-stu-id="994eb-136">clientContext</span></span> | <span data-ttu-id="994eb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994eb-137">String</span></span> | <span data-ttu-id="994eb-138">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="994eb-138">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="994eb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="994eb-139">Response</span></span>

<span data-ttu-id="994eb-140">Se tiver êxito, este método retornará um `200 OK` código de resposta http e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="994eb-140">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="994eb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="994eb-141">Example</span></span>

<span data-ttu-id="994eb-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="994eb-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="994eb-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="994eb-143">Request</span></span>

<span data-ttu-id="994eb-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="994eb-144">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "clientContext": "clientContext-value"
}
```

---

##### <a name="response"></a><span data-ttu-id="994eb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="994eb-145">Response</span></span>

> <span data-ttu-id="994eb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="994eb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
} -->

```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5"
}
```

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="994eb-148">Notificação-operação cancelada para recordResponse</span><span class="sxs-lookup"><span data-stu-id="994eb-148">Notification - Operation canceled for recordResponse</span></span>

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
