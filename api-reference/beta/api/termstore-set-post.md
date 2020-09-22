---
title: Criar conjunto
description: Criar um novo objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ecf1327333ddd9a38d3199c01a0c6b2436eb27a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064585"
---
# <a name="create-set"></a>Criar conjunto
Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo objeto [set](../resources/termstore-set.md) .

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
POST /termStore/sets
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [set](../resources/termstore-set.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar o [conjunto](../resources/termstore-set.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|localizadores|coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble|Nome do conjunto a ser criado|
|parentGroup|[Microsoft. Graph. termos. Group](../resources/termstore-group.md)|termos-grupo sob o qual o conjunto precisa ser criado|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [set](../resources/termstore-set.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
``` http
POST https://graph.microsoft.com/beta/termStore/sets
Content-Type: application/json
Content-length: 288

{
  "@odata.type": "#microsoft.graph.termStore.set",
  "parentGroup":{
      "id": "fc733b51-10f1-40fd-b784-dc6d1e42804b"
   },
   "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.set"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termSet",
  "suppressions": [
  ]
}
-->


