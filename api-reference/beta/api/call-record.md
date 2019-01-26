---
title: 'chamar: registro'
description: Registre a chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1f119cfece969c01e68773e5985eab4010dc9874
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574856"
---
# <a name="call-record"></a><span data-ttu-id="da74e-103">chamar: registro</span><span class="sxs-lookup"><span data-stu-id="da74e-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da74e-104">Registre a chamada.</span><span class="sxs-lookup"><span data-stu-id="da74e-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="da74e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da74e-105">Permissions</span></span>
<span data-ttu-id="da74e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da74e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da74e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da74e-108">Permission type</span></span> | <span data-ttu-id="da74e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da74e-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="da74e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da74e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="da74e-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="da74e-111">Not Supported</span></span>        |
| <span data-ttu-id="da74e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da74e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da74e-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="da74e-113">Not Supported</span></span>        |
| <span data-ttu-id="da74e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da74e-114">Application</span></span>     | <span data-ttu-id="da74e-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="da74e-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="da74e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da74e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="da74e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da74e-117">Request headers</span></span>
| <span data-ttu-id="da74e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="da74e-118">Name</span></span>          | <span data-ttu-id="da74e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="da74e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="da74e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="da74e-120">Authorization</span></span> | <span data-ttu-id="da74e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da74e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da74e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da74e-123">Request body</span></span>
<span data-ttu-id="da74e-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da74e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da74e-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="da74e-125">Parameter</span></span>      | <span data-ttu-id="da74e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="da74e-126">Type</span></span>    |<span data-ttu-id="da74e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="da74e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da74e-128">solicita</span><span class="sxs-lookup"><span data-stu-id="da74e-128">prompts</span></span>|<span data-ttu-id="da74e-129">coleção [mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="da74e-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="da74e-130">Inicia a coleção de prompts para reproduzir (se houver) antes da gravação.</span><span class="sxs-lookup"><span data-stu-id="da74e-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="da74e-131">Os clientes podem escolher especificar a ação de "playPrompt" separadamente ou especificar como parte do "Registro" - principalmente todos os registros são precedido por um prompt</span><span class="sxs-lookup"><span data-stu-id="da74e-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="da74e-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="da74e-132">bargeInAllowed</span></span>|<span data-ttu-id="da74e-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="da74e-133">Boolean</span></span>| <span data-ttu-id="da74e-134">Permitir que os usuários insiram opção antes de concluir o prompt.</span><span class="sxs-lookup"><span data-stu-id="da74e-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="da74e-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="da74e-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="da74e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="da74e-136">Int32</span></span>| <span data-ttu-id="da74e-137">Silêncio inicial máximo permitido desde o momento em que iniciamos a operação de registro antes de tempo limite e a operação de falha.</span><span class="sxs-lookup"><span data-stu-id="da74e-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="da74e-138">Se podemos estiver reproduzindo um prompt, este timer começa após a conclusão da prompt.</span><span class="sxs-lookup"><span data-stu-id="da74e-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="da74e-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="da74e-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="da74e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="da74e-140">Int32</span></span>| <span data-ttu-id="da74e-141">O tempo limite de silêncio máximo em segundos.</span><span class="sxs-lookup"><span data-stu-id="da74e-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="da74e-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="da74e-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="da74e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="da74e-143">Int32</span></span>| <span data-ttu-id="da74e-144">A duração máxima de registro em segundos.</span><span class="sxs-lookup"><span data-stu-id="da74e-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="da74e-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="da74e-145">playBeep</span></span>|<span data-ttu-id="da74e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="da74e-146">Boolean</span></span>| <span data-ttu-id="da74e-147">Reproduz um alarme sonoro depois de reproduzir o prompt.</span><span class="sxs-lookup"><span data-stu-id="da74e-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="da74e-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="da74e-148">streamWhileRecording</span></span>|<span data-ttu-id="da74e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="da74e-149">Boolean</span></span>|<span data-ttu-id="da74e-150">Se definido como true, um local de recurso serão fornecidas assim que a gravação é iniciado.</span><span class="sxs-lookup"><span data-stu-id="da74e-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="da74e-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="da74e-151">stopTones</span></span>|<span data-ttu-id="da74e-152">String collection</span><span class="sxs-lookup"><span data-stu-id="da74e-152">String collection</span></span>|<span data-ttu-id="da74e-153">Pare de toques especificados para terminar gravação.</span><span class="sxs-lookup"><span data-stu-id="da74e-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="da74e-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="da74e-154">clientContext</span></span>|<span data-ttu-id="da74e-155">String</span><span class="sxs-lookup"><span data-stu-id="da74e-155">String</span></span>|<span data-ttu-id="da74e-156">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="da74e-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="da74e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="da74e-157">Response</span></span>
<span data-ttu-id="da74e-158">Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="da74e-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="da74e-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da74e-159">Example</span></span>
<span data-ttu-id="da74e-160">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="da74e-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="da74e-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da74e-161">Request</span></span>
<span data-ttu-id="da74e-162">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="da74e-162">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="da74e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="da74e-163">Response</span></span>

> <span data-ttu-id="da74e-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da74e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="da74e-166">Notificação - operação concluída</span><span class="sxs-lookup"><span data-stu-id="da74e-166">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/call-record.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
