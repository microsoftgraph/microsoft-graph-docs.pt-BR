---
title: Conjunto de atualização
description: Atualiza as propriedades de um objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: cf2910e70b9eabf79a925f36be911427b31a8d9e
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539181"
---
# <a name="update-set"></a>Conjunto de atualização
Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [set](../resources/termstore-set.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
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
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [set](../resources/termstore-set.md) .

A tabela a seguir mostra as propriedades que podem ser editadas para o [conjunto](../resources/termstore-set.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|localizadores|coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble|Nome do conjunto|
|description|String|Descrição do conjunto|
|properties|coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)|Propriedades de um conjunto|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [set](../resources/termstore-set.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_set"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}
Content-Type: application/json
Content-length: 288

{
  "description": "mySet"
}
```


### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "description": "mySet",    
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termSet",
  "suppressions": [
  ]
}
-->
