---
title: 'Call: recordResponse'
description: Registra uma resposta de áudio curta do chamador. Isso será útil se o bot quiser capturar uma resposta de voz do chamador seguindo um prompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fe4db80727bc2af3dc3e1d41be6d4207ffacf96d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682142"
---
# <a name="call-recordresponse"></a><span data-ttu-id="22e6c-104">Call: recordResponse</span><span class="sxs-lookup"><span data-stu-id="22e6c-104">call: recordResponse</span></span>

<span data-ttu-id="22e6c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22e6c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22e6c-106">Registra uma resposta de áudio curta do chamador.</span><span class="sxs-lookup"><span data-stu-id="22e6c-106">Records a short audio response from the caller.</span></span>
<span data-ttu-id="22e6c-107">Um bot pode usá-la para capturar uma resposta de voz de um chamador depois de ser solicitada uma resposta.</span><span class="sxs-lookup"><span data-stu-id="22e6c-107">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="22e6c-108">Para obter mais informações sobre como lidar com operações, confira [commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="22e6c-108">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="22e6c-109">**Observação:** Isso só é suportado para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="22e6c-109">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="22e6c-110">Esta ação não deve ser registrada em toda a chamada.</span><span class="sxs-lookup"><span data-stu-id="22e6c-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="22e6c-111">O tamanho máximo da gravação é de 2 minutos.</span><span class="sxs-lookup"><span data-stu-id="22e6c-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="22e6c-112">A gravação não é salva permanentemente pela plataforma de comunicação em nuvem e é descartada logo após o término da chamada.</span><span class="sxs-lookup"><span data-stu-id="22e6c-112">The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="22e6c-113">O bot deve baixar a gravação imediatamente após a conclusão da operação de gravação usando o valor recordingLocation fornecido na notificação de conclusão.</span><span class="sxs-lookup"><span data-stu-id="22e6c-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="22e6c-114">**Observação:** Qualquer mídia coletada pode **não** ser persistente.</span><span class="sxs-lookup"><span data-stu-id="22e6c-114">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="22e6c-115">Certifique-se de que você está em conformidade com as leis e regulamentos da sua área quando se trata de gravação de chamada.</span><span class="sxs-lookup"><span data-stu-id="22e6c-115">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="22e6c-116">Consulte um advogado legal para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="22e6c-116">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="22e6c-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="22e6c-117">Permissions</span></span>
<span data-ttu-id="22e6c-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22e6c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22e6c-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22e6c-120">Permission type</span></span> | <span data-ttu-id="22e6c-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22e6c-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="22e6c-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22e6c-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="22e6c-123">Não suportado</span><span class="sxs-lookup"><span data-stu-id="22e6c-123">Not Supported</span></span>        |
| <span data-ttu-id="22e6c-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22e6c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22e6c-125">Não suportado</span><span class="sxs-lookup"><span data-stu-id="22e6c-125">Not Supported</span></span>        |
| <span data-ttu-id="22e6c-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22e6c-126">Application</span></span>     | <span data-ttu-id="22e6c-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="22e6c-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="22e6c-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22e6c-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a><span data-ttu-id="22e6c-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22e6c-129">Request headers</span></span>
| <span data-ttu-id="22e6c-130">Nome</span><span class="sxs-lookup"><span data-stu-id="22e6c-130">Name</span></span>          | <span data-ttu-id="22e6c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="22e6c-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="22e6c-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="22e6c-132">Authorization</span></span> | <span data-ttu-id="22e6c-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22e6c-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22e6c-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22e6c-135">Request body</span></span>
<span data-ttu-id="22e6c-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22e6c-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22e6c-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="22e6c-137">Parameter</span></span>      | <span data-ttu-id="22e6c-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="22e6c-138">Type</span></span>    |<span data-ttu-id="22e6c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="22e6c-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22e6c-140">prompts</span><span class="sxs-lookup"><span data-stu-id="22e6c-140">prompts</span></span>|<span data-ttu-id="22e6c-141">coleção [mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="22e6c-141">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="22e6c-142">Os prompts a serem reproduzidos.</span><span class="sxs-lookup"><span data-stu-id="22e6c-142">The prompts to be played.</span></span> <span data-ttu-id="22e6c-143">O tamanho máximo da coleção mediaPrompt compatível é 1.</span><span class="sxs-lookup"><span data-stu-id="22e6c-143">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="22e6c-144">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="22e6c-144">bargeInAllowed</span></span>|<span data-ttu-id="22e6c-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="22e6c-145">Boolean</span></span>| <span data-ttu-id="22e6c-146">Se for true, a solicitação recordResponse será Barge para outras solicitações de registro/playprompt em fila existentes/em processamento no momento.</span><span class="sxs-lookup"><span data-stu-id="22e6c-146">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="22e6c-147">Padrão = false.</span><span class="sxs-lookup"><span data-stu-id="22e6c-147">Default = false.</span></span> |
|<span data-ttu-id="22e6c-148">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="22e6c-148">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="22e6c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="22e6c-149">Int32</span></span>| <span data-ttu-id="22e6c-150">Silêncio inicial máximo (silêncio do usuário) permitido a partir da hora em que começamos a operação de resposta de registro antes do tempo limite e falha na operação.</span><span class="sxs-lookup"><span data-stu-id="22e6c-150">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="22e6c-151">Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt.</span><span class="sxs-lookup"><span data-stu-id="22e6c-151">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="22e6c-152">Padrão = 5 segundos, mín = 1 segundo, máx. = 120 segundos</span><span class="sxs-lookup"><span data-stu-id="22e6c-152">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="22e6c-153">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="22e6c-153">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="22e6c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="22e6c-154">Int32</span></span>| <span data-ttu-id="22e6c-155">Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar.</span><span class="sxs-lookup"><span data-stu-id="22e6c-155">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="22e6c-156">Padrão = 5 segundos, mín = 1 segundo, máximo = 120 segundos.</span><span class="sxs-lookup"><span data-stu-id="22e6c-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="22e6c-157">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="22e6c-157">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="22e6c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="22e6c-158">Int32</span></span>| <span data-ttu-id="22e6c-159">Duração máxima para a operação recordResponse antes de parar a gravação.</span><span class="sxs-lookup"><span data-stu-id="22e6c-159">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="22e6c-160">Padrão = 5 segundos, mín = 1 segundo, máximo = 120 segundos.</span><span class="sxs-lookup"><span data-stu-id="22e6c-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="22e6c-161">playBeep</span><span class="sxs-lookup"><span data-stu-id="22e6c-161">playBeep</span></span>|<span data-ttu-id="22e6c-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="22e6c-162">Boolean</span></span>| <span data-ttu-id="22e6c-163">Se true, reproduz um aviso sonoro para indicar ao usuário que eles podem começar a gravar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="22e6c-163">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="22e6c-164">Padrão = true.</span><span class="sxs-lookup"><span data-stu-id="22e6c-164">Default = true.</span></span>|
|<span data-ttu-id="22e6c-165">stopTones</span><span class="sxs-lookup"><span data-stu-id="22e6c-165">stopTones</span></span>|<span data-ttu-id="22e6c-166">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="22e6c-166">String collection</span></span>|<span data-ttu-id="22e6c-167">Pare os toques especificados para terminar a gravação.</span><span class="sxs-lookup"><span data-stu-id="22e6c-167">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="22e6c-168">clientContext</span><span class="sxs-lookup"><span data-stu-id="22e6c-168">clientContext</span></span>|<span data-ttu-id="22e6c-169">String</span><span class="sxs-lookup"><span data-stu-id="22e6c-169">String</span></span>|<span data-ttu-id="22e6c-170">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="22e6c-170">Unique Client Context string.</span></span> <span data-ttu-id="22e6c-171">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="22e6c-171">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="22e6c-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e6c-172">Response</span></span>
<span data-ttu-id="22e6c-173">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="22e6c-173">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="22e6c-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22e6c-174">Example</span></span>
<span data-ttu-id="22e6c-175">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="22e6c-175">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="22e6c-176">Exemplo 1: grava uma breve resposta de áudio do chamador</span><span class="sxs-lookup"><span data-stu-id="22e6c-176">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="22e6c-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22e6c-177">Request</span></span>
<span data-ttu-id="22e6c-178">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="22e6c-178">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22e6c-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="22e6c-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/recordResponse
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
# <a name="javascript"></a>[<span data-ttu-id="22e6c-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22e6c-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="22e6c-181">C#</span><span class="sxs-lookup"><span data-stu-id="22e6c-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22e6c-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22e6c-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22e6c-183">Java</span><span class="sxs-lookup"><span data-stu-id="22e6c-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="22e6c-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e6c-184">Response</span></span>
<span data-ttu-id="22e6c-185">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="22e6c-185">The following example shows the response.</span></span>

> <span data-ttu-id="22e6c-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22e6c-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="22e6c-188">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="22e6c-188">Notification - operation completed</span></span>

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
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 200,
          "subcode": 8515,
          "message": "Action completed, max record duration reached."
        },
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="22e6c-189">Exemplo 2: Recuperando o arquivo de gravação</span><span class="sxs-lookup"><span data-stu-id="22e6c-189">Example 2: Retrieving the recording file</span></span>

><span data-ttu-id="22e6c-190">**Observação:** Você não pode gravar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="22e6c-190">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="22e6c-191">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="22e6c-191">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="22e6c-192">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="22e6c-192">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="22e6c-193">Solicitar</span><span class="sxs-lookup"><span data-stu-id="22e6c-193">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="22e6c-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="22e6c-194">Response</span></span>

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
