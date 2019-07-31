---
author: daspek
description: O recurso ItemActivityTimeSet fornece informações sobre quando uma atividade em um item foi realizada.
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c81bf7885ee1466e293236a987e90e21323daefd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010088"
---
# <a name="itemactivitytimeset-resource-type"></a>Tipo de recurso ItemActivityTimeSet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **ItemActivityTimeSet** fornece informações sobre quando uma [atividade][activity] em um item foi realizada.

[activity]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Nome da propriedade    | Tipo           | Descrição
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | Quando observamos a atividade ocorrer.
| recordedDateTime | DateTimeOffset | Quando a observação foi gravada no serviço.

A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.
Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.
Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
