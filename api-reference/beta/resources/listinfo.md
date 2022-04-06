---
author: JeremyKelley
description: O tipo complexo listInfo oferece informações adicionais sobre uma lista.
ms.date: 09/11/2017
title: ListInfo
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a2174c4fda353d0bfa5148f8ec5985f925ff0070
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723801"
---
# <a name="listinfo-resource"></a>Recurso de ListInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Propriedade                | Tipo    | Descrição                                                                                                                                                                                              |
| :---------------------- | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **contentTypesEnabled** | Booliano | Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.                                                                                                                                       |
| **hidden**              | Booliano | Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.                                                                                                            |
| **template**            | String  | Um valor enumerado que representa o modelo de lista básica usado na criação da lista. Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais. |

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
  "suppressions": []
}
-->
