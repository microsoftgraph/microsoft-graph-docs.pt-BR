---
author: daspek
description: A presença do recurso VersionAction em uma itemActivity indica que a atividade fez uma nova versão a ser criada.
ms.date: 09/14/2017
title: VersionAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0061e53ea03d2dbca8bb4c29d0fb88c1909b592a
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722647"
---
# <a name="versionaction-resource-type"></a>Tipo de recurso VersionAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **VersionAction** em uma [**itemActivity**][activity] indica que a atividade fez uma nova versão a ser criada.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.versionAction"
}-->

```json
{
  "newVersion&quot;: &quot;string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo   | Descrição                                                  |
| :--------- | :----- | :----------------------------------------------------------- |
| newVersion | string | O nome da nova versão que foi criada por esta ação. |

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->
