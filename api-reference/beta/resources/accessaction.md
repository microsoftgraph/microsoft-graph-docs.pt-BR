---
author: daspek
ms.author: dspektor
ms.date: 09/12/2018
title: Accessaction
localization_priority: Normal
ms.openlocfilehash: bef6444fd42080c6f5b7cdabb69dbe9a50bab8d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535815"
---
# <a name="accessaction-resource-type"></a>tipo de recurso accessaction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **accessaction** em uma myactivity [****] [ activity] indica que a atividade acessou um item.

>**Observação:** Os registros de atividade do Access atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

Esse tipo de recurso não tem propriedades.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.accessAction"
}-->

```json
{
}
```


<!--
{
  "type": "#page.annotation",
  "description": "The AccessAction object provides information about accesses of an item.",
  "keywords": "activities,activity,action,access",
  "section": "documentation",
  "tocPath": "Resources/AccessAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
