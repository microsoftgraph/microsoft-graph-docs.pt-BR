---
title: 'Call: Record'
description: Registre a chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc1a98374c34986e2a4430f5b50c5a2801dcd0e8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328277"
---
# <a name="call-record"></a><span data-ttu-id="15fc1-103">Call: Record</span><span class="sxs-lookup"><span data-stu-id="15fc1-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15fc1-104">Registre a chamada.</span><span class="sxs-lookup"><span data-stu-id="15fc1-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="15fc1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="15fc1-105">Permissions</span></span>
<span data-ttu-id="15fc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15fc1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15fc1-108">Permission type</span></span> | <span data-ttu-id="15fc1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15fc1-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="15fc1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15fc1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="15fc1-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="15fc1-111">Not Supported</span></span>        |
| <span data-ttu-id="15fc1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15fc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15fc1-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="15fc1-113">Not Supported</span></span>        |
| <span data-ttu-id="15fc1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15fc1-114">Application</span></span>     | <span data-ttu-id="15fc1-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="15fc1-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="15fc1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15fc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="15fc1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15fc1-117">Request headers</span></span>
| <span data-ttu-id="15fc1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="15fc1-118">Name</span></span>          | <span data-ttu-id="15fc1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="15fc1-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="15fc1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="15fc1-120">Authorization</span></span> | <span data-ttu-id="15fc1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15fc1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15fc1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15fc1-123">Request body</span></span>
<span data-ttu-id="15fc1-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15fc1-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="15fc1-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="15fc1-125">Parameter</span></span>      | <span data-ttu-id="15fc1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="15fc1-126">Type</span></span>    |<span data-ttu-id="15fc1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="15fc1-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15fc1-128">prompts</span><span class="sxs-lookup"><span data-stu-id="15fc1-128">prompts</span></span>|<span data-ttu-id="15fc1-129">coleção [mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="15fc1-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="15fc1-130">Coleção de prompts a serem executados (se houver) antes da gravação começar.</span><span class="sxs-lookup"><span data-stu-id="15fc1-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="15fc1-131">Os clientes podem optar por especificar a ação "playPrompt" separadamente ou especificar como parte de "Record"-principalmente todos os registros são precedidos por um prompt</span><span class="sxs-lookup"><span data-stu-id="15fc1-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="15fc1-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="15fc1-132">bargeInAllowed</span></span>|<span data-ttu-id="15fc1-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fc1-133">Boolean</span></span>| <span data-ttu-id="15fc1-134">Permite que os usuários insiram opções antes de concluir o prompt.</span><span class="sxs-lookup"><span data-stu-id="15fc1-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="15fc1-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="15fc1-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="15fc1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="15fc1-136">Int32</span></span>| <span data-ttu-id="15fc1-137">O silêncio inicial máximo permitido a partir da hora em que começamos a operação de registro antes do tempo limite e falha na operação.</span><span class="sxs-lookup"><span data-stu-id="15fc1-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="15fc1-138">Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt.</span><span class="sxs-lookup"><span data-stu-id="15fc1-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="15fc1-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="15fc1-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="15fc1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="15fc1-140">Int32</span></span>| <span data-ttu-id="15fc1-141">O tempo limite de silêncio máximo em segundos.</span><span class="sxs-lookup"><span data-stu-id="15fc1-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="15fc1-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="15fc1-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="15fc1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="15fc1-143">Int32</span></span>| <span data-ttu-id="15fc1-144">A duração máxima do registro em segundos.</span><span class="sxs-lookup"><span data-stu-id="15fc1-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="15fc1-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="15fc1-145">playBeep</span></span>|<span data-ttu-id="15fc1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fc1-146">Boolean</span></span>| <span data-ttu-id="15fc1-147">ReProduz um aviso sonoro após a execução do prompt.</span><span class="sxs-lookup"><span data-stu-id="15fc1-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="15fc1-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="15fc1-148">streamWhileRecording</span></span>|<span data-ttu-id="15fc1-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fc1-149">Boolean</span></span>|<span data-ttu-id="15fc1-150">Se for definido como true, um local de recurso será fornecido assim que a gravação for iniciada.</span><span class="sxs-lookup"><span data-stu-id="15fc1-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="15fc1-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="15fc1-151">stopTones</span></span>|<span data-ttu-id="15fc1-152">Coleção String</span><span class="sxs-lookup"><span data-stu-id="15fc1-152">String collection</span></span>|<span data-ttu-id="15fc1-153">Pare os toques especificados para terminar a gravação.</span><span class="sxs-lookup"><span data-stu-id="15fc1-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="15fc1-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="15fc1-154">clientContext</span></span>|<span data-ttu-id="15fc1-155">String</span><span class="sxs-lookup"><span data-stu-id="15fc1-155">String</span></span>|<span data-ttu-id="15fc1-156">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="15fc1-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="15fc1-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="15fc1-157">Response</span></span>
<span data-ttu-id="15fc1-158">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="15fc1-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="15fc1-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15fc1-159">Example</span></span>
<span data-ttu-id="15fc1-160">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="15fc1-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="15fc1-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15fc1-161">Request</span></span>
<span data-ttu-id="15fc1-162">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="15fc1-162">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="15fc1-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="15fc1-163">Response</span></span>

> <span data-ttu-id="15fc1-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15fc1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="15fc1-166">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="15fc1-166">Notification - operation completed</span></span>

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
  "suppressions": []
}
-->
