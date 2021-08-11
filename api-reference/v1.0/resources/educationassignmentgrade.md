---
title: Tipo de recurso educationAssignmentGrade
description: Representa o objeto Grade em um Envio.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a165203242f13805cab7dbf159519deaf42e9cb146358a4406362ae2a8ba9507
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230757"
---
# <a name="educationassignmentgrade-resource-type"></a>Tipo de recurso educationAssignmentGrade

Namespace: microsoft.graph

Representa o **objeto Grade** em um Envio. 

Esse é um tipo abstrato que nunca será instaurou; no entanto, todos os tipos de classificação (pontos, passagem/falha e assim por diante) são subclasses desse tipo de recurso. Esse objeto também rastreia quem está fazendo a classificação. Isso é usado na **propriedade submission.grade.**


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Usuário que fez a classificação. |
|gradedDateTime|DateTimeOffset| Momento no tempo em que a nota foi aplicada a esse objeto de envio. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


