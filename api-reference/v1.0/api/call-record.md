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
# <a name="call-recordresponse"></a>Call: recordResponse

Namespace: microsoft.graph

Registra uma resposta de áudio curta do chamador.
Um bot pode usá-la para capturar uma resposta de voz de um chamador depois de ser solicitada uma resposta.

Para obter mais informações sobre como lidar com operações, confira [commsOperation](../resources/commsOperation.md)

>**Observação:** Isso só é suportado para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).

Esta ação não deve ser registrada em toda a chamada. O tamanho máximo da gravação é de 2 minutos. A gravação não é salva permanentemente pela plataforma de comunicação em nuvem e é descartada logo após o término da chamada. O bot deve baixar a gravação imediatamente após a conclusão da operação de gravação usando o valor recordingLocation fornecido na notificação de conclusão.

>**Observação:** Qualquer mídia coletada pode **não** ser persistente. Certifique-se de que você está em conformidade com as leis e regulamentos da sua área quando se trata de gravação de chamada. Consulte um advogado legal para obter mais informações.

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
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|prompts|coleção [mediaPrompt](../resources/mediaprompt.md) | Os prompts a serem reproduzidos. O tamanho máximo da coleção mediaPrompt compatível é 1.|
|bargeInAllowed|Booliano| Se for true, a solicitação recordResponse será Barge para outras solicitações de registro/playprompt em fila existentes/em processamento no momento. Padrão = false. |
|initialSilenceTimeoutInSeconds | Int32| Silêncio inicial máximo (silêncio do usuário) permitido a partir da hora em que começamos a operação de resposta de registro antes do tempo limite e falha na operação. Se estivermos reproduzindo um prompt, este cronômetro será iniciado após a conclusão do prompt. Padrão = 5 segundos, mín = 1 segundo, máx. = 120 segundos |
|maxSilenceTimeoutInSeconds|Int32| Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar. Padrão = 5 segundos, mín = 1 segundo, máximo = 120 segundos.|
|maxRecordDurationInSeconds|Int32| Duração máxima para a operação recordResponse antes de parar a gravação. Padrão = 5 segundos, mín = 1 segundo, máximo = 120 segundos.|
|playBeep|Booliano| Se true, reproduz um aviso sonoro para indicar ao usuário que eles podem começar a gravar suas mensagens. Padrão = true.|
|stopTones|Conjunto de cadeias de caracteres|Pare os toques especificados para terminar a gravação.|
|clientContext|String|Cadeia de caracteres de contexto de cliente exclusivo. O limite máximo é de 256 caracteres.|

## <a name="response"></a>Resposta
Este método retorna um `200 OK` código de resposta e um cabeçalho de local com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a>Exemplo 1: grava uma breve resposta de áudio do chamador

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
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

##### <a name="notification---operation-completed"></a>Notificação-operação concluída

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

### <a name="example-2-retrieving-the-recording-file"></a>Exemplo 2: Recuperando o arquivo de gravação

>**Observação:** Você não pode gravar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia. Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

##### <a name="request"></a>Solicitar

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a>Resposta

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
