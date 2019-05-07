---
title: 'Call: Record'
description: Registre a chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4e864027297f9b96dd6ce3a1ecb08e59444c5cef
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635719"
---
# <a name="call-record"></a><span data-ttu-id="e0e85-103">Call: Record</span><span class="sxs-lookup"><span data-stu-id="e0e85-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e85-104">Registre a chamada.</span><span class="sxs-lookup"><span data-stu-id="e0e85-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e85-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0e85-105">Permissions</span></span>
<span data-ttu-id="e0e85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0e85-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0e85-108">Permission type</span></span> | <span data-ttu-id="e0e85-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0e85-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e0e85-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0e85-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0e85-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e0e85-111">Not Supported</span></span>        |
| <span data-ttu-id="e0e85-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0e85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0e85-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="e0e85-113">Not Supported</span></span>        |
| <span data-ttu-id="e0e85-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0e85-114">Application</span></span>     | <span data-ttu-id="e0e85-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="e0e85-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="e0e85-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e85-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="e0e85-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e85-117">Request headers</span></span>
| <span data-ttu-id="e0e85-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e0e85-118">Name</span></span>          | <span data-ttu-id="e0e85-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0e85-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e0e85-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0e85-120">Authorization</span></span> | <span data-ttu-id="e0e85-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0e85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0e85-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e85-123">Request body</span></span>
<span data-ttu-id="e0e85-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0e85-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0e85-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e0e85-125">Parameter</span></span>      | <span data-ttu-id="e0e85-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0e85-126">Type</span></span>    |<span data-ttu-id="e0e85-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0e85-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0e85-128">prompts</span><span class="sxs-lookup"><span data-stu-id="e0e85-128">prompts</span></span>|<span data-ttu-id="e0e85-129">coleção [mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="e0e85-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="e0e85-130">Coleção de prompts a serem executados (se houver) antes da gravação começar.</span><span class="sxs-lookup"><span data-stu-id="e0e85-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="e0e85-131">Os clientes podem optar por especificar a ação "playPrompt" separadamente ou especificar como parte de "Record"-principalmente todos os registros são precedidos por um prompt</span><span class="sxs-lookup"><span data-stu-id="e0e85-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="e0e85-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="e0e85-132">bargeInAllowed</span></span>|<span data-ttu-id="e0e85-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0e85-133">Boolean</span></span>| <span data-ttu-id="e0e85-134">Permite que os usuários insiram opções antes de concluir o prompt.</span><span class="sxs-lookup"><span data-stu-id="e0e85-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="e0e85-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="e0e85-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="e0e85-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e85-136">Int32</span></span>| <span data-ttu-id="e0e85-137">O silêncio inicial máximo permitido a partir da hora em que começamos a operação de registro antes do tempo limite e falha na operação.</span><span class="sxs-lookup"><span data-stu-id="e0e85-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="e0e85-138">Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt.</span><span class="sxs-lookup"><span data-stu-id="e0e85-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="e0e85-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="e0e85-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="e0e85-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e85-140">Int32</span></span>| <span data-ttu-id="e0e85-141">O tempo limite de silêncio máximo em segundos.</span><span class="sxs-lookup"><span data-stu-id="e0e85-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="e0e85-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="e0e85-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="e0e85-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e85-143">Int32</span></span>| <span data-ttu-id="e0e85-144">A duração máxima do registro em segundos.</span><span class="sxs-lookup"><span data-stu-id="e0e85-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="e0e85-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="e0e85-145">playBeep</span></span>|<span data-ttu-id="e0e85-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0e85-146">Boolean</span></span>| <span data-ttu-id="e0e85-147">Reproduz um aviso sonoro após a execução do prompt.</span><span class="sxs-lookup"><span data-stu-id="e0e85-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="e0e85-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="e0e85-148">streamWhileRecording</span></span>|<span data-ttu-id="e0e85-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0e85-149">Boolean</span></span>|<span data-ttu-id="e0e85-150">Se for definido como true, um local de recurso será fornecido assim que a gravação for iniciada.</span><span class="sxs-lookup"><span data-stu-id="e0e85-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="e0e85-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="e0e85-151">stopTones</span></span>|<span data-ttu-id="e0e85-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0e85-152">String collection</span></span>|<span data-ttu-id="e0e85-153">Pare os toques especificados para terminar a gravação.</span><span class="sxs-lookup"><span data-stu-id="e0e85-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="e0e85-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="e0e85-154">clientContext</span></span>|<span data-ttu-id="e0e85-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0e85-155">String</span></span>|<span data-ttu-id="e0e85-156">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="e0e85-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e0e85-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e85-157">Response</span></span>
<span data-ttu-id="e0e85-158">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0e85-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="e0e85-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0e85-159">Example</span></span>
<span data-ttu-id="e0e85-160">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e0e85-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e0e85-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e85-161">Request</span></span>
<span data-ttu-id="e0e85-162">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0e85-162">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/record
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ],
  "maxRecordDurationInSeconds": 1800,
  "initialSilenceTimeoutInSeconds": 10,
  "maxSilenceTimeoutInSeconds": 2,
  "recordingFormat": "wav",
  "playBeep": true,
  "streamWhileRecording": true,
  "stopTones": [ "#", "11", "*" ]
}
```

##### <a name="response"></a><span data-ttu-id="e0e85-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e85-163">Response</span></span>

> <span data-ttu-id="e0e85-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0e85-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0e85-166">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e0e85-166">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0e85-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e85-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-record-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="e0e85-168">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="e0e85-168">Notification - operation completed</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "recordResourceLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordResourceAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
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
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-record.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
