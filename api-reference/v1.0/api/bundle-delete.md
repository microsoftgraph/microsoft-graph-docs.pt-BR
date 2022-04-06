---
author: JeremyKelley
title: Excluir pacote
description: Excluir um pacote de driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b574c73db2f4e0dd71d0e2e5c6685b58f8ad8143
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561578"
---
# <a name="delete-bundle"></a>Excluir pacote

Namespace: microsoft.graph

[Exclua um pacote][] de driveItems usando sua **id**. Observe que excluir um pacote usando esse método exclui permanentemente o pacote e não o move para a Lixeira.
No entanto, ele não remove os itens que foram referenciados pelo pacote.
Eles permanecerão em suas pastas pai.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.                             |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All   |
|Aplicativo          | Sem suporte.                                           |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | \{token\} de portador. Obrigatório. |
| if-match      | eTag. Opcional. Se esse header de solicitação estiver incluído e a eTag (ou cTag) fornecida não corresponder à marca atual no pacote, `412 Precondition Failed` uma resposta será retornada e o pacote não será excluído.

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação com esse método.

## <a name="response"></a>Resposta

Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.

Para obter informações sobre respostas de erro, consulte [Respostas de erro][error-response].

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Delete"
} -->


