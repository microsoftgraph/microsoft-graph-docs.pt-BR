---
author: daspek
title: Tipo de recurso versionAction
description: O objeto VersionAction fornece informações sobre uma atividade que resultou em uma nova versão do item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f47d90c899ea9eb011837ae3c47dd6ec7ae22f30
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238985"
---
# <a name="versionaction-resource-type"></a>Tipo de recurso versionAction

Namespace: microsoft.graph

A presença do recurso **versionAction** em um [**itemActivity**][activity] indica que a atividade causou a criação de uma nova versão.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

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

