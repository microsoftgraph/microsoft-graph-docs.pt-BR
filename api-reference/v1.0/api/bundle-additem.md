---
author: JeremyKelley
title: Adicionar item a um pacote
description: Adicionar item a um pacote de driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ed5ded16b1577a4931b28d24ac22a785eaed2d2a
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561567"
---
# <a name="add-item-to-a-bundle"></a>Adicionar item a um pacote

Namespace: microsoft.graph

Adicione um [driveItem][] adicional de uma unidade a um [pacote][].

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>Permissões

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

Se tiver êxito, a resposta será `204 No Content`.

Para obter informações sobre respostas de erro, consulte [Respostas de erro][error-response].

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Essa solicitação adicionará um item existente ao pacote especificado.

<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```

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
  "section&quot;: &quot;documentation"
} -->


