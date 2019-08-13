---
title: 'Call: Record'
description: Registre a chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f20b096964b92db4ce393922efc635142698483
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317655"
---
# <a name="call-record"></a><span data-ttu-id="b47bf-103">Call: Record</span><span class="sxs-lookup"><span data-stu-id="b47bf-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b47bf-104">Grave um pequeno clipe de áudio da chamada.</span><span class="sxs-lookup"><span data-stu-id="b47bf-104">Record a short audio clip from the call.</span></span> <span data-ttu-id="b47bf-105">Isso será útil se o bot quiser capturar uma resposta de voz do chamador seguindo um prompt.</span><span class="sxs-lookup"><span data-stu-id="b47bf-105">This is useful if the bot wants to capture a voice response from the caller following a prompt.</span></span>

> [!Note]
> <span data-ttu-id="b47bf-106">A ação de registro é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="b47bf-106">The record action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span> <span data-ttu-id="b47bf-107">Esta ação não grava toda a chamada.</span><span class="sxs-lookup"><span data-stu-id="b47bf-107">This action does not record the entire call.</span></span> <span data-ttu-id="b47bf-108">O tamanho máximo da gravação é de 5 minutos.</span><span class="sxs-lookup"><span data-stu-id="b47bf-108">The maximum length of the recording is 5 minutes.</span></span> <span data-ttu-id="b47bf-109">A gravação não é salva permamently pela plataforma de comunicação em nuvem e é descartada logo após o término da chamada.</span><span class="sxs-lookup"><span data-stu-id="b47bf-109">The recording is not saved permamently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="b47bf-110">O bot deve baixar a gravação imediatamente (usando o valor **recordingLocation** fornecido na notificação concluída) após a conclusão da operação de gravação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-110">The bot must download the recording promptly (using the **recordingLocation** value given in the completed notification) after the recording operation finishes.</span></span>


