---
title: 'call: playPrompt'
description: Reproduza um prompt na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ce89f0bbdaf665bb9f459f554a2e605324ead609
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051603"
---
# <a name="call-playprompt"></a><span data-ttu-id="683fa-103">call: playPrompt</span><span class="sxs-lookup"><span data-stu-id="683fa-103">call: playPrompt</span></span>

<span data-ttu-id="683fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="683fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="683fa-105">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="683fa-105">Play a prompt in the call.</span></span>

<span data-ttu-id="683fa-106">Para obter mais informações sobre como lidar com operações, consulte [commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="683fa-106">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="683fa-107">A **ação playPrompt** só tem suporte para [chamadas](../resources/call.md) iniciadas com [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="683fa-107">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="683fa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="683fa-108">Permissions</span></span>
<span data-ttu-id="683fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="683fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="683fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="683fa-111">Permission type</span></span>                        | <span data-ttu-id="683fa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="683fa-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="683fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="683fa-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="683fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="683fa-114">Not Supported.</span></span>                               |
| <span data-ttu-id="683fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="683fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="683fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="683fa-116">Not Supported.</span></span>                               |
| <span data-ttu-id="683fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="683fa-117">Application</span></span>                            | <span data-ttu-id="683fa-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="683fa-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="683fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="683fa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="683fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="683fa-120">Request headers</span></span>
| <span data-ttu-id="683fa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="683fa-121">Name</span></span>          | <span data-ttu-id="683fa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="683fa-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="683fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="683fa-123">Authorization</span></span> | <span data-ttu-id="683fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="683fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="683fa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="683fa-126">Request body</span></span>
<span data-ttu-id="683fa-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="683fa-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="683fa-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="683fa-128">Parameter</span></span>      | <span data-ttu-id="683fa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="683fa-129">Type</span></span>    |<span data-ttu-id="683fa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="683fa-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="683fa-131">prompts</span><span class="sxs-lookup"><span data-stu-id="683fa-131">prompts</span></span>|<span data-ttu-id="683fa-132">[Coleção MediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="683fa-132">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="683fa-133">Os prompts a serem tocados.</span><span class="sxs-lookup"><span data-stu-id="683fa-133">The prompts to be played.</span></span> <span data-ttu-id="683fa-134">O tamanho máximo da coleção MediaPrompt suportado é 20.</span><span class="sxs-lookup"><span data-stu-id="683fa-134">The maximum supported MediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="683fa-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="683fa-135">clientContext</span></span>|<span data-ttu-id="683fa-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="683fa-136">String</span></span>|<span data-ttu-id="683fa-137">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="683fa-137">Unique client context string.</span></span> <span data-ttu-id="683fa-138">Pode ter no máximo 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="683fa-138">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="683fa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="683fa-139">Response</span></span>
<span data-ttu-id="683fa-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto playPromptOperation](../resources/playpromptoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="683fa-140">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="683fa-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="683fa-141">Example</span></span>
<span data-ttu-id="683fa-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="683fa-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="683fa-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="683fa-143">Request</span></span>
<span data-ttu-id="683fa-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="683fa-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="683fa-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="683fa-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="683fa-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="683fa-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="683fa-147">C#</span><span class="sxs-lookup"><span data-stu-id="683fa-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-playprompt-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="683fa-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="683fa-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-playprompt-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="683fa-149">Java</span><span class="sxs-lookup"><span data-stu-id="683fa-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-playprompt-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="683fa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="683fa-150">Response</span></span>
<span data-ttu-id="683fa-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="683fa-151">The following is an example of the response.</span></span>

> <span data-ttu-id="683fa-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="683fa-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="683fa-153">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="683fa-153">Notification - operation completed</span></span>
 
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

