---
title: 'Call: playPrompt'
description: Reproduza um prompt na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4712af56948b880cabbc51c1b6a0e61dc20827b7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317652"
---
# <a name="call-playprompt"></a><span data-ttu-id="98a00-103">Call: playPrompt</span><span class="sxs-lookup"><span data-stu-id="98a00-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98a00-104">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="98a00-104">Play a prompt in the call.</span></span>

<span data-ttu-id="98a00-105">Para obter mais informações sobre como lidar com as operações, consulte [commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="98a00-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="98a00-106">A ação **playPrompt** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="98a00-106">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="98a00-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="98a00-107">Permissions</span></span>
<span data-ttu-id="98a00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98a00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98a00-110">Permission type</span></span>                        | <span data-ttu-id="98a00-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98a00-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98a00-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98a00-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="98a00-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98a00-113">Not Supported.</span></span>                               |
| <span data-ttu-id="98a00-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98a00-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98a00-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98a00-115">Not Supported.</span></span>                               |
| <span data-ttu-id="98a00-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98a00-116">Application</span></span>                            | <span data-ttu-id="98a00-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="98a00-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="98a00-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98a00-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="98a00-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98a00-119">Request headers</span></span>
| <span data-ttu-id="98a00-120">Nome</span><span class="sxs-lookup"><span data-stu-id="98a00-120">Name</span></span>          | <span data-ttu-id="98a00-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="98a00-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="98a00-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98a00-122">Authorization</span></span> | <span data-ttu-id="98a00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98a00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98a00-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98a00-125">Request body</span></span>
<span data-ttu-id="98a00-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98a00-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98a00-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="98a00-127">Parameter</span></span>      | <span data-ttu-id="98a00-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="98a00-128">Type</span></span>    |<span data-ttu-id="98a00-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="98a00-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98a00-130">prompts</span><span class="sxs-lookup"><span data-stu-id="98a00-130">prompts</span></span>|<span data-ttu-id="98a00-131">Coleção MediaPrompt</span><span class="sxs-lookup"><span data-stu-id="98a00-131">MediaPrompt collection</span></span>| <span data-ttu-id="98a00-132">Atualmente, apenas uma única solicitação e do tipo [MediaPrompt](../resources/mediaprompt.md) é suportada.</span><span class="sxs-lookup"><span data-stu-id="98a00-132">Currently only a single prompt and of type [MediaPrompt](../resources/mediaprompt.md) is supported.</span></span>|
|<span data-ttu-id="98a00-133">ciclo</span><span class="sxs-lookup"><span data-stu-id="98a00-133">loop</span></span>|<span data-ttu-id="98a00-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="98a00-134">Boolean</span></span>| <span data-ttu-id="98a00-135">O valor do loop.</span><span class="sxs-lookup"><span data-stu-id="98a00-135">The loop value.</span></span> <span data-ttu-id="98a00-136">True indica o loop infinitamente.</span><span class="sxs-lookup"><span data-stu-id="98a00-136">True indicates to loop infinitely.</span></span> <span data-ttu-id="98a00-137">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="98a00-137">The default value is false.</span></span> |
|<span data-ttu-id="98a00-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="98a00-138">clientContext</span></span>|<span data-ttu-id="98a00-139">String</span><span class="sxs-lookup"><span data-stu-id="98a00-139">String</span></span>|<span data-ttu-id="98a00-140">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="98a00-140">Unique client context string.</span></span> <span data-ttu-id="98a00-141">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="98a00-141">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="98a00-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="98a00-142">Response</span></span>
<span data-ttu-id="98a00-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [playPromptOperation](../resources/playpromptoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98a00-143">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98a00-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98a00-144">Example</span></span>
<span data-ttu-id="98a00-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="98a00-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="98a00-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98a00-146">Request</span></span>
<span data-ttu-id="98a00-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="98a00-147">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="98a00-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="98a00-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
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
      },
    },
  ],
  "loop": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98a00-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98a00-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98a00-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="98a00-150">Response</span></span>
<span data-ttu-id="98a00-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="98a00-151">The following is an example of the response.</span></span>

> <span data-ttu-id="98a00-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98a00-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="98a00-154">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="98a00-154">Notification - operation completed</span></span>

 ><span data-ttu-id="98a00-155">**Observação:** Se ocorrer um loop infinito, esta notificação não será enviada.</span><span class="sxs-lookup"><span data-stu-id="98a00-155">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.playPromptOperation",
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
