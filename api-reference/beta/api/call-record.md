---
title: 'Call: recordResponse'
description: Grave uma resposta de áudio curta do chamador. Isso será útil se o bot quiser capturar uma resposta de voz do chamador seguindo um prompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0e3aab1564d6007924d696a8d07a86c5cc4854b0
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912836"
---
# <a name="call-recordresponse"></a><span data-ttu-id="5a311-104">Call: recordResponse</span><span class="sxs-lookup"><span data-stu-id="5a311-104">call: recordResponse</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a311-105">Grave uma resposta de áudio curta do chamador.</span><span class="sxs-lookup"><span data-stu-id="5a311-105">Record a short audio response from the caller.</span></span>

<span data-ttu-id="5a311-106">Um bot pode usá-la para capturar uma resposta de voz de um chamador depois de ser solicitada uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5a311-106">A bot can use this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="5a311-107">Para obter mais informações sobre como lidar com as operações, consulte [commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="5a311-107">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="5a311-108">**Observação:** Essa API tem suporte apenas para [chamadas](../resources/call.md) iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="5a311-108">**Note:** This API is only supported for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="5a311-109">Esta ação não deve ser registrada em toda a chamada.</span><span class="sxs-lookup"><span data-stu-id="5a311-109">This action is not intended to record the entire call.</span></span> <span data-ttu-id="5a311-110">O tamanho máximo da gravação é de 2 minutos.</span><span class="sxs-lookup"><span data-stu-id="5a311-110">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="5a311-111">A gravação não é salva permanentemente pela plataforma de comunicação na nuvem e é descartada logo após o término da chamada.</span><span class="sxs-lookup"><span data-stu-id="5a311-111">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="5a311-112">O bot deve baixar a gravação imediatamente após a conclusão da operação de gravação usando o valor recordingLocation fornecido na notificação de conclusão.</span><span class="sxs-lookup"><span data-stu-id="5a311-112">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="5a311-113">**Observação:** Você não pode gravar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="5a311-113">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="5a311-114">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="5a311-114">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="5a311-115">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="5a311-115">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a311-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a311-116">Permissions</span></span>
<span data-ttu-id="5a311-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a311-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a311-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a311-119">Permission type</span></span> | <span data-ttu-id="5a311-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a311-120">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="5a311-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a311-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a311-122">Não suportado</span><span class="sxs-lookup"><span data-stu-id="5a311-122">Not Supported</span></span>        |
| <span data-ttu-id="5a311-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a311-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a311-124">Não suportado</span><span class="sxs-lookup"><span data-stu-id="5a311-124">Not Supported</span></span>        |
| <span data-ttu-id="5a311-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a311-125">Application</span></span>     | <span data-ttu-id="5a311-126">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="5a311-126">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="5a311-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a311-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> <span data-ttu-id="5a311-128">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="5a311-128">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="5a311-129">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="5a311-129">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a311-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a311-130">Request headers</span></span>
| <span data-ttu-id="5a311-131">Nome</span><span class="sxs-lookup"><span data-stu-id="5a311-131">Name</span></span>          | <span data-ttu-id="5a311-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a311-132">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5a311-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a311-133">Authorization</span></span> | <span data-ttu-id="5a311-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a311-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a311-136">Content-type</span><span class="sxs-lookup"><span data-stu-id="5a311-136">Content-type</span></span>| <span data-ttu-id="5a311-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a311-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a311-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a311-139">Request body</span></span>
<span data-ttu-id="5a311-140">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a311-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a311-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5a311-141">Parameter</span></span>      | <span data-ttu-id="5a311-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a311-142">Type</span></span>    |<span data-ttu-id="5a311-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a311-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a311-144">prompts</span><span class="sxs-lookup"><span data-stu-id="5a311-144">prompts</span></span>|<span data-ttu-id="5a311-145">Coleção [MediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="5a311-145">[MediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="5a311-146">Os prompts a serem reproduzidos.</span><span class="sxs-lookup"><span data-stu-id="5a311-146">The prompts to be played.</span></span> <span data-ttu-id="5a311-147">O tamanho máximo da coleção mediaPrompt compatível é 1.</span><span class="sxs-lookup"><span data-stu-id="5a311-147">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="5a311-148">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="5a311-148">bargeInAllowed</span></span>|<span data-ttu-id="5a311-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a311-149">Boolean</span></span>| <span data-ttu-id="5a311-150">Se for true, a solicitação recordResponse será Barge para outras solicitações de registro/playprompt em fila existentes/em processamento no momento.</span><span class="sxs-lookup"><span data-stu-id="5a311-150">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="5a311-151">Padrão = false.</span><span class="sxs-lookup"><span data-stu-id="5a311-151">Default = false.</span></span> |
|<span data-ttu-id="5a311-152">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="5a311-152">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="5a311-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5a311-153">Int32</span></span>| <span data-ttu-id="5a311-154">Silêncio inicial máximo (silêncio do usuário) permitido a partir da hora em que começamos a operação de resposta de registro antes do tempo limite e falha na operação.</span><span class="sxs-lookup"><span data-stu-id="5a311-154">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="5a311-155">Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt.</span><span class="sxs-lookup"><span data-stu-id="5a311-155">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="5a311-156">Padrão = 5 segundos, mín = 1 segundo, máx. = 120 segundos</span><span class="sxs-lookup"><span data-stu-id="5a311-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="5a311-157">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="5a311-157">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="5a311-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5a311-158">Int32</span></span>| <span data-ttu-id="5a311-159">Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar.</span><span class="sxs-lookup"><span data-stu-id="5a311-159">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="5a311-160">Padrão = 5 segundos, mín = 1 segundo, máximo = 120 segundos.</span><span class="sxs-lookup"><span data-stu-id="5a311-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="5a311-161">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="5a311-161">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="5a311-162">Int32</span><span class="sxs-lookup"><span data-stu-id="5a311-162">Int32</span></span>| <span data-ttu-id="5a311-163">Duração máxima para a operação recordResponse antes de parar a gravação.</span><span class="sxs-lookup"><span data-stu-id="5a311-163">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="5a311-164">Padrão = 5 segundos, mín = 1 segundo, máximo = 120 segundos.</span><span class="sxs-lookup"><span data-stu-id="5a311-164">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="5a311-165">playBeep</span><span class="sxs-lookup"><span data-stu-id="5a311-165">playBeep</span></span>|<span data-ttu-id="5a311-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a311-166">Boolean</span></span>| <span data-ttu-id="5a311-167">Se true, reproduz um aviso sonoro para indicar ao usuário que eles podem começar a gravar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="5a311-167">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="5a311-168">Padrão = true.</span><span class="sxs-lookup"><span data-stu-id="5a311-168">Default = true.</span></span>|
|<span data-ttu-id="5a311-169">stopTones</span><span class="sxs-lookup"><span data-stu-id="5a311-169">stopTones</span></span>|<span data-ttu-id="5a311-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a311-170">String collection</span></span>|<span data-ttu-id="5a311-171">Pare os toques especificados para terminar a gravação.</span><span class="sxs-lookup"><span data-stu-id="5a311-171">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="5a311-172">clientContext</span><span class="sxs-lookup"><span data-stu-id="5a311-172">clientContext</span></span>|<span data-ttu-id="5a311-173">String</span><span class="sxs-lookup"><span data-stu-id="5a311-173">String</span></span>|<span data-ttu-id="5a311-174">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="5a311-174">Unique Client Context string.</span></span> <span data-ttu-id="5a311-175">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="5a311-175">Max limit is 256 chars.</span></span>|

