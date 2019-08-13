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
# <a name="call-record"></a>Call: Record

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Grave um pequeno clipe de áudio da chamada. Isso será útil se o bot quiser capturar uma resposta de voz do chamador seguindo um prompt.

> [!Note]
> A ação de registro é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md). Esta ação não grava toda a chamada. O tamanho máximo da gravação é de 5 minutos. A gravação não é salva permamently pela plataforma de comunicação em nuvem e é descartada logo após o término da chamada. O bot deve baixar a gravação imediatamente (usando o valor **recordingLocation** fornecido na notificação concluída) após a conclusão da operação de gravação.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
| :-------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Não suportado        |
| Delegado (conta pessoal da Microsoft) | Não suportado        |
| Aplicativo     | Calls.AccessMedia.All                       |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|prompts|coleção [mediaPrompt](../resources/mediaprompt.md) | Coleção de prompts a serem executados (se houver) antes da gravação começar. Os clientes podem optar por especificar a ação "playPrompt" separadamente ou especificar como parte de "Record"-principalmente todos os registros são precedidos por um prompt. O suporte atual é apenas para um único prompt como parte do conjunto. |
|bargeInAllowed|Booliano| Se for true, essa solicitação de registro será Barge em outras solicitações de registro/playprompt da fila existente/no momento. Padrão = false. |
|initialSilenceTimeoutInSeconds | Int32| Silêncio inicial máximo (silêncio do usuário) permitido a partir da hora em que começamos a operação de registro antes do tempo limite e falha na operação. Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt. Padrão = 5 segundos, mín = 1 segundo, máx. = 300 segundos |
|maxSilenceTimeoutInSeconds|Int32| Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar. Padrão = 5 segundos, mín = 1 segundo, máximo = 300 segundos.|
|maxRecordDurationInSeconds|Int32| Duração máxima de uma operação de registro antes de parar a gravação. Padrão = 5 segundos, mín = 1 segundo, máximo = 300 segundos.|
|playBeep|Booliano| Se true, reproduz um aviso sonoro para indicar ao usuário que eles podem começar a gravar suas mensagens. Padrão = true.|
|stopTones|Coleção de cadeias de caracteres|Pare os toques especificados para terminar a gravação.|
|clientContext|String|Cadeia de caracteres de contexto de cliente exclusivo. Pode ter um máximo de 256 caracteres.|

## <a name="response"></a>Resposta
Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

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

##### <a name="notification---operation-completed"></a>Notificação-operação concluída

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

##### <a name="get-recording-file---request"></a>Obter arquivo de gravação-solicitação
O exemplo a seguir mostra a solicitação para obter o conteúdo da gravação.

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a>Obter arquivo de gravação-resposta
Veja a seguir um exemplo da resposta. 

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
