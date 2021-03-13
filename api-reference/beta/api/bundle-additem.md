---
author: JeremyKelley
title: Adicionar item a um pacote
description: Adicionar item a um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f632b8054c1819c1af8bdd632c0d13092117cb30
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50774380"
---
# <a name="add-item-to-a-bundle"></a>Adicionar item a um pacote

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione um [driveItem][] adicional de uma unidade a um [pacote][].

[pacote]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.                             |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All   |
|Aplicativo          | Sem suporte.                                           |

## <a name="http-request"></a>Solicitação HTTP

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação inclui o identificador de um item que deve ser adicionado à coleção de filhos do pacote.

## <a name="response"></a>Resposta

Se tiver êxito, a resposta será `204 No Content` .

Leia o tópico [Respostas de Erro][error-response] para obter mais informações sobre como os erros são retornados.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Essa solicitação adicionará um item existente ao pacote especificado.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->


