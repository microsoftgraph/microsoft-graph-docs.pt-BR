---
title: " tipo de recurso complianceInformation"
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543361"
---
#  <a name="complianceinformation-resource-type"></a>tipo de recurso complianceInformation

Contém dados de conformidade associados ao controle de Pontuação segura.

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|certificaname | string | Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171) |
|certificationControls | coleção [certificationControl](certificationcontrol.md) | Coleção de controles de certificação associados à certificação |

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
