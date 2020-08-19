---
title: " tipo de recurso complianceInformation"
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2c8bb3b2a016ec58da1ad58b01843a2691ad13b7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811137"
---
#  <a name="complianceinformation-resource-type"></a>tipo de recurso complianceInformation

Namespace: microsoft.graph

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
