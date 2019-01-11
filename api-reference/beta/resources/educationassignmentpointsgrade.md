---
title: tipo de recurso de educationAssignmentPointsGrade
description: Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** . Isso cria uma subclasse do educationAssignmentGrade,
localization_priority: Normal
ms.openlocfilehash: 2084a1bda6784165576c3ec454fa9ee88601c952
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861401"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>tipo de recurso de educationAssignmentPointsGrade

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** . Isso cria uma subclasse do [educationAssignmentGrade](educationassignmentgrade.md), que adicionará a quem dados para esta propriedade. Os pontos máximo é armazenado na propriedade **assignments.grading** .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|points|Single|Número de pontos um professor está dando este objeto de envio.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
