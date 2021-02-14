---
author: daspek
title: Tipo de recurso itemActivityTimeSet
description: O objeto itemActionSet fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1f614c597efdb95b04c4079bd68240aa865d66dd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238670"
---
# <a name="itemactivitytimeset-resource-type"></a>Tipo de recurso itemActivityTimeSet

Namespace: microsoft.graph

O **recurso itemActivityTimeSet** fornece informações sobre quando [ocorreu uma atividade][activity] em um item.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

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

