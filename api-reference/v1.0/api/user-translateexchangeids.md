---
title: 'usuário: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6c3d3401f898b0b086503723ff6de8ff56bc2275
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036414"
---
# <a name="user-translateexchangeids"></a>usuário: translateExchangeIds

Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | User. ReadBasic, User. Read, User. ReadWrite |
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
| inputIds | Coleção de cadeias de caracteres | Uma coleção de identificadores a serem convertidos. Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio. O tamanho máximo dessa coleção é de 1000 cadeias de caracteres. |
| sourceIdType | exchangeIdFormat | O tipo de ID dos identificadores no `InputIds` parâmetro. |
| targetIdType | exchangeIdFormat | O tipo de ID solicitado a ser convertido. |

### <a name="exchangeidformat-values"></a>valores de exchangeIdFormat

| Valores | Descrição |
|:-------|:------------|
| entryId | O formato de ID de entrada binária usado por clientes MAPI. |
| ewsId | O formato de ID usado pelos clientes dos serviços Web do Exchange. |
| immutableEntryId | O formato de ID imutável binário compatível com MAPI. |
| restid | O formato de ID padrão usado pelo Microsoft Graph. |
| restImmutableEntryId | O formato de ID imutável usado pelo Microsoft Graph. |

Os formatos binários`entryId` ( `immutableEntryId`e) são codificados por URL com base em base64. A segurança de URL é implementada modificando a codificação Base64 dos dados binários da seguinte maneira:

- Substituir `+` por`-`
- Substituir `/` por`_`
- Remover os caracteres de preenchimento à direita`=`()
- Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original (`0`, `1`, ou) `2`

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como converter vários identificadores do formato de API REST normal (`restId`) para o formato imutável (`restImmutableEntryId`) do REST.

### <a name="request"></a>Solicitação

Aqui está a solicitação de exemplo.

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

### <a name="response"></a>Resposta

Veja a seguir o exemplo de resposta
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
