---
title: tipo de recurso informationProtectionContentLabel
description: Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8422f83db0c94eed74d5690343c51b70e2d87d82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016447"
---
# <a name="informationprotectioncontentlabel-resource-type"></a>tipo de recurso informationProtectionContentLabel

Namespace: microsoft.graph

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