> <span data-ttu-id="5a311-176">**Observação:** O tempo máximo de gravação foi reduzido de cinco minutos para 2 minutos.</span><span class="sxs-lookup"><span data-stu-id="5a311-176">**Note:** The maximum recording time has been reduced from 5 minutes to 2 minutes.</span></span>

## <a name="response"></a><span data-ttu-id="5a311-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a311-177">Response</span></span>
<span data-ttu-id="5a311-178">Este método retorna um `200 OK` código de resposta http e um cabeçalho de local com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a311-178">This method returns a `200 OK` HTTP response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="5a311-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a311-179">Example</span></span>
<span data-ttu-id="5a311-180">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5a311-180">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="5a311-181">Exemplo 1: grava uma breve resposta de áudio do chamador</span><span class="sxs-lookup"><span data-stu-id="5a311-181">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="5a311-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a311-182">Request</span></span>
<span data-ttu-id="5a311-183">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a311-183">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5a311-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a311-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/recordResponse
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a311-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a311-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a311-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a311-186">Response</span></span>
<span data-ttu-id="5a311-187">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a311-187">The following example shows the response.</span></span>

> <span data-ttu-id="5a311-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a311-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="5a311-190">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="5a311-190">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="5a311-191">Exemplo 2: Recuperando o arquivo de gravação</span><span class="sxs-lookup"><span data-stu-id="5a311-191">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="5a311-192">**Observação:** Você não pode gravar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="5a311-192">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="5a311-193">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="5a311-193">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="5a311-194">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="5a311-194">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="5a311-195">Solicitar</span><span class="sxs-lookup"><span data-stu-id="5a311-195">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="5a311-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a311-196">Response</span></span>

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

> <span data-ttu-id="5a311-197">**Observação:** Você não pode gravar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="5a311-197">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="5a311-198">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="5a311-198">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="5a311-199">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="5a311-199">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: recordResponse",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
