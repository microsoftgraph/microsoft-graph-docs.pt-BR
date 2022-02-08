---
title: Criar relação
description: Crie um novo objeto relation.
author: vishriv
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 7e2c77a47f89eadf5140da215a0386917520f644
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443399"
---
# <a name="create-relation"></a>Criar relação
Namespace: microsoft.graph.termStore

Crie um novo [objeto relation](../resources/termstore-relation.md) . Eles são usados para criar relações fixadas e reutilizadas entre termos ou entre um termo e um conjunto. Se você criar um termo fixado/reutilizado entre o termo e o conjunto, **fromTerm**  deve ser definido como *nulo* no corpo da postagem.

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
POST sites/{site-id}/termStore/sets/{set-id}/terms/{term-id}/relations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto relation](../resources/termstore-relation.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar o [objeto relation](../resources/termstore-relation.md) .

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|relação|microsoft.graph.termStore.relationType|Tipo de relação a ser criada. Os valores possíveis são: `pin` e `reuse`.|
|set| [microsoft.graph.termStore.set](../resources/termstore-set.md)| O conjunto onde a relação precisa ser criada.|
|fromTerm| [microsoft.graph.termStore.term](../resources/termstore-term.md) | O termo com o qual a relação precisa ser criada.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto microsoft.graph.termStore.relation](../resources/termstore-relation.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_relation_from_"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/27fd2d26-60d3-485c-9420-0c71f74a0cfd/terms/8861b57a-c777-49e7-826f-47d6afecf80d/relations
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "pin",
  "fromTerm" : {
    "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "set" : {
    "id": "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.relation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "052c749c-749c-052c-9c74-2c059c742c05",
  "relationship": "pin",
  "fromTerm" : {
      "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "toTerm" : {
      "id" : "226e8ee3-f4b6-49d7-92d5-ec9d5475eec5"
  },
  "set" : {
      "id" : "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Pinned term",
  "suppressions": [
  ]
}
-->


