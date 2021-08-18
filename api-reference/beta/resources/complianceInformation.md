---
title: " Tipo de recurso complianceInformation"
description: Esse recurso contém dados de conformidade associados ao controle de pontuação seguro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 0b9b7385ae06b01747c0fc1c9c9001add515f43b472c3f7d419374f6e015a8a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253758"
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


