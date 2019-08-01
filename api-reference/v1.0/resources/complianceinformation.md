---
title: tipo de recurso complianceInformation
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9fc47940b8a9f249e66092ee016453a9eb5152ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032855"
---
#  <a name="complianceinformation-resource-type"></a>tipo de recurso complianceInformation

Contém dados de conformidade associados ao controle de Pontuação segura.

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|certificaname|String| Nome de certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171) |
|certificationControls|coleção [certificationControl](certificationcontrol.md)|Coleção de controles de certificação associados à certificação|

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
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
