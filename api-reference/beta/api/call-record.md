---
title: 'call: recordResponse'
description: Grave uma resposta de áudio curta do chamador. Isso será útil se o bot quiser capturar uma resposta de voz do chamador após um prompt.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2722f649f5d30be05af9d469905b134171e856e0
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346959"
---
# <a name="call-recordresponse"></a>call: recordResponse

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Grave uma resposta de áudio curta do chamador.

Um bot pode usar isso para capturar uma resposta de voz de um chamador depois de ser solicitado a uma resposta.

Para obter mais informações sobre como lidar com operações, consulte [commsOperation](../resources/commsOperation.md)

>**Observação:** Essa API só tem [suporte para chamadas](../resources/call.md) iniciadas com [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).

Essa ação não se destina a gravar a chamada inteira. O comprimento máximo da gravação é de 2 minutos. A gravação não é salva permanentemente pela Plataforma de Comunicações na Nuvem e é descartada logo após o final da chamada. O bot deve baixar a gravação imediatamente após a conclusão da operação de gravação usando o valor recordingLocation que é dado na notificação concluída.

>**Observação:** Você pode não registrar ou persistir conteúdo de mídia de chamadas ou reuniões acessadas pelo aplicativo ou dados derivados desse conteúdo de mídia. Certifique-se de estar em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

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
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> **Observação:** o caminho `/app` foi preterido. Daqui em diante, use o caminho `/communications`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type| application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|prompts|[Coleção MediaPrompt](../resources/mediaprompt.md) | Os prompts a serem tocados. O tamanho máximo da coleção mediaPrompt suportado é 1.|
|bargeInAllowed|Booliano| Se for true, a solicitação recordResponse invadirá outras solicitações existentes de registro/playprompt em fila/processamento atual. Padrão = false. |
|initialSilenceTimeoutInSeconds | Int32| Máximo de silêncio inicial (silêncio do usuário) permitido a partir do momento em que iniciamos a operação de resposta do registro antes do tempo limite e falhamos na operação. Se estamos tocando um prompt, esse temporizador será iniciado após a finalização do prompt. Padrão = 5 segundos, Min = 1 segundo, Máx = 120 segundos |
|maxSilenceTimeoutInSeconds|Int32| Tempo máximo de silêncio (pausa) permitido após um usuário começar a falar. Padrão = 5 segundos, Min = 1 segundo, Máx = 120 segundos.|
|maxRecordDurationInSeconds|Int32| Duração máxima da operação recordResponse antes de interromper a gravação. Padrão = 5 segundos, Min = 1 segundo, Máx = 120 segundos.|
|playBeep|Boolean| Se for true, reproduz um sinal sonoro para indicar ao usuário que ele pode começar a gravar a mensagem. Padrão = true.|
|stopTones|Conjunto de cadeias de caracteres|Pare os tons especificados para encerrar a gravação.|
|clientContext|Cadeia de caracteres|Cadeia de caracteres de contexto de cliente exclusiva. O limite máximo é 256 caracteres.|

> **Observação:** O tempo máximo de gravação foi reduzido de 5 minutos para 2 minutos.

## <a name="response"></a>Resposta
Este método retorna um código `200 OK` de resposta HTTP e um cabeçalho Location com um URI para o [recordOperation](../resources/recordoperation.md) criado para essa solicitação.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a>Exemplo 1: registra uma resposta de áudio curta do chamador

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.


# <a name="http"></a>[HTTP](#tab/http)
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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-recordresponse-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/call-recordresponse-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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

##### <a name="notification---operation-completed"></a>Notificação - operação concluída

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

### <a name="example-2-retrieving-the-recording-file"></a>Exemplo 2: Recuperar o arquivo de gravação

> **Observação:** Você pode NÃO gravar ou persistir conteúdo de mídia de chamadas ou reuniões acessadas pelo aplicativo ou dados derivados desse conteúdo de mídia. Certifique-se de estar em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

##### <a name="request"></a>Solicitação

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

> **Observação:** Você pode NÃO gravar ou persistir conteúdo de mídia de chamadas ou reuniões acessadas pelo aplicativo ou dados derivados desse conteúdo de mídia. Certifique-se de estar em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

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
