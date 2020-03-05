---
title: " tipo de recurso complianceInformation"
description: Este recurso contém dados de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 65eda1c24fee112ef18fc6682b537f92f924dcf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507573"
---
#  <a name="complianceinformation-resource-type"></a>tipo de recurso complianceInformation

Namespace: Microsoft. Graph

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
