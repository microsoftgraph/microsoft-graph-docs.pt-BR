---
title: 'Call: playPrompt'
description: Reproduza um prompt na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 527797215da0ef961c83679fcec313c183a1cd63
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682173"
---
# <a name="call-playprompt"></a><span data-ttu-id="7b288-103">Call: playPrompt</span><span class="sxs-lookup"><span data-stu-id="7b288-103">call: playPrompt</span></span>

<span data-ttu-id="7b288-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b288-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b288-105">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="7b288-105">Play a prompt in the call.</span></span>

<span data-ttu-id="7b288-106">Para obter mais informações sobre como lidar com as operações, consulte [commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="7b288-106">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="7b288-107">A ação **playPrompt** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="7b288-107">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b288-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b288-108">Permissions</span></span>
<span data-ttu-id="7b288-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b288-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b288-111">Permission type</span></span>                        | <span data-ttu-id="7b288-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b288-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b288-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b288-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b288-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b288-114">Not Supported.</span></span>                               |
| <span data-ttu-id="7b288-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b288-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b288-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b288-116">Not Supported.</span></span>                               |
| <span data-ttu-id="7b288-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b288-117">Application</span></span>                            | <span data-ttu-id="7b288-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b288-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="7b288-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b288-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="7b288-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b288-120">Request headers</span></span>
| <span data-ttu-id="7b288-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7b288-121">Name</span></span>          | <span data-ttu-id="7b288-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b288-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7b288-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b288-123">Authorization</span></span> | <span data-ttu-id="7b288-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b288-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b288-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b288-126">Request body</span></span>
<span data-ttu-id="7b288-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b288-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b288-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7b288-128">Parameter</span></span>      | <span data-ttu-id="7b288-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b288-129">Type</span></span>    |<span data-ttu-id="7b288-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b288-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b288-131">prompts</span><span class="sxs-lookup"><span data-stu-id="7b288-131">prompts</span></span>|<span data-ttu-id="7b288-132">Coleção [MediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="7b288-132">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="7b288-133">Os prompts a serem reproduzidos.</span><span class="sxs-lookup"><span data-stu-id="7b288-133">The prompts to be played.</span></span> <span data-ttu-id="7b288-134">O tamanho máximo de coleção MediaPrompt compatível é 20.</span><span class="sxs-lookup"><span data-stu-id="7b288-134">The maximum supported MediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="7b288-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="7b288-135">clientContext</span></span>|<span data-ttu-id="7b288-136">String</span><span class="sxs-lookup"><span data-stu-id="7b288-136">String</span></span>|<span data-ttu-id="7b288-137">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="7b288-137">Unique client context string.</span></span> <span data-ttu-id="7b288-138">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7b288-138">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="7b288-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b288-139">Response</span></span>
<span data-ttu-id="7b288-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [playPromptOperation](../resources/playpromptoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b288-140">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b288-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b288-141">Example</span></span>
<span data-ttu-id="7b288-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7b288-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7b288-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b288-143">Request</span></span>
<span data-ttu-id="7b288-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b288-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b288-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b288-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="7b288-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b288-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7b288-147">C#</span><span class="sxs-lookup"><span data-stu-id="7b288-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-playprompt-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b288-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b288-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-playprompt-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b288-149">Java</span><span class="sxs-lookup"><span data-stu-id="7b288-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-playprompt-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7b288-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b288-150">Response</span></span>
<span data-ttu-id="7b288-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b288-151">The following is an example of the response.</span></span>

> <span data-ttu-id="7b288-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b288-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="7b288-154">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="7b288-154">Notification - operation completed</span></span>
 
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
