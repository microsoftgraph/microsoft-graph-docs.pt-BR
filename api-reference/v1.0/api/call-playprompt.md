---
title: 'Call: playPrompt'
description: Reproduza um prompt na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e6d41fd97ea52588d1d68c3439d39400acb95014
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913265"
---
# <a name="call-playprompt"></a><span data-ttu-id="e6e0f-103">Call: playPrompt</span><span class="sxs-lookup"><span data-stu-id="e6e0f-103">call: playPrompt</span></span>

<span data-ttu-id="e6e0f-104">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-104">Play a prompt in the call.</span></span>

<span data-ttu-id="e6e0f-105">Para obter mais informações sobre como lidar com as operações, consulte [commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e6e0f-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="e6e0f-106">A ação **playPrompt** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="e6e0f-106">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6e0f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6e0f-107">Permissions</span></span>
<span data-ttu-id="e6e0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6e0f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6e0f-110">Permission type</span></span>                        | <span data-ttu-id="e6e0f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6e0f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e6e0f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6e0f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6e0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-113">Not Supported.</span></span>                               |
| <span data-ttu-id="e6e0f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6e0f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6e0f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-115">Not Supported.</span></span>                               |
| <span data-ttu-id="e6e0f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6e0f-116">Application</span></span>                            | <span data-ttu-id="e6e0f-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e6e0f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6e0f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="e6e0f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6e0f-119">Request headers</span></span>
| <span data-ttu-id="e6e0f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6e0f-120">Name</span></span>          | <span data-ttu-id="e6e0f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6e0f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e6e0f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6e0f-122">Authorization</span></span> | <span data-ttu-id="e6e0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6e0f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6e0f-125">Request body</span></span>
<span data-ttu-id="e6e0f-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6e0f-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6e0f-127">Parameter</span></span>      | <span data-ttu-id="e6e0f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6e0f-128">Type</span></span>    |<span data-ttu-id="e6e0f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6e0f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6e0f-130">prompts</span><span class="sxs-lookup"><span data-stu-id="e6e0f-130">prompts</span></span>|<span data-ttu-id="e6e0f-131">Coleção [MediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="e6e0f-131">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="e6e0f-132">Os prompts a serem reproduzidos.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-132">The prompts to be played.</span></span> <span data-ttu-id="e6e0f-133">O tamanho máximo de coleção MediaPrompt compatível é 20.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-133">The maximum supported MediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="e6e0f-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="e6e0f-134">clientContext</span></span>|<span data-ttu-id="e6e0f-135">String</span><span class="sxs-lookup"><span data-stu-id="e6e0f-135">String</span></span>|<span data-ttu-id="e6e0f-136">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-136">Unique client context string.</span></span> <span data-ttu-id="e6e0f-137">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-137">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="e6e0f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6e0f-138">Response</span></span>
<span data-ttu-id="e6e0f-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [playPromptOperation](../resources/playpromptoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-139">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6e0f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6e0f-140">Example</span></span>
<span data-ttu-id="e6e0f-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-141">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e6e0f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6e0f-142">Request</span></span>
<span data-ttu-id="e6e0f-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-143">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e6e0f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6e0f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "#microsoft.graph.mediaInfo",
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6e0f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6e0f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6e0f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6e0f-146">Response</span></span>
<span data-ttu-id="e6e0f-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-147">The following is an example of the response.</span></span>

> <span data-ttu-id="e6e0f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6e0f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="e6e0f-150">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="e6e0f-150">Notification - operation completed</span></span>
 
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
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 200,
          "subcode": 0,
          "message": "Action completed successfully."
        },
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
