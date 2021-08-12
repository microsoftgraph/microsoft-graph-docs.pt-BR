---
title: Tipo de recurso complianceInformation
description: Esse recurso contém dados de conformidade associados ao controle de pontuação seguro.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 427660aa0f7227a4536a01cedcc7df818e8a499348c7be3f5be764f0764cad24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180870"
---
#  <a name="complianceinformation-resource-type"></a>Tipo de recurso complianceInformation

Namespace: microsoft.graph

Contém dados de conformidade associados ao controle de pontuação seguro.

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|certificationName|Cadeia de caracteres| Nome da certificação de conformidade (por exemplo, ISO 27018:2014, RGPD, FedRAMP, NIST 800-171) |
|certificationControls|[Coleção certificationControl](certificationcontrol.md)|Coleção dos controles de certificação associados à certificação|

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

