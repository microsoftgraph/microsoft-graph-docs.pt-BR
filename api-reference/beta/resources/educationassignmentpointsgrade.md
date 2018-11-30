---
title: tipo de recurso de educationAssignmentPointsGrade
description: Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** . Isso cria uma subclasse do educationAssignmentGrade,
ms.openlocfilehash: 2439ac8946fea588bd7bc1afe7f1ff1042b9179a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035167"
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