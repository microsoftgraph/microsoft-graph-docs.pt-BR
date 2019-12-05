---
title: 'cloudCommunications: getPresencesByUserId'
description: Obtenha as informações de presença de vários usuários.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 5303c39584822a68afa559eb99c9fa579121e515
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844110"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>cloudCommunications: getPresencesByUserId

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as informações de [presença](../resources/presence.md) de vários usuários.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é necessária para chamar essas APIs. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                  |
| :-------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Presence. Read. All                         |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                         |
| Application                            | Sem suporte.                                  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |
|Content-type | application/json. Obrigatório. |


## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça um objeto JSON com o seguinte parâmetro.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|ids|Coleção de cadeias de caracteres|As IDs de objeto de usuário.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Presence](../resources/presence.md) no corpo da resposta.


## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação.

<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta.

> **Observação:** Os objetos Response podem ser reduzidos para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
