---
author: daspek
ms.author: dspektor
title: tipo de recurso versionaction
description: O objeto Versionaction fornece informações sobre uma atividade que resultou em uma nova versão do item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: cde5c906c41972950431d5219bea73e4095f74e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533411"
---
# <a name="versionaction-resource-type"></a>tipo de recurso versionaction

Namespace: microsoft.graph

A presença do recurso **versionaction** em um [**myactivity**][activity] indica que a atividade causou a criação de uma nova versão.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | O nome da nova versão que foi criada por esta ação.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

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
