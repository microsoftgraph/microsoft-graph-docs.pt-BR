---
title: tipo de recurso informationProtectionContentLabel
description: Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4f615655110ffdc6b76469d3d29cd4d13663d511
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938825"
---
# <a name="informationprotectioncontentlabel-resource-type"></a>tipo de recurso informationProtectionContentLabel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto. **informationProtectionContentLabel** é retornado pela API [extractLabel](../api/informationprotectionlabel-extractLabel.md) resolvida para o rótulo atualmente aplicado a um arquivo. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|AssignmentMethod for utilizado|String| Os valores possíveis são: `standard`, `privileged`, `auto`.|
|creationDatetime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|rótulo|[labelDetails](labeldetails.md)| Detalhes sobre o rótulo que é aplicado atualmente ao arquivo. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->