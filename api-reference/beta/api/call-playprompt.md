---
title: 'Call: playPrompt'
description: Reproduza um prompt na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2c62afeac5870d288c546aa3761b60a270d85219
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868265"
---
# <a name="call-playprompt"></a><span data-ttu-id="6cc26-103">Call: playPrompt</span><span class="sxs-lookup"><span data-stu-id="6cc26-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cc26-104">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="6cc26-104">Play a prompt in the call.</span></span>

<span data-ttu-id="6cc26-105">Para obter mais informações sobre como lidar com as operações, consulte [commsOperation](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6cc26-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="6cc26-106">A ação **playPrompt** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="6cc26-106">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cc26-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cc26-107">Permissions</span></span>
<span data-ttu-id="6cc26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cc26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cc26-110">Permission type</span></span>                        | <span data-ttu-id="6cc26-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cc26-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6cc26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cc26-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cc26-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc26-113">Not Supported.</span></span>                               |
| <span data-ttu-id="6cc26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cc26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cc26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc26-115">Not Supported.</span></span>                               |
| <span data-ttu-id="6cc26-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc26-116">Application</span></span>                            | <span data-ttu-id="6cc26-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6cc26-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="6cc26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc26-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /communications/calls/{id}/playPrompt
```
> <span data-ttu-id="6cc26-119">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="6cc26-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6cc26-120">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="6cc26-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cc26-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc26-121">Request headers</span></span>
| <span data-ttu-id="6cc26-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6cc26-122">Name</span></span>          | <span data-ttu-id="6cc26-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc26-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6cc26-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cc26-124">Authorization</span></span> | <span data-ttu-id="6cc26-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cc26-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cc26-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc26-127">Request body</span></span>
<span data-ttu-id="6cc26-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cc26-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cc26-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6cc26-129">Parameter</span></span>      | <span data-ttu-id="6cc26-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cc26-130">Type</span></span>    |<span data-ttu-id="6cc26-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc26-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cc26-132">prompts</span><span class="sxs-lookup"><span data-stu-id="6cc26-132">prompts</span></span>|<span data-ttu-id="6cc26-133">Coleção [MediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="6cc26-133">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="6cc26-134">Os prompts a serem reproduzidos.</span><span class="sxs-lookup"><span data-stu-id="6cc26-134">The prompts to be played.</span></span> <span data-ttu-id="6cc26-135">O tamanho máximo de coleção mediaPrompt compatível é 20.</span><span class="sxs-lookup"><span data-stu-id="6cc26-135">The maximum supported mediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="6cc26-136">ciclo</span><span class="sxs-lookup"><span data-stu-id="6cc26-136">loop</span></span>|<span data-ttu-id="6cc26-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cc26-137">Boolean</span></span>| <span data-ttu-id="6cc26-138">O valor do loop.</span><span class="sxs-lookup"><span data-stu-id="6cc26-138">The loop value.</span></span> <span data-ttu-id="6cc26-139">True indica o loop infinitamente.</span><span class="sxs-lookup"><span data-stu-id="6cc26-139">True indicates to loop infinitely.</span></span> <span data-ttu-id="6cc26-140">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="6cc26-140">The default value is false.</span></span> |
|<span data-ttu-id="6cc26-141">clientContext</span><span class="sxs-lookup"><span data-stu-id="6cc26-141">clientContext</span></span>|<span data-ttu-id="6cc26-142">String</span><span class="sxs-lookup"><span data-stu-id="6cc26-142">String</span></span>|<span data-ttu-id="6cc26-143">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="6cc26-143">Unique client context string.</span></span> <span data-ttu-id="6cc26-144">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6cc26-144">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="6cc26-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc26-145">Response</span></span>
<span data-ttu-id="6cc26-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [playPromptOperation](../resources/playpromptoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cc26-146">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc26-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cc26-147">Example</span></span>
<span data-ttu-id="6cc26-148">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6cc26-148">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6cc26-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc26-149">Request</span></span>
<span data-ttu-id="6cc26-150">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cc26-150">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6cc26-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc26-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cc26-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cc26-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6cc26-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc26-153">Response</span></span>
<span data-ttu-id="6cc26-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6cc26-154">The following is an example of the response.</span></span>

> <span data-ttu-id="6cc26-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cc26-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="6cc26-157">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="6cc26-157">Notification - operation completed</span></span>

 ><span data-ttu-id="6cc26-158">**Observação:** Se ocorrer um loop infinito, esta notificação não será enviada.</span><span class="sxs-lookup"><span data-stu-id="6cc26-158">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
