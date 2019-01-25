---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1f94bf51169a6b056e010386f88d859aeaf41b9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512371"
---
# <a name="listinfo-resource"></a>Recurso de ListInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| **template**            | String  | Um valor enumerado que representa o modelo de lista básica usado na criação da lista. Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.

### <a name="remarks"></a>Comentários

Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.
Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.
Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/listinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
