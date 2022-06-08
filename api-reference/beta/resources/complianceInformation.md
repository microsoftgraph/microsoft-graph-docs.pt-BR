---
title: " Tipo de recurso complianceInformation"
description: Esse recurso contém dados de conformidade associados ao controle de pontuação segura.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 9d65043ca09ce945bbc87b83bfe2ec84d7f512bb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944924"
---
#  <a name="complianceinformation-resource-type"></a>Tipo de recurso complianceInformation

Namespace: microsoft.graph

Contém dados de conformidade associados ao controle de pontuação segura.

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|certificationName | cadeia de caracteres | Nome de certificação de conformidade (por exemplo, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171) |
|certificationControls | [coleção certificationControl](certificationcontrol.md) | Coleção dos controles de certificação associados à certificação |

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


