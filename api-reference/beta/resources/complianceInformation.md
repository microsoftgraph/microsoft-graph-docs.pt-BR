---
title: " tipo de recurso de complianceInformation"
description: Este recurso contém conformidade dados associados a proteger o controle de pontuação.
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380956"
---
#  <a name="complianceinformation-resource-type"></a>tipo de recurso de complianceInformation

Conformidade de contém dados associados a proteger o controle de pontuação.

|Propriedade	 |Tipo |Descrição |
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
