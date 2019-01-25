---
title: tipo de recurso de educationWordResource
description: 'Uma subclasse de educationResource. Esse é um recurso de documento do Word. O arquivo do Word deve ser carregado no diretório **fileResource** associado a '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9d92b993ab920a894590346bf5fde0ff86c73e8d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529667"
---
# <a name="educationwordresource-resource-type"></a>tipo de recurso de educationWordResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma subclasse de [educationResource](educationresource.md). Esse é um recurso de documento do Word. O arquivo do Word deve ser carregado no diretório **fileResource** associado a atribuição ou o envio.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|FileURL|String|Local do arquivo no disco.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationwordresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
