---
title: 'cloudCommunications: getPresencesByUserId'
description: Obtenha as informações de presença de vários usuários.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 1eae5f86955732829c3eed56be531588f5155eb5
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689147"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>cloudCommunications: getPresencesByUserId

Namespace: microsoft.graph

Obtenha as informações de [presença](../resources/presence.md) de vários usuários.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é necessária para chamar essas APIs. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                  |
| :-------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Presence.Read.All                         |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                         |
| Application                            | Sem suporte.                                  |

> **Observação:**
> * O máximo de 650 IDs de usuário têm suporte por solicitação de API.
> * A taxa máxima de solicitações dessa API são 1500 solicitações de API em um período de 30 segundos, por aplicativo por locatário.

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

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Presence](../resources/presence.md) no corpo da resposta.


## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

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


