---
title: 'user: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0bcacfa2d17b6105b943cb2391da0db423d120c0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137197"
---
# <a name="user-translateexchangeids"></a>user: translateExchangeIds

Namespace: microsoft.graph

Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante) | User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | User.ReadBasic.All, User.Read, User.ReadWrite |
| Aplicativo | User.Read.All, User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Valor |
|:-----|:------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

| Parâmetro | Tipo | Descrição |
|:----------|:-----|:------------|
| inputIds | String collection | Uma coleção de identificadores a converter. Todos os identificadores na coleção DEVEM ter o mesmo tipo de ID de origem e DEVEM ser para itens na mesma caixa de correio. O tamanho máximo dessa coleção é de 1000 cadeias de caracteres. |
| sourceIdType | exchangeIdFormat | O tipo de identificação dos identificadores no `InputIds` parâmetro. |
| targetIdType | exchangeIdFormat | O tipo de ID solicitado para o qual converter. |

### <a name="exchangeidformat-values"></a>Valores de exchangeIdFormat

| Valores | Descrição |
|:-------|:------------|
| entryId | O formato de ID de entrada binária usado por clientes MAPI. |
| ewsId | O formato de ID usado pelos clientes dos Serviços Web do Exchange. |
| immutableEntryId | O formato de ID imutável compatível com MAPI binário. |
| restId | O formato de ID padrão usado pelo Microsoft Graph. |
| restImmutableEntryId | O formato de ID imutável usado pelo Microsoft Graph. |

Os formatos binários ( `entryId` e `immutableEntryId` ) são codificados como base64 seguro para URL. A segurança de URL é implementada modificando a codificação base64 dos dados binários da seguinte maneira:

- Substituir `+` por `-`
- Substituir `/` por `_`
- Remover todos os caracteres de preenchimento à sua parte ( `=` )
- Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original ( `0` , `1` ou `2` )

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` o código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como converter vários identificadores do formato normal da API REST ( ) para o `restId` formato imutável REST ( `restImmutableEntryId` ).

### <a name="request"></a>Solicitação

Aqui está a solicitação de exemplo.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Aqui está a resposta de exemplo
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```

