---
author: swapnil1993
ms.date: 08/30/2020
title: Criar uma columnDefinition em um tipo de conteúdo
description: Adicione uma coluna a um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ece60217b08c6487a7d1cf33c725665f9ede38ac
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696470"
---
# <a name="create-a-columndefinition-in-a-content-type"></a>Criar uma columnDefinition em um tipo de conteúdo
Namespace: microsoft.graph


Adicione uma coluna a um [tipo de conteúdo][contentType] in a site, or a list with a request that specifies a [columnDefinition][columnDefinition] .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/concepts/permissions_reference.md).

  

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [recurso columnDefinition][] a adicionar.  

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e `200 OK` [um objeto columnDefinition][] no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/v1.0/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103"
}
```

### <a name="response"></a>Resposta

A resposta retorna a coluna adicionada a um tipo de conteúdo.

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}

```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
  

