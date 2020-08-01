---
title: Atualizar termo
description: Atualiza as propriedades de um objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: cce2fadc8dd2990f4b58b74dad554050f8e526d2
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539141"
---
# <a name="update-term"></a>Atualizar termo
Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [Term](../resources/termstore-term.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | TermStore.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [Term](../resources/termstore-term.md) .

A tabela a seguir mostra as propriedades que podem ser atualizadas para um [termo](../resources/termstore-term.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Legendas|coleção [Microsoft. Graph. termos. localizedLabel](../resources/termstore-localizedlabel.md)|rótulos de um termo|
|descrições|coleção [Microsoft. Graph. termos. localizedDescription](../resources/termstore-localizeddescription.md)|descrição sobre o termo|
|properties|coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)|Propriedades associadas ao termo|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Term](../resources/termstore-term.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_term"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
Content-Type: application/json
Content-length: 366

{
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update term",
  "suppressions": [
  ]
}
-->
