---
title: 'chamar: cancelMediaProcessing'
description: Mídia cancela o processamento para todos quaisquer operações PlayPrompt ou o registro em andamento.
ms.openlocfilehash: 27a978a28c94cc161e2d62137c5afc0e9ff085df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033644"
---
# <a name="call-cancelmediaprocessing"></a>chamar: cancelMediaProcessing

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Mídia cancela o processamento para todos quaisquer operações PlayPrompt ou o registro em andamento.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Não são suportados.                              |
| Delegado (conta pessoal da Microsoft) | Não são suportados.                              |
| Aplicativo                            | Nenhum.                                       |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    | Descrição                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| todos os            | Booliano | O sinalizador indicando se pare todas as operações ou atual. |
| clientContext  | String  | O contexto de cliente.                                            |

## <a name="response"></a>Resposta
Retorna `202 Accepted` código de resposta e um cabeçalho de local com um uri para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "call_cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a>Resposta

> **Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a>Notificação - operação concluída

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
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
