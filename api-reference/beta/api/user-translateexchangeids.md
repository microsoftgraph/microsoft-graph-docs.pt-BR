---
title: 'usuário: translateExchangeIds'
description: Traduza os identificadores de recursos relacionados ao Outlook entre formatos.
ms.openlocfilehash: e18c59df5a7ecbaa16b954bf74221c8d8d1de5d3
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184487"
---
# <a name="user-translateexchangeids"></a>usuário: translateExchangeIds

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Traduza os identificadores de recursos relacionados ao Outlook entre formatos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | User.ReadBasic, User.Read, User.ReadWrite |
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
| inputIds | Coleção Edm.String | Uma coleção de identificadores para converter. Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio. Tamanho máximo dessa coleção é 1000 cadeias de caracteres. |
| sourceIdType | exchangeIdFormat | O tipo de identificadores de na ID do `InputIds` parâmetro. |
| targetIdType | exchangeIdFormat | O tipo de ID solicitado para converter em. |

### <a name="exchangeidformat-values"></a>valores de exchangeIdFormat

| Valores | Descrição |
|:-------|:------------|
| entryId | O formato de ID de entrada binário usado pelos clientes MAPI. |
| ewsId | O formato de ID usado pelos clientes de serviços Web do Exchange. |
| immutableEntryId | O formato de ID imutável compatível com MAPI. |
| restId | O formato de ID padrão usado pelo Microsoft Graph. |
| restImmutableEntryId | O formato de ID imutável usado pelo Microsoft Graph. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` código de resposta e um conjunto de [convertIdResult](../resources/convertidresult.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como converter vários identificadores do formato de API REST do normal (`restId`) para o formato de imutável REST (`restImmutableEntryId`).

##### <a name="request"></a>Solicitação

Aqui está a solicitação de exemplo.
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

##### <a name="response"></a>Resposta

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
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```