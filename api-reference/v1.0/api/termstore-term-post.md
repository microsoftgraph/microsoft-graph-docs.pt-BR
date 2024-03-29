---
title: Criar termo
description: Crie um novo objeto de termo.
author: vishriv
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 1b8dc16cdc36e50b777c64189fd5ffd2e8f85acc
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191412"
---
# <a name="create-term"></a>Criar termo
Namespace: microsoft.graph.termStore

Crie um novo [objeto de](../resources/termstore-term.md) termo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | TermStore.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
} -->

``` http
POST sites/{site-id}/termStore/sets/{set-id}/children
POST sites/{site-id}/termStore/sets/{set-id}/terms/{term-id}/children
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto de](../resources/termstore-term.md) termo.

A tabela a seguir mostra as propriedades que são necessárias ao criar o [objeto de](../resources/termstore-term.md) termo.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Rótulos|[coleção microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)|Rótulo para o termo a ser criado.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto microsoft.graph.termStore.term](../resources/termstore-term.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_term_from_"
} -->

``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/462bd0ae-30bb-4c58-845c-761ff6481ac1/children
Content-Type: application/json

{
  "labels": [
    {
      "languageTag" : "en-US",
      "name" : "Car",
      "isDefault" : true
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-term-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-term-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-term-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-term-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-term-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-term-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "labels" : [
      {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Post term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Post term",
  "suppressions": [
  ]
}
-->


