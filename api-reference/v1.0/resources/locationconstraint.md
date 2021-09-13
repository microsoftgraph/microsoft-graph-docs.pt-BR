---
title: Tipo de recurso locationConstraint
description: As condições indicadas por um cliente para o local de uma reunião.
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a2cafad390f0283ddefa09ea25f9ddf8d16b4dd5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134693"
---
# <a name="locationconstraint-resource-type"></a>Tipo de recurso locationConstraint

Namespace: microsoft.graph

As condições indicadas por um cliente para o local de uma reunião.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|isRequired|Booliano|O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local. |
|locations|Coleção [locationConstraintItem](locationconstraintitem.md)|Informações de restrição de um ou mais locais que o cliente solicita para a reunião.|
|suggestLocation|Booliano|O cliente solicita o serviço para sugerir um ou mais locais para a reunião.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