## <a name="permissions"></a><span data-ttu-id="b47bf-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b47bf-111">Permissions</span></span>
<span data-ttu-id="b47bf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b47bf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b47bf-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b47bf-114">Permission type</span></span> | <span data-ttu-id="b47bf-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b47bf-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b47bf-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b47bf-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b47bf-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b47bf-117">Not Supported</span></span>        |
| <span data-ttu-id="b47bf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b47bf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b47bf-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b47bf-119">Not Supported</span></span>        |
| <span data-ttu-id="b47bf-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b47bf-120">Application</span></span>     | <span data-ttu-id="b47bf-121">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="b47bf-121">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="b47bf-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b47bf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="b47bf-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b47bf-123">Request headers</span></span>
| <span data-ttu-id="b47bf-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b47bf-124">Name</span></span>          | <span data-ttu-id="b47bf-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b47bf-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b47bf-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b47bf-126">Authorization</span></span> | <span data-ttu-id="b47bf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b47bf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b47bf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b47bf-129">Request body</span></span>
<span data-ttu-id="b47bf-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b47bf-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b47bf-131">Parameter</span></span>      | <span data-ttu-id="b47bf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b47bf-132">Type</span></span>    |<span data-ttu-id="b47bf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b47bf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b47bf-134">prompts</span><span class="sxs-lookup"><span data-stu-id="b47bf-134">prompts</span></span>|<span data-ttu-id="b47bf-135">coleção [mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="b47bf-135">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="b47bf-136">Coleção de prompts a serem executados (se houver) antes da gravação começar.</span><span class="sxs-lookup"><span data-stu-id="b47bf-136">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="b47bf-137">Os clientes podem optar por especificar a ação "playPrompt" separadamente ou especificar como parte de "Record"-principalmente todos os registros são precedidos por um prompt.</span><span class="sxs-lookup"><span data-stu-id="b47bf-137">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="b47bf-138">O suporte atual é apenas para um único prompt como parte do conjunto.</span><span class="sxs-lookup"><span data-stu-id="b47bf-138">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="b47bf-139">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="b47bf-139">bargeInAllowed</span></span>|<span data-ttu-id="b47bf-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="b47bf-140">Boolean</span></span>| <span data-ttu-id="b47bf-141">Se for true, essa solicitação de registro será Barge em outras solicitações de registro/playprompt da fila existente/no momento.</span><span class="sxs-lookup"><span data-stu-id="b47bf-141">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="b47bf-142">Padrão = false.</span><span class="sxs-lookup"><span data-stu-id="b47bf-142">Default = false.</span></span> |
|<span data-ttu-id="b47bf-143">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b47bf-143">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="b47bf-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b47bf-144">Int32</span></span>| <span data-ttu-id="b47bf-145">Silêncio inicial máximo (silêncio do usuário) permitido a partir da hora em que começamos a operação de registro antes do tempo limite e falha na operação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-145">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="b47bf-146">Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt.</span><span class="sxs-lookup"><span data-stu-id="b47bf-146">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="b47bf-147">Padrão = 5 segundos, mín = 1 segundo, máx. = 300 segundos</span><span class="sxs-lookup"><span data-stu-id="b47bf-147">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="b47bf-148">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b47bf-148">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="b47bf-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b47bf-149">Int32</span></span>| <span data-ttu-id="b47bf-150">Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar.</span><span class="sxs-lookup"><span data-stu-id="b47bf-150">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="b47bf-151">Padrão = 5 segundos, mín = 1 segundo, máximo = 300 segundos.</span><span class="sxs-lookup"><span data-stu-id="b47bf-151">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="b47bf-152">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="b47bf-152">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="b47bf-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b47bf-153">Int32</span></span>| <span data-ttu-id="b47bf-154">Duração máxima de uma operação de registro antes de parar a gravação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-154">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="b47bf-155">Padrão = 5 segundos, mín = 1 segundo, máximo = 300 segundos.</span><span class="sxs-lookup"><span data-stu-id="b47bf-155">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="b47bf-156">playBeep</span><span class="sxs-lookup"><span data-stu-id="b47bf-156">playBeep</span></span>|<span data-ttu-id="b47bf-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="b47bf-157">Boolean</span></span>| <span data-ttu-id="b47bf-158">Se true, reproduz um aviso sonoro para indicar ao usuário que eles podem começar a gravar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="b47bf-158">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="b47bf-159">Padrão = true.</span><span class="sxs-lookup"><span data-stu-id="b47bf-159">Default = true.</span></span>|
|<span data-ttu-id="b47bf-160">stopTones</span><span class="sxs-lookup"><span data-stu-id="b47bf-160">stopTones</span></span>|<span data-ttu-id="b47bf-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b47bf-161">String collection</span></span>|<span data-ttu-id="b47bf-162">Pare os toques especificados para terminar a gravação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-162">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="b47bf-163">clientContext</span><span class="sxs-lookup"><span data-stu-id="b47bf-163">clientContext</span></span>|<span data-ttu-id="b47bf-164">String</span><span class="sxs-lookup"><span data-stu-id="b47bf-164">String</span></span>|<span data-ttu-id="b47bf-165">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="b47bf-165">Unique Client Context string.</span></span> <span data-ttu-id="b47bf-166">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b47bf-166">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="b47bf-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b47bf-167">Response</span></span>
<span data-ttu-id="b47bf-168">Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-168">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b47bf-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b47bf-169">Example</span></span>
<span data-ttu-id="b47bf-170">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b47bf-170">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b47bf-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b47bf-171">Request</span></span>
<span data-ttu-id="b47bf-172">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-172">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b47bf-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="b47bf-173">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b47bf-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b47bf-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b47bf-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="b47bf-175">Response</span></span>
<span data-ttu-id="b47bf-176">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b47bf-176">The following example shows the response.</span></span>

> <span data-ttu-id="b47bf-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b47bf-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="b47bf-179">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="b47bf-179">Notification - operation completed</span></span>

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
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

##### <a name="get-recording-file---request"></a><span data-ttu-id="b47bf-180">Obter arquivo de gravação-solicitação</span><span class="sxs-lookup"><span data-stu-id="b47bf-180">Get recording file - Request</span></span>
<span data-ttu-id="b47bf-181">O exemplo a seguir mostra a solicitação para obter o conteúdo da gravação.</span><span class="sxs-lookup"><span data-stu-id="b47bf-181">The following example shows the request to get the content of the recording.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a><span data-ttu-id="b47bf-182">Obter arquivo de gravação-resposta</span><span class="sxs-lookup"><span data-stu-id="b47bf-182">Get recording file - Response</span></span>
<span data-ttu-id="b47bf-183">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b47bf-183">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
  "truncated": true
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
