---
title: Criar grupo
description: Crie um novo objeto group em um armazenamento de termos.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 8f26a6dc8b5c29face38f3e20d82bc8ff9c36594
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514858"
---
# <a name="create-termstore-group"></a>Criar grupo termStore
Namespace: microsoft.graph.termStore

Crie um novo [objeto group](../resources/termstore-group.md) em um armazenamento de termos.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) |TermStore.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST sites/{site-id}/termStore/groups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto group.](../resources/termstore-group.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar o [objeto group.](../resources/termstore-group.md)

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome do grupo a ser criado.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [microsoft.graph.termStore.group](../resources/termstore-group.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "displayName": "myGroup"
}-->

``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/groups
Content-Type: application/json
Content-length: 135

{
  "displayName" : "myGroup"
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "85825593-5593-8582-9355-828593558285",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "displayName": "myGroup"  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termGroup",
  "suppressions": [
  ]
}
-->


