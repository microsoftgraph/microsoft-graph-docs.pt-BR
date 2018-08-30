---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
ms.openlocfilehash: da8398bbb87111648ea561e1799e062ed46b0ee6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270773"
---
# <a name="listinfo-resource"></a>Recurso de ListInfo

O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].

[lista]: list.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade           | Tipo    | Descrição
|:------------------------|:--------|:------------------------------------------------
| **contentTypesEnabled** | Booliano | Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.
| **hidden**              | Booliano | Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.
| **template**            | Sequência de caracteres  | Um valor enumerado que representa o modelo de lista básica usado na criação da lista. Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.

### <a name="remarks"></a>Comentários

Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.
Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.
Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->
