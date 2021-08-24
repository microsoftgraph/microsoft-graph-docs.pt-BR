---
author: swapnil1993
ms.date: 08/30/2020
title: Criar columnDefinition em um tipo de conteúdo
description: Adicione coluna a um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 785e75b114574f48d2874797cc3d3975dc997e3d
ms.sourcegitcommit: c6f7a931a8d83ac54f577b7bec08237fd17ce51a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2021
ms.locfileid: "58490104"
---
# <a name="create-columndefinition-for-a-content-type"></a>Criar columnDefinition para um tipo de conteúdo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Adicione uma coluna a um [tipo de conteúdo][contentType] in a site or list by specifying a [columnDefinition][columnDefinition] .

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
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
   "sourceColumn@odata.bind":"https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103"
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
  

