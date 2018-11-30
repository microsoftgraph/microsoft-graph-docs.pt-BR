---
title: tipo de recurso de educationAssignmentGrade
description: " No entanto, todos os tipos de classificação (pontos, aprovação/reprovação e assim por diante) são subclasses isso"
ms.openlocfilehash: c9cd043f8887fda9427d7b56cf832001361d03a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038541"
---
# <a name="educationassignmentgrade-resource-type"></a>tipo de recurso de educationAssignmentGrade

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o objeto de **nível** em um envio. Este é um tipo abstrato que nunca será instanciado; No entanto, todos os tipos de classificação (pontos, aprovação/reprovação e assim por diante) são subclasses desse tipo de recurso. Este objeto também controla quem está fazendo a classificação. Isso é usado na propriedade **submission.grade** .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Usuário que fez a classificação. |
|gradedDateTime|DateTimeOffset| Momento específico quando o nível foi aplicada a este objeto de envio. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->