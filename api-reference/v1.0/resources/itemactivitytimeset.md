---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActivityTimeSet
description: O objeto doactionset fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4ef0b56471afe78b13edc2f6efb25941c9a749df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970616"
---
# <a name="itemactivitytimeset-resource-type"></a>tipo de recurso itemActivityTimeSet

O recurso **itemActivityTimeSet** fornece informações sobre quando uma [atividade] [ activity] em um item ocorreu.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade    | Tipo           | Descrição
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | Quando observamos a atividade ocorrer.
| recordedDateTime | DateTimeOffset | Quando a observação foi gravada no serviço.

A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.
Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.
Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
