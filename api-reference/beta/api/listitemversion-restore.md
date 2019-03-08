---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Restaurar uma versão anterior de um item de lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 20cf0460aa679fc40a4bb11d0887bc4946ddcd74
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482081"
---
# <a name="restore-a-previous-version-of-a-listitem"></a>Restaura uma versão anterior de um ListItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|            Tipo de permissão             |         Permissões (da com menos para a com mais privilégios)          |
| :------------------------------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |
| Delegada (conta pessoal da Microsoft) | n/d                                                          |
| Aplicativo                            | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>Corpo da solicitação

Nenhum corpo de solicitação é obrigatório.

## <a name="example"></a>Exemplo

Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>Resposta

Se tiver êxito, a chamada API retorna um código `204 No content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
