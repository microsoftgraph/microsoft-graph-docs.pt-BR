---
title: 'Call: Record'
description: Grave um clipe de áudio curto da chamada. Isso será útil se o bot quiser capturar uma resposta de voz do chamador seguindo um prompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2961bacfa9092aa580801e42e44aa1d2adbfaa97
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636698"
---
# <a name="call-record"></a><span data-ttu-id="eac1e-104">Call: Record</span><span class="sxs-lookup"><span data-stu-id="eac1e-104">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eac1e-105">Gravar um clipe de áudio curto de uma chamada.</span><span class="sxs-lookup"><span data-stu-id="eac1e-105">Record a short audio clip from a call.</span></span>
<span data-ttu-id="eac1e-106">Um bot pode usá-la para capturar uma resposta de voz de um chamador depois de ser solicitada uma resposta.</span><span class="sxs-lookup"><span data-stu-id="eac1e-106">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="eac1e-107">Para obter mais informações sobre como lidar com operações, confira [commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="eac1e-107">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="eac1e-108">**Observação:** Isso só é suportado para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="eac1e-108">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="eac1e-109">Esta ação não deve ser registrada em toda a chamada.</span><span class="sxs-lookup"><span data-stu-id="eac1e-109">This action is not intended to record the entire call.</span></span> <span data-ttu-id="eac1e-110">O tamanho máximo da gravação é de 5 minutos.</span><span class="sxs-lookup"><span data-stu-id="eac1e-110">The maximum length of recording is 5 minutes.</span></span> <span data-ttu-id="eac1e-111">A gravação não é salva permanentemente pela plataforma de comunicação na nuvem e é descartada logo após o término da chamada.</span><span class="sxs-lookup"><span data-stu-id="eac1e-111">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="eac1e-112">O bot deve baixar a gravação imediatamente após a conclusão da operação de gravação usando o valor recordingLocation fornecido na notificação de conclusão.</span><span class="sxs-lookup"><span data-stu-id="eac1e-112">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="eac1e-113">**Observação:** Qualquer mídia coletada pode **não** ser persistente.</span><span class="sxs-lookup"><span data-stu-id="eac1e-113">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="eac1e-114">Certifique-se de que você está em conformidade com as leis e regulamentos da sua área quando se trata de gravação de chamada.</span><span class="sxs-lookup"><span data-stu-id="eac1e-114">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="eac1e-115">Consulte um advogado legal para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="eac1e-115">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="eac1e-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="eac1e-116">Permissions</span></span>
<span data-ttu-id="eac1e-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac1e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eac1e-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eac1e-119">Permission type</span></span> | <span data-ttu-id="eac1e-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eac1e-120">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="eac1e-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eac1e-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="eac1e-122">Não suportado</span><span class="sxs-lookup"><span data-stu-id="eac1e-122">Not Supported</span></span>        |
| <span data-ttu-id="eac1e-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eac1e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eac1e-124">Não suportado</span><span class="sxs-lookup"><span data-stu-id="eac1e-124">Not Supported</span></span>        |
| <span data-ttu-id="eac1e-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eac1e-125">Application</span></span>     | <span data-ttu-id="eac1e-126">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="eac1e-126">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="eac1e-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eac1e-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /communications/calls/{id}/record
```
> <span data-ttu-id="eac1e-128">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="eac1e-128">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="eac1e-129">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="eac1e-129">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eac1e-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eac1e-130">Request headers</span></span>
| <span data-ttu-id="eac1e-131">Nome</span><span class="sxs-lookup"><span data-stu-id="eac1e-131">Name</span></span>          | <span data-ttu-id="eac1e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac1e-132">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="eac1e-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="eac1e-133">Authorization</span></span> | <span data-ttu-id="eac1e-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac1e-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eac1e-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eac1e-136">Request body</span></span>
<span data-ttu-id="eac1e-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac1e-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eac1e-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eac1e-138">Parameter</span></span>      | <span data-ttu-id="eac1e-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac1e-139">Type</span></span>    |<span data-ttu-id="eac1e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac1e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eac1e-141">prompts</span><span class="sxs-lookup"><span data-stu-id="eac1e-141">prompts</span></span>|<span data-ttu-id="eac1e-142">coleção [mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="eac1e-142">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="eac1e-143">Coleção de prompts a serem executados (se houver) antes da gravação começar.</span><span class="sxs-lookup"><span data-stu-id="eac1e-143">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="eac1e-144">Os clientes podem optar por especificar a ação "playPrompt" separadamente ou especificar como parte de "Record"-principalmente todos os registros são precedidos por um prompt.</span><span class="sxs-lookup"><span data-stu-id="eac1e-144">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="eac1e-145">O suporte atual é apenas para um único prompt como parte do conjunto.</span><span class="sxs-lookup"><span data-stu-id="eac1e-145">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="eac1e-146">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="eac1e-146">bargeInAllowed</span></span>|<span data-ttu-id="eac1e-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="eac1e-147">Boolean</span></span>| <span data-ttu-id="eac1e-148">Se for true, essa solicitação de registro será Barge em outras solicitações de registro/playprompt da fila existente/no momento.</span><span class="sxs-lookup"><span data-stu-id="eac1e-148">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="eac1e-149">Padrão = false.</span><span class="sxs-lookup"><span data-stu-id="eac1e-149">Default = false.</span></span> |
|<span data-ttu-id="eac1e-150">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="eac1e-150">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="eac1e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="eac1e-151">Int32</span></span>| <span data-ttu-id="eac1e-152">Silêncio inicial máximo (silêncio do usuário) permitido a partir da hora em que começamos a operação de registro antes do tempo limite e falha na operação.</span><span class="sxs-lookup"><span data-stu-id="eac1e-152">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="eac1e-153">Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt.</span><span class="sxs-lookup"><span data-stu-id="eac1e-153">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="eac1e-154">Padrão = 5 segundos, mín = 1 segundo, máx. = 300 segundos</span><span class="sxs-lookup"><span data-stu-id="eac1e-154">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="eac1e-155">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="eac1e-155">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="eac1e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="eac1e-156">Int32</span></span>| <span data-ttu-id="eac1e-157">Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar.</span><span class="sxs-lookup"><span data-stu-id="eac1e-157">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="eac1e-158">Padrão = 5 segundos, mín = 1 segundo, máximo = 300 segundos.</span><span class="sxs-lookup"><span data-stu-id="eac1e-158">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="eac1e-159">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="eac1e-159">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="eac1e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="eac1e-160">Int32</span></span>| <span data-ttu-id="eac1e-161">Duração máxima de uma operação de registro antes de parar a gravação.</span><span class="sxs-lookup"><span data-stu-id="eac1e-161">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="eac1e-162">Padrão = 5 segundos, mín = 1 segundo, máximo = 300 segundos.</span><span class="sxs-lookup"><span data-stu-id="eac1e-162">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="eac1e-163">playBeep</span><span class="sxs-lookup"><span data-stu-id="eac1e-163">playBeep</span></span>|<span data-ttu-id="eac1e-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="eac1e-164">Boolean</span></span>| <span data-ttu-id="eac1e-165">Se true, reproduz um aviso sonoro para indicar ao usuário que eles podem começar a gravar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="eac1e-165">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="eac1e-166">Padrão = true.</span><span class="sxs-lookup"><span data-stu-id="eac1e-166">Default = true.</span></span>|
|<span data-ttu-id="eac1e-167">stopTones</span><span class="sxs-lookup"><span data-stu-id="eac1e-167">stopTones</span></span>|<span data-ttu-id="eac1e-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eac1e-168">String collection</span></span>|<span data-ttu-id="eac1e-169">Pare os toques especificados para terminar a gravação.</span><span class="sxs-lookup"><span data-stu-id="eac1e-169">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="eac1e-170">clientContext</span><span class="sxs-lookup"><span data-stu-id="eac1e-170">clientContext</span></span>|<span data-ttu-id="eac1e-171">String</span><span class="sxs-lookup"><span data-stu-id="eac1e-171">String</span></span>|<span data-ttu-id="eac1e-172">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="eac1e-172">Unique Client Context string.</span></span> <span data-ttu-id="eac1e-173">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="eac1e-173">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="eac1e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac1e-174">Response</span></span>
<span data-ttu-id="eac1e-175">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac1e-175">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="eac1e-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eac1e-176">Example</span></span>
<span data-ttu-id="eac1e-177">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="eac1e-177">The following example shows how to call this API.</span></span>

### <a name="example-1-record-a-short-audio-clip-from-a-call"></a><span data-ttu-id="eac1e-178">Exemplo 1: gravar um clipe de áudio curto de uma chamada</span><span class="sxs-lookup"><span data-stu-id="eac1e-178">Example 1: Record a short audio clip from a call</span></span>

##### <a name="request"></a><span data-ttu-id="eac1e-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac1e-179">Request</span></span>
<span data-ttu-id="eac1e-180">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac1e-180">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eac1e-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="eac1e-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/record
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
      }
    }
  ],
  "maxRecordDurationInSeconds": 10,
  "initialSilenceTimeoutInSeconds": 5,
  "maxSilenceTimeoutInSeconds": 2,
  "playBeep": true,
  "stopTones": [ "#", "1", "*" ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eac1e-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eac1e-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eac1e-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac1e-183">Response</span></span>
<span data-ttu-id="eac1e-184">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="eac1e-184">The following example shows the response.</span></span>

> <span data-ttu-id="eac1e-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eac1e-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="eac1e-187">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="eac1e-187">Notification - operation completed</span></span>

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
        "status": "completed",
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="eac1e-188">Exemplo 2: Recuperando o arquivo de gravação</span><span class="sxs-lookup"><span data-stu-id="eac1e-188">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="eac1e-189">**Observação:** Embora você possa buscar a gravação e processá-la, você **deve** excluí-la posteriormente.</span><span class="sxs-lookup"><span data-stu-id="eac1e-189">**Note:** While you're able to fetch the recording and process it, you **must** delete it afterwards.</span></span> <span data-ttu-id="eac1e-190">Não é possível persistir a mídia.</span><span class="sxs-lookup"><span data-stu-id="eac1e-190">Media cannot be persisted.</span></span>

##### <a name="request"></a><span data-ttu-id="eac1e-191">Solicitar</span><span class="sxs-lookup"><span data-stu-id="eac1e-191">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="eac1e-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac1e-192">Response</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Transfer-Encoding: chunked
Date: Thu, 17 Jan 2019 01:46:37 GMT
Content-Type: application/octet-stream

(application/octet-stream of size 160696 bytes)
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
  ]
}
-->
