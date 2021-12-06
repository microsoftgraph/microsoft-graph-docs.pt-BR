---
title: 'user: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: abheek-das
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7036a86ccadedbbfa354a5f230fe8525b2a67e9c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984959"
---
# <a name="user-translateexchangeids"></a>user: translateExchangeIds

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | User.ReadBasic.All, User.Read, User.ReadWrite |
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
| inputIds | Conjunto de cadeias de caracteres | Uma coleção de identificadores a converter. Todos os identificadores da coleção DEVEM ter o mesmo tipo de ID de origem e DEVEM ser para itens na mesma caixa de correio. O tamanho máximo dessa coleção é de 1000 cadeias de caracteres. |
| sourceIdType | exchangeIdFormat | O tipo de ID dos identificadores no `InputIds` parâmetro. |
| targetIdType | exchangeIdFormat | O tipo de ID solicitado a ser convertido. |

### <a name="exchangeidformat-values"></a>Valores exchangeIdFormat

| Member | Descrição |
|:-------|:------------|
| entryId | O formato de ID de entrada binária usado pelos clientes MAPI. |
| ewsId | O formato de ID usado pelos clientes Exchange Web Services. |
| immutableEntryId | O formato de ID imutável compatível com MAPI binário. |
| restId | O formato de ID padrão usado pela Microsoft Graph. |
| restImmutableEntryId | O formato ID imutável usado pela Microsoft Graph. |

Os formatos binários ( e ) são codificados com `entryId` base em URL `immutableEntryId` segura64. A segurança de URL é implementada modificando a codificação base64 dos dados binários da seguinte maneira:

- Substituir `+` por `-`
- Substituir `/` por `_`
- Remover quaisquer caracteres de preenchimento à parte ( `=` )
- Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original ( `0` , `1` ou `2` )

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` o código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.

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
POST https://graph.microsoft.com/beta/me/translateExchangeIds
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-translateexchangeids-go-snippets.md)]
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


