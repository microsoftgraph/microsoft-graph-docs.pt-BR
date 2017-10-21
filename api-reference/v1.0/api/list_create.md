---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Criar uma lista do SharePoint
ms.openlocfilehash: ff7b20e828d8136a9cd6274d533191fd22d903ff
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="create-a-new-list"></a>Criar uma nova lista

Criar uma nova [lista][] em um [site][].

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|            Tipo de permissão             | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Sites.Manage.All                            |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Sites.ReadWrite.All                         |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do recurso [list][] a criar.

## <a name="example"></a>Exemplo

Aqui está um exemplo de como criar uma nova lista genérica.

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

**Observação:** Colunas personalizadas são opcionais.

Além de todas as colunas especificadas aqui, novas listas são criadas com colunas definidas no **modelo** referenciado.
Se a faceta **lista** ou **modelo** não for especificada, a lista considera como padrão o modelo `genericList`, que inclui uma coluna _Título_.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará uma [lista][] no corpo da resposta da lista criada.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

**Observação:** O objeto Response será truncado para mais clareza.
As propriedades padrão serão retornadas da chamada real.

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
