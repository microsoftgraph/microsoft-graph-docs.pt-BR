---
title: tipo de recurso positionDetail
description: tipo de recurso positionDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: fbd013292754dea43dd69b645dcd2ab735559b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971479"
---
# <a name="positiondetail-resource-type"></a>tipo de recurso positionDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre posições relacionadas a entidades dentro de um [perfil](profile.md)de usuário.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                             | Descrição                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|empresarial         |[companyDetail](companydetail.md) | Detalhes sobre a empresa ou o empregador.                  |
|description     |String                            | Descrição da posição em questão.               |
|endMonthYear    |Data                              | Quando a posição terminou.                               |
|jobTitle        |String                            | O título mantido na posição.                  |
|role            |String                            | A função em que a posição é encaudada.                        |
|startMonthYear  |Data                              | O mês e o ano de início da posição.              |
|summary         |String                            |Breve resumo da posição.                          |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

