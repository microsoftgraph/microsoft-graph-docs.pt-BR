---
author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: O tipo complexo listInfo oferece informações adicionais sobre uma lista.
doc_type: resourcePageType
ms.openlocfilehash: 90d216101ba9844e1c607fcdfc92bd774add11d8258ec6dd42984b3eadb50b06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196947"
---
# <a name="listinfo-resource"></a>Recurso de ListInfo

Namespace: microsoft.graph

O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].

[lista]: list.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type&quot;: &quot;microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template&quot;: &quot;documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade           | Tipo    | Descrição
|:------------------------|:--------|:------------------------------------------------
| **contentTypesEnabled** | Booliano | Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.
| **hidden**              | Booliano | Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.
| **template**            | String  | Um valor enumerado que representa o modelo de lista básica usado na criação da lista. Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.

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

