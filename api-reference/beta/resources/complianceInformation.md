---
title: " Tipo de recurso complianceInformation"
description: Esse recurso contém dados de conformidade associados ao controle de pontuação seguro.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d5d59735dd8dc3dac96607bfc012f127283ca966
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023749"
---
#  <a name="complianceinformation-resource-type"></a>Tipo de recurso complianceInformation

Namespace: microsoft.graph

Contém dados de conformidade associados ao controle de pontuação seguro.

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|certificationName | cadeia de caracteres | Nome da certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171) |
|certificationControls | [Coleção certificationControl](certificationcontrol.md) | Coleção dos controles de certificação associados à certificação |

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


