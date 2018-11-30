---
title: 'chamar: registro'
description: Registre a chamada.
ms.openlocfilehash: 2d876b30205594e162ac9f5aa1b2068058efea7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035624"
---
# <a name="call-record"></a><span data-ttu-id="01f32-103">chamar: registro</span><span class="sxs-lookup"><span data-stu-id="01f32-103">call: record</span></span>

> <span data-ttu-id="01f32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01f32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01f32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01f32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01f32-106">Registre a chamada.</span><span class="sxs-lookup"><span data-stu-id="01f32-106">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="01f32-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="01f32-107">Permissions</span></span>
<span data-ttu-id="01f32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01f32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01f32-110">Permission type</span></span> | <span data-ttu-id="01f32-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01f32-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="01f32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01f32-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01f32-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="01f32-113">Not Supported</span></span>        |
| <span data-ttu-id="01f32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01f32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f32-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="01f32-115">Not Supported</span></span>        |
| <span data-ttu-id="01f32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01f32-116">Application</span></span>     | <span data-ttu-id="01f32-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="01f32-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="01f32-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01f32-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="01f32-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01f32-119">Request headers</span></span>
| <span data-ttu-id="01f32-120">Nome</span><span class="sxs-lookup"><span data-stu-id="01f32-120">Name</span></span>          | <span data-ttu-id="01f32-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="01f32-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="01f32-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="01f32-122">Authorization</span></span> | <span data-ttu-id="01f32-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01f32-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01f32-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01f32-125">Request body</span></span>
<span data-ttu-id="01f32-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01f32-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01f32-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01f32-127">Parameter</span></span>      | <span data-ttu-id="01f32-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="01f32-128">Type</span></span>    |<span data-ttu-id="01f32-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="01f32-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01f32-130">solicita</span><span class="sxs-lookup"><span data-stu-id="01f32-130">prompts</span></span>|<span data-ttu-id="01f32-131">coleção [mediaprompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="01f32-131">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="01f32-132">Inicia a coleção de prompts para reproduzir (se houver) antes da gravação.</span><span class="sxs-lookup"><span data-stu-id="01f32-132">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="01f32-133">Os clientes podem escolher especificar a ação de "playPrompt" separadamente ou especificar como parte do "Registro" - principalmente todos os registros são precedido por um prompt</span><span class="sxs-lookup"><span data-stu-id="01f32-133">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="01f32-134">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="01f32-134">bargeInAllowed</span></span>|<span data-ttu-id="01f32-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="01f32-135">Boolean</span></span>| <span data-ttu-id="01f32-136">Permitir que os usuários insiram opção antes de concluir o prompt.</span><span class="sxs-lookup"><span data-stu-id="01f32-136">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="01f32-137">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="01f32-137">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="01f32-138">Int32</span><span class="sxs-lookup"><span data-stu-id="01f32-138">Int32</span></span>| <span data-ttu-id="01f32-139">Silêncio inicial máximo permitido desde o momento em que iniciamos a operação de registro antes de tempo limite e a operação de falha.</span><span class="sxs-lookup"><span data-stu-id="01f32-139">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="01f32-140">Se podemos estiver reproduzindo um prompt, este timer começa após a conclusão da prompt.</span><span class="sxs-lookup"><span data-stu-id="01f32-140">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="01f32-141">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="01f32-141">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="01f32-142">Int32</span><span class="sxs-lookup"><span data-stu-id="01f32-142">Int32</span></span>| <span data-ttu-id="01f32-143">O tempo limite de silêncio máximo em segundos.</span><span class="sxs-lookup"><span data-stu-id="01f32-143">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="01f32-144">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="01f32-144">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="01f32-145">Int32</span><span class="sxs-lookup"><span data-stu-id="01f32-145">Int32</span></span>| <span data-ttu-id="01f32-146">A duração máxima de registro em segundos.</span><span class="sxs-lookup"><span data-stu-id="01f32-146">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="01f32-147">playBeep</span><span class="sxs-lookup"><span data-stu-id="01f32-147">playBeep</span></span>|<span data-ttu-id="01f32-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="01f32-148">Boolean</span></span>| <span data-ttu-id="01f32-149">Reproduz um alarme sonoro depois de reproduzir o prompt.</span><span class="sxs-lookup"><span data-stu-id="01f32-149">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="01f32-150">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="01f32-150">streamWhileRecording</span></span>|<span data-ttu-id="01f32-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="01f32-151">Boolean</span></span>|<span data-ttu-id="01f32-152">Se definido como true, um local de recurso serão fornecidas assim que a gravação é iniciado.</span><span class="sxs-lookup"><span data-stu-id="01f32-152">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="01f32-153">stopTones</span><span class="sxs-lookup"><span data-stu-id="01f32-153">stopTones</span></span>|<span data-ttu-id="01f32-154">String collection</span><span class="sxs-lookup"><span data-stu-id="01f32-154">String collection</span></span>|<span data-ttu-id="01f32-155">Pare de toques especificados para terminar gravação.</span><span class="sxs-lookup"><span data-stu-id="01f32-155">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="01f32-156">clientContext</span><span class="sxs-lookup"><span data-stu-id="01f32-156">clientContext</span></span>|<span data-ttu-id="01f32-157">String</span><span class="sxs-lookup"><span data-stu-id="01f32-157">String</span></span>|<span data-ttu-id="01f32-158">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="01f32-158">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="01f32-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="01f32-159">Response</span></span>
<span data-ttu-id="01f32-160">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="01f32-160">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="01f32-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01f32-161">Example</span></span>
<span data-ttu-id="01f32-162">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="01f32-162">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="01f32-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01f32-163">Request</span></span>
<span data-ttu-id="01f32-164">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="01f32-164">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_record"
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

##### <a name="response"></a><span data-ttu-id="01f32-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="01f32-165">Response</span></span>

> <span data-ttu-id="01f32-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01f32-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="01f32-168">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="01f32-168">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
