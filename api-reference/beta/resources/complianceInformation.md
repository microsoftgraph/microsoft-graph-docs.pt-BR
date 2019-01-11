---
title: " tipo de recurso de complianceInformation"
description: Este recurso contém conformidade dados associados a proteger o controle de pontuação.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820598"
---
#  <a name="complianceinformation-resource-type"></a>tipo de recurso de complianceInformation

Conformidade de contém dados associados a proteger o controle de pontuação.

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|certificationName | string | Nome de certificação de conformidade (por exemplo, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
|certificationControls | coleção [certificationControl](certificationcontrol.md) | Coleção de controles certificação associados a certificação |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
