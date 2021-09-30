---
title: 'participante: startHoldMusic'
description: Coloque um participante em espera e toque música em segundo plano.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2ddab154b1c856568aed23186a3d6ba5276e1ac5
ms.sourcegitcommit: cbad97d6a8ccb89b1822b30a11cc9b6f2670deda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2021
ms.locfileid: "60016549"
---
# <a name="participant-startholdmusic"></a>participante: startHoldMusic

Namespace: microsoft.graph

Coloque um [participante em](../resources/participant.md) espera e toque música em segundo plano.
 
> **Observação:** Somente um participante pode ser colocado em espera a qualquer momento.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                               |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                               |
| Aplicativo                            | Nenhum. |

> **Observação:** A verificação de permissão acontece quando o aplicativo entra ou tenta iniciar a chamada. Nenhuma verificação de permissão adicional é executada quando `startHoldMusic` é chamada.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/startHoldMusic
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|customPrompt|microsoft.graph.mediaPrompt|Opcional. Prompt de áudio que o participante ouvirá quando colocado em espera.|
|clientContext|String|Opcional. Cadeia de caracteres de contexto de cliente exclusiva. Pode ter no máximo 256 caracteres.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `202 Accepted` [objeto startHoldMusicOperation](../resources/startholdmusicoperation.md) no corpo da resposta.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

<!-- { 
  "blockType": "request", 
  "name": "participant-startHoldMusic" 
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/participants/fa1e9582-7145-4ca3-bcd8-577f561fcb6e/startHoldMusic
Content-type: application/json

{
  "customPrompt": {
    "@odata.type": "#microsoft.graph.mediaPrompt",
    "mediaInfo": {
      "@odata.type": "#microsoft.graph.mediaInfo",
      "uri": "https://bot.contoso.com/onHold.wav",
    },
  },
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
}
```

---


### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.startHoldMusicOperation" 
} --> 
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.startHoldMusicOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

### <a name="notification-sent-to-the-application-after-the-startholdmusicoperation-finishes"></a>Notificação enviada ao aplicativo após a finalização do startHoldMusicOperation

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
      "resourceUrl": "communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.startHoldMusicOperation",
        "@odata.id": "communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```
